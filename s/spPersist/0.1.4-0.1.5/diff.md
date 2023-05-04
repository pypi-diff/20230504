# Comparing `tmp/sppersist-0.1.4.tar.gz` & `tmp/sppersist-0.1.5.tar.gz`

## Comparing `sppersist-0.1.4.tar` & `sppersist-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.4/src/spPersist/__init__.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 sppersist-0.1.4/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.4/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.4/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.5/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 sppersist-0.1.5/src/spPersist/dp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.5/LICENSE
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.5/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.5/PKG-INFO
```

### Comparing `sppersist-0.1.4/LICENSE` & `sppersist-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.4/pyproject.toml` & `sppersist-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.4/PKG-INFO` & `sppersist-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.4
+Version: 0.1.5
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Spatial analysis package
+# Spatial Transcriptomics with Persistent Homology
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
```

