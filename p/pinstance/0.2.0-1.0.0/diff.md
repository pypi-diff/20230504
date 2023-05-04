# Comparing `tmp/pinstance-0.2.0.tar.gz` & `tmp/pinstance-1.0.0.tar.gz`

## Comparing `pinstance-0.2.0.tar` & `pinstance-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pinstance-0.2.0/src/pinstance/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pinstance-0.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pinstance-0.2.0/LICENSE
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pinstance-0.2.0/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pinstance-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pinstance-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pinstance-1.0.0/src/pinstance/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pinstance-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pinstance-1.0.0/LICENSE
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pinstance-1.0.0/README.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pinstance-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pinstance-1.0.0/PKG-INFO
```

### Comparing `pinstance-0.2.0/src/pinstance/__init__.py` & `pinstance-1.0.0/src/pinstance/__init__.py`

 * *Files identical despite different names*

### Comparing `pinstance-0.2.0/LICENSE` & `pinstance-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinstance-0.2.0/README.md` & `pinstance-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Nohead
+# Pinstance
 
 Simple [singleton](https://en.wikipedia.org/wiki/Singleton_pattern) class decorator with
 ability to call bounded methods with 0 overhead.
 
 Decorated class can not be collected till the end of a programm
 
 ## Usage
```

### Comparing `pinstance-0.2.0/pyproject.toml` & `pinstance-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pinstance"
-version = "0.2.0"
+version = "1.0.0"
 description = "Simple singleton class and function decorators with 0 overhead"
 readme = "README.md"
 authors = [
   { name="Nazarov Pavel", email="unyite8@gmail.com" },
 ]
 license = {text = "MIT"}
 keywords = [
@@ -22,8 +22,8 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
-homepage = "https://github.com/Nyite/pyInstance"
+homepage = "https://github.com/Nyite/Pinstance"
```

### Comparing `pinstance-0.2.0/PKG-INFO` & `pinstance-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pinstance
-Version: 0.2.0
+Version: 1.0.0
 Summary: Simple singleton class and function decorators with 0 overhead
-Project-URL: homepage, https://github.com/Nyite/pyInstance
+Project-URL: homepage, https://github.com/Nyite/Pinstance
 Author-email: Nazarov Pavel <unyite8@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: decorator,singleton
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Nohead
+# Pinstance
 
 Simple [singleton](https://en.wikipedia.org/wiki/Singleton_pattern) class decorator with
 ability to call bounded methods with 0 overhead.
 
 Decorated class can not be collected till the end of a programm
 
 ## Usage
```

