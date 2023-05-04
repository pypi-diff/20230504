# Comparing `tmp/aws_assumptions-0.1.0.tar.gz` & `tmp/aws_assumptions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_assumptions-0.1.0.tar", max compression
+gzip compressed data, was "aws_assumptions-0.2.0.tar", max compression
```

## Comparing `aws_assumptions-0.1.0.tar` & `aws_assumptions-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3617 2023-05-03 20:32:04.272210 aws_assumptions-0.1.0/README.md
--rw-r--r--   0        0        0        1 2023-05-03 20:32:09.274067 aws_assumptions-0.1.0/aws_assumptions/__init__.py
--rwxr-xr-x   0        0        0     6306 2023-05-03 20:08:54.547756 aws_assumptions-0.1.0/aws_assumptions/identity.py
--rwxr-xr-x   0        0        0     3422 2023-05-03 20:16:08.533105 aws_assumptions-0.1.0/aws_assumptions/scripts.py
--rw-r--r--   0        0        0      604 2023-05-03 19:02:40.642925 aws_assumptions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 aws_assumptions-0.1.0/setup.py
--rw-r--r--   0        0        0     4236 1970-01-01 00:00:00.000000 aws_assumptions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6191 2023-05-04 15:45:21.952366 aws_assumptions-0.2.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-03 20:32:09.274067 aws_assumptions-0.2.0/aws_assumptions/__init__.py
+-rwxr-xr-x   0        0        0     6306 2023-05-03 20:08:54.547756 aws_assumptions-0.2.0/aws_assumptions/identity.py
+-rwxr-xr-x   0        0        0     5345 2023-05-04 15:42:05.111942 aws_assumptions-0.2.0/aws_assumptions/scripts.py
+-rw-r--r--   0        0        0      661 2023-05-04 15:47:21.765634 aws_assumptions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7230 1970-01-01 00:00:00.000000 aws_assumptions-0.2.0/setup.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 aws_assumptions-0.2.0/PKG-INFO
```

### Comparing `aws_assumptions-0.1.0/aws_assumptions/identity.py` & `aws_assumptions-0.2.0/aws_assumptions/identity.py`

 * *Files identical despite different names*

### Comparing `aws_assumptions-0.1.0/aws_assumptions/scripts.py` & `aws_assumptions-0.2.0/aws_assumptions/scripts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 #!/usr/bin/env python3
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace, REMAINDER
 from json import dumps
+from os import environ
+from subprocess import run
 from textwrap import dedent
+
+from dotenv import dotenv_values
+
 from .identity import Identity, PolicyArn, Tag, DEFAULT_CLIENT
 
 
-def main():
-    cmd_funcs = {"whoami": whoami, "assume": assume_role}
+def main(help=False):
+    cmd_funcs = {"whoami": whoami, "assume": assume_role, "exec": executor}
 
     parser = ArgumentParser(
         epilog="Switch roles, or through a chain or roles, or print identity information from AWS STS"
     )
