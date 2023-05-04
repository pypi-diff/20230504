# Comparing `tmp/aquasec-cli-0.0.5.tar.gz` & `tmp/aquasec-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquasec-cli-0.0.5.tar", last modified: Thu Apr 27 15:26:49 2023, max compression
+gzip compressed data, was "aquasec-cli-0.0.6.tar", last modified: Thu May  4 18:39:54 2023, max compression
```

## Comparing `aquasec-cli-0.0.5.tar` & `aquasec-cli-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.215618 aquasec-cli-0.0.5/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/LICENSE
--rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/MANIFEST.in
--rw-r--r--   0 adamt      (501) staff       (20)    43887 2023-04-27 15:26:49.216049 aquasec-cli-0.0.5/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     2458 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/README.md
--rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/README.rst
--rw-rw-r--   0 adamt      (501) staff       (20)      509 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/SECURITY.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.208872 aquasec-cli-0.0.5/aquasec_cli/
--rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/_version.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.214779 aquasec-cli-0.0.5/aquasec_cli/commands/
--rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1530 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1916 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/commands/report.py
--rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/main.py
--rw-rw-r--   0 adamt      (501) staff       (20)      570 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/aquasec_cli/utils.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-27 15:26:49.212665 aquasec-cli-0.0.5/aquasec_cli.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    43887 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      526 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       53 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/entry_points.txt
--rw-r--r--   0 adamt      (501) staff       (20)      107 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/top_level.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-27 15:26:49.000000 aquasec-cli-0.0.5/aquasec_cli.egg-info/zip-safe
--rw-rw-r--   0 adamt      (501) staff       (20)      953 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/pyproject.toml
--rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/requirements.txt
--rw-rw-r--   0 adamt      (501) staff       (20)      740 2023-04-27 15:26:49.217424 aquasec-cli-0.0.5/setup.cfg
--rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-04-27 15:25:40.000000 aquasec-cli-0.0.5/setup.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:39:54.562624 aquasec-cli-0.0.6/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/LICENSE
+-rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/MANIFEST.in
+-rw-r--r--   0 adamt      (501) staff       (20)    45390 2023-05-04 18:39:54.563103 aquasec-cli-0.0.6/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     3961 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/README.md
+-rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/README.rst
+-rw-rw-r--   0 adamt      (501) staff       (20)      509 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/SECURITY.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:39:54.555521 aquasec-cli-0.0.6/aquasec_cli/
+-rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/_version.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:39:54.561963 aquasec-cli-0.0.6/aquasec_cli/commands/
+-rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/commands/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1939 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/commands/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     2241 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/commands/report.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/main.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      859 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/aquasec_cli/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:39:54.559764 aquasec-cli-0.0.6/aquasec_cli.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    45390 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      526 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       53 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/entry_points.txt
+-rw-r--r--   0 adamt      (501) staff       (20)      107 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/top_level.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-05-04 18:39:54.000000 aquasec-cli-0.0.6/aquasec_cli.egg-info/zip-safe
+-rw-rw-r--   0 adamt      (501) staff       (20)      953 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/requirements.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)      740 2023-05-04 18:39:54.564167 aquasec-cli-0.0.6/setup.cfg
+-rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-05-04 18:37:45.000000 aquasec-cli-0.0.6/setup.py
```

### Comparing `aquasec-cli-0.0.5/LICENSE` & `aquasec-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.5/PKG-INFO` & `aquasec-cli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -711,42 +711,92 @@
 
 Commands:
   delete   Deletes created API Auth
   init     Initializes API Auth
   reports  Generate CIS Bench Reports
 ```
 
+```bash
+>>> aquasec-cli init --help   
+Usage: aquasec-cli init [OPTIONS]
+
+  Initializes API Authentication token used to run commands; required to
+  generate before a command can be executed
+
+Options:
+  --csp_roles TEXT  Creates Aquasec auth token
+  --endpoints TEXT  Endpoint Call Allowed
+  --help            Show this message and exit.
+```
+
+```bash
+>>> aquasec-cli reports --help
+Usage: aquasec-cli reports [OPTIONS]
+
+  Generate CIS Bench Reports
+
+  Used to generate CIS Bench Reports in different formats
+
+Options:
+  -r, --report_type [cis|kube_bench|linux|openshift|disa_stig|all]
+                                  Report type to genorate
+  -c, --cluster_name TEXT         Supply Cluster name
+  -l, --report_location TEXT      Directory to write out report to; please
+                                  ensure proper formatting given the system
+                                  you are on  [required]
+  --report_format [list|flat_list|raw]
+                                  Report Format
+  --help                          Show this message and exit.
+```
+
+```bash
+>>> aquasec-cli delete --help
+Usage: aquasec-cli delete [OPTIONS]
+
+  Deletes created API Auth
+
+Options:
+  --yes
+  --help  Show this message and exit.
+```
+
 __NOTE:__ Each subcommand has a help menu to assist with the calls being made. This project relies on the yaml or localized configurations being help as they are not passed in the commands as of this release.
 
 __Create API Auth Token:__
 
 ```bash
 >>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
 Initializing API
 INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
 ```
 
 __Run Report:__
 
 ```bash
