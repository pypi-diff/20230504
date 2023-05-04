# Comparing `tmp/hagis-0.5.0.tar.gz` & `tmp/hagis-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.0.tar", last modified: Thu May  4 16:05:52 2023, max compression
+gzip compressed data, was "hagis-0.5.1.tar", last modified: Thu May  4 16:32:00 2023, max compression
```

## Comparing `hagis-0.5.0.tar` & `hagis-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:05:52.932939 hagis-0.5.0/
--rw-rw-rw-   0        0        0      923 2023-05-04 16:05:52.932438 hagis-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:05:52.929801 hagis-0.5.0/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20384 2023-05-04 15:56:16.000000 hagis-0.5.0/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-04 16:02:56.000000 hagis-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 16:05:52.933935 hagis-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 16:32:00.210054 hagis-0.5.1/
+-rw-rw-rw-   0        0        0      923 2023-05-04 16:32:00.208933 hagis-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:32:00.206928 hagis-0.5.1/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20415 2023-05-04 16:30:32.000000 hagis-0.5.1/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-04 16:31:31.000000 hagis-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:32:00.210577 hagis-0.5.1/setup.cfg
```

### Comparing `hagis-0.5.0/PKG-INFO` & `hagis-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.0
+Version: 0.5.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.0/hagis.egg-info/PKG-INFO` & `hagis-0.5.1/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.0
+Version: 0.5.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.0/hagis.py` & `hagis-0.5.1/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,16 @@
 
         class LambdaFinder(ast.NodeVisitor):
 
             expression: ast.Lambda
 
             def __init__(self, code: str) -> None:
                 super().__init__()
-                self.visit(ast.parse(f"{code}    pass" if code.strip().endswith(":") else code))
+                line = code.strip()
+                self.visit(ast.parse(f"{line}\n    pass" if line.endswith(":") else line))
 
             def visit_Lambda(self, node: ast.Lambda) -> Any:  # pylint: disable-all
                 self.expression = node
 
             @staticmethod
             def find(expression: Any):  # pylint: disable-all
                 return LambdaFinder(getsource(expression)).expression
```

### Comparing `hagis-0.5.0/pyproject.toml` & `hagis-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

