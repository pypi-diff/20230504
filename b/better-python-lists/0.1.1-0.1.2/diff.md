# Comparing `tmp/better_python_lists-0.1.1.tar.gz` & `tmp/better_python_lists-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_python_lists-0.1.1.tar", max compression
+gzip compressed data, was "better_python_lists-0.1.2.tar", max compression
```

## Comparing `better_python_lists-0.1.1.tar` & `better_python_lists-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.1/LICENSE
--rw-r--r--   0        0        0      138 2023-05-04 18:16:21.769517 better_python_lists-0.1.1/README.md
--rw-r--r--   0        0        0       23 2023-05-04 17:38:53.402760 better_python_lists-0.1.1/better_python_lists/__init__.py
--rw-r--r--   0        0        0      892 2023-05-04 18:12:22.339636 better_python_lists-0.1.1/better_python_lists/list.py
--rw-r--r--   0        0        0      480 2023-05-04 18:18:56.725386 better_python_lists-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 better_python_lists-0.1.1/setup.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 better_python_lists-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.2/LICENSE
+-rw-r--r--   0        0        0      981 2023-05-04 18:31:27.446961 better_python_lists-0.1.2/README.md
+-rw-r--r--   0        0        0       23 2023-05-04 17:38:53.402760 better_python_lists-0.1.2/better_python_lists/__init__.py
+-rw-r--r--   0        0        0      892 2023-05-04 18:12:22.339636 better_python_lists-0.1.2/better_python_lists/list.py
+-rw-r--r--   0        0        0      480 2023-05-04 18:31:57.675723 better_python_lists-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 better_python_lists-0.1.2/setup.py
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 better_python_lists-0.1.2/PKG-INFO
```

### Comparing `better_python_lists-0.1.1/LICENSE` & `better_python_lists-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `better_python_lists-0.1.1/better_python_lists/list.py` & `better_python_lists-0.1.2/better_python_lists/list.py`

 * *Files identical despite different names*

