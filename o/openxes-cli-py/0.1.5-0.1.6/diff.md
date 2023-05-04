# Comparing `tmp/openxes_cli_py-0.1.5.tar.gz` & `tmp/openxes_cli_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxes_cli_py-0.1.5.tar", max compression
+gzip compressed data, was "openxes_cli_py-0.1.6.tar", max compression
```

## Comparing `openxes_cli_py-0.1.5.tar` & `openxes_cli_py-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      615 2023-05-04 13:07:00.340312 openxes_cli_py-0.1.5/README.md
--rw-r--r--   0        0        0  3717515 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/lib/openxes-cli.jar
--rw-r--r--   0        0        0      481 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/src/openxes_cli/__init__.py
--rw-r--r--   0        0        0     1196 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/src/openxes_cli/lib.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-05-04 13:13:35.117868 openxes_cli_py-0.1.6/README.md
+-rw-r--r--   0        0        0  3717515 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/lib/openxes-cli.jar
+-rw-r--r--   0        0        0      481 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/src/openxes_cli/__init__.py
+-rw-r--r--   0        0        0     1196 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/src/openxes_cli/lib.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.6/PKG-INFO
```

### Comparing `openxes_cli_py-0.1.5/README.md` & `openxes_cli_py-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.5/lib/openxes-cli.jar` & `openxes_cli_py-0.1.6/lib/openxes-cli.jar`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.5/src/openxes_cli/lib.py` & `openxes_cli_py-0.1.6/src/openxes_cli/lib.py`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.5/PKG-INFO` & `openxes_cli_py-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxes-cli-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Ihar Suvorau
 Author-email: ihar.suvorau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