-aquasec-cli  reports --report_type kube_bench --report_location /var/tmp
+aquasec-cli  reports --report_type kube_bench --report_location /var/tmp --report_format list
 Report completed Saving
 Report written out to /var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
 ```
 
 __Delete API Auth:__
 
 ```bash
 >>> aquasec-cli delete                                              
 Are you sure you want to delete the auth api token? [y/N]: y
 Deleted Auth
 ```
 
 ## Release Info
 
+### v0.0.6
+
+* Added error handling
+* Added ability to generate different reports
+* Updated requirements to new aquasec-api
+
 ### v0.0.5
 
 * Updated Readme and changed type from RST to MD
 * Reverted snyk workflow file
 
 ### v0.0.4
 
@@ -772,14 +822,16 @@
 | __0.0.3__ | __a3__ | migrating to toml and setup.cfg |
 | __0.0.3__ | __a4__ | cleaned up utils and updated snyk to confirm pass locally; added to git ignore |
 | __0.0.3__ | __a5__ | setup.cfg issues wiht pip |
 | __0.0.3__ | __final__ | found issue with toml and other dependencies |
 | __0.0.4__ | __final__ | fixed issue with aquaapi dependency |
 | __0.0.5__ | __a1__ | fixed readme to point to md file; adjusting snyk |
 | __0.0.5__ | __final__ | tested and released |
+| __0.0.6__ | __a1__ | removed README.rst updated snyk |
+| __0.0.6__ | __a2__ | make delete more efficent added adjustments to report |
 
 ### Warnings
 
 Use at your own risk!!!
 
 # Security Policy
```

### Comparing `aquasec-cli-0.0.5/README.rst` & `aquasec-cli-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.5/aquasec_cli/commands/report.py` & `aquasec-cli-0.0.6/aquasec_cli/commands/report.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 import sys
 import json
 import pickle
 import datetime
 from pathlib import Path
 
 from aquasec.api import API
+from aquasec.orchestration.bench_report import BenchReport
+
 import click
 
-from aquasec_cli.utils import get_tmpdir
+from aquasec_cli.utils import get_tmpdir, reformat_exception
 
 
 @click.command()
 @click.option("--report_type", "-r", default="all", type=click.Choice(['cis', 'kube_bench', 'linux', 'openshift', 'disa_stig', 'all'], case_sensitive=True), help="Report type to genorate")
 @click.option("--cluster_name", "-c", required=False, type=str, help="Supply Cluster name")
 @click.option("--report_location", "-l", required=True, type=str, help="Directory to write out report to; please ensure proper formatting given the system you are on")
-def reports(report_type, cluster_name, report_location):
+@click.option("--report_format", required=False, default="list",type=click.Choice(['list', 'flat_list', 'raw'], case_sensitive=True), help="Report Format")
+def reports(report_type, cluster_name, report_location, report_format):
     """Generate CIS Bench Reports
 
-    Args:
-        report_type (_type_): _description_
-        cluster_name (_type_): _description_
-        report_location (_type_): _description_
+    Used to generate CIS Bench Reports in different formats
     """
     # check on report directory
     if not Path.is_dir(Path(report_location)):
         click.secho(
             "Report Directory does not exist unable to run report", color="red")
         sys.exit()
     #  pull credentials
