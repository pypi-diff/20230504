# Comparing `tmp/netcheck-0.2.0a1.tar.gz` & `tmp/netcheck-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.2.0a1.tar", max compression
+gzip compressed data, was "netcheck-0.3.3.tar", max compression
```

## Comparing `netcheck-0.2.0a1.tar` & `netcheck-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     7020 2023-04-15 04:20:27.771741 netcheck-0.2.0a1/README.md
--rw-r--r--   0        0        0        0 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/__init__.py
--rw-r--r--   0        0        0     5896 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/cli.py
--rw-r--r--   0        0        0     2418 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/dns.py
--rw-r--r--   0        0        0     2192 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/http.py
--rw-r--r--   0        0        0     3406 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/runner.py
--rw-r--r--   0        0        0     1146 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/validation.py
--rw-r--r--   0        0        0      229 2023-04-15 04:20:27.779741 netcheck-0.2.0a1/netcheck/version.py
--rw-r--r--   0        0        0      634 2023-04-15 04:20:27.791741 netcheck-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 netcheck-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 21:41:09.154313 netcheck-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7609 2023-05-04 21:41:09.154313 netcheck-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/cli.py
+-rw-r--r--   0        0        0     2374 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/dns.py
+-rw-r--r--   0        0        0     2150 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/http.py
+-rw-r--r--   0        0        0     3438 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/runner.py
+-rw-r--r--   0        0        0     1184 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/validation.py
+-rw-r--r--   0        0        0      232 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/version.py
+-rw-r--r--   0        0        0      850 2023-05-04 21:41:09.170313 netcheck-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8401 1970-01-01 00:00:00.000000 netcheck-0.3.3/PKG-INFO
```

### Comparing `netcheck-0.2.0a1/LICENSE` & `netcheck-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.2.0a1/README.md` & `netcheck-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck) [![Coverage Status](https://coveralls.io/repos/github/hardbyte/netcheck/badge.svg?branch=main)](https://coveralls.io/github/hardbyte/netcheck?branch=main) ![PyPI - Downloads](https://img.shields.io/pypi/dm/netcheck)
-
-# Netchecks 
+# Netchecks
 
 <p align="center">
   <img alt="Netchecks Logo" src=".github/logo.png" width="150" />
 </p>
 
-**Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
-
-There are two main components:
-- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources.
-- **Netchecks CLI** - Command line tool for running network checks and asserting that they are as expected.
-
+<div align="center">
 
-Documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+[![PyPI](https://img.shields.io/pypi/v/netcheck.svg)](https://pypi.org/project/netcheck/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck)
+[![ArtifactHub - Netchecks](https://img.shields.io/badge/ArtifactHub-Netchecks-informational)](https://artifacthub.io/packages/helm/netchecks/netchecks)
+[![Coverage Status](https://coveralls.io/repos/github/hardbyte/netcheck/badge.svg?branch=main)](https://coveralls.io/github/hardbyte/netcheck?branch=main)
+[![CI status](https://github.com/hardbyte/netchecks/workflows/CI/badge.svg?branch=main)](https://github.com/hardbyte/netchecks/actions?query=branch%3Amain)
+[![PyPI Downloads](https://static.pepy.tech/badge/netcheck)](https://pypi.org/project/netcheck/)
 
-# Python Library and Command Line Tool
+</div>
 
-Configurable command line application that can be used to test network conditions are as expected.
+**Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
 
+There are two main components:
+- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+- **Netcheck CLI and Python Library** - Command line tool for running network checks and asserting that they are as expected. Keep reading for the quickstart.
 
-## Quickstart
 
+# Netcheck Command Line Tool Quickstart
 
+`netcheck` is a configurable command line application that can be used to test network conditions are as expected.
 
-### Installation
+## Installation
 
 Install the Python package:
 
 ```
 pip install netcheck
 ```
 
@@ -109,29 +110,29 @@
 ```
 
 Note the resulting status will show **pass** if the check fails as expected, and **fail** if the check passes unexpectedly!
 
 netcheck has built in default validation for each check type. For example, the `dns` check will pass if the DNS response code is `NOERROR`, there is at least one `A` record, and resolver responds in under 10 seconds. Custom validation is also possible, see the [Custom Validation](#custom-validation) section below.
 
 
-### Custom Validation
+## Custom Validation
 
 Custom validation can be added to checks by providing a `validation-rule` option on the command line, or a `validation` key in the rules of a test spec when configuring via json. 
 
 For example to override the default validation for the `dns` check to check that the A record resolves to a particular IP:
 
 ```shell
 netcheck dns --host github.com --validation-rule "data['A'].contains('20.248.137.48')"
 ```
 
 The validation rule is a CEL expression that is evaluated with the `data` returned by the check and `spec` objects in scope. For an introduction to CEL see https://github.com/google/cel-spec/blob/master/doc/intro.md
 
 
 
-### http checks
+## http checks
 
 `http` checks are also available:
 
 Assert that GitHub's status page includes the text "GitHub lives!" and that the response code is 200:
 
 ```shell
 netcheck http --url=https://github.com/status --validation-rule "data.body.contains('GitHub lives!') && data['status-code'] in [200, 201]"
@@ -155,15 +156,15 @@
 Ensure that a POST request fails:
 
 ```shell
 $ netcheck http --method=post --url=https://s3.ap-southeast-2.amazonaws.com --should-fail
 ```
 
 
-### Configuration via file
+## Configuration via file
 
 The main way to run `netcheck` is passing in a list of assertions. 
 A json file can be provided with a list of assertions to be checked:
 
 ```json
 {
   "assertions": [
@@ -236,15 +237,15 @@
 ## Development
 
 Update version in pyproject.toml, push to `main` and create a release on GitHub. Pypi release will be carried
 out by GitHub actions. 
 
 Install dev dependencies with Poetry:
 
-```
+```shell
 poetry install --with dev
 ```
 
 ### Manual Release 
 To release manually, use Poetry:
 
 ```shell
```

### Comparing `netcheck-0.2.0a1/netcheck/cli.py` & `netcheck-0.3.3/netcheck/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,58 +10,64 @@
 from netcheck.dns import DEFAULT_DNS_VALIDATION_RULE
 from .validation import validate_probe_result
 from .version import NETCHECK_VERSION
 from .http import NetcheckHttpMethod, DEFAULT_HTTP_VALIDATION_RULE
 from .runner import run_from_config, check_individual_assertion
 
 
-
-
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True)
 logger = logging.getLogger("netcheck")
-#logging.basicConfig(level=logging.INFO)
+# logging.basicConfig(level=logging.INFO)
 logging.captureWarnings(True)
 
 err_console = Console(stderr=True)
 
 
 class NetcheckOutputType(str, Enum):
-    json = 'json'
+    json = "json"
 
 
 class NetcheckTestType(str, Enum):
     dns = "dns"
-    http = 'http'
+    http = "http"
+
 
 def show_version(value: bool = True):
     """Print netcheck version"""
     if value:
         typer.echo(f"Netcheck version {NETCHECK_VERSION}")
         raise typer.Exit()
 
+
 @app.callback()
 def common(
     ctx: typer.Context,
-    version: bool = typer.Option(None, "--version", callback=show_version, is_eager=True),
+    version: bool = typer.Option(
+        None, "--version", callback=show_version, is_eager=True
+    ),
 ):
     pass
 
 
 @app.command()
 def run(
-        config: Path = typer.Option(..., exists=True, file_okay=True,
-                                    help='Config file with netcheck assertions'),
-        output: Optional[NetcheckOutputType] = typer.Option(NetcheckOutputType.json,
-                                                            '-o',
-                                                            '--output',
-                                                            help="Output format"),
-        verbose: bool = typer.Option(False, '-v')
-        ):
-    """Carry out all network assertions in given config file.
-    """
+    config: Path = typer.Option(
+        ...,
+        "--config",
+        "-c",
+        exists=True,
+        file_okay=True,
+        help="Config file with netcheck assertions",
+    ),
+    output: Optional[NetcheckOutputType] = typer.Option(
+        NetcheckOutputType.json, "-o", "--output", help="Output format"
+    ),
+    verbose: bool = typer.Option(False, "-v", "--verbose"),
+):
+    """Carry out all network assertions in given config file."""
     if verbose:
         err_console.print(f"Loading assertions from {config}")
     with config.open() as f:
         data = json.load(f)
 
     # TODO: Validate the config format once stable
     overall_results = run_from_config(data, err_console, verbose)
@@ -70,84 +76,95 @@
         err_console.print(f"Output type {output}")
 
     print_json(data=overall_results)
 
 
 @app.command()
 def http(
-        url: str = typer.Option('https://github.com/status', help="URL to request", rich_help_panel="http test"),
-        method: NetcheckHttpMethod = typer.Option(NetcheckHttpMethod.get,
-                                                  help="HTTP method",
-                                                  rich_help_panel='http test'),
-        timeout: float = typer.Option(30.0, '-t', '--timeout', help='Timeout in seconds'),
-        should_fail: bool = typer.Option(False, "--should-fail/--should-pass"),
-        validation_rule: str = typer.Option(None, "--validation-rule", help="Validation rule in CEL to apply to result"),
-        headers: Optional[List[str]] = typer.Option(
-            None,
-            '-h',
-            '--header',
-            help="Headers to send with request. Format: 'key:value'"),
-        verbose: bool = typer.Option(False, '-v', '--verbose')
+    url: str = typer.Option(
+        "https://github.com/status", help="URL to request", rich_help_panel="http test"
+    ),
+    method: NetcheckHttpMethod = typer.Option(
+        NetcheckHttpMethod.get,
+        help="HTTP method",
+        rich_help_panel="http test",
+        case_sensitive=False,
+    ),
+    timeout: float = typer.Option(30.0, "-t", "--timeout", help="Timeout in seconds"),
+    should_fail: bool = typer.Option(False, "--should-fail/--should-pass"),
+    validation_rule: str = typer.Option(
+        None, "--validation-rule", help="Validation rule in CEL to apply to result"
+    ),
+    headers: Optional[List[str]] = typer.Option(
+        None, "-h", "--header", help="Headers to send with request. Format: 'key:value'"
+    ),
+    verbose: bool = typer.Option(False, "-v", "--verbose"),
 ):
     """Carry out a http network check"""
     parsed_headers = {}
     for h in headers:
         if ":" in h:
-            key, value = h.split(':')
+            key, value = h.split(":")
             parsed_headers[key.strip()] = value.strip()
 
     test_config = {
         "url": url,
-        'method': method,
-        'timeout': timeout,
-        'headers': parsed_headers,
-        'expected': "fail" if should_fail else None
+        "method": method,
+        "timeout": timeout,
+        "headers": parsed_headers,
+        "expected": "fail" if should_fail else None,
     }
 
     if verbose:
-
         err_console.print(f"Netcheck http configuration:")
         err_console.print_json(data=test_config)
 
-
-
     result = check_individual_assertion(
         NetcheckTestType.http,
         test_config,
         err_console,
         validation_rule,
-        verbose=verbose
+        verbose=verbose,
     )
 
-
     output_result(result, should_fail, verbose)
 
 
 def output_result(result, should_fail, verbose):
-    failed = result['status'] == 'fail'
+    failed = result["status"] == "fail"
     notify_for_unexpected_test_result(failed, should_fail, verbose=verbose)
     print_json(data=result)
 
 
 @app.command()
 def dns(
-        server: str = typer.Option(None, help="DNS server to use for dns tests.", rich_help_panel="dns test"),
-        host: str = typer.Option('github.com', help='Host to search for', rich_help_panel="dns test"),
-        should_fail: bool = typer.Option(False, "--should-fail/--should-pass"),
-        validation_rule: str = typer.Option(None, "--validation-rule", help="Validation rule in CEL to apply to result"),
-        timeout: float = typer.Option(30.0, '-t', '--timeout', help='Timeout in seconds'),
-        verbose: bool = typer.Option(False, '-v', '--verbose')
+    server: str = typer.Option(
+        None,
+        "--server",
+        "-s",
+        help="DNS server to use for dns tests.",
+        rich_help_panel="dns test",
+    ),
+    host: str = typer.Option(
+        "github.com", help="Host to search for", rich_help_panel="dns test"
+    ),
+    should_fail: bool = typer.Option(False, "--should-fail/--should-pass"),
+    validation_rule: str = typer.Option(
+        None, "--validation-rule", help="Validation rule in CEL to apply to result"
+    ),
+    timeout: float = typer.Option(30.0, "-t", "--timeout", help="Timeout in seconds"),
+    verbose: bool = typer.Option(False, "-v", "--verbose"),
 ):
     """Carry out a dns check"""
 
     test_config = {
         "server": server,
         "host": host,
         "timeout": timeout,
-        'expected': "fail" if should_fail else None
+        "expected": "fail" if should_fail else None,
     }
     if verbose:
         err_console.print(f"netcheck dns")
         err_console.print(f"Options")
         err_console.print_json(data=test_config)
 
     if validation_rule is None:
@@ -157,30 +174,31 @@
         err_console.print("Validating result against custom validation rule")
 
     result = check_individual_assertion(
         NetcheckTestType.dns,
         test_config,
         err_console,
         validation_rule=validation_rule,
-        verbose=verbose
+        verbose=verbose,
     )
 
-
     output_result(result, should_fail, verbose)
 
 
 def notify_for_unexpected_test_result(failed, should_fail, verbose=False):
     if verbose:
         if failed:
             if not should_fail:
                 err_console.print("[bold red]:boom: Failed but was expected to pass[/]")
             else:
                 err_console.print("[yellow]:cross_mark: Failed. As expected.[/]")
         else:
             if not should_fail:
                 err_console.print("[green]✔ Passed (as expected)[/]")
             else:
-                err_console.print("[bold red]:bomb: The network test worked but was expected to fail![/]")
+                err_console.print(
+                    "[bold red]:bomb: The network test worked but was expected to fail![/]"
+                )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app()
```

### Comparing `netcheck-0.2.0a1/netcheck/dns.py` & `netcheck-0.3.3/netcheck/dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 import datetime
 import logging
 
 import dns.resolver
 from dns.exception import Timeout
+
 logger = logging.getLogger("netcheck.dns")
 
 
 DEFAULT_DNS_VALIDATION_RULE = """
 data['response-code'] == 'NOERROR' &&
 size(data['A']) >= 1 && 
 (timestamp(data['endTimestamp']) - timestamp(data['startTimestamp']) < duration('10s'))
 """
 
+
 def get_A_records_by_dns_lookup(target, nameserver=None, timeout=60):
     # We always reset the default dns resolver
     dns.resolver.reset_default_resolver()
     resolver = dns.resolver.get_default_resolver()
 
     result = {}
 
     if nameserver is not None:
         resolver.nameservers = [nameserver]
 
     # this resolver can also be used with the default nameserver
     # search=True is required to use the OS search path!
     # E.g. `kubernetes` -> `kubernetes.default.svc.cluster.local`
     try:
-        answer = resolver.resolve(target, 'A', lifetime=timeout, search=True)
+        answer = resolver.resolve(target, "A", lifetime=timeout, search=True)
 
         # canonical name of the target
-        result['canonical_name'] = answer.canonical_name.to_text()
+        result["canonical_name"] = answer.canonical_name.to_text()
         # answer.expiration is the TTL as a float timestamp
-        result['expiration'] = answer.expiration
+        result["expiration"] = answer.expiration
 
         # str(answer.response) is the raw DNS response
-        result['response'] = str(answer.response)
+        result["response"] = str(answer.response)
 
-        result['A'] = []
+        result["A"] = []
         for IPval in answer:
-            result['A'].append(IPval.to_text())
-        result['response-code'] = "NOERROR"
+            result["A"].append(IPval.to_text())
+        result["response-code"] = "NOERROR"
     except Timeout as e:
-        result['response-code'] = "TIMEOUT"
+        result["response-code"] = "TIMEOUT"
     except dns.resolver.NXDOMAIN:
-        result['response-code'] = "NXDOMAIN"
+        result["response-code"] = "NXDOMAIN"
     except dns.exception.DNSException as e:
-        result['response-code'] = "DNSERROR"
-        result['exception-name'] = e.__class__.__name__
-        result['exception-type'] = type(e)
-        result['exception'] = str(e)
+        result["response-code"] = "DNSERROR"
+        result["exception-type"] = e.__class__.__name__
+        result["exception"] = str(e)
 
     return result
 
 
 def dns_lookup_check(host, server, timeout=10):
-
     test_spec = {
-        'type': 'dns',
-        'nameserver': server,
-        'host': host,
-        'timeout': timeout,
+        "type": "dns",
+        "nameserver": server,
+        "host": host,
+        "timeout": timeout,
     }
     startTimestamp = datetime.datetime.utcnow().isoformat()
 
-
-
     try:
-        result_data = get_A_records_by_dns_lookup(host, nameserver=server, timeout=timeout)
+        result_data = get_A_records_by_dns_lookup(
+            host, nameserver=server, timeout=timeout
+        )
 
     except Exception as e:
         logger.info(f"Unexpected exception:\n\n{e}")
         raise
 
-    result_data['startTimestamp'] = startTimestamp
-    result_data['endTimestamp'] = datetime.datetime.utcnow().isoformat()
+    result_data["startTimestamp"] = startTimestamp
+    result_data["endTimestamp"] = datetime.datetime.utcnow().isoformat()
 
-    output = {
-        'spec': test_spec,
-        'data': result_data
-    }
+    output = {"spec": test_spec, "data": result_data}
     return output
```

### Comparing `netcheck-0.2.0a1/netcheck/http.py` & `netcheck-0.3.3/netcheck/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,78 +14,75 @@
 from pydantic import BaseModel
 
 logger = logging.getLogger("netcheck.http")
 DEFAULT_HTTP_VALIDATION_RULE = """
 data['status-code'] in [200, 201]
 """
 
+
 class NetcheckHttpHeaderType(str, Enum):
     bearer = "bearer"
 
 
 class NetcheckHttpHeaders(BaseModel):
     name: str
     value: str
     type: Optional[NetcheckHttpHeaderType] = None
 
 
 class NetcheckHttpMethod(str, Enum):
-    get = 'get'
-    post = 'post'
-    patch = 'patch'
-    put = 'put'
-    delete = 'delete'
+    get = "get"
+    post = "post"
+    patch = "patch"
+    put = "put"
+    delete = "delete"
 
 
 def http_request_check(
-        url,
-        method: NetcheckHttpMethod = 'get',
-        headers: Dict[str, str] = None,
-        timeout=5,
-        verify: bool = True,
+    url,
+    method: NetcheckHttpMethod = "get",
+    headers: Dict[str, str] = None,
+    timeout=5,
+    verify: bool = True,
 ):
     if headers is None:
         headers = {}
-    if 'User-Agent' not in headers:
-        headers['User-Agent'] = 'netcheck'
+    if "User-Agent" not in headers:
+        headers["User-Agent"] = "netcheck"
 
     # This structure gets stored along with the test results
     test_spec = {
-        'type': 'http',
-        'timeout': timeout,
-        'verify-tls-cert': verify,
-        'method': method,
-        'headers': headers,
-        'url': url,
+        "type": "http",
+        "timeout": timeout,
+        "verify-tls-cert": verify,
+        "method": method,
+        "headers": headers,
+        "url": url,
     }
 
     result_data = {
-        'startTimestamp': datetime.datetime.utcnow().isoformat(),
+        "startTimestamp": datetime.datetime.utcnow().isoformat(),
     }
 
-    output = {
-        'spec': test_spec,
-        'data': result_data
-    }
+    output = {"spec": test_spec, "data": result_data}
 
     # Prepare the arguments for requests
     requests_kwargs = {
-        'timeout': test_spec['timeout'],
-        'verify': test_spec['verify-tls-cert'],
-        'headers': test_spec['headers'],
+        "timeout": test_spec["timeout"],
+        "verify": test_spec["verify-tls-cert"],
+        "headers": test_spec["headers"],
     }
 
     try:
         response = getattr(requests, method)(url, **requests_kwargs)
-        result_data['status-code'] = response.status_code
-        result_data['headers'] = dict(response.headers)
-        result_data['body'] = response.text
+        result_data["status-code"] = response.status_code
+        result_data["headers"] = dict(response.headers)
+        result_data["body"] = response.text
         response.raise_for_status()
     except Exception as e:
         logger.debug(f"Caught exception:\n\n{e}")
-        result_data['exception-type'] = e.__class__.__name__
-        result_data['exception'] = str(e)
+        result_data["exception-type"] = e.__class__.__name__
+        result_data["exception"] = str(e)
 
-    result_data['endTimestamp'] = datetime.datetime.utcnow().isoformat()
+    result_data["endTimestamp"] = datetime.datetime.utcnow().isoformat()
 
     return output
-
```

### Comparing `netcheck-0.2.0a1/netcheck/runner.py` & `netcheck-0.3.3/netcheck/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,83 +12,83 @@
 logger = logging.getLogger("netcheck.runner")
 
 
 def run_from_config(netchecks_config: Dict, err_console, verbose: bool = False):
     if verbose:
         err_console.print(f"Loaded {len(netchecks_config['assertions'])} assertions")
     overall_results = {
-        'type': 'netcheck-output',
-        'outputVersion': OUTPUT_JSON_VERSION,
-        'metadata': {
-            'creationTimestamp': datetime.datetime.utcnow().isoformat(),
-            'version': NETCHECK_VERSION,
+        "type": "netcheck-output",
+        "outputVersion": OUTPUT_JSON_VERSION,
+        "metadata": {
+            "creationTimestamp": datetime.datetime.utcnow().isoformat(),
+            "version": NETCHECK_VERSION,
         },
-        'assertions': []
+        "assertions": [],
     }
     # Run each test
-    for assertion in netchecks_config['assertions']:
+    for assertion in netchecks_config["assertions"]:
         assertion_results = []
         if verbose:
             err_console.print(f"Running tests for assertion '{assertion['name']}'")
-        for rule in assertion['rules']:
+        for rule in assertion["rules"]:
             result = check_individual_assertion(
-                rule['type'],
+                rule["type"],
                 rule,
                 err_console=err_console,
-                validation_rule=rule.get('validation'),
+                validation_rule=rule.get("validation"),
                 verbose=verbose,
             )
             assertion_results.append(result)
 
-        overall_results['assertions'].append({
-            'name': assertion['name'],
-            'results': assertion_results
-        })
+        overall_results["assertions"].append(
+            {"name": assertion["name"], "results": assertion_results}
+        )
     return overall_results
 
 
-def check_individual_assertion(test_type: str, test_config, err_console, validation_rule=None, verbose=False):
+def check_individual_assertion(
+    test_type: str, test_config, err_console, validation_rule=None, verbose=False
+):
     match test_type:
-
-        case 'dns':
+        case "dns":
             if verbose:
                 err_console.print(f"DNS check looking up host '{test_config['host']}'")
             test_detail = dns_lookup_check(
-                host=test_config['host'],
-                server=test_config.get('server'),
-                timeout=test_config.get('timeout'),
-
+                host=test_config["host"],
+                server=test_config.get("server"),
+                timeout=test_config.get("timeout"),
             )
-        case 'http':
+        case "http":
             if verbose:
                 err_console.print(f"http check with url '{test_config['url']}'")
             test_detail = http_request_check(
-                test_config['url'],
-                test_config.get('method', 'get'),
-                headers=test_config.get('headers'),
-                timeout=test_config.get('timeout'),
-                verify=test_config.get('verify-tls-cert', True),
-
+                test_config["url"],
+                test_config.get("method", "get").lower(),
+                headers=test_config.get("headers"),
+                timeout=test_config.get("timeout"),
+                verify=test_config.get("verify-tls-cert", True),
             )
         case _:
             logger.warning("Unhandled test type")
             raise NotImplemented("Unknown test type")
 
     if validation_rule is None:
         # use the default validation rule
         match test_type:
-            case 'http': validation_rule = DEFAULT_HTTP_VALIDATION_RULE
-            case 'dns': validation_rule = DEFAULT_DNS_VALIDATION_RULE
+            case "http":
+                validation_rule = DEFAULT_HTTP_VALIDATION_RULE
+            case "dns":
+                validation_rule = DEFAULT_DNS_VALIDATION_RULE
     elif verbose:
         err_console.print("Using custom validation rule")
 
-    test_detail['spec']['pattern'] = validation_rule
+    test_detail["spec"]["pattern"] = validation_rule
     passed = validate_probe_result(test_detail, validation_rule)
 
     # Add the pass/status to the individual result. We also support an "expected": "fail" option
     # which will cause the test to fail if the validation passes.
-    if test_config.get('expected') == 'fail':
-        test_detail['status'] = 'fail' if passed else 'pass'
+    if test_config.get("expected") == "fail":
+        test_detail["status"] = "fail" if passed else "pass"
     else:
-        test_detail['status'] = 'pass' if passed else 'fail'
+        test_detail["status"] = "pass" if passed else "fail"
 
     return test_detail
```

### Comparing `netcheck-0.2.0a1/netcheck/validation.py` & `netcheck-0.3.3/netcheck/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from typing import Dict
 
 import celpy
 from celpy import CELParseError, CELEvalError, json_to_cel
 
 logger = logging.getLogger("netcheck.validation")
 
+
 def validate_probe_result(result: Dict, validation_rule: str):
     logger.info(f"Validating probe result with rule: {validation_rule}")
     logger.info(f"Probe result: {result}")
 
     env = celpy.Environment()
 
     # Validate the CEL validation rule and compile to ast
     try:
         ast = env.compile(validation_rule)
     except CELParseError as e:
         print("Invalid CEL expression. Treating as error.")
-        raise
+        raise ValueError("Invalid CEL expression")
 
     # create the CEL program
     functions = {
         "parse_json": lambda s: json_to_cel(json.loads(s)),
     }
     prgm = env.program(ast, functions=functions)
```

### Comparing `netcheck-0.2.0a1/PKG-INFO` & `netcheck-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.2.0a1
-Summary: 
+Version: 0.3.3
+Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cel-python (>=0.1.5,<0.2.0)
 Requires-Dist: dnspython (>=2.2,<3.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: rich (>=10.11.0,<14.0.0)
-Requires-Dist: typer (>=0.7,<0.8)
+Requires-Dist: typer (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck) [![Coverage Status](https://coveralls.io/repos/github/hardbyte/netcheck/badge.svg?branch=main)](https://coveralls.io/github/hardbyte/netcheck?branch=main) ![PyPI - Downloads](https://img.shields.io/pypi/dm/netcheck)
-
-# Netchecks 
+# Netchecks
 
 <p align="center">
   <img alt="Netchecks Logo" src=".github/logo.png" width="150" />
 </p>
 
-**Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
-
-There are two main components:
-- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources.
-- **Netchecks CLI** - Command line tool for running network checks and asserting that they are as expected.
-
+<div align="center">
 
-Documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+[![PyPI](https://img.shields.io/pypi/v/netcheck.svg)](https://pypi.org/project/netcheck/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck)
+[![ArtifactHub - Netchecks](https://img.shields.io/badge/ArtifactHub-Netchecks-informational)](https://artifacthub.io/packages/helm/netchecks/netchecks)
+[![Coverage Status](https://coveralls.io/repos/github/hardbyte/netcheck/badge.svg?branch=main)](https://coveralls.io/github/hardbyte/netcheck?branch=main)
+[![CI status](https://github.com/hardbyte/netchecks/workflows/CI/badge.svg?branch=main)](https://github.com/hardbyte/netchecks/actions?query=branch%3Amain)
+[![PyPI Downloads](https://static.pepy.tech/badge/netcheck)](https://pypi.org/project/netcheck/)
 
-# Python Library and Command Line Tool
+</div>
 
-Configurable command line application that can be used to test network conditions are as expected.
+**Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
 
+There are two main components:
+- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+- **Netcheck CLI and Python Library** - Command line tool for running network checks and asserting that they are as expected. Keep reading for the quickstart.
 
-## Quickstart
 
+# Netcheck Command Line Tool Quickstart
 
+`netcheck` is a configurable command line application that can be used to test network conditions are as expected.
 
-### Installation
+## Installation
 
 Install the Python package:
 
 ```
 pip install netcheck
 ```
 
@@ -127,29 +128,29 @@
 ```
 
 Note the resulting status will show **pass** if the check fails as expected, and **fail** if the check passes unexpectedly!
 
 netcheck has built in default validation for each check type. For example, the `dns` check will pass if the DNS response code is `NOERROR`, there is at least one `A` record, and resolver responds in under 10 seconds. Custom validation is also possible, see the [Custom Validation](#custom-validation) section below.
 
 
-### Custom Validation
+## Custom Validation
 
 Custom validation can be added to checks by providing a `validation-rule` option on the command line, or a `validation` key in the rules of a test spec when configuring via json. 
 
 For example to override the default validation for the `dns` check to check that the A record resolves to a particular IP:
 
 ```shell
 netcheck dns --host github.com --validation-rule "data['A'].contains('20.248.137.48')"
 ```
 
 The validation rule is a CEL expression that is evaluated with the `data` returned by the check and `spec` objects in scope. For an introduction to CEL see https://github.com/google/cel-spec/blob/master/doc/intro.md
 
 
 
-### http checks
+## http checks
 
 `http` checks are also available:
 
 Assert that GitHub's status page includes the text "GitHub lives!" and that the response code is 200:
 
 ```shell
 netcheck http --url=https://github.com/status --validation-rule "data.body.contains('GitHub lives!') && data['status-code'] in [200, 201]"
@@ -173,15 +174,15 @@
 Ensure that a POST request fails:
 
 ```shell
 $ netcheck http --method=post --url=https://s3.ap-southeast-2.amazonaws.com --should-fail
 ```
 
 
-### Configuration via file
+## Configuration via file
 
 The main way to run `netcheck` is passing in a list of assertions. 
 A json file can be provided with a list of assertions to be checked:
 
 ```json
 {
   "assertions": [
@@ -254,15 +255,15 @@
 ## Development
 
 Update version in pyproject.toml, push to `main` and create a release on GitHub. Pypi release will be carried
 out by GitHub actions. 
 
 Install dev dependencies with Poetry:
 
-```
+```shell
 poetry install --with dev
 ```
 
 ### Manual Release 
 To release manually, use Poetry:
 
 ```shell
```

