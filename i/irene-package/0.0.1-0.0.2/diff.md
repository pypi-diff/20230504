# Comparing `tmp/irene_package-0.0.1.tar.gz` & `tmp/irene_package-0.0.2.tar.gz`

## Comparing `irene_package-0.0.1.tar` & `irene_package-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 irene_package-0.0.1/LINCENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irene_package-0.0.1/irene_package/__init__.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 irene_package-0.0.1/irene_package/calc.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 irene_package-0.0.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 irene_package-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 irene_package-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 irene_package-0.0.2/LINCENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irene_package-0.0.2/irene_package/__init__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 irene_package-0.0.2/irene_package/calc.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 irene_package-0.0.2/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 irene_package-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 irene_package-0.0.2/PKG-INFO
```

### Comparing `irene_package-0.0.1/LINCENSE.txt` & `irene_package-0.0.2/LINCENSE.txt`

 * *Files identical despite different names*

### Comparing `irene_package-0.0.1/pyproject.toml` & `irene_package-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "opencv-python"]
 build-backend = "hatchling.build"
 
 [project]
 name = "irene_package"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="coldsober", email="coldsober3@gmail.com" },
 ]
 description = "image displayer and calculator for x + y"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `irene_package-0.0.1/PKG-INFO` & `irene_package-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_package
-Version: 0.0.1
+Version: 0.0.2
 Summary: image displayer and calculator for x + y
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: coldsober <coldsober3@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

