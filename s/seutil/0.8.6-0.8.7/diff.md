# Comparing `tmp/seutil-0.8.6.tar.gz` & `tmp/seutil-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seutil-0.8.6.tar", last modified: Sun Oct  9 06:30:31 2022, max compression
+gzip compressed data, was "seutil-0.8.7.tar", last modified: Wed May  3 22:40:14 2023, max compression
```

## Comparing `seutil-0.8.6.tar` & `seutil-0.8.7.tar`

### file list

```diff
@@ -1,45 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-09 06:30:17.000000 seutil-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-10-09 06:30:31.570366 seutil-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-10-09 06:30:17.000000 seutil-0.8.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-09 06:30:31.570366 seutil-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-09 06:30:17.000000 seutil-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/seutil/
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/BashUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3766 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/CliUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11418 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16042 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/IOUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/LoggingUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/MiscUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/Stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/TimeUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/arg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/bash.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/seutil/ds/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5864 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/ds/graph_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/ds/lattice.py
--rw-r--r--   0 runner    (1001) docker     (121)    13453 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/ds/trie.py
--rw-r--r--   0 runner    (1001) docker     (121)    28925 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/seutil/latex/
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/latex/File.py
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/latex/Macro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/latex/Table.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     7965 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/maven.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/pbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    11814 2022-10-09 06:30:17.000000 seutil-0.8.6/seutil/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/seutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-10-09 06:30:31.000000 seutil-0.8.6/seutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-10-09 06:30:31.000000 seutil-0.8.6/seutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-09 06:30:31.000000 seutil-0.8.6/seutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-10-09 06:30:31.000000 seutil-0.8.6/seutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-09 06:30:31.000000 seutil-0.8.6/seutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.566366 seutil-0.8.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:31.570366 seutil-0.8.6/tests/ds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-09 06:30:17.000000 seutil-0.8.6/tests/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-10-09 06:30:17.000000 seutil-0.8.6/tests/ds/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (121)     6287 2022-10-09 06:30:17.000000 seutil-0.8.6/tests/ds/test_trie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.252116 seutil-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 22:40:03.000000 seutil-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 22:40:14.248116 seutil-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 22:40:03.000000 seutil-0.8.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:40:14.252116 seutil-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-03 22:40:03.000000 seutil-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/BashUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/CliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/IOUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/LoggingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/MiscUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/Stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/TimeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/bash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/graph_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31481 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/latex_old/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/Macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/maven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/tests/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/test_trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_BashUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_IOUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_ser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_ser_3rd_party.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_latex_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_project.py
```

### Comparing `seutil-0.8.6/LICENSE` & `seutil-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/PKG-INFO` & `seutil-0.8.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seutil
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python utilities for SE research
 Home-page: https://github.com/pengyunie/seutil
 Author: Pengyu Nie
 Author-email: prodigy.sov@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -12,16 +12,15 @@
 Provides-Extra: dev
 Provides-Extra: io-3rd-party
 License-File: LICENSE
 
 Project ``seutil``
 ==================
 
-|PyPI| |GitHub release (latest by date including pre-releases)| |GitHub
-Workflow Status|
+|PyPI|_ |GitHubRelease|_ |GitHubWorkflow|_
 
 Python utilities for SE(+ML) research. This library stays reasonably
 up-to-date with the latest Python 3, currently 3.8.
 
 **Mature functions:**
 
 * bash: running Bash command; 
@@ -43,11 +42,14 @@
 * BashUtils: the previous version of bash; 
 * IOUtils: the previous version of io; 
 * CliUtils: for command line argument parsing without the need to declare each argument, recommended to use jsonargparse library; 
 * LoggingUtils: the previous version of log;
 
 Full documentation can be found at `readthedocs`_.
 
-.. |PyPI| image:: https://img.shields.io/pypi/v/seutil
-.. |GitHub release (latest by date including pre-releases)| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
-.. |GitHub Workflow Status| image:: https://img.shields.io/github/workflow/status/pengyunie/seutil/Python%20package
+.. |PyPI| image:: https://img.shields.io/pypi/v/seutil 
+.. _PyPI: https://pypi.org/project/seutil/
+.. |GitHubRelease| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
+.. _GitHubRelease: https://github.com/pengyunie/seutil/releases
+.. |GitHubWorkflow| image:: https://img.shields.io/github/actions/workflow/status/pengyunie/seutil/python-package.yml?branch=master
+.. _GitHubWorkflow: https://github.com/pengyunie/seutil/actions/workflows/python-package.yml
 .. _readthedocs: https://seutil.readthedocs.io/en/latest/
```

### Comparing `seutil-0.8.6/README.rst` & `seutil-0.8.7/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Project ``seutil``
 ==================
 
-|PyPI| |GitHub release (latest by date including pre-releases)| |GitHub
-Workflow Status|
+|PyPI|_ |GitHubRelease|_ |GitHubWorkflow|_
 
 Python utilities for SE(+ML) research. This library stays reasonably
 up-to-date with the latest Python 3, currently 3.8.
 
 **Mature functions:**
 
 * bash: running Bash command; 
