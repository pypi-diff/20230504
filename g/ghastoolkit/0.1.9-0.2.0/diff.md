# Comparing `tmp/ghastoolkit-0.1.9.tar.gz` & `tmp/ghastoolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.9.tar", last modified: Thu Apr 27 14:00:31 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.0.tar", last modified: Thu May  4 12:12:15 2023, max compression
```

## Comparing `ghastoolkit-0.1.9.tar` & `ghastoolkit-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.565283 ghastoolkit-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.1.9/LICENSE` & `ghastoolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.9/PKG-INFO` & `ghastoolkit-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.9
+Version: 0.2.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.9/README.md` & `ghastoolkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.9/pyproject.toml` & `ghastoolkit-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.0/src/ghastoolkit/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import logging
 import argparse
 
-from ghastoolkit import __name__ as name
+from ghastoolkit import __name__ as name, __banner__
 from ghastoolkit.octokit.github import GitHub
 from ghastoolkit.octokit.codescanning import CodeScanning
 from ghastoolkit.octokit.dependencygraph import (
     DependencyGraph,
 )
 
 # Arguments
@@ -52,14 +52,16 @@
 
 # logger
 logging.basicConfig(
     level=logging.DEBUG if arguments.debug or os.environ.get("DEBUG") else logging.INFO,
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 )
 
+print(__banner__)
+
 # GitHub Init
 GitHub.init(
     repository=arguments.github_repository,
     instance=arguments.github_instance,
     token=arguments.github_token,
 )
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.0/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.0/src/ghastoolkit/octokit/codescanning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,60 @@
+from dataclasses import dataclass
 import json
 import logging
 from typing import Any, Optional
 from ghastoolkit.octokit.github import GitHub, Repository
-from ghastoolkit.octokit.octokit import RestRequest
+from ghastoolkit.octokit.octokit import OctoItem, RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
+@dataclass
+class CodeAlert(OctoItem):
+    number: int
+    state: str
+
+    created_at: str
+
+    rule: dict
+    tool: dict
+
+    _instances: Optional[list[dict]] = None
+
+    @property
+    def rule_id(self):
+        return self.rule.get("id")
+
+    @property
+    def description(self):
+        return self.rule.get("description")
+
+    @property
+    def tool_name(self):
+        return self.tool.get("name")
+
+    @property
+    def tool_fullname(self):
+        version = self.tool.get("version")
+        return f"{self.tool_name}@{version}"
+
+    @property
+    def severity(self):
+        return self.rule.get("severity")
+
+    @property
+    def instances(self) -> list[dict]:
+        if not self._instances:
+            self._instances = CodeScanning().getAlertInstances(self.number)
+        return self._instances
+
+    def __str__(self) -> str:
+        return f"CodeAlert({self.number}, '{self.state}', '{self.tool_name}', '{self.rule_id}')"
+
+
 class CodeScanning:
     def __init__(self, repository: Optional[Repository] = None) -> None:
         """GitHub Code Scanning REST API
 
         https://docs.github.com/en/rest/code-scanning
         """
         self.repository = repository or GitHub.repository
@@ -34,48 +78,54 @@
         "/repos/{owner}/{repo}/code-scanning/alerts", authenticated=True
     )
     def getAlerts(
         self,
         state: str = "open",
         tool_name: Optional[str] = None,
         ref: Optional[str] = None,
-    ) -> list[dict]:
-        """Get a code scanning alert
+    ) -> list[CodeAlert]:
+        """Get all code scanning alerts
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-a-repository
         """
         return []
 
     def getAlertsInPR(self, base: str) -> list[dict]:
-        """Get Alerts in Pull Request (diff)
+        """Get the open alerts in a Pull Request (delta / diff).
+
+        Note this operation is slow due to it needing to lookup each alert instance
+        information.
 
         base: str - Base reference
         https://docs.github.com/en/rest/code-scanning#list-instances-of-a-code-scanning-alert
         """
         if not self.repository.reference or not self.repository.isInPullRequest():
             return []
+
         results = []
         alerts = self.getAlerts("open", ref=self.repository.reference)
