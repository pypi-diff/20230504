# Comparing `tmp/openxes_cli_py-0.1.2.tar.gz` & `tmp/openxes_cli_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxes_cli_py-0.1.2.tar", max compression
+gzip compressed data, was "openxes_cli_py-0.1.5.tar", max compression
```

## Comparing `openxes_cli_py-0.1.2.tar` & `openxes_cli_py-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0  3717515 2023-05-04 11:52:40.155848 openxes_cli_py-0.1.2/lib/openxes-cli.jar
--rw-r--r--   0        0        0      460 2023-05-04 12:50:02.542115 openxes_cli_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 10:04:18.083309 openxes_cli_py-0.1.2/src/openxes_cli/__init__.py
--rw-r--r--   0        0        0     1196 2023-05-04 12:19:58.747945 openxes_cli_py-0.1.2/src/openxes_cli/lib.py
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-05-04 13:07:00.340312 openxes_cli_py-0.1.5/README.md
+-rw-r--r--   0        0        0  3717515 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/lib/openxes-cli.jar
+-rw-r--r--   0        0        0      481 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/src/openxes_cli/__init__.py
+-rw-r--r--   0        0        0     1196 2023-05-04 13:07:00.356312 openxes_cli_py-0.1.5/src/openxes_cli/lib.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.5/PKG-INFO
```

### Comparing `openxes_cli_py-0.1.2/lib/openxes-cli.jar` & `openxes_cli_py-0.1.5/lib/openxes-cli.jar`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.2/src/openxes_cli/lib.py` & `openxes_cli_py-0.1.5/src/openxes_cli/lib.py`

 * *Files identical despite different names*