@@ -28,11 +27,14 @@
 * BashUtils: the previous version of bash; 
 * IOUtils: the previous version of io; 
 * CliUtils: for command line argument parsing without the need to declare each argument, recommended to use jsonargparse library; 
 * LoggingUtils: the previous version of log;
 
 Full documentation can be found at `readthedocs`_.
 
-.. |PyPI| image:: https://img.shields.io/pypi/v/seutil
-.. |GitHub release (latest by date including pre-releases)| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
-.. |GitHub Workflow Status| image:: https://img.shields.io/github/workflow/status/pengyunie/seutil/Python%20package
+.. |PyPI| image:: https://img.shields.io/pypi/v/seutil 
+.. _PyPI: https://pypi.org/project/seutil/
+.. |GitHubRelease| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
+.. _GitHubRelease: https://github.com/pengyunie/seutil/releases
+.. |GitHubWorkflow| image:: https://img.shields.io/github/actions/workflow/status/pengyunie/seutil/python-package.yml?branch=master
+.. _GitHubWorkflow: https://github.com/pengyunie/seutil/actions/workflows/python-package.yml
 .. _readthedocs: https://seutil.readthedocs.io/en/latest/
```

### Comparing `seutil-0.8.6/setup.py` & `seutil-0.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seutil",
-    version="0.8.6",
+    version="0.8.7",
     author="Pengyu Nie",
     author_email="prodigy.sov@gmail.com",
     description="Python utilities for SE research",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/pengyunie/seutil",
     packages=setuptools.find_packages(exclude=["tests"]),
@@ -29,11 +29,11 @@
         "recordclass>=0.11.1",
         "tqdm>=4.62.3",
         "typing_inspect>=0.4.0",
         "unidiff>=0.5.5",
         "xmltodict>=0.2.2",
     ],
     extras_require={
-        "dev": ["pytest", "flake8", "black", "pytest-cov"],
+        "dev": ["pytest", "flake8", "black", "pytest-cov", "ipykernel"],
         "io-3rd-party": ["numpy", "pandas", "torch"],
     },
 )
```

### Comparing `seutil-0.8.6/seutil/BashUtils.py` & `seutil-0.8.7/seutil/BashUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/CliUtils.py` & `seutil-0.8.7/seutil/CliUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/GitHubUtils.py` & `seutil-0.8.7/seutil/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/IOUtils.py` & `seutil-0.8.7/seutil/IOUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/LoggingUtils.py` & `seutil-0.8.7/seutil/LoggingUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/MiscUtils.py` & `seutil-0.8.7/seutil/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/Stream.py` & `seutil-0.8.7/seutil/Stream.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/_config.py` & `seutil-0.8.7/seutil/_config.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/arg.py` & `seutil-0.8.7/seutil/arg.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/bash.py` & `seutil-0.8.7/seutil/bash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
+import signal
 import subprocess
 import warnings
 from typing import Optional
 
 from seutil import io
 
