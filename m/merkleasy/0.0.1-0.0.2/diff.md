# Comparing `tmp/merkleasy-0.0.1.tar.gz` & `tmp/merkleasy-0.0.2.tar.gz`

## Comparing `merkleasy-0.0.1.tar` & `merkleasy-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 merkleasy-0.0.1/merkleasy/__init__.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 merkleasy-0.0.1/merkleasy/classes.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 merkleasy-0.0.1/merkleasy/interfaces.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 merkleasy-0.0.1/tests/context.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 merkleasy-0.0.1/tests/test_classes.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 merkleasy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.1/license
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 merkleasy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 merkleasy-0.0.1/readme.md
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 merkleasy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/__init__.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/classes.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 merkleasy-0.0.2/merkleasy/interfaces.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 merkleasy-0.0.2/tests/context.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 merkleasy-0.0.2/tests/test_classes.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 merkleasy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 merkleasy-0.0.2/license
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 merkleasy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 merkleasy-0.0.2/readme.md
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 merkleasy-0.0.2/PKG-INFO
```

### Comparing `merkleasy-0.0.1/merkleasy/classes.py` & `merkleasy-0.0.2/merkleasy/classes.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.1/merkleasy/interfaces.py` & `merkleasy-0.0.2/merkleasy/interfaces.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.1/tests/test_classes.py` & `merkleasy-0.0.2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.1/license` & `merkleasy-0.0.2/license`

 * *Files identical despite different names*

### Comparing `merkleasy-0.0.1/pyproject.toml` & `merkleasy-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "merkleasy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Simple, easy-to-use merkle tree library"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,8 +16,13 @@
     "License :: OSI Approved :: ISC License (ISCL)",
     "Operating System :: OS Independent",
     "Topic :: Security :: Cryptography"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/k98kurz/merkle"
-"Bug Tracker" = "https://github.com/k98kurz/merkle/issues"
+"Bug Tracker" = "https://github.com/k98kurz/merkle/issues"
+
+[tool.hatch.build.targets.dist]
+exclude = [
+  "tests"
+]
```

### Comparing `merkleasy-0.0.1/readme.md` & `merkleasy-0.0.2/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Status
 
 - [x] Interface
 - [x] Tests
 - [x] Implementation
 - [x] Proofs
 - [x] Usage Documentation
-- [ ] Publish to pypi
+- [x] Publish to pypi
 
 # Installation
 
 ```bash
 pip install merkleasy
 ```
 
@@ -168,14 +168,28 @@
 the leaf and ends with the root, and then it follows the proof operations.
 
 If the call to `Tree.verify` is provided invalid parameters or an invalid proof,
 it will throw an `AssertionError` or `ValueError`. If all checks pass, it
 executes without error and returns `None`.
 
 
+# Security / Usage Note
+
+Any application/library that uses this package should use a schema for leaves
+that is anything except exactly 32 bytes. This prevents the second-preimage
+attack whereby the application is tricked into thinking that an intermediate
+node in the tree is a leaf. It is hard to envision a scenario in which this
+could actually become a serious security issue, but it is worth keeping in mind
+during application development.
+
+So in addition to verifying an inclusion proof, verify that the data fits the
+leaf schema. Preferably, leaf schema should not be bytes, and a serializer to
+bytes from the schema should be used on the leaf before verifying the inclusion
+proof.
+
 # ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
```

### Comparing `merkleasy-0.0.1/PKG-INFO` & `merkleasy-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkleasy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple, easy-to-use merkle tree library
 Project-URL: Homepage, https://github.com/k98kurz/merkle
 Project-URL: Bug Tracker, https://github.com/k98kurz/merkle/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 # Status
 
 - [x] Interface
 - [x] Tests
 - [x] Implementation
 - [x] Proofs
 - [x] Usage Documentation
-- [ ] Publish to pypi
+- [x] Publish to pypi
 
 # Installation
 
 ```bash
 pip install merkleasy
 ```
 
@@ -183,14 +183,28 @@
 the leaf and ends with the root, and then it follows the proof operations.
 
 If the call to `Tree.verify` is provided invalid parameters or an invalid proof,
 it will throw an `AssertionError` or `ValueError`. If all checks pass, it
 executes without error and returns `None`.
 
 
+# Security / Usage Note
+
+Any application/library that uses this package should use a schema for leaves
+that is anything except exactly 32 bytes. This prevents the second-preimage
+attack whereby the application is tricked into thinking that an intermediate
+node in the tree is a leaf. It is hard to envision a scenario in which this
+could actually become a serious security issue, but it is worth keeping in mind
+during application development.
+
+So in addition to verifying an inclusion proof, verify that the data fits the
+leaf schema. Preferably, leaf schema should not be bytes, and a serializer to
+bytes from the schema should be used on the leaf before verifying the inclusion
+proof.
+
 # ISC License
 
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
```