-        print(f" $ {self.repository.reference} == {len(alerts)}")
+
         for alert in alerts:
-            alert_info = self.getAlertInstances(alert.get("number", 0), ref=base)
-            print(f" >> {alert.get('number')} -> {len(alert_info)}")
+            number = alert.get("number")
+            alert_info = self.getAlertInstances(number, ref=base)
             if len(alert_info) == 0:
-                results.append(alert_info)
+                results.append(alert)
         return results
 
     @RestRequest.restGet(
         "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}", authenticated=True
     )
     def getAlert(self, alert_number: int) -> dict:
         """Get Single Alert
         https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
         """
         return {}
 
-    def getAlertInstances(self, alert_number: int, ref: Optional[str] = None) -> dict:
+    def getAlertInstances(
+        self, alert_number: int, ref: Optional[str] = None
+    ) -> list[dict]:
         result = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}/instances",
             {"alert_number": alert_number, "ref": ref},
         )
         return result
 
     def getAnalyses(
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,86 @@
-import fnmatch
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 import re
-from ghastoolkit.octokit.github import GitHub, Repository
+from typing import Optional
 
-from ghastoolkit.octokit.octokit import GraphQLRequest, Optional, RestRequest
+from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 
-logger = logging.getLogger("ghastoolkit.octokit.dependencygraph")
+logger = logging.getLogger("ghastoolkit.supplychain.dependencies")
 
 
 @dataclass
 class Dependency:
     name: str
     namespace: Optional[str] = None
     version: Optional[str] = None
     manager: Optional[str] = None
     path: Optional[str] = None
-    qualifiers: dict[str, str] = field(default_factory=list)
+    qualifiers: dict[str, str] = field(default_factory=dict)
 
+    # Licensing information
     licence: Optional[str] = None
+    # Security Alerts
+    alerts: list[DependencyAlert] = field(default_factory=list)
 
-    def getPurl(self) -> str:
+    def getPurl(self, version: bool = True) -> str:
         """Get PURL
         https://github.com/package-url/purl-spec
         """
         result = f"pkg:"
         if self.manager:
-            result += f"{self.manager}/"
+            result += f"{self.manager.lower()}/"
         if self.namespace:
             result += f"{self.namespace}/"
         result += f"{self.name}"
-        if self.version:
+        if version and self.version:
             result += f"@{self.version}"
 
         return result
 
     @staticmethod
     def fromPurl(purl: str) -> "Dependency":
         dep = Dependency("")
-        pkg, dep.version = purl.split("@", 1)
+        # version (at end)
+        if "@" in purl:
+            pkg, dep.version = purl.split("@", 1)
+        else:
+            pkg = purl
 
-        if pkg.count("/") == 2:
+        slashes = pkg.count("/")
+        if slashes == 0 and pkg.count(":", 1):
+            # basic purl `npm:name`
+            manager, dep.name = pkg.split(":", 1)
+        elif slashes == 2:
             manager, dep.namespace, dep.name = pkg.split("/", 3)
-        elif pkg.count("/") == 1:
+        elif slashes == 1:
             manager, dep.name = pkg.split("/", 2)
-        elif pkg.count("/") > 2:
+        elif slashes > 2:
             manager, dep.namespace, dep.name = pkg.split("/", 2)
         else:
             raise Exception(f"Unable to parse PURL :: {purl}")
 
-        _, dep.manager = manager.split(":", 1)
+        if manager.startswith("pkg:"):
+            _, dep.manager = manager.split(":", 1)
+        else:
+            dep.manager = manager
 
         return dep
 
+    @property
+    def fullname(self) -> str:
+        """Full Name of the Dependency"""
+        if self.namespace:
+            sep = "/"
+            if self.manager == "maven":
+                sep = ":"
+            return f"{self.namespace}{sep}{self.name}"
+        return self.name
+
     def __str__(self) -> str:
         return self.getPurl()
 
     def __repr__(self) -> str:
         return self.getPurl()
 
 
@@ -104,71 +127,41 @@
             [
                 dep
                 for dep in self
                 if any(regex.search(dep.licence or "NA") for regex in regex_list)
             ]
         )
 
