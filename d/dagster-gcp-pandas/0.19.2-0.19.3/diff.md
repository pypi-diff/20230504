# Comparing `tmp/dagster-gcp-pandas-0.19.2.tar.gz` & `tmp/dagster-gcp-pandas-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.19.2.tar", last modified: Thu Apr 27 19:32:35 2023, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.19.3.tar", last modified: Thu May  4 17:52:22 2023, max compression
```

## Comparing `dagster-gcp-pandas-0.19.2.tar` & `dagster-gcp-pandas-0.19.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:32:35.199998 dagster-gcp-pandas-0.19.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-27 19:32:35.199998 dagster-gcp-pandas-0.19.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:32:35.195998 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      394 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:32:35.195998 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9688 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:32:35.195998 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 19:32:34.000000 dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-27 19:32:35.199998 dagster-gcp-pandas-0.19.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-27 18:30:35.000000 dagster-gcp-pandas-0.19.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:22.868505 dagster-gcp-pandas-0.19.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-04 17:52:22.868505 dagster-gcp-pandas-0.19.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:22.864505 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:22.868505 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9688 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:22.868505 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-04 17:52:22.000000 dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-04 17:52:22.868505 dagster-gcp-pandas-0.19.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-04 17:42:14.000000 dagster-gcp-pandas-0.19.3/setup.py
```

### Comparing `dagster-gcp-pandas-0.19.2/LICENSE` & `dagster-gcp-pandas-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.19.2/PKG-INFO` & `dagster-gcp-pandas-0.19.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-gcp-pandas-0.19.2/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.19.3/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.19.2/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.19.3/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-gcp-pandas-0.19.2/setup.py` & `dagster-gcp-pandas-0.19.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.2",
-        "dagster-gcp==0.19.2",
+        "dagster==1.3.3",
+        "dagster-gcp==0.19.3",
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