+TimeoutExpired = subprocess.TimeoutExpired
+
 
 class BashError(RuntimeError):
     def __init__(
         self,
         cmd: str,
         completed_process: subprocess.CompletedProcess,
         check_returncode: int,
@@ -50,14 +53,15 @@
 
 def run(
     cmd: str,
     check_returncode: Optional[int] = None,
     warn_nonzero: bool = True,
     update_env: bool = False,
     update_env_clear_existing: bool = False,
+    timeout: Optional[float] = None,
     **kwargs,
 ) -> subprocess.CompletedProcess:
     """
     Run a bash command using subprocess.run.  The command will be run using "bash -c".
 
     Some arguments' default values are changed (but can be overridden with kwargs):
     * capture_output=True, text=True:  capture all stdout and stderr.
@@ -65,37 +69,61 @@
     This function is able to check if return code match a given value (subprocess only supports
     checking non-zero values, but this function supports any).  Nevertheless, this function
     warns about any non-zero values if check_returncode is not set, to avoid silent failures;
     this behavior can be turned off via warn_nonzero=False.
 
     In addition, this function can try to update the environment variables in this process
     with the ones after running the command (if the command finished successfully).
-    The retrival of the sub shell's environments is done by `env` into a temporary file.
+    The retrieval of the sub shell's environments is done by `env` into a temporary file.
 
     :param cmd: the command to run
     :param check_returncode: the return code to expect from the command
     :param warn_nonzero: whether to warn about non-zero exit codes
     :param update_env: whether to update the environment variables in this process
     :param update_env_clear_existing: whether to clear existing environment variables before updating
-    :param kwargs: other arguments passed to subprocess.run
+    :param timeout: number of seconds to wait
+    :param kwargs: other arguments passed to subprocess.Popen
     :return: the subprocess.CompletedProcess object, has stdout, stderr, returncode fields
     :raises: BashError if the command's output did not match check_returncode
     :raises: subprocess.TimeoutExpired if the command timed out
     """
-    # If update env is requested, append `env` to command
+    # potentially append `env` to command to collect the environment variables
+    # TODO: this is hacky: it may mess up some commands; the env won't be collected when timeout; and variable values longer than 1 line will break the collection
     if update_env:
         tempfile_update_env = io.mktmp("seutil-bash", ".txt")
         cmd += f" ; env > {tempfile_update_env}"
 
-    kwargs.setdefault("capture_output", True)
+    # set up popen kwargs
+    # > by default collect stdout/stderr in text mode
     kwargs.setdefault("text", True)
-
-    completed_process = subprocess.run(
-        ["bash", "-c", cmd],
-        **kwargs,
+    # > connect to stdin/stdout/stderr pipes
+    # TODO: allow controlling these pipes via arguments
+    kwargs["stdin"] = subprocess.PIPE
+    kwargs["stdout"] = subprocess.PIPE
+    kwargs["stderr"] = subprocess.PIPE
+    # > start a new session to properly kill all ancestor processes upon timeout (https://alexandra-zaharia.github.io/posts/kill-subprocess-and-its-children-on-timeout-python/)
+    # TODO: when the minimum Python requirement is >= 3.11, use process_group instead of start_new_session
+    kwargs["start_new_session"] = True
+
+    # run the command, similar to `subprocess.run` but is specific to Bash and handle timeout more properly
+    with subprocess.Popen(["bash", "-c", cmd], **kwargs) as process:
+        try:
+            stdout, stderr = process.communicate(timeout=timeout)
+        except TimeoutExpired:
+            # kill the entire process group upon timeout
+            os.killpg(os.getpgid(process.pid), signal.SIGKILL)
+            process.wait()
+            raise
+        except:  # including KeyboardInterrupt, communicate handled that.
+            process.kill()
+            # we don't call process.wait() as .__exit__ does that for us.
+            raise
+        retcode = process.poll()
+    completed_process = subprocess.CompletedProcess(
+        process.args, retcode, stdout, stderr
     )
 
     # check return code
     if (
         check_returncode is not None
         and completed_process.returncode != check_returncode
     ):
@@ -107,14 +135,15 @@
         and warn_nonzero
     ):
         warnings.warn(
             f"Bash command `{cmd}` returned non-zero exit code: {completed_process.returncode}",
             RuntimeWarning,
         )
 
+    # potentially update the environment variables
     if update_env:
         envs = io.load(tempfile_update_env, io.Fmt.txtList)
         if update_env_clear_existing:
             os.environ.clear()
         for env in envs:
             key, value = env.split("=", 1)
             os.environ[key] = value
```

### Comparing `seutil-0.8.6/seutil/ds/graph_common.py` & `seutil-0.8.7/seutil/ds/graph_common.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/ds/lattice.py` & `seutil-0.8.7/seutil/ds/lattice.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/ds/trie.py` & `seutil-0.8.7/seutil/ds/trie.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/io.py` & `seutil-0.8.7/seutil/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,39 @@
+import bz2
 import collections
+import csv
 import dataclasses
+import gzip
 import inspect
 import io
 import json
+import lzma
 import os
 import pickle as pkl
 import pydoc
 import shutil
 import tempfile
 import warnings
 from enum import Enum
 from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    NamedTuple,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-    get_type_hints,
-)
+from typing import (Any, Callable, Dict, Iterator, List, Optional, Tuple, Type,
+                    TypeVar, Union, get_type_hints)
 
 import recordclass
 import typing_inspect
 import yaml
