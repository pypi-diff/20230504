# Comparing `tmp/gh_utils-0.6.5.tar.gz` & `tmp/gh_utils-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_utils-0.6.5.tar", max compression
+gzip compressed data, was "gh_utils-0.6.6.tar", max compression
```

## Comparing `gh_utils-0.6.5.tar` & `gh_utils-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.5/LICENSE
--rw-r--r--   0        0        0     2055 2023-03-20 11:39:20.380308 gh_utils-0.6.5/README.md
--rw-r--r--   0        0        0       90 2023-03-20 11:42:45.125857 gh_utils-0.6.5/gh_utils/__init__.py
--rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.5/gh_utils/config.py
--rwxr-xr-x   0        0        0     4808 2023-03-20 11:41:26.712132 gh_utils-0.6.5/gh_utils/gh_create_repo_and_add_to_remote.py
--rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.5/gh_utils/types.py
--rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.5/gh_utils/utils.py
--rw-r--r--   0        0        0      806 2023-03-20 11:42:45.125375 gh_utils-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 gh_utils-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2055 2023-03-20 11:39:20.380308 gh_utils-0.6.6/README.md
+-rw-r--r--   0        0        0       90 2023-05-04 16:18:51.488409 gh_utils-0.6.6/gh_utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.6/gh_utils/config.py
+-rwxr-xr-x   0        0        0     5119 2023-05-04 16:16:16.753048 gh_utils-0.6.6/gh_utils/gh_create_repo_and_add_to_remote.py
+-rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.6/gh_utils/types.py
+-rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.6/gh_utils/utils.py
+-rw-r--r--   0        0        0      806 2023-05-04 16:18:51.487407 gh_utils-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 gh_utils-0.6.6/PKG-INFO
```

### Comparing `gh_utils-0.6.5/LICENSE` & `gh_utils-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.5/README.md` & `gh_utils-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.5/gh_utils/config.py` & `gh_utils-0.6.6/gh_utils/config.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.5/gh_utils/gh_create_repo_and_add_to_remote.py` & `gh_utils-0.6.6/gh_utils/gh_create_repo_and_add_to_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,28 @@
         '--name',
         help='The string to use as GitHub repo name, or <user|org>/<repo-name> with a slash',
         metavar='GITHUB REPO NAME',
         type=str,
         default=None,
     )
 
+    # -r, --remote string          Specify remote name for the new repository
+    parser.add_argument('-r', '--remote', help='Specify remote name for the new repository', type=str, default='origin')
+
     parser.add_argument(
         '--public',
         help='Create a public repository',
         action='store_true',
         default=False,
     )
 
     parser.add_argument(
-        '--overwrite-remote-origin',
+        '--overwrite-remote',
         '--force',
-        help='Overwrites remote origin if exists',
+        help='Overwrites remote if exists',
         action='store_true',
         default=False,
     )
 
     parser.add_argument(
         '-H',
         '--hostname',
@@ -83,17 +86,18 @@
 
 
 def main():
     args = get_args()
     append = args.append
     name = args.name
     public = args.public
-    overwrite_remote_origin = args.overwrite_remote_origin
+    overwrite_remote_origin = args.overwrite_remote
     hostname = args.hostname
     protocol = args.protocol
+    desired_remote_name = args.remote
 
     curr_path_name = Path.cwd().name
     if name is not None:
         repo_name = name
     else:
         repo_name = curr_path_name if append is None else f'{curr_path_name}-{append}'
     visibility_flag = '--public' if public else '--private'
@@ -101,43 +105,43 @@
     # (re) init the repo
     subprocess.run(['git', 'init'])
 
     # add to remote
     remotes_p = subprocess.run(['git', 'remote'], capture_output=True)
     remotes = remotes_p.stdout.splitlines()
     # print(remotes)
-    remote_origin_exists = b'origin' in remotes
+    remote_origin_exists = desired_remote_name.encode() in remotes
     gh_username = hostname_to_user(hostname)
     desired_remote_url = get_desired_remote_url(
         hostname, protocol, repo_name, gh_username
     )
     if not args.no_set_default:
         print(f'Running `gh repo set-default {gh_username}/{repo_name}`')
         subprocess.run(['gh', 'repo', 'set-default', f'{gh_username}/{repo_name}'])
     if remote_origin_exists:
-        print('Remote origin exists.')
+        print(f'Remote {desired_remote_name} exists.')
         # run `git remote get-url origin` to get the url for the remote
         remote_origin_url = (
-            subprocess.run(['git', 'remote', 'get-url', 'origin'], capture_output=True)
+            subprocess.run(['git', 'remote', 'get-url', desired_remote_name], capture_output=True)
             .stdout.decode()
             .strip()
         )
         if remote_origin_url.removesuffix('.git') == desired_remote_url.removesuffix(
             '.git'
         ):
-            print(f'Remote origin URL {remote_origin_url} is already the desired one.')
+            print(f'Remote {desired_remote_name} URL {remote_origin_url} is already the desired one.')
             print('Exiting.')
             return
         if overwrite_remote_origin:
-            subprocess.run(['git', 'remote', 'remove', 'origin'])
+            subprocess.run(['git', 'remote', 'remove', desired_remote_name])
             print('Removed previous remote.')
         else:
-            subprocess.run(['git', 'remote', 'rename', 'origin', 'upstream'])
+            subprocess.run(['git', 'remote', 'rename', desired_remote_name, 'upstream'])
             print('Renamed previous remote to upstream.')
-    subprocess.run(['git', 'remote', 'add', 'origin', desired_remote_url])
+    subprocess.run(['git', 'remote', 'add', desired_remote_name, desired_remote_url])
     print(f'Added remote: {desired_remote_url}')
 
     # create a repo on github, may fail if already exists
     subprocess.run(['gh', 'repo', 'create', repo_name, visibility_flag])
 
 
 @cache
```

### Comparing `gh_utils-0.6.5/gh_utils/utils.py` & `gh_utils-0.6.6/gh_utils/utils.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.5/pyproject.toml` & `gh_utils-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gh-utils"
-version = "0.6.5"
+version = "0.6.6"
 description = "GitHub CLI Utilities"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/gh-utils"
 repository = "https://github.com/tddschn/gh-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `gh_utils-0.6.5/PKG-INFO` & `gh_utils-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-utils
-Version: 0.6.5
+Version: 0.6.6
 Summary: GitHub CLI Utilities
 Home-page: https://github.com/tddschn/gh-utils
 License: MIT
 Keywords: gh,github,utils
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