+
     subparsers = parser.add_subparsers(dest="command")
 
     subparsers.add_parser(
         "whoami", epilog="Prints get-caller-identity info in JSON format"
     )
 
     assume = subparsers.add_parser(
@@ -75,47 +81,126 @@
     assume.add_argument(
         "-d",
         "--duration-seconds",
         help="Optional duration for the session.",
         type=int,
         default=3600,
     )
+
+    # The order this comes in is imperative. It MUST come after all args in the parent
+    # that we want but BEFORE those that we don't
+    exec = subparsers.add_parser(
+        "exec",
+        epilog="Execute a command in a shell with newly created credentials.",
+        parents=[assume],
+        add_help=False
+    )
+
+    exec.add_argument(
+       "-N",
+       "--no-inherit-env",
+       action="store_true",
+       help="Don't allow the executed command to inherit the parent's env."
+    )
+
+    exec.add_argument(
+       "-e",
+       "--env-var",
+       action="append",
+       type=str,
+       help="Env var in the format `MYVAR=foo` to pass to the executed command's environment. Can be declared multiple times."
+    )
+
+    exec.add_argument(
+      "--env-file",
+      type=str,
+      help="Load env vars from a .env file."
+    )
+
     assume.add_argument(
         "-e",
         "--env-vars",
         help="Output env vars usable from a terminal. If not set the output will match the output of aws-cli's `aws sts assume-role` JSON",
         action="store_true",
     )
 
+    exec.add_argument(
+        "exec_command",
+        nargs=REMAINDER
+    )
+
+    if help:
+      parser.print_help()
+      return
+
     args = parser.parse_args()
+
     if args.command is None:
         parser.print_help()
         exit()
 
     return cmd_funcs[args.command](args)
 
 
-def assume_role(args):
+def assume_role(args: Namespace, print_vars: bool = True):
     opts = dict(
         RoleArn=args.role_arn,
         RoleSessionName=args.role_session_name,
         PolicyArns=[PolicyArn(arn) for arn in (args.policy_arn or [])],
         Tags=[Tag(*pair) for pair in [tag.split("=") for tag in (args.tag or [])]],
         TransitiveTagKeys=args.transitive_tag_key or [],
     )
 
     if args.external_id:
         opts["ExternalId"] = args.external_id
 
     role = Identity(**opts)
 
-    if args.env_vars:
-        print(role.credentials.env_vars)
-    else:
-        res = dumps(role.credentials, indent=2)
-        print(res)
+    if print_vars:
+      if args.env_vars:
+          print(role.credentials.env_vars)
+      else:
+          res = dumps(role.credentials, indent=2)
+          print(res)
 
+    return role
 
-def whoami(_):
+
+def whoami(_: Namespace):
     res = DEFAULT_CLIENT.get_caller_identity()
     del res["ResponseMetadata"]
     print(dumps(res, indent=2))
+
+
+def executor(args: Namespace):
+  if not args.exec_command:
+    print("Must supply a command to run.")
+    main(help=True)
+    exit()
+
+  role = assume_role(args, print_vars=False)
+
+  env = environ if not args.no_inherit_env else {}
+
+  if args.env_var:
+    env.update({
+      pair[0]: pair[1] for pair in [ env_var.split("=") for env_var in args.env_var]
+    })
+
+  env.update({
+    "AWS_ACCESS_KEY_ID": role.credentials.AccessKeyId,
+    "AWS_SECRET_ACCESS_KEY": role.credentials.SecretAccessKey,
+    "AWS_SESSION_TOKEN": role.credentials.SessionToken
+  })
+
+  if args.env_file:
+    env.update(dotenv_values(args.env_file))
+
+  run(
+    args.exec_command,
+    env=env,
+    shell=False
+  )
+
+
+if __name__ == "__main__":
+  main()
```

### Comparing `aws_assumptions-0.1.0/pyproject.toml` & `aws_assumptions-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "aws-assumptions"
-version = "0.1.0"
-description = "Easily export env vars for assuming AWS roles using STS Assume Role"
+version = "0.2.0"
+description = "Assume role(s) from a terminal and easily manage boto3 clients for multiple identities at once."
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 packages = [
     { include = "aws_assumptions"}
 ]
 homepage = "https://github.com/mathewmoon/aws-assumptions"
 documentation = "https://github.com/mathewmoon/aws-assumptions"
 readme = "README.md"
 [tool.poetry.dependencies]
-python = "^3.9"
+python   = "^3.9"
 boto3    = ">=1.26"
+python-dotenv   = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 assumptions = "aws_assumptions.scripts:main"
```

### Comparing `aws_assumptions-0.1.0/setup.py` & `aws_assumptions-0.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['aws_assumptions']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.26']
+['boto3>=1.26', 'python-dotenv>=1.0.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['assumptions = aws_assumptions.scripts:main']}
 
 setup_kwargs = {
     'name': 'aws-assumptions',
-    'version': '0.1.0',
-    'description': 'Easily export env vars for assuming AWS roles using STS Assume Role',
-    'long_description': '# aws-assumptions\n\nEasily switch between roles, or a chain of roles and create boto3 clients and resources off of those assumed identities.\nAlong with being able to use this package as an import a cli script is included.\n\n## CLI Usage\n\nAvailable commands\n```\n~  > assumptions -h\nusage: assumptions [-h] {whoami,assume} ...\n\npositional arguments:\n  {whoami,assume}\n\noptional arguments:\n  -h, --help       show this help message and exit\n\nSwitch roles, or through a chain or roles, or print identity information from AWS STS\n```\n\nGetting current identity\n```\n> assumptions whoami -h\nusage: assumptions whoami [-h]\n\noptional arguments:\n  -h, --help  show this help message and exit\n\nPrints get-caller-identity info in JSON format\n```\n\nAssuming a role\n```\n~  > assumptions assume -h\nusage: assumptions assume [-h] -r ROLE_ARN [-n ROLE_SESSION_NAME] [-p POLICY_ARN] [-t TAG] [-T TRANSITIVE_TAG_KEY] [-E EXTERNAL_ID] [-d DURATION_SECONDS] [-e]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r ROLE_ARN, --role-arn ROLE_ARN\n                        Role to assume. If declared multiple times each role will assume the next in the order given. All other options will be applied to all roles in the chain.\n  -n ROLE_SESSION_NAME, --role-session-name ROLE_SESSION_NAME\n                        The session name to use with the role.\n  -p POLICY_ARN, --policy-arn POLICY_ARN\n                        Optional policy to attach to a session. Can be declared multiple times.\n  -t TAG, --tag TAG     Optional tag to add to the session in the format of `mytagkey=myvalue`. Can be declared multiple times for multiple tags.\n  -T TRANSITIVE_TAG_KEY, --transitive-tag-key TRANSITIVE_TAG_KEY\n                        Transitive tag key. Can be declared multiple times.\n  -E EXTERNAL_ID, --external-id EXTERNAL_ID\n                        Optional External ID for the session. Required by some AssumeRole policies\n  -d DURATION_SECONDS, --duration-seconds DURATION_SECONDS\n                        Optional duration for the session.\n  -e, --env-vars        Output env vars usable from a terminal. If not set the output will match the output of aws-cli\'s `aws sts assume-role` JSON\n\nAssume a role or a chain of roles with optional attributes, outputting the newly acquired credentials. Maintains parity with boto3\'s sts.assume_role except for MFA\n```\n\nExample of assuming a role with env vars\n```\n> assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com -e > creds.env\n> . creds.env\n```\n\nor\n\n```\n$(assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com)\n```\n\n## Switching through multiple roles\nIf you need to chain roles (EG: Assume a role that assumes a role that assumes a role) you can pass the `-r` flag multiple times.\nNote however that all other options, such as `--external-id` or `--tag` will be applied to every session in the chain.\n\n## As a library\n\nAssuming a role and creating clients\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn="arn:aws:iam::123456789876:role/my-role",\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\nChaining roles\n\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn=[\n    "arn:aws:iam::123456789876:role/my-role",\n    "arn:aws:iam::123456789876:role/my-second-role"\n  ],\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\n',
+    'version': '0.2.0',
+    'description': 'Assume role(s) from a terminal and easily manage boto3 clients for multiple identities at once.',
+    'long_description': '# aws-assumptions\n\n* Easily switch between roles, or a chain of roles and create boto3 clients and resources off of those assumed identities.\n* Can be used as a library to assume roles. The created object also provides a factory for creating boto3 clients/resources off of the object\n* CLI script that allows printing credentials to stdout as either the standard response from boto3.sts.assume_role or formatted to use as env vars in a *nix terminal.\n* CLI provides `exec` command to execute terminal commands in a subshell with the newly minted credentials injected into the environment\n\n\n### Available CLI commands\n```\n~  > assumptions -h\nusage: assumptions [-h] {whoami,assume} ...\n\npositional arguments:\n  {whoami,assume,exec}\n\noptional arguments:\n  -h, --help       show this help message and exit\n\nSwitch roles, or through a chain or roles, or print identity information from AWS STS\n```\n\n### Getting current identity\n```\n> assumptions whoami -h\nusage: assumptions whoami [-h]\n\noptional arguments:\n  -h, --help  show this help message and exit\n\nPrints get-caller-identity info in JSON format\n```\n\n### Assuming a role\n```\n~  > assumptions assume -h\nusage: assumptions assume [-h] -r ROLE_ARN [-n ROLE_SESSION_NAME] [-p POLICY_ARN] [-t TAG] [-T TRANSITIVE_TAG_KEY] [-E EXTERNAL_ID] [-d DURATION_SECONDS] [-e]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r ROLE_ARN, --role-arn ROLE_ARN\n                        Role to assume. If declared multiple times each role will assume the next in the order given. All other options will be applied to all roles in the chain.\n  -n ROLE_SESSION_NAME, --role-session-name ROLE_SESSION_NAME\n                        The session name to use with the role.\n  -p POLICY_ARN, --policy-arn POLICY_ARN\n                        Optional policy to attach to a session. Can be declared multiple times.\n  -t TAG, --tag TAG     Optional tag to add to the session in the format of `mytagkey=myvalue`. Can be declared multiple times for multiple tags.\n  -T TRANSITIVE_TAG_KEY, --transitive-tag-key TRANSITIVE_TAG_KEY\n                        Transitive tag key. Can be declared multiple times.\n  -E EXTERNAL_ID, --external-id EXTERNAL_ID\n                        Optional External ID for the session. Required by some AssumeRole policies\n  -d DURATION_SECONDS, --duration-seconds DURATION_SECONDS\n                        Optional duration for the session.\n  -e, --env-vars        Output env vars usable from a terminal. If not set the output will match the output of aws-cli\'s `aws sts assume-role` JSON\n\nAssume a role or a chain of roles with optional attributes, outputting the newly acquired credentials. Maintains parity with boto3\'s sts.assume_role except for MFA\n```\n\nExample of assuming a role with env vars\n```\n> assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com -e > creds.env\n> . creds.env\n```\n\nor\n\n```\n$(assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com)\n```\n\n### Using `exec`\n\n```\nusage: scripts.py exec [-h] -r ROLE_ARN [-n ROLE_SESSION_NAME] [-p POLICY_ARN] [-t TAG] [-T TRANSITIVE_TAG_KEY] [-E EXTERNAL_ID] [-d DURATION_SECONDS] [-N] [-e ENV_VAR] [--env-file ENV_FILE] ...\n\npositional arguments:\n  exec_command\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r ROLE_ARN, --role-arn ROLE_ARN\n                        Role to assume. If declared multiple times each role will assume the next in the order given. All other options will be applied to all roles in the chain.\n  -n ROLE_SESSION_NAME, --role-session-name ROLE_SESSION_NAME\n                        The session name to use with the role.\n  -p POLICY_ARN, --policy-arn POLICY_ARN\n                        Optional policy to attach to a session. Can be declared multiple times.\n  -t TAG, --tag TAG     Optional tag to add to the session in the format of `mytagkey=myvalue`. Can be declared multiple times for multiple tags.\n  -T TRANSITIVE_TAG_KEY, --transitive-tag-key TRANSITIVE_TAG_KEY\n                        Transitive tag key. Can be declared multiple times.\n  -E EXTERNAL_ID, --external-id EXTERNAL_ID\n                        Optional External ID for the session. Required by some AssumeRole policies\n  -d DURATION_SECONDS, --duration-seconds DURATION_SECONDS\n                        Optional duration for the session.\n  -N, --no-inherit-env  Don\'t allow the executed command to inherit the parent\'s env.\n  -e ENV_VAR, --env-var ENV_VAR\n                        Env var in the format `MYVAR=foo` to pass to the executed command\'s environment. Can be declared multiple times.\n  --env-file ENV_FILE   Load env vars from a .env file.\n\nExecute a command in a shell with newly created credentials.\n```\n\nExample\n```\n> assumptions exec -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com aws sts get-caller-identity\n{\n    "UserId": "AROA4HO3IAI67GZHCWWWQ:bob@nowhere.com",\n    "Account": "840662778429",\n    "Arn": "arn:aws:sts::123456789876:assumed-role/my-role/bob@nowhere.com"\n}\n```\n\nExample passing env vars to an interactive shell\n```\n> assumptions exec -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com -e FOO=bar bash\n$ echo $FOO\nbar\n```\n\n## Switching through multiple roles\nIf you need to chain roles (EG: Assume a role that assumes a role that assumes a role) you can pass the `-r` flag multiple times.\nNote however that all other options, such as `--external-id` or `--tag` will be applied to every session in the chain.\n\n## As a library\n\nAssuming a role and creating clients\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn="arn:aws:iam::123456789876:role/my-role",\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\nChaining roles\n\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn=[\n    "arn:aws:iam::123456789876:role/my-role",\n    "arn:aws:iam::123456789876:role/my-second-role"\n  ],\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\n',
     'author': 'Mathew Moon',
     'author_email': 'me@mathewmoon.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mathewmoon/aws-assumptions',
     'packages': packages,
     'package_data': package_data,
```