-import csv
 
 __all__ = [
     "cd",
     "rmdir",
     "rm",
     "mkdir",
     "mktmp",
     "mktmp_dir",
+    "fmts",
     "Fmt",
     "serialize",
     "deserialize",
     "load",
     "dump",
     "DeserializationError",
     "InfoLossWarning",
@@ -304,21 +297,21 @@
             del _DESERIALIZERS[clz]
             changed = True
     return changed
 
 
 def serialize(
     obj: TObj,
-    fmt: Optional["Fmt"] = None,
+    fmt: Optional["Formatter"] = None,
 ) -> TData:
     """
     Serializes an object into a data structure with only primitive types, list, dict.
     If fmt is provided, its formatting constraints are taken into account. Supported fmts:
     * json, jsonPretty, jsonNoSort, jsonList: dict only have str keys.
-    TODO: move this considering of formatting constraints to a spearate function, and let it automatically happen during dump; probably also add a reverse function which happens during load.
+    TODO: move this considering of formatting constraints to a separate function, and let it automatically happen during dump; probably also add a reverse function which happens during load.
 
     :param obj: the object to be serialized.
     :param fmt: (optional) the target format.
     :return: the serialized object.
     """
     # Examine the type of object and use the appropriate serialization method
     # Check for simple types first
@@ -343,15 +336,15 @@
         # List-like: uniform to list; recursively serialize content
         return [serialize(item, fmt) for item in obj]
     elif isinstance(obj, dict):
         # Dict: recursively serialize content
         ret = {serialize(k, fmt): serialize(v, fmt) for k, v in obj.items()}
 
         # Json-like formats constraint: dict key must be str
-        if fmt in [Fmt.json, Fmt.jsonPretty, Fmt.jsonNoSort, Fmt.jsonList]:
+        if fmt in [fmts.json, fmts.jsonPretty, fmts.jsonNoSort, fmts.jsonList]:
             ret = {str(k): v for k, v in ret.items()}
         return ret
     elif isinstance(obj, Enum):
         # Enum: use name
         return serialize(obj.name, fmt)
     elif _is_obj_record_class(obj):
         # RecordClass: convert to dict
@@ -679,118 +672,179 @@
 
 
 # ==========
 # file read and write
 # ==========
 
 
-class FmtProperty(NamedTuple):
+@dataclasses.dataclass(frozen=True)
+class Formatter:
     # The function used by dump
     # * line_mode=False:  takes a file-object and obj as input, writes the obj to the file-object
     # * line_mode=True:  takes an item in the obj as input (from for loop), returns one line of text *without* "\n"
     writer: Union[Callable[[io.IOBase, Any], None], Callable[[Any], str]]
 
     # The function used by load
     # * line_mode=False:  takes a file-object as input, reads the entire file and returns the obtained obj
     # * line_mode=True:  takes one line of text as input, returns the obtained obj
     reader: Union[Callable[[io.IOBase], Any], Callable[[str], Any]]
 
     # File extensions, used for format inference; the first extension is used for output
-    exts: List[str] = None
+    exts: Optional[List[str]] = None
 
     # If the file should be opened in binary mode
     binary: bool = False
 
-    # If the file should be read/writen one line at a time
+    # If the file should be read/written one line at a time
     line_mode: bool = False
 
     # If this format requires (de)serialization
     serialize: bool = False
 
 
-class Fmt(FmtProperty, Enum):
+class fmts:
     # === txt ===
-    txt = FmtProperty(
+    txt = Formatter(
         writer=lambda f, obj: f.write(str(obj)),
         reader=lambda f: f.read(),
         exts=["txt"],
     )
+
     # === pickle ===
-    pickle = FmtProperty(
+    pickle = Formatter(
         writer=lambda f, obj: pkl.dump(obj, f),
         reader=lambda f: pkl.load(f),
         exts=["pkl", "pickle"],
         binary=True,
     )
+
     # === json ===
-    json = FmtProperty(
+    json = Formatter(
         writer=lambda f, obj: json.dump(obj, f, sort_keys=True),
         reader=lambda f: json.load(f),
         exts=["json"],
         serialize=True,
     )
     # Use yaml loader to allow formatting errors (e.g., trailing commas), but cannot handle unprintable chars
-    jsonFlexible = json._replace(reader=lambda f: yaml.load(f, Loader=yaml.FullLoader))
+    jsonFlexible = dataclasses.replace(
+        json, reader=lambda f: yaml.load(f, Loader=yaml.FullLoader)
+    )
+    json_flexible = jsonFlexible
     # Pretty-print version with sorting keys
-    jsonPretty = json._replace(
-        writer=lambda f, obj: json.dump(obj, f, sort_keys=True, indent=4),
+    jsonPretty = dataclasses.replace(
+        json, writer=lambda f, obj: json.dump(obj, f, sort_keys=True, indent=4)
     )
+    json_pretty = jsonPretty
     # Pretty-print version without sorting keys
-    jsonNoSort = json._replace(
-        writer=lambda f, obj: json.dump(obj, f, indent=4),
+    jsonNoSort = dataclasses.replace(
+        json, writer=lambda f, obj: json.dump(obj, f, indent=4)
     )
+    json_no_sort = jsonNoSort
+
     # === jsonl (json list) ===
-    jsonList = FmtProperty(
+    jsonList = Formatter(
         writer=lambda item: json.dumps(item),
         reader=lambda line: json.loads(line),
         exts=["jsonl"],
         line_mode=True,
         serialize=True,
     )
+    json_list = jsonList
+
     # === text list ===
-    txtList = FmtProperty(
+    txtList = Formatter(
         writer=lambda item: str(item),
         reader=lambda line: line.replace("\n", ""),
         exts=["txt"],
         line_mode=True,
     )
+    txt_list = txtList
+
     # === yaml ===
-    yaml = FmtProperty(
+    yaml = Formatter(
         writer=lambda f, obj: yaml.dump(obj, f),
         reader=lambda f: yaml.load(f, Loader=yaml.FullLoader),
         exts=["yml", "yaml"],
         serialize=True,
     )
+
     # === csv list ===
-    csvList = FmtProperty(
+    csvList = Formatter(
+        # TODO: add a checker to ensure the input is list of list
         writer=lambda f, obj: csv.writer(f).writerows(obj),
         reader=lambda f: "".join([",".join(row) for row in csv.reader(f)]),
         exts=["csv"],
         serialize=True,
     )
+    csv_list = csvList
 
+    all_fmts = [v for v in locals().values() if isinstance(v, Formatter)]
 
-def infer_fmt_from_ext(ext: str, default: Optional[Fmt] = None) -> Fmt:
-    if ext.startswith("."):
-        ext = ext[1:]
-
-    for fmt in Fmt:
-        if fmt.exts is not None and ext in fmt.exts:
-            return fmt
 
-    if default is not None:
-        return default
-    else:
-        raise RuntimeError(f'Cannot infer format for extension "{ext}"')
+# backward compatibility
+Fmt = fmts
+
+
+@dataclasses.dataclass(frozen=True)
+class Compressor:
+    # open function alternative to os.open
+    open_fn: Callable
+
+    # File extensions, used for format inference; the first extension is used for output
+    exts: Optional[List[str]] = None
+
+
+class compressors:
+    # === gzip ===
+    gzip = Compressor(open_fn=gzip.open)
+
+    # === bz2 ===
+    bz2 = Compressor(open_fn=bz2.open)
+
+    # === lzma ===
+    lzma = Compressor(open_fn=lzma.open)
+
+    all_compressors = [v for v in locals().values() if isinstance(v, Compressor)]
+
+
+def _infer_from_path(path: Path) -> Tuple[Formatter, Compressor]:
+    name = path.name
+    fmt = None
+    compressor = None
+
+    if "." not in name:
+        return fmt, compressor
+    name, ext = name.rsplit(".", 1)
+
+    # detect possible compressor extension
+    for x in compressors.all_compressors:
+        if x.exts is not None and ext in x.exts:
+            compressor = x
+
+            # take the next extension
+            if "." not in name:
+                return fmt, compressor
+            name, ext = name.rsplit(".", 1)
+
+            break
+
+    # detect possible format extension
+    for x in fmts.all_fmts:
+        if x.exts is not None and ext in x.exts:
+            fmt = x
+            break
+
+    return fmt, compressor
 
 
 def dump(
     path: Union[str, Path],
     obj: object,
-    fmt: Optional[Fmt] = None,
+    fmt: Optional[Formatter] = None,
+    compressor: Optional[Compressor] = None,
     serialization: Optional[bool] = None,
     parents: bool = True,
     append: bool = False,
     exists_ok: bool = True,
     serialization_fmt_aware: bool = True,
 ) -> None:
     """
@@ -798,14 +852,15 @@
     The format is automatically inferred from the file name, if not otherwise specified.
     By default, serialization (i.e., converting to primitive types and data structures) is
     automatically performed for the formats that needs it (e.g., json).
 
     :param path: the path to save the file.
     :param obj: the object to be saved.
     :param fmt: the format of the file; if None (default), inferred from path.
+    :param compressor: the compression format of the file; if None (default), inferred from path.
     :param serialization: whether or not to serialize the object before saving:
         * True: always serialize;
         * None (default): only serialize for the formats that needs it;
         * False: never serialize.
     :param parents: what to do if parent directories of path do not exist:
         * True (default): automatically create them;
         * False: raise Exception.
@@ -816,32 +871,41 @@
     :param serialization_fmt_aware: let the serialization function be aware of the target
         format to fit its constraints (e.g., dictionaries in json format can only have
         str keys).
     """
     path = _unify_path(path)
 
     # Check path existence
-    if path.exists() and not exists_ok:
-        raise FileExistsError(str(path))
+    if path.exists():
+        if exists_ok and not append:
+            # make sure the existing file is removed in non-append mode
+            rm(path)
+        else:
+            raise FileExistsError(str(path))
 
     # Create parent directories
     if not path.parent.is_dir():
         if parents:
             path.parent.mkdir(parents=True)
         else:
             raise FileNotFoundError(str(path.parent))
 
     # Infer format
+    if fmt is None or compressor is None:
+        inferred_fmt, inferred_compressor = _infer_from_path(path)
+        if fmt is None:
+            fmt = inferred_fmt
+        if compressor is None:
+            compressor = inferred_compressor
+
     if fmt is None:
-        fmt = infer_fmt_from_ext(path.suffix)
+        raise RuntimeError(f"Cannot infer format for file {path}")
 
     if append and not fmt.line_mode:
-        raise RuntimeWarning(
-            f"Appending to a format that's not list-like ({fmt}) may result in invalid file"
-        )
+        raise RuntimeWarning(f"Cannot append to a non-list-like format ({fmt})")
 
     # Serialize (when appropriate)
     if serialization is None:
         serialization = fmt.serialize
 
     if serialization:
         obj = serialize(
@@ -849,95 +913,115 @@
             fmt=fmt if serialization_fmt_aware else None,
         )
 
     # Open file
     file_mode = "w" if not append else "a"
     if fmt.binary:
         file_mode += "b"
+    elif compressor is not None:
+        file_mode += "t"
 
-    with open(path, file_mode) as f:
+    open_fn = open if compressor is None else compressor.open_fn
+
+    with open_fn(path, file_mode) as f:
         # Write content
         if not fmt.line_mode:
             fmt.writer(f, obj)
         else:
             for item in obj:
                 # Removing all "\n" inside the line
                 f.write(fmt.writer(item).replace("\n", " ") + "\n")
 
 
 def load(
     path: Union[str, Path],
-    fmt: Optional[Fmt] = None,
+    fmt: Optional[Formatter] = None,
+    compressor: Optional[Compressor] = None,
     serialization: Optional[bool] = None,
     clz: Optional[Type] = None,
     error: str = "ignore",
     iter_line: bool = False,
 ) -> Union[object, Iterator[object]]:
     """
     Loads an object from a file.
     The format is automatically inferred from the file name, if not otherwise specified.
-    By default, if clz is given, deserialization (i.e., unpackingn from primitive types
+    By default, if clz is given, deserialization (i.e., unpacking from primitive types
     and data structures) is automatically performed for the formats that needs it (e.g., json).
 
     :param path: the path to load the object.
     :param fmt: the format of the file; if None (default), inferred from path.
+    :param compressor: the compression format of the file; if None (default), inferred from path.
     :param serialization: whether or not to deserialize the object after loading:
         * True: always serialize;
         * None (default): only serialize for the formats that needs it;
         * False: never serialize.
     :param clz: the class to use for deserialization; if None (default), deserialization is a no-op.
     :param error: what to do if deserialization fails:
         * raise: raise a DeserializationError.
         * ignore (default): return the data as-is.
     :param iter_line: whether to iterate over the lines of the file instead of loading the whole file.
     """
     path = _unify_path(path)
 
     # Infer format
+    if fmt is None or compressor is None:
+        inferred_fmt, inferred_compressor = _infer_from_path(path)
+        if fmt is None:
+            fmt = inferred_fmt
+        if compressor is None:
+            compressor = inferred_compressor
+
     if fmt is None:
-        fmt = infer_fmt_from_ext(path.suffix)
+        raise RuntimeError(f"Cannot infer format for file {path}")
 
     # Check arguments
     if iter_line and not fmt.line_mode:
-        raise RuntimeError(f"Cannot load format {fmt} file under line mode")
+        raise RuntimeWarning(f"Cannot iteratively load a non-list-like format ({fmt})")
 
     if serialization is None:
         serialization = fmt.serialize
 
     # Open file
     file_mode = "r"
     if fmt.binary:
         file_mode += "b"
+    elif compressor is not None:
+        file_mode += "t"
+
+    open_fn = open if compressor is None else compressor.open_fn
 
     # Load content
     if not fmt.line_mode:
-        with open(path, file_mode) as f:
+        with open_fn(path, file_mode) as f:
             obj = fmt.reader(f)
             if serialization:
                 obj = deserialize(obj, clz, error=error)
             return obj
     else:
-        iterator = LoadIterator(path, file_mode, fmt, serialization, clz, error)
+        iterator = LoadIterator(
+            path, file_mode, open_fn, fmt, serialization, clz, error
+        )
         if iter_line:
             return iterator
         else:
             return list(iterator)
 
 
 class LoadIterator(Iterator):
     def __init__(
         self,
         path: Path,
         file_mode: str,
-        fmt: FmtProperty,
+        open_fn: Callable,
+        fmt: Formatter,
         serialization: bool,
         clz: Optional[Type],
         error: str = "ignore",
     ):
-        self.fd = open(path, file_mode)
+        self.fd = open_fn(path, file_mode)
         self.fmt = fmt
         self.serialization = serialization
         self.clz = clz
         self.error = error
 
     def __next__(self):
         line = self.fd.readline()
```

### Comparing `seutil-0.8.6/seutil/latex/File.py` & `seutil-0.8.7/seutil/latex_old/File.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+import sys
 from pathlib import Path
-from typing import *
+from typing import Dict, List, Union
 
-from .. import IOUtils, LoggingUtils
+from .. import io, log
 from .Macro import Macro
 from .Table import Table
 
+logger = log.get_logger("latex.File")
 
-class File:
-
-    logger = LoggingUtils.get_logger("latex.File")
 
+class File:
     def __init__(self, path: Path, is_append: bool = False):
         """
         Creates a latex file, currently for numbers/macros or tables.
         :param path: the path to the file.
         :param is_append: if set to true, then append to any existing file; otherwise overwrite the file.
         """
         self.path: Path = path
         self.is_append: bool = is_append
 
         self.old_content: str = ""
         if self.is_append:
             if path.is_file():
-                self.old_content = IOUtils.load(path, "txt")
-        # end if, if
+                self.old_content = io.load(path, io.Fmt.txt)
 
         # Contents
         self.items: List[Union[str, Macro, Table]] = list()
         self.macros_indexed: Dict[str, Macro] = dict()
         return
 
     def append(self, line: str) -> "File":
@@ -35,55 +34,51 @@
         Appends one line of text into the file.
         """
         self.items.append(line)
         return self
 
     def append_macro(self, macro: Macro) -> "File":
         if macro.key in self.macros_indexed:
-            self.logger.warning(f"Redefining macro {macro.key}")
-        # end if
+            logger.warning(f"Redefining macro {macro.key}")
         self.macros_indexed[macro.key] = macro
         self.items.append(macro)
         return self
 
     def append_comment(self, line: str) -> "File":
         self.items.append("%% " + line)
         return self
 
     def save(self) -> None:
         content = self.old_content + "\n" + self.eval_content()
-        IOUtils.dump(self.path, content, "txt")
+        io.dump(self.path, content, io.Fmt.txt)
         return
 
     def eval_content(self) -> str:
         content_lines: List[str] = list()
         if not self.is_append:
             content_lines.append(self.autogen_notice())
         # end if
         for item in self.items:
             if isinstance(item, str):
                 content_lines.append(item)
             elif isinstance(item, Macro):
                 content_lines.append(item.eval_content(self.macros_indexed))
             else:
-                self.logger.warning("Skipping unsupported item")
-            # end if
-        # end for
-        return "\n".join(content_lines)+"\n"
+                logger.warning("Skipping unsupported item")
+        return "\n".join(content_lines) + "\n"
 
     def load_macros_from_file(self, file: Path) -> "File":
         self.macros_indexed.update(Macro.load_from_file(file))
         return self
 
     def __iadd__(self, other: Union[str, Macro]):
         if isinstance(other, str):
             self.append(other)
         elif isinstance(other, Macro):
             self.append_macro(other)
         else:
-            self.logger.warning("Skipping unsupported item")
-        # end if
+            logger.warning("Skipping unsupported item")
         return self
 
     @classmethod
     def autogen_notice(cls) -> str:
-        return "%% Automatically generated by pyutil.latex \n"
+        return f"%% Automatically generated by: {sys.argv[0]} \n"
```

### Comparing `seutil-0.8.6/seutil/latex/Macro.py` & `seutil-0.8.7/seutil/latex_old/Macro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from pathlib import Path
 import re
-from typing import *
-from .. import LoggingUtils, IOUtils
+from pathlib import Path
+from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
 
+from .. import io, log
 
-class Macro:
+logger = log.get_logger("latex.Macro")
 
-    logger = LoggingUtils.get_logger("latex.Macro")
+
+class Macro:
 
     T = TypeVar("T")
-    def __init__(self,
-                 key: str,
-                 value: Optional[T] = None,
-                 value_func: Optional[Callable[[Dict[str, "Macro"]], T]] = None,
-                 tostring_func: Optional[Callable[[T], str]] = None):
+
+    def __init__(
+        self,
+        key: str,
+        value: Optional[T] = None,
+        value_func: Optional[Callable[[Dict[str, "Macro"]], T]] = None,
+        tostring_func: Optional[Callable[[T], str]] = None,
+    ):
         """
         Defines a latex macro, using "\DefMacro{key}{value}".
         :param key: the key of the macro.
         :param value: the value of the macro, can be None.
         :param value_func: the (lazily evaluated) function to get the value of the macro, can be None. The function will receive one argument of a dictionary of {macro.key, macro} of macros defined in the same file, and should return the evaluated value.
         :param tostring_func: the function to format the value to string, can be None. If set to None, __str__() will be used.
         """
@@ -34,65 +38,62 @@
 
         :param macros_indexed: the indexed dictionary of {macro.key, macro}.
         :requires: not (self.value is None and self.value_func is None)
         :return: the string representation of the macro.
         """
         if self.value is None and self.value_func is None:
             raise ValueError("Cannot evaluate a macro without any value definition")
-        # end if
 
         if self.value_func is not None:
             self.value = self.value_func(macros_indexed)
-        # end if
-        self.logger.info(f"Macro {self.key} evaluates to {self.value}")
+        logger.info(f"Macro {self.key} evaluates to {self.value}")
 
         tostring_func = self.tostring_func if self.tostring_func is not None else str
         return f"\\DefMacro{{{self.key}}}{{{tostring_func(self.value)}}}"
 
     # Deprecated
     @classmethod
-    def define(cls, key: str, value_fmt: Union[str, Any], *values, **values_items) -> "Macro":
+    def define(
+        cls, key: str, value_fmt: Union[str, Any], *values, **values_items
+    ) -> "Macro":
         if len(values) != 0 or len(values_items) != 0:
             return Macro(key, value=value_fmt.format(*values, **values_items))
         else:
             return Macro(key, value=value_fmt)
-        # end if
 
     def use(self) -> str:
         latex_line = f"\\UseMacro{{{self.key}}}"
         return latex_line
 
     RE_DEF_MACRO = re.compile(r"\\DefMacro{(?P<key>[^}]+)}{(?P<value>[^}]*)}")
 
     @classmethod
     def load_from_file(cls, file: Path) -> Dict[str, "Macro"]:
         """
         Loads the macros from a latex file.
         Will convert the value of the macros to int or float, if possible.
+        TODO: does not work if the macro spans multiple lines.
 
         :param file: the latex file.
         :return: the indexed dictionary of {macro.key, macro}.
         """
         macros_indexed: Dict[str, Macro] = dict()
 
-        lines: List[str] = IOUtils.load(file, "txt").split("\n")
+        lines: List[str] = io.load(file, io.Fmt.txtList)
         for line in lines:
             match = cls.RE_DEF_MACRO.fullmatch(line.strip())
             if match is not None:
                 key = match.group("key")
                 value = match.group("value")
 
                 # Try to convert to int, then (if failing) float.
                 try:
                     value = int(value)
                 except:
                     try:
                         value = float(value)
                     except:
                         pass
-                # end try, try
 
                 macros_indexed[key] = Macro(key, value)
-            # end if
-        # end for
 
         return macros_indexed
```

### Comparing `seutil-0.8.6/seutil/latex/Table.py` & `seutil-0.8.7/seutil/latex_old/Table.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/log.py` & `seutil-0.8.7/seutil/log.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/maven.py` & `seutil-0.8.7/seutil/maven.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,19 @@
             logger.debug(f"pom.xml for {self.coordinate} already did {modification}")
             return
 
         pom = xmltodict.parse(
             su.io.load(self.project.dir / self.rel_path / "pom.xml", fmt=su.io.Fmt.txt)
         )
 
-        plugins = pom.get("build", {}).get("plugins", {}).get("plugin", [])
+        plugins = pom.get("project", {}).get("build", {}).get("plugins", {}).get("plugin", [])
+        if not isinstance(plugins, list):
+            plugins = [plugins]
+            pom.get("build", {}).get("plugins", {})["plugin"] = plugins
+            
         to_remove = None
         for i, plugin in enumerate(plugins):
             if plugin.get("artifactId") == artifact_id:
                 to_remove = i
                 break
         if to_remove is not None:
             del plugins[to_remove]
```

### Comparing `seutil-0.8.6/seutil/pbar.py` & `seutil-0.8.7/seutil/pbar.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil/project.py` & `seutil-0.8.7/seutil/project.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/seutil.egg-info/PKG-INFO` & `seutil-0.8.7/seutil.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seutil
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python utilities for SE research
 Home-page: https://github.com/pengyunie/seutil
 Author: Pengyu Nie
 Author-email: prodigy.sov@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -12,16 +12,15 @@
 Provides-Extra: dev
 Provides-Extra: io-3rd-party
 License-File: LICENSE
 
 Project ``seutil``
 ==================
 
-|PyPI| |GitHub release (latest by date including pre-releases)| |GitHub
-Workflow Status|
+|PyPI|_ |GitHubRelease|_ |GitHubWorkflow|_
 
 Python utilities for SE(+ML) research. This library stays reasonably
 up-to-date with the latest Python 3, currently 3.8.
 
 **Mature functions:**
 
 * bash: running Bash command; 
@@ -43,11 +42,14 @@
 * BashUtils: the previous version of bash; 
 * IOUtils: the previous version of io; 
 * CliUtils: for command line argument parsing without the need to declare each argument, recommended to use jsonargparse library; 
 * LoggingUtils: the previous version of log;
 
 Full documentation can be found at `readthedocs`_.
 
-.. |PyPI| image:: https://img.shields.io/pypi/v/seutil
-.. |GitHub release (latest by date including pre-releases)| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
-.. |GitHub Workflow Status| image:: https://img.shields.io/github/workflow/status/pengyunie/seutil/Python%20package
+.. |PyPI| image:: https://img.shields.io/pypi/v/seutil 
+.. _PyPI: https://pypi.org/project/seutil/
+.. |GitHubRelease| image:: https://img.shields.io/github/v/release/pengyunie/seutil?include_prereleases
+.. _GitHubRelease: https://github.com/pengyunie/seutil/releases
+.. |GitHubWorkflow| image:: https://img.shields.io/github/actions/workflow/status/pengyunie/seutil/python-package.yml?branch=master
+.. _GitHubWorkflow: https://github.com/pengyunie/seutil/actions/workflows/python-package.yml
 .. _readthedocs: https://seutil.readthedocs.io/en/latest/
```

### Comparing `seutil-0.8.6/tests/ds/test_lattice.py` & `seutil-0.8.7/tests/ds/test_lattice.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.6/tests/ds/test_trie.py` & `seutil-0.8.7/tests/ds/test_trie.py`

 * *Files identical despite different names*