+    def findUnknownLicenses(
+        self, licenses: Optional[list[str]] = None
+    ) -> "Dependencies":
+        licenses = licenses or ["NA", "NOASSERTION"]
+        return self.findLicenses(licenses)
+
+    def contains(self, dependency: Dependency) -> bool:
+        purl = dependency.getPurl(version=False)
+        for dep in self:
+            if dep.name == dependency.name or dep.getPurl(version=False) == purl:
+                return True
+        return False
+
+    def find(self, name: str) -> Optional[Dependency]:
+        """Find by name"""
+        for dep in self:
+            if dep.name == name or dep.fullname == name:
+                return dep
+        logger.debug(f"Unable to find by name :: {name}")
+
+    def findPurl(self, purl: str) -> Optional[Dependency]:
+        """Find by PURL"""
+        purldep = Dependency.fromPurl(purl)
+        for dep in self:
+            if purldep.name == purldep.fullname or dep.fullname == dep.fullname:
+                return dep
+        logger.debug(f"Unable to find by PURL :: {purl}")
+
     def findNames(self, names: list[str]) -> "Dependencies":
         """Find by Name using wildcards"""
         regex_list = [re.compile(name_filter) for name_filter in names]
         return Dependencies(
             [dep for dep in self if any(regex.search(dep.name) for regex in regex_list)]
         )
-
-
-class DependencyGraph:
-    def __init__(self, repository: Optional[Repository] = None) -> None:
-        self.repository = repository or GitHub.repository
-        self.rest = RestRequest(repository)
-        self.graphql = GraphQLRequest(repository)
-
-    def getDependencies(self) -> Dependencies:
-        """Get Dependencies from SBOM"""
-        result = Dependencies()
-        spdx_bom = self.exportBOM()
-
-        for package in spdx_bom.get("sbom", {}).get("packages", []):
-            extref = False
-            dep = Dependency("")
-            for ref in package.get("externalRefs", []):
-                if ref.get("referenceType"):
-                    dep = Dependency.fromPurl(ref.get("referenceLocator"))
-                    extref = True
-
-            if extref:
-                dep.licence = package.get("licenseConcluded")
-            else:
-                manager, name = package.get("name", "").split(":")
-                dep = Dependency(
-                    name,
-                    version=package.get("versionInfo"),
-                    manager=manager,
-                    licence=package.get("licenseConcluded"),
-                )
-
-            result.append(dep)
-
-        return result
-
-    def exportBOM(self) -> Dependencies:
-        """Download / Export DependencyGraph SBOM"""
-        return self.rest.get("/repos/{owner}/{repo}/dependency-graph/sbom")
-
-    def submitDependencies(
-        self,
-        dependencies: Dependencies,
-        tool: str,
-        path: str,
-        sha: str = "",
-        ref: str = "",
-        version: str = "0.0.0",
-        url: str = "",
-    ):
-        """
-        https://docs.github.com/en/rest/dependency-graph/dependency-submission?apiVersion=2022-11-28#create-a-snapshot-of-dependencies-for-a-repository
-        """
-        self.rest.postJson(
-            "/repos/{owner}/{repo}/dependency-graph/snapshots",
-            dependencies.exportBOM(tool, path, sha, ref, version, url),
-            expected=201,
-        )
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.0/src/ghastoolkit/octokit/octokit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import json
 import os
 import inspect
 import logging
-from os.path import isdir
 from string import Template
 from typing import Any, Optional, Union
+from dataclasses import field, is_dataclass
 
 from requests import Session
-from requests.models import Response
 from ratelimit import limits, sleep_and_retry
 
 from ghastoolkit.octokit.github import GitHub, Repository
 
 
 # Assume REST requests are being done by a GitHub Token, not
 # a GitHub App which has a higher limit
+# https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=2022-11-28#rate-limiting
 REST_MAX_CALLS = 80  # ~5000 per hour
 
 __OCTOKIT_PATH__ = os.path.dirname(os.path.realpath(__file__))
 
 __OCTOKIT_ERRORS__ = {401: "Authentication Issue"}
 
 
