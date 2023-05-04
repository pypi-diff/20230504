# Comparing `tmp/better_python_lists-0.1.0.tar.gz` & `tmp/better_python_lists-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_python_lists-0.1.0.tar", max compression
+gzip compressed data, was "better_python_lists-0.1.1.tar", max compression
```

## Comparing `better_python_lists-0.1.0.tar` & `better_python_lists-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.0/LICENSE
--rw-r--r--   0        0        0       70 2023-05-04 16:25:45.098190 better_python_lists-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 16:41:32.322993 better_python_lists-0.1.0/better_python_lists/__init__.py
--rw-r--r--   0        0        0       27 2023-05-04 16:39:45.370818 better_python_lists-0.1.0/better_python_lists/list.py
--rw-r--r--   0        0        0      480 2023-05-04 16:38:44.827053 better_python_lists-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 better_python_lists-0.1.0/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 better_python_lists-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.1/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-04 18:16:21.769517 better_python_lists-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2023-05-04 17:38:53.402760 better_python_lists-0.1.1/better_python_lists/__init__.py
+-rw-r--r--   0        0        0      892 2023-05-04 18:12:22.339636 better_python_lists-0.1.1/better_python_lists/list.py
+-rw-r--r--   0        0        0      480 2023-05-04 18:18:56.725386 better_python_lists-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 better_python_lists-0.1.1/setup.py
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 better_python_lists-0.1.1/PKG-INFO
```

### Comparing `better_python_lists-0.1.0/LICENSE` & `better_python_lists-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `better_python_lists-0.1.0/setup.py` & `better_python_lists-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['better_python_lists']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'better-python-lists',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Adds some useful methods on top of Python lists',
-    'long_description': '# better-python-lists\nAdds some useful methods on top of Python lists\n',
+    'long_description': '# Better Python Lists\n\nMakes lists in Python better, by adding some useful functions.\n\n## Installation\n\n`pip install better-python-lists`\n',
     'author': 'Bradley Marques',
     'author_email': 'bradleyrcmarques@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

