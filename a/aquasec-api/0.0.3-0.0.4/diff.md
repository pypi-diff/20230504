# Comparing `tmp/aquasec-api-0.0.3.tar.gz` & `tmp/aquasec-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquasec-api-0.0.3.tar", last modified: Tue Apr 25 18:40:28 2023, max compression
+gzip compressed data, was "aquasec-api-0.0.4.tar", last modified: Thu May  4 18:10:05 2023, max compression
```

## Comparing `aquasec-api-0.0.3.tar` & `aquasec-api-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.270132 aquasec-api-0.0.3/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/LICENSE
--rw-rw-r--   0 adamt      (501) staff       (20)       78 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/MANIFEST.in
--rw-r--r--   0 adamt      (501) staff       (20)    10017 2023-04-25 18:40:28.269550 aquasec-api-0.0.3/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     9635 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.266155 aquasec-api-0.0.3/aquasec/
--rw-rw-r--   0 adamt      (501) staff       (20)     4281 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       37 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     4157 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6621 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1202 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/configs.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1694 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/delete.py
--rw-rw-r--   0 adamt      (501) staff       (20)      447 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7431 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/get.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3708 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/logging.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.266807 aquasec-api-0.0.3/aquasec/orchestration/
--rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/orchestration/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3723 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/orchestration/bench_report.py
--rw-rw-r--   0 adamt      (501) staff       (20)     2128 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/post.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1163 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/put.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7764 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      200 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/statics.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1713 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/structures.py
--rw-rw-r--   0 adamt      (501) staff       (20)     2400 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/aquasec/utilities.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:40:28.268845 aquasec-api-0.0.3/aquasec_api.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    10017 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      592 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       84 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)        8 2023-04-25 18:40:28.000000 aquasec-api-0.0.3/aquasec_api.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)       84 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/requirements.txt
--rw-rw-r--   0 adamt      (501) staff       (20)      125 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/sample.yaml
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-04-25 18:40:28.270296 aquasec-api-0.0.3/setup.cfg
--rw-rw-r--   0 adamt      (501) staff       (20)     1122 2023-04-25 18:38:14.000000 aquasec-api-0.0.3/setup.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:10:05.378442 aquasec-api-0.0.4/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/LICENSE
+-rw-rw-r--   0 adamt      (501) staff       (20)       99 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/MANIFEST.in
+-rw-r--r--   0 adamt      (501) staff       (20)    52198 2023-05-04 18:10:05.378939 aquasec-api-0.0.4/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)    10621 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/README.md
+-rw-rw-r--   0 adamt      (501) staff       (20)      538 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/SECURITY.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:10:05.374135 aquasec-api-0.0.4/aquasec/
+-rw-rw-r--   0 adamt      (501) staff       (20)     4322 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       37 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     4157 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6621 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1202 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/configs.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1694 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/delete.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      447 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7517 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/get.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     3708 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/logging.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:10:05.375042 aquasec-api-0.0.4/aquasec/orchestration/
+-rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/orchestration/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    12881 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/orchestration/bench_report.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     2128 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/post.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1163 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/put.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6710 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      200 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/statics.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1713 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/structures.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     2400 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/aquasec/utilities.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-05-04 18:10:05.377912 aquasec-api-0.0.4/aquasec_api.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    52198 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      659 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)      130 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        8 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/top_level.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-05-04 18:10:05.000000 aquasec-api-0.0.4/aquasec_api.egg-info/zip-safe
+-rw-rw-r--   0 adamt      (501) staff       (20)     1000 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       84 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/requirements.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)      125 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/sample.yaml
+-rw-rw-r--   0 adamt      (501) staff       (20)      736 2023-05-04 18:10:05.380241 aquasec-api-0.0.4/setup.cfg
+-rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-05-04 18:08:51.000000 aquasec-api-0.0.4/setup.py
```

### Comparing `aquasec-api-0.0.3/LICENSE` & `aquasec-api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/PKG-INFO` & `aquasec-api-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: aquasec-api
-Version: 0.0.3
-Summary: Aqua Security SDK to pull data from Aquasec Tenant and CSPM for auditing
-Home-page: https://github.com/atav928/aquasec-api
-Author: atav928
-Author-email: dev@tavnets.com
-Maintainer-email: dev@tavnets.com
-Keywords: aquasec,aqua security,workload protection
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # aquasec-api
 
 Aqua Sec Cloud Secuirty API Tool used for interacting with Aqua Security CSPM Enterprise and Workload.
 
 ## Documents
 
 * [CSPM API Docs](https://cloudsploit.docs.apiary.io/#)
@@ -206,16 +194,48 @@
     >>> all_linux_report = api.get.bench_reports(report_type='linux')
     # disa_stig Report
     >>> disa_stig_report = api.get.bench_reports(report_type='disa_stig')
     # Full CIS Benchmark Report on all Hosts
     >>> full_cis_report = api.get.bench_reports(report_type='all')
     ```
 
+    __NOTE:__ The report published here is a standard collecion of host key values with the raw report generated as the output. See Orchestration for adjusted reports.
+
+### Orchestration
+
+Building customized CIS Bench Reports
+
+```python
+"""Sample Bench Report"""
+
+import json
+
+from aquasec.orchestration.bench_report import BenchReport
+from aquasec.api import API
+
+# create api token
+api = API(api_key="7d6c02219a99", api_secret="0b3b928a1acd4c2580583cc160f49f5e",api_csp_roles=["CSP_USER"],allowed_endpoints=["ANY"])
+
+# create and run report Bench Object
+bench = BenchReport(api=api, report_type='all')
+bench.run()
+
+# write out report
+with open('/var/tmp/bench_report_20230501.json','w', encoding='utf-8') as f:
+    json.dump(bench.bench_report, f)
+
+```
+
 ## Release Info
 
+### v0.0.4
+
+* Added Orchestration and adjustment of bench report
+* bug with full flat_list need to build that
+
 ### v0.0.3
 
 * Added ability to POST
 * Adding PUT
 * Additional Datastructures
 * Additional Delete Functionality
 * Introducing Orchestration on Actions
@@ -254,9 +274,11 @@
 | __0.0.1__ | __rc8__ | final release that solves how the auth works for CSPM and Workload Protection |
 | __0.0.2__ | __a1__ | Updated readme testing some additional modeling and possible integration scripts |
 | __0.0.2__ | __a2__ | Added ability to retrieve all functions leveraging paging |
 | __0.0.2__ | __a3__ | Added CIS benchmark reports, Fix bug with infinate get_all |
 | __0.0.2__ | __rc1__ | Bug with providing direct api information into api function with WorkloadAuth |
 | __0.0.2__ | __final__ | completed orchestration of bench report and standard get workload checks |
 | __0.0.3__ | __a1__ | Intro to POST, PUT, DELETE and adding some datastructures for creating and manipluating AquaSec |
+| __0.0.4__ | __a1__ | updates to report structure |
+| __0.0.4__ | __a2__ | updates to some docstring in BenchReport |
 
 __NOTE:__ Use at your own risk!!!! API as is and building on it.
```

### Comparing `aquasec-api-0.0.3/aquasec/__init__.py` & `aquasec-api-0.0.4/aquasec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import yaml
 
 from aquasec.auth import WorkloadAuth
 from aquasec.configs import Config
 from aquasec.logging import RotatingLog
 
+from aquasec._version import __version__
 
 config = Config()
 home = expanduser("~")
 filename = f"{home}/.config/.aquaconf"
 # Prefer Yaml configs over OS ENV Settings
 if exists(filename):
     with open(filename, 'r', encoding='utf-8') as yam:
```

### Comparing `aquasec-api-0.0.3/aquasec/api.py` & `aquasec-api-0.0.4/aquasec/api.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/auth.py` & `aquasec-api-0.0.4/aquasec/auth.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/configs.py` & `aquasec-api-0.0.4/aquasec/configs.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/delete.py` & `aquasec-api-0.0.4/aquasec/delete.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/get.py` & `aquasec-api-0.0.4/aquasec/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pylint: disable=line-too-long
 """Get Method"""
 
 from aquasec import config, logger
 
-from aquasec.auth import (refresh_workload_token, WorkloadAuth)
 from aquasec.statics import BENCH_REPORTS
-from aquasec.requestapi import (aqua_cloudsploit_request, aqua_workload_request, retrieve_full_list)
+from aquasec.requestapi import (
+    aqua_cloudsploit_request, aqua_workload_request, retrieve_full_list)
 from aquasec.utilities import (reformat_exception, UrlUtils)
-from aquasec.exceptions import (AquaSecWrongParam, AquaSecAPIError)
+from aquasec.exceptions import (AquaSecWrongParam)
 
 logger.addLogger(__name__)
 aquasec_logger = logger.getLogger(__name__)
 if not config.SET_LOG:
     aquasec_logger.disabled = True
 
 
@@ -30,20 +30,22 @@
             url_path (str, required): The URL resource path. Ex "alerts"
             params (dict, optional): RestAPI parameters
             api_version (str, optional): Defaults to configured version
 
         Returns:
             dict: JSON results
         """
-        api_version: str = kwargs.pop("api_verison", self._parent_class.api_version)  # type: ignore
+        api_version: str = kwargs.pop(
+            "api_verison", self._parent_class.api_version)  # type: ignore
         url = self._parent_class.cloudsploit_url.format(  # type:ignore
             api_version,
             url_path)
         aquasec_logger.info("Created URL=%s", url)
-        response = aqua_cloudsploit_request(url=url, method=self.method, **kwargs)
+        response = aqua_cloudsploit_request(
+            url=url, method=self.method, **kwargs)
         aquasec_logger.debug("Response=%s", response)
         return response
 
     def workload_protection(self, url_path: str, **kwargs):
         """Workload Protection Requests, see README.md for some assistance here.
             this is difficult to get as there is no documentation and most is pulled
             from the cloud portal. But there are some examples to help on readme.
@@ -91,20 +93,23 @@
 
 
         Returns:
             dict: _description_
         """
         report_type = report_type.lower()
         if report_type not in BENCH_REPORTS:
-            aquasec_logger.error("AquaSecWrongParam: Invalid report_type value %s", report_type)
-            raise AquaSecWrongParam(f"Invalid report_type value: {report_type=}")
+            aquasec_logger.error(
+                "AquaSecWrongParam: Invalid report_type value %s", report_type)
+            raise AquaSecWrongParam(
+                f"Invalid report_type value: {report_type=}")
         cluster_name: str = kwargs.pop('cluster_name', "")
         hosts: list = self._get_hosts_id_list(cluster_name=cluster_name)
         # TODO: Paralize
-        bench_report: dict = self._get_bench_report(host_id_list=hosts, report_type=report_type)
+        bench_report: dict = self._get_bench_report(
+            host_id_list=hosts, report_type=report_type)
         return bench_report
 
     def _get_hosts_id_list(self, cluster_name: str) -> list:
         """Gets all hosts by ID
 
         Args:
             cluster_name (str, optional): _description_. Defaults to "".
@@ -119,15 +124,16 @@
             get_all=True)
         try:
             all_hosts: list = response['result']
         except KeyError as err:
             error = reformat_exception(err)
             aquasec_logger.error("AquaSecAPIError: %s", error)
         if cluster_name:
-            aquasec_logger.info("Searching for hosts that belong to cluster_name=%s", cluster_name)
+            aquasec_logger.info(
+                "Searching for hosts that belong to cluster_name=%s", cluster_name)
         for _ in all_hosts:
             if cluster_name and _['cluster_name'] == cluster_name:
                 host_id_list.append(_['id'])
             else:
                 host_id_list.append(_['id'])
         return host_id_list
 
@@ -140,33 +146,37 @@
 
         Returns:
             dict: _description_
         """
         bench_report: dict = {}
         for _ in host_id_list:
             bench_report[_] = self.workload_protection(
-                url_path=config.WORKLOAD_URL_PATHS['host_bench_report']['path'].format(_),
+                url_path=config.WORKLOAD_URL_PATHS['host_bench_report']['path'].format(
+                    _),
                 api_version=config.WORKLOAD_URL_PATHS['host_bench_report']['version'])
-        if report_type in ['all', 'full']:
+        if report_type.lower() in ['all', 'full']:
             aquasec_logger.info("Retrieved full bench report")
             return bench_report
         # Gets specific report
         specific_bench_report: dict = {identifier: {report_type: {}}
                                        for identifier in bench_report}
         for _ in list(bench_report):
-            specific_bench_report[_][f"{report_type}"] = bench_report[_].get(report_type, {})
-        aquasec_logger.info("Retrieved %s_report for specified hosts", report_type)
+            specific_bench_report[_][f"{report_type}"] = bench_report[_].get(
+                report_type, {})
+        aquasec_logger.info(
+            "Retrieved %s_report for specified hosts", report_type)
         return specific_bench_report
 
     def _endpoint(self, url_path: str, **kwargs) -> str:
         """Creates endpoint for Cloudsploit
 
         Args:
             endpoint (str): _description_
 
         Returns:
             str: _description_
         """
         api_version: str = kwargs.pop(
             'api_version', self._parent_class.api_version)  # type: ignore # type :ignore
-        url = self._parent_class.cloudsploit_url.format(api_version, url_path)  # type: ignore
+        url = self._parent_class.cloudsploit_url.format(
+            api_version, url_path)  # type: ignore
         return url
```

### Comparing `aquasec-api-0.0.3/aquasec/logging.py` & `aquasec-api-0.0.4/aquasec/logging.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/post.py` & `aquasec-api-0.0.4/aquasec/post.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/put.py` & `aquasec-api-0.0.4/aquasec/put.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/requestapi.py` & `aquasec-api-0.0.4/aquasec/requestapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import json
 from typing import Any, Dict
 import requests
 from requests import Response
 
 from aquasec import config, logger, create_cspm_headers
 from aquasec.auth import WorkloadAuth, refresh_workload_token
-from aquasec.exceptions import (AquaSecAPIError, AquaSecMissingParam, AquaSecPermission)
+from aquasec.exceptions import (
+    AquaSecAPIError, AquaSecMissingParam, AquaSecPermission)
 from aquasec.utilities import reformat_exception
 
 logger.addLogger(__name__)
 aquasec_logger = logger.getLogger(__name__)
 if not config.SET_LOG:
     aquasec_logger.disabled = True
 
@@ -56,15 +57,16 @@
                                 params=params,
                                 verify=verify,
                                 timeout=timeout)
     aquasec_logger.debug("Response Code=%s|Full Response=%s",
                          str(response.status_code), response.text.rstrip())
     api_raise_error(response=response)
     if response.status_code == 204:
-        json_response = {"message": "Data Created", "code": response.status_code}
+        json_response = {"message": "Data Created",
+                         "code": response.status_code}
     else:
         json_response = response.json()
     return json_response
 
 
 def retrieve_full_list(workload_auth: WorkloadAuth, **kwargs):
     """Retrieves fulll list of requirements based on multiple calls