@@ -41,14 +40,47 @@
     def formatPath(path: str, repo: Repository, **options) -> str:
         formatted_path = path.format(
             owner=repo.owner, org=repo.owner, repo=repo.repo, **options
         )
         return formatted_path
 
 
+class OctoItem:
+    """OctoItem"""
+
+    __data__: dict = field(default_factory=dict)
+
+    def get(self, name: str, default: Any = None) -> Any:
+        try:
+            return self.__getattr__(name)
+        except:
+            return default
+
+    def __getattr__(self, name) -> Any:
+        """Get Attr"""
+        if hasattr(self, name):
+            return getattr(self, name)
+        elif self.__data__ and self.__data__.get(name):
+            return self.__data__.get(name)
+        raise Exception(f"Unknown key: {name}")
+
+
+def loadOctoItem(classtype, data: dict):
+    if not issubclass(classtype, OctoItem) and is_dataclass(classtype):
+        raise Exception(f"Class should be a OctoItem")
+
+    initdata = {}
+    for key, value in data.items():
+        if classtype.__annotations__.get(key):
+            initdata[key] = value
+    new = classtype(**initdata)
+    new.__data__ = data
+    return new
+
+
 class RestRequest:
     PER_PAGE = 100
     VERSION: str = "2022-11-28"
 
     def __init__(self, repository: Optional[Repository] = None) -> None:
         self.repository = repository or GitHub.repository
         self.session = Session()
@@ -68,14 +100,15 @@
                 # if the current class has a rest variable, use it
                 rest = getattr(self, "rest") if hasattr(self, "rest") else RestRequest()
 
                 params = {}
                 args_index = 0
                 response = False
                 func_info = inspect.getfullargspec(func)
+                return_type = func_info.annotations.get("return")
                 defaults = func_info.defaults or ()
 
                 # if len(func_info.args) - 1 != len(defaults):
                 #     raise Exception("restGet does not support non-default function variables (yet)")
 
                 for argv in func_info.args:
                     if argv == "self":
@@ -83,33 +116,51 @@
                     elif argv == "response":
                         response = True
 
                     argv_value = None
                     # if provided
                     if len(args) > args_index:
                         argv_value = args[args_index]
+                    elif kwargs.get(argv):
+                        argv_value = kwargs.get(argv)
 
-                    if not argv_value and len(defaults) < 0:
+                    elif not argv_value and len(defaults) < 0:
                         argv_value = defaults[len(defaults) - args_index]
 
                     params[argv] = argv_value
                     args_index += 1
 
-                result = rest.get(url, parameters=params)
+                result = rest.get(url, parameters=params, authenticated=authenticated)
 
                 if response:
                     return func(self, responce=result, **kwargs)
 
                 # TODO: runtime type checking
 
                 # return_type = func_info.annotations.get("return")
                 # if return_type and not type(result) is return_type.__origin__:
                 #     name = f"{self.__class__.__name__}.{func.__name__}()"
                 #     raise Exception(f"Unexpected type returned for `{name}`")
 
+                # return is a list
+                if return_type.__origin__ == Union:
+                    logger.debug(f"Ignoring Union type")
+                elif (
+                    return_type
+                    and isinstance(result, return_type.__origin__)
+                    and return_type.__origin__ == list
+                ):
+                    subtype = return_type.__args__[0]
+                    if issubclass(subtype, OctoItem):
+                        new_results = []
+                        for rslt in result:
+                            new_results.append(loadOctoItem(subtype, rslt))
+
+                        return new_results
+
                 return result
 
             return wrap
 
         return decorator
 
     @sleep_and_retry
@@ -132,15 +183,20 @@
         url = Octokit.route(path, repo, rtype="rest", **parameters)
         logger.debug(f"Fetching content from URL :: {url}")
 
         if authenticated and not self.session.headers.get("Authorization"):
             raise Exception(f"GitHub Token required for this request")
 
         result = []
