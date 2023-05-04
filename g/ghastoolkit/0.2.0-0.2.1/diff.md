# Comparing `tmp/ghastoolkit-0.2.0.tar.gz` & `tmp/ghastoolkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.2.0.tar", last modified: Thu May  4 12:12:15 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.1.tar", last modified: Thu May  4 14:16:07 2023, max compression
```

## Comparing `ghastoolkit-0.2.0.tar` & `ghastoolkit-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.565283 ghastoolkit-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.569283 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:12:15.000000 ghastoolkit-0.2.0/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:15.573283 ghastoolkit-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:11:47.000000 ghastoolkit-0.2.0/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.0/LICENSE` & `ghastoolkit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/PKG-INFO` & `ghastoolkit-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.0/README.md` & `ghastoolkit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/pyproject.toml` & `ghastoolkit-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/__init__.py` & `ghastoolkit-0.2.1/src/ghastoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.1/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.1/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,21 @@
 
         cmd = self._cloneCmd(self.clone_path, depth=depth)
         logger.debug(f"Cloning Command :: {cmd}")
 
         with open(os.devnull, "w") as null:
             subprocess.check_call(cmd, stdout=null, stderr=null)
 
+    def gitsha(self) -> str:
+        cmd = ["git", "rev-parse", "HEAD"]
+        result = (
+            subprocess.check_output(cmd, cwd=self.clone_path).decode("ascii").strip()
+        )
+        return result
+
     def getFile(self, path: str) -> str:
         """Get a path relative from the base of the cloned repository"""
         if not self.clone_path:
             raise Exception(f"Unknown clone path")
         return os.path.join(self.clone_path, path)
 
     def display(self):
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.1/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 import re
 from typing import Optional
 
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
+from ghastoolkit.supplychain.licensing import Licenses
 
 logger = logging.getLogger("ghastoolkit.supplychain.dependencies")
 
 
 @dataclass
 class Dependency:
     name: str
@@ -133,14 +134,25 @@
 
     def findUnknownLicenses(
         self, licenses: Optional[list[str]] = None
     ) -> "Dependencies":
         licenses = licenses or ["NA", "NOASSERTION"]
         return self.findLicenses(licenses)
 
+    def applyLicenses(self, licenses: Licenses):
+        """Apply Linceses"""
+        for i, dep in enumerate(self):
+            if dep.licence:
+                continue
+            purl = dep.getPurl(version=False)
+            dblicense = licenses.find(purl)
+            if dblicense:
+                dep.licence = " OR ".join(dblicense)
+                self[i] = dep
+
     def contains(self, dependency: Dependency) -> bool:
         purl = dependency.getPurl(version=False)
         for dep in self:
             if dep.name == dependency.name or dep.getPurl(version=False) == purl:
                 return True
         return False
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/licensing.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,25 +20,26 @@
         if not os.path.isfile(path):
             raise Exception("Path provided needs to be a file")
 
         logger.debug(f"Loading licenseing file :: {path}")
         with open(path, "r") as handle:
             data = json.load(handle)
 
-        Licenses.data = data.get("data", {})
+        Licenses.data = data
         logger.debug(f"Loaded licenses :: {len(data)}")
 
     def add(self, purl: str, licenses: str | list):
         """Add license"""
         if Licenses.data.get(purl):
             return
         licenses = licenses if isinstance(licenses, list) else [licenses]
         Licenses.data[purl] = licenses
 
     def find(self, purl: str) -> Optional[list[str]]:
+        """Find by PURL"""
         return Licenses.data.get(purl)
 
     def export(self, path: str):
         with open(path, "w") as handle:
             json.dump(Licenses.data, handle)
 
     def __len__(self) -> int:
@@ -63,14 +64,19 @@
 
     licenses = Licenses()
 
     repository = Repository.parseRepository("clearlydefined/curated-data")
     logging.info(f"Cloning / Using `clearlydefined` repo: {repository.clone_path}")
     repository.clone(clobber=True, depth=1)
 
+    lock_content = {
+        "repository": repository.display(),
+        "version": repository.gitsha(),
+    }
+
     # https://github.com/clearlydefined/curated-data/tree/master/curations
     curations = repository.getFile("curations")
 
     for root, dirs, files in os.walk(curations):
         for filename in files:
             name, ext = os.path.splitext(filename)
             if ext not in [".yml", ".yaml"]:
@@ -78,20 +84,26 @@
 
             path = os.path.join(root, filename)
 
             with open(path, "r") as handle:
                 curation_data = yaml.safe_load(handle)
 
             coordinates = curation_data.get("coordinates", {})
-            purl = f"{coordinates.get('type')}/{coordinates.get('namespace')}/{coordinates.get('name')}"
+            purl = f"pkg:{coordinates.get('type')}/{coordinates.get('namespace')}/{coordinates.get('name')}"
 
             revision_licenses = set()
             for _, revision in curation_data.get("revisions", {}).items():
                 l = revision.get("licensed")
                 if l and l.get("declaired"):
                     revision_licenses.add(l.get("declaired"))
 
             licenses.add(purl, list(revision_licenses))
 
-    print(f"Licenses Loaded :: {len(licenses)}")
+    logging.info(f"Licenses Loaded :: {len(licenses)}")
+
+    # lock file
+    lock_path = arguments.output.replace(".json", ".lock.json")
+    logging.info(f"Saving lock file :: {lock_path}")
+    with open(lock_path, "w") as handle:
+        json.dump(lock_content, handle, sort_keys=True, indent=2)
 
     licenses.export(arguments.output)
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.1/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.2.1/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
 tests/test_codeqldb.py
 tests/test_codescanning.py
 tests/test_default.py
 tests/test_depgraph.py
 tests/test_github.py
+tests/test_licenses.py
 tests/test_octokit.py
 tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.0/tests/test_codeqldb.py` & `ghastoolkit-0.2.1/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_codescanning.py` & `ghastoolkit-0.2.1/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_default.py` & `ghastoolkit-0.2.1/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_depgraph.py` & `ghastoolkit-0.2.1/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_github.py` & `ghastoolkit-0.2.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_octokit.py` & `ghastoolkit-0.2.1/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.0/tests/test_secretscanning.py` & `ghastoolkit-0.2.1/tests/test_secretscanning.py`

 * *Files identical despite different names*

