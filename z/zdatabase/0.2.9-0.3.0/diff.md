# Comparing `tmp/zdatabase-0.2.9.tar.gz` & `tmp/zdatabase-0.3.0.tar.gz`

## Comparing `zdatabase-0.2.9.tar` & `zdatabase-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 zdatabase-0.2.9/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 zdatabase-0.2.9/src/zdatabase/model.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 zdatabase-0.2.9/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.2.9/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.2.9/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.2.9/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 zdatabase-0.3.0/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 zdatabase-0.3.0/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 zdatabase-0.3.0/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.3.0/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.3.0/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.3.0/PKG-INFO
```

### Comparing `zdatabase-0.2.9/src/zdatabase/__init__.py` & `zdatabase-0.3.0/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.2.9/src/zdatabase/model.py` & `zdatabase-0.3.0/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.2.9/src/zdatabase/utility.py` & `zdatabase-0.3.0/src/zdatabase/utility.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.2.9/LICENSE` & `zdatabase-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.2.9/pyproject.toml` & `zdatabase-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.2.9"
+version = "0.3.0"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-  "flask_sqlalchemy==2.5.1",
+  "flask_sqlalchemy==3.0.3",
   "sqlalchemy==1.4.39",
   "inspirare"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `zdatabase-0.2.9/PKG-INFO` & `zdatabase-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.2.9
+Version: 0.3.0
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: flask-sqlalchemy==2.5.1
+Requires-Dist: flask-sqlalchemy==3.0.3
 Requires-Dist: inspirare
 Requires-Dist: sqlalchemy==1.4.39
 Description-Content-Type: text/markdown
 
 # zdb
 
 Zen database library.
```