-        params = parameters
+        params = {}
+        # if the parameter is in the path, ignore it
+        for key, param in parameters.items():
+            if "{" + key + "}" not in path:
+                params[key] = param
+
         params["per_page"] = RestRequest.PER_PAGE
 
         page = 1  # index starts at 1
 
         while True:
             params["page"] = page
 
@@ -194,28 +250,34 @@
 DEFAULT_GRAPHQL_PATHS = [os.path.join(__OCTOKIT_PATH__, "graphql")]
 
 
 class GraphQLRequest:
     def __init__(self, repository: Optional[Repository] = None) -> None:
         self.repository = repository or GitHub.repository
         self.session = Session()
+        self.cursor = ""
         # https://docs.github.com/en/rest/overview/authenticating-to-the-rest-api
         self.session.headers = {
             "Accept": "application/vnd.github.hawkgirl-preview+json",
             "Authorization": f"token {GitHub.token}",
         }
         self.queries = {}
 
         self.loadQueries(DEFAULT_GRAPHQL_PATHS)
 
-    def query(self, name: str, options: dict[str, Any]) -> dict:
+    def query(self, name: str, options: dict[str, Any] = {}) -> dict:
+        logger.debug(f"Loading Query by Name :: {name}")
         query_content = self.queries.get(name)
+
         if not query_content:
-            return {}
-        query = self.formatQuery(query_content, **options)
+            raise Exception(f"Failed to load GraphQL query :: {name}")
+
+        cursor = f'after: "{self.cursor}"' if self.cursor != "" else ""
+
+        query = self.formatQuery(query_content, cursor=cursor, **options)
 
         response = self.session.post(
             GitHub.api_graphql, json={"query": query}, timeout=30
         )
         if response.status_code != 200:
             logger.error(f"GraphQL API Status :: {response.status_code}")
             logger.error(f"GraphQL Content :: {response.content}")
@@ -226,15 +288,19 @@
             for err in rjson.get("errors"):
                 logger.warning(f"GraphQL Query failed :: {err.get('message')}")
 
         return rjson
 
     def loadQueries(self, paths: list[str]):
         for path in paths:
+            if not os.path.exists(path):
+                logger.debug(f"Query load path does not exist :: {path}")
+                continue
             if not os.path.isdir(path):
+                logger.debug(f"Query path is not a dir :: {path}")
                 continue
             for file in os.listdir(path):
                 root = os.path.join(path, file)
                 name, ext = os.path.splitext(file)
                 if ext not in [".graphql"]:
                     continue
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.0/src/ghastoolkit/octokit/secretscanning.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,51 @@
-from os import stat
+import logging
+from dataclasses import dataclass, field
 from typing import Optional
 
 from ghastoolkit.octokit.github import GitHub, Repository
-from ghastoolkit.octokit.octokit import RestRequest
+from ghastoolkit.octokit.octokit import OctoItem, RestRequest, loadOctoItem
+
+
+logger = logging.getLogger("ghastoolkit.octokit.secretscanning")
+
+
+@dataclass
+class SecretAlert(OctoItem):
+    number: int
+    state: str
+
+    created_at: str
+
+    secret_type: str
+    secret_type_display_name: str
+    secret: str
+
+    _locations: list[dict] = field(default_factory=list)
+    _sha: Optional[str] = None
+
+    @property
+    def locations(self) -> list[dict]:
+        """Get Alert locations (use cache or request from API)"""
+        if not self._locations:
+            self._locations = SecretScanning().getAlertLocations(self.number)
+        return self._locations
+
+    @property
+    def commit_sha(self) -> Optional[str]:
+        """Get commit sha if present"""
+        if self._sha is None:
+            for loc in self.locations:
+                if loc.get("type") == "commit":
+                    self._sha = loc.get("details", {}).get("blob_sha")
+                    break
+        return self._sha
+
+    def __str__(self) -> str:
+        return f"SecretAlert({self.number}, '{self.secret_type}')"
 
 
 class SecretScanning:
     def __init__(self, repository: Optional[Repository] = None) -> None:
         self.repository = repository or GitHub.repository
         if not self.repository:
             raise Exception("SecretScanning requires Repository to be set")