@@ -165,28 +167,7 @@
         message = response.json().get("message", "Permission Denied")
         aquasec_logger.error("AquaSecPermission: %s", message)
         raise AquaSecPermission(message)
     if not (response.status_code >= 200 and response.status_code < 299):
         aquasec_logger.error("Status Code: %s| Error: %s", str(
             response.status_code), response.json())
         raise AquaSecAPIError(response.json())
-
-
-Traceback (most recent call last):
-  File "/.env/lib/python3.8/site-packages/requests/models.py", line 971, in json
-    return complexjson.loads(self.text, **kwargs)
-  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/__init__.py", line 357, in loads
-    return _default_decoder.decode(s)
-  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/decoder.py", line 337, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/Users/adamt/.pyenv/versions/3.8.15/lib/python3.8/json/decoder.py", line 355, in raw_decode
-    raise JSONDecodeError("Expecting value", s, err.value) from None
-json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
-
-During handling of the above exception, another exception occurred:
-
-Traceback (most recent call last):
-  File "test_call.py", line 41, in <module>
-    print(response.json())
-  File "/.env/lib/python3.8/site-packages/requests/models.py", line 975, in json
-    raise RequestsJSONDecodeError(e.msg, e.doc, e.pos)
-requests.exceptions.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
```

### Comparing `aquasec-api-0.0.3/aquasec/structures.py` & `aquasec-api-0.0.4/aquasec/structures.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec/utilities.py` & `aquasec-api-0.0.4/aquasec/utilities.py`

 * *Files identical despite different names*

### Comparing `aquasec-api-0.0.3/aquasec_api.egg-info/SOURCES.txt` & `aquasec-api-0.0.4/aquasec_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
+SECURITY.md
+pyproject.toml
 requirements.txt
 sample.yaml
+setup.cfg
 setup.py
 aquasec/__init__.py
 aquasec/_version.py
 aquasec/api.py
 aquasec/auth.py
 aquasec/configs.py
 aquasec/delete.py
@@ -21,8 +24,9 @@
 aquasec/utilities.py
 aquasec/orchestration/__init__.py
 aquasec/orchestration/bench_report.py
 aquasec_api.egg-info/PKG-INFO
 aquasec_api.egg-info/SOURCES.txt
 aquasec_api.egg-info/dependency_links.txt
 aquasec_api.egg-info/requires.txt
-aquasec_api.egg-info/top_level.txt
+aquasec_api.egg-info/top_level.txt
+aquasec_api.egg-info/zip-safe
```