-    tmpdir = get_tmpdir()
-    pkl_filename = Path.joinpath(tmpdir, 'aqua_api.pkl')
-    with open(pkl_filename, 'rb') as f:
-        pkl_file = pickle.load(f)
-    api: API = API(workload_auth=pkl_file)
-    arguments = {
-        "report_type": report_type,
-    }
-    if cluster_name:
-        arguments['cluster_name'] = cluster_name
-    report = api.get.bench_reports(**arguments)
-    click.secho("Report completed Saving", color='green')
-    filename = Path.joinpath(Path(
-        report_location),
-        f"aquasec_report_type_{report_type}_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.json")
-    with open(filename, 'w', encoding='utf-8') as f:
-        json.dump(report, f, indent=2)
-    click.secho(f"Report written out to {filename}", color='green')
+    try:
+        tmpdir = get_tmpdir()
+        pkl_filename = Path.joinpath(tmpdir, 'aqua_api.pkl')
+        with open(pkl_filename, 'rb') as f:
+            pkl_file = pickle.load(f)
+        api: API = API(workload_auth=pkl_file)
+        bench = BenchReport(api=api, report_type=report_type, report_format=report_format, cluster_name=cluster_name if cluster_name else "")
+        bench.run()
+        click.secho("Report completed Saving", color='green')
+        filename = Path.joinpath(Path(
+            report_location),
+            f"aquasec_report_type_{report_type}_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.json")
+        with open(filename, 'w', encoding='utf-8') as f:
+            json.dump(bench.bench_report, f, indent=2)
+        click.secho(f"Report written out to {filename}", color='green')
+    except Exception as err:
+        error = reformat_exception(err)
+        click.secho(f"Error: {error}")
```

### Comparing `aquasec-cli-0.0.5/aquasec_cli.egg-info/PKG-INFO` & `aquasec-cli-0.0.6/aquasec_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -711,42 +711,92 @@
 
 Commands:
   delete   Deletes created API Auth
   init     Initializes API Auth
   reports  Generate CIS Bench Reports
 ```
 
+```bash
+>>> aquasec-cli init --help   
+Usage: aquasec-cli init [OPTIONS]
+
+  Initializes API Authentication token used to run commands; required to
+  generate before a command can be executed
+
+Options:
+  --csp_roles TEXT  Creates Aquasec auth token
+  --endpoints TEXT  Endpoint Call Allowed
+  --help            Show this message and exit.
+```
+
+```bash
+>>> aquasec-cli reports --help
+Usage: aquasec-cli reports [OPTIONS]
+
+  Generate CIS Bench Reports
+
+  Used to generate CIS Bench Reports in different formats
+
+Options:
+  -r, --report_type [cis|kube_bench|linux|openshift|disa_stig|all]
+                                  Report type to genorate
+  -c, --cluster_name TEXT         Supply Cluster name
+  -l, --report_location TEXT      Directory to write out report to; please
+                                  ensure proper formatting given the system
+                                  you are on  [required]
+  --report_format [list|flat_list|raw]
+                                  Report Format
+  --help                          Show this message and exit.
+```
+
+```bash
+>>> aquasec-cli delete --help
+Usage: aquasec-cli delete [OPTIONS]
+
+  Deletes created API Auth
+
+Options:
+  --yes
+  --help  Show this message and exit.
+```
+
 __NOTE:__ Each subcommand has a help menu to assist with the calls being made. This project relies on the yaml or localized configurations being help as they are not passed in the commands as of this release.
 
 __Create API Auth Token:__
 
 ```bash
 >>> aquasec-cli init --csp_roles="Auditor" --csp_roles="Admin" --endpoints="Any"
 Initializing API
 INFO    : Created WorkloadAuth Token for URL https://1234abcff1.cloud.aquasec.com
 ```
 
 __Run Report:__
 
 ```bash
-aquasec-cli  reports --report_type kube_bench --report_location /var/tmp
+aquasec-cli  reports --report_type kube_bench --report_location /var/tmp --report_format list
 Report completed Saving
 Report written out to /var/tmp/aquasec_report_type_kube_bench_20230424T153825.json
 ```
 
 __Delete API Auth:__
 
 ```bash
 >>> aquasec-cli delete                                              
 Are you sure you want to delete the auth api token? [y/N]: y
 Deleted Auth
 ```
 
 ## Release Info
 
+### v0.0.6
+
+* Added error handling
+* Added ability to generate different reports
+* Updated requirements to new aquasec-api
+
 ### v0.0.5
 
 * Updated Readme and changed type from RST to MD
 * Reverted snyk workflow file
 
 ### v0.0.4
 
@@ -772,14 +822,16 @@
 | __0.0.3__ | __a3__ | migrating to toml and setup.cfg |
 | __0.0.3__ | __a4__ | cleaned up utils and updated snyk to confirm pass locally; added to git ignore |
 | __0.0.3__ | __a5__ | setup.cfg issues wiht pip |
 | __0.0.3__ | __final__ | found issue with toml and other dependencies |
 | __0.0.4__ | __final__ | fixed issue with aquaapi dependency |
 | __0.0.5__ | __a1__ | fixed readme to point to md file; adjusting snyk |
 | __0.0.5__ | __final__ | tested and released |
+| __0.0.6__ | __a1__ | removed README.rst updated snyk |
+| __0.0.6__ | __a2__ | make delete more efficent added adjustments to report |
 
 ### Warnings
 
 Use at your own risk!!!
 
 # Security Policy
```

### Comparing `aquasec-cli-0.0.5/aquasec_cli.egg-info/SOURCES.txt` & `aquasec-cli-0.0.6/aquasec_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.5/pyproject.toml` & `aquasec-cli-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requires-python = ">=3.8"
 keywords = ['aquasec', 'aqua security', 'workload protection']
 license = {file = "LICENSE", content-type = "text"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "aquasec-api==0.0.2",
+    "aquasec-api==0.0.4",
     "click>=8.1.3",
     "dataclasses>=0.6",
     "PyYAML>=6.0",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version", "readme", "entry-points"]
```

### Comparing `aquasec-cli-0.0.5/setup.cfg` & `aquasec-cli-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license_files = LICENSE
 
 [options]
 python_requires = >3.8, <4
 include_package_data = True
 packages = find:
 install_requires = 
-	aquasec-api == 0.0.2
+	aquasec-api == 0.0.4
 	click >= 8.1.3
 	dataclasses >= 0.6
 	PyYAML >= 6.0
 zip_safe = True
 
 [options.packages.find]
 include = aquasec_cli*
```