@@ -19,38 +58,47 @@
         https://docs.github.com/en/rest/secret-scanning#list-secret-scanning-alerts-for-an-organization
         """
         results = self.rest.get("/orgs/{org}/secret-scanning/alerts", {"state": state})
         if isinstance(results, list):
             return results
         raise Exception(f"Error getting organization secret scanning results")
 
-    def getAlerts(self, state: Optional[str] = None) -> list[dict]:
+    @RestRequest.restGet("/repos/{owner}/{repo}/secret-scanning/alerts")
+    def getAlerts(self, state: str = "open") -> list[SecretAlert]:
         """Get Repository alerts
 
         https://docs.github.com/en/rest/secret-scanning#list-secret-scanning-alerts-for-a-repository
         """
-        results = self.rest.get(
-            "/repos/{owner}/{repo}/secret-scanning/alerts", {"state": state}
-        )
-        if isinstance(results, list):
-            return results
-        raise Exception(f"Error getting repository secret scanning results")
+        return []
 
-    def getAlert(self, alert_number: int, state: Optional[str] = None) -> dict:
+    def getAlert(
+        self, alert_number: int, state: Optional[str] = None
+    ) -> Optional[SecretAlert]:
         """Get Alert by `alert_number`
 
         https://docs.github.com/en/rest/secret-scanning#get-a-secret-scanning-alert
         """
         results = self.rest.get(
             "/repos/{owner}/{repo}/secret-scanning/alerts/{alert_number}",
             {"alert_number": alert_number, "state": state},
         )
         if isinstance(results, dict):
-            return results
-        raise Exception(f"Error getting repository secret scanning result")
+            return loadOctoItem(SecretAlert, results)
+
+    def getAlertsInPR(self) -> list[SecretAlert]:
+        """Get Alerts in a Pull Request"""
+        results = []
+        pr_commits = self.repository.getPullRequestCommits()
+        logger.debug(f"Number of Commits in PR :: {len(pr_commits)}")
+
+        for alert in self.getAlerts("open"):
+            if alert.commit_sha in pr_commits:
+                results.append(alert)
+
+        return results
 
     def getAlertLocations(self, alert_number: int) -> list[dict]:
         """Get Alert Locations by `alert_number`
 
         https://docs.github.com/en/rest/secret-scanning#list-locations-for-a-secret-scanning-alert
         """
         results = self.rest.get(
```

### Comparing `ghastoolkit-0.1.9/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.0/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.9
+Version: 0.2.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.9/tests/test_codeqldb.py` & `ghastoolkit-0.2.0/tests/test_codeqldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     def setUp(self):
         self.repo = Repository("GeekMasher", "ghastoolkit")
 
     def test_path(self):
         codeql = CodeQLDatabase("db", "java", self.repo)
         self.assertEqual(
             codeql.createDownloadPath("/tmp"),
-            os.path.join("/tmp", "java", "GeekMasher", "ghastoolkit")
+            os.path.join("/tmp", "java", "GeekMasher", "ghastoolkit"),
         )
 
         codeql = CodeQLDatabase("db", "java")
         self.assertEqual(
-            codeql.createDownloadPath("/tmp"),
-            os.path.join("/tmp", "java", "db")
+            codeql.createDownloadPath("/tmp"), os.path.join("/tmp", "java", "db")
         )
-
```

### Comparing `ghastoolkit-0.1.9/tests/test_codescanning.py` & `ghastoolkit-0.2.0/tests/test_codescanning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-
 import unittest
 
 from ghastoolkit.octokit.codescanning import CodeScanning
-from ghastoolkit.octokit.github import GitHub 
+from ghastoolkit.octokit.github import GitHub
 
 
 class TestCodeScanning(unittest.TestCase):
     def setUp(self) -> None:
         GitHub.init("GeekMasher/ghastoolkit")
         return super().setUp()
 
     def test_codescanning_default(self):
         cs = CodeScanning()
-        self.assertEqual(cs.repository.display(), "GeekMasher/ghastoolkit")    
-        
+        self.assertEqual(cs.repository.display(), "GeekMasher/ghastoolkit")
+
         cs = CodeScanning(GitHub.repository)
-        self.assertEqual(cs.repository.display(), "GeekMasher/ghastoolkit")    
+        self.assertEqual(cs.repository.display(), "GeekMasher/ghastoolkit")
 
         GitHub.init("Sample/Repo")
         cs = CodeScanning(GitHub.repository)
         self.assertEqual(cs.repository.display(), "Sample/Repo")
-
```

### Comparing `ghastoolkit-0.1.9/tests/test_depgraph.py` & `ghastoolkit-0.2.0/tests/test_depgraph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-
 import unittest
 
 from ghastoolkit.octokit.dependencygraph import Dependency, Dependencies
 
+
 class TestDepGraph(unittest.TestCase):
     def test_dependency(self):
         dep = Dependency("django", version="1.11.1", manager="pypi")
 
         self.assertEqual(dep.name, "django")
         self.assertEqual(dep.manager, "pypi")
         self.assertEqual(dep.version, "1.11.1")
 
+    def test_fullname_maven(self):
+        dep = Dependency("express", manager="npm")
+        self.assertEqual(dep.fullname, "express")
+
+        dep = Dependency(
+            "spring-boot-starter-web", "org.springframework.boot", manager="maven"
+        )
+        self.assertEqual(
+            dep.fullname, "org.springframework.boot:spring-boot-starter-web"
+        )
 
     def test_purl(self):
         # python
         dep = Dependency("django", version="1.11.1", manager="pypi")
         self.assertEqual(dep.getPurl(), "pkg:pypi/django@1.11.1")
-        
+
         # go
         dep = Dependency("genproto", "google.golang.org", manager="golang")
         self.assertEqual(dep.getPurl(), "pkg:golang/google.golang.org/genproto")
 
     def test_purl_from(self):
         # GitHub Actions
         dep = Dependency.fromPurl("pkg:githubactions/actions/setup-python@3")
@@ -31,20 +41,26 @@
 
         dep = Dependency.fromPurl("pkg:githubactions/github/codeql-action/analyze@2")
         self.assertEqual(dep.name, "codeql-action/analyze")
         self.assertEqual(dep.namespace, "github")
         self.assertEqual(dep.manager, "githubactions")
         self.assertEqual(dep.version, "2")
 
-        # PyPi 
+        # PyPi
         dep = Dependency.fromPurl("pkg:pypi/requests@2.28.2")
         self.assertEqual(dep.name, "requests")
         self.assertEqual(dep.manager, "pypi")
         self.assertEqual(dep.version, "2.28.2")
 
+    def test_purl_from_basic(self):
+        dep = Dependency.fromPurl("npm/ini")
+        self.assertEqual(dep.name, "ini")
+        self.assertEqual(dep.manager, "npm")
+
+
 class TestDependencies(unittest.TestCase):
     def setUp(self) -> None:
         self.deps = Dependencies()
         self.deps.append(Dependency("urllib3", licence="MIT"))
         self.deps.append(Dependency("rich", licence="NOASSERTION"))
         self.deps.append(Dependency("pyyaml", licence="GPL-3.0"))
         self.deps.append(Dependency("pyproject-hooks", licence="Apache-2.0"))
@@ -69,8 +85,12 @@
 
     def test_findName(self):
         pys = self.deps.findNames(["py*"])
         self.assertEqual(len(pys), 2)
         self.assertEqual(pys[0].name, "pyyaml")
         self.assertEqual(pys[1].name, "pyproject-hooks")
 
-
+    def test_find(self):
+        dep = self.deps.find("pyyaml")
+        self.assertIsNotNone(dep)
+        assert dep is not None
+        self.assertEqual(dep.name, "pyyaml")
```

### Comparing `ghastoolkit-0.1.9/tests/test_github.py` & `ghastoolkit-0.2.0/tests/test_github.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import unittest
 
 from ghastoolkit.octokit.github import GitHub, Repository
 
 
 class TestGitHub(unittest.TestCase):
     def setUp(self) -> None:
@@ -14,25 +13,27 @@
         GitHub.api_rest = "https://api.github.com"
         GitHub.api_graphql = "https://api.github.com/graphql"
 
         return super().tearDown()
 
     def test_default(self):
         GitHub.init("GeekMasher/ghastoolkit")
-        
+
         self.assertEqual(GitHub.instance, "https://github.com")
         self.assertEqual(GitHub.api_rest, "https://api.github.com")
         self.assertEqual(GitHub.api_graphql, "https://api.github.com/graphql")
 
     def test_server(self):
         GitHub.init("GeekMasher/ghastoolkit", instance="https://github.geekmasher.dev")
-        
+
         self.assertEqual(GitHub.instance, "https://github.geekmasher.dev")
-        self.assertEqual(GitHub.api_rest, "https://github.geekmasher.dev/api")
-        self.assertEqual(GitHub.api_graphql, "https://github.geekmasher.dev/api/graphql")
+        self.assertEqual(GitHub.api_rest, "https://github.geekmasher.dev/api/v3")
+        self.assertEqual(
+            GitHub.api_graphql, "https://github.geekmasher.dev/api/v3/graphql"
+        )
 
     def test_parseReference(self):
         repo = Repository.parseRepository("GeekMasher/ghastoolkit")
         self.assertEqual(repo.owner, "GeekMasher")
         self.assertEqual(repo.repo, "ghastoolkit")
 
         repo = Repository.parseRepository("GeekMasher/ghastoolkit@main")
@@ -41,15 +42,18 @@
         self.assertEqual(repo.branch, "main")
         self.assertEqual(repo.reference, "refs/heads/main")
 
 
 class TestRepository(unittest.TestCase):
     def setUp(self) -> None:
         GitHub.token = None
+        GitHub.github_app = False
+
         return super().setUp()
+
     def test_branch(self):
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/heads/main")
         self.assertEqual(repo.reference, "refs/heads/main")
         self.assertEqual(repo.branch, "main")
 
     def test_pull_request(self):
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/heads/main")
@@ -57,12 +61,41 @@
 
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/pull/1/merge")
         self.assertTrue(repo.isInPullRequest())
         self.assertEqual(repo.getPullRequestNumber(), 1)
 
     def test_clone_url(self):
         repo = Repository("GeekMasher", "ghastoolkit")
-        self.assertEqual(repo.clone_url, "https://github.com/GeekMasher/ghastoolkit.git")
-        
+        self.assertEqual(
+            repo.clone_url, "https://github.com/GeekMasher/ghastoolkit.git"
+        )
+
+        GitHub.token = "test_token"
+        self.assertEqual(
+            repo.clone_url, "https://test_token@github.com/GeekMasher/ghastoolkit.git"
+        )
+
+        GitHub.github_app = True
         GitHub.token = "test_token"
-        self.assertEqual(repo.clone_url, "https://test_token@github.com/GeekMasher/ghastoolkit.git")
+        self.assertEqual(
+            repo.clone_url,
+            "https://x-access-token:test_token@github.com/GeekMasher/ghastoolkit.git",
+        )
+
+    def test_clone_cmd(self):
+        path = "/tml/ghastoolkit"
+        repo = Repository("GeekMasher", "ghastoolkit")
+
+        cmd = ["git", "clone", repo.clone_url, path]
+        self.assertEqual(repo._cloneCmd(path), cmd)
 
+        cmd = ["git", "clone", "--depth", "1", repo.clone_url, path]
+        self.assertEqual(repo._cloneCmd(path, depth=1), cmd)
+
+        repo.branch = "main"
+        cmd = ["git", "clone", "-b", "main", repo.clone_url, path]
+        self.assertEqual(repo._cloneCmd(path), cmd)
+
+    def test_clone_file(self):
+        path = "README.md"
+        repo = Repository("GeekMasher", "ghastoolkit")
+        repo.getFile(path)
```

