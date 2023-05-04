# Comparing `tmp/swh.journal-1.3.1.tar.gz` & `tmp/swh.journal-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.journal-1.3.1.tar", last modified: Mon Mar 13 16:23:11 2023, max compression
+gzip compressed data, was "dist/swh.journal-1.3.2.tar", last modified: Thu May  4 09:42:11 2023, max compression
```

## Comparing `swh.journal-1.3.1.tar` & `swh.journal-1.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-03-13 16:23:09.000000 swh.journal-1.3.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-03-13 16:23:09.000000 swh.journal-1.3.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-03-13 16:23:09.000000 swh.journal-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-13 16:23:09.000000 swh.journal-1.3.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-13 16:23:09.000000 swh.journal-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-03-13 16:23:09.000000 swh.journal-1.3.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-13 16:23:09.000000 swh.journal-1.3.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-03-13 16:23:09.000000 swh.journal-1.3.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-13 16:23:09.000000 swh.journal-1.3.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-03-13 16:23:11.000000 swh.journal-1.3.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-03-13 16:23:09.000000 swh.journal-1.3.1/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-03-13 16:23:09.000000 swh.journal-1.3.1/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-03-13 16:23:09.000000 swh.journal-1.3.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-13 16:23:09.000000 swh.journal-1.3.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-03-13 16:23:09.000000 swh.journal-1.3.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-03-13 16:23:09.000000 swh.journal-1.3.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-03-13 16:23:09.000000 swh.journal-1.3.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      277 2023-03-13 16:23:09.000000 swh.journal-1.3.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-13 16:23:11.000000 swh.journal-1.3.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-03-13 16:23:09.000000 swh.journal-1.3.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh/journal/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17345 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     7859 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) docker     (999)    17937 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-03-13 16:23:09.000000 swh.journal-1.3.1/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      127 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-13 16:23:11.000000 swh.journal-1.3.1/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-03-13 16:23:09.000000 swh.journal-1.3.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-04 09:42:08.000000 swh.journal-1.3.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-04 09:42:08.000000 swh.journal-1.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-04 09:42:08.000000 swh.journal-1.3.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-04 09:42:08.000000 swh.journal-1.3.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-04 09:42:08.000000 swh.journal-1.3.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-04 09:42:08.000000 swh.journal-1.3.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-04 09:42:11.000000 swh.journal-1.3.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-05-04 09:42:08.000000 swh.journal-1.3.2/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-05-04 09:42:08.000000 swh.journal-1.3.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-04 09:42:08.000000 swh.journal-1.3.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-05-04 09:42:08.000000 swh.journal-1.3.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      277 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-04 09:42:11.000000 swh.journal-1.3.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-05-04 09:42:08.000000 swh.journal-1.3.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17402 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     7859 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) docker     (999)    18361 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      127 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-05-04 09:42:08.000000 swh.journal-1.3.2/tox.ini
```

### Comparing `swh.journal-1.3.1/.pre-commit-config.yaml` & `swh.journal-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/CODE_OF_CONDUCT.md` & `swh.journal-1.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/LICENSE` & `swh.journal-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/PKG-INFO` & `swh.journal-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.1
+Version: 1.3.2
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.1/README.md` & `swh.journal-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/docs/example-journal-client.py` & `swh.journal-1.3.2/docs/example-journal-client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/docs/journal-clients.rst` & `swh.journal-1.3.2/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/setup.py` & `swh.journal-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/client.py` & `swh.journal-1.3.2/swh/journal/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,17 @@
             logger.debug("Consumer settings:")
             for k, v in consumer_settings.items():
                 if k in filtered_keys:
                     v = "**filtered**"
 
                 logger.debug("    %s: %s", k, v)
 
-        self.statsd = Statsd(namespace="swh_journal_client")
+        self.statsd = Statsd(
+            namespace="swh_journal_client", constant_tags={"group": group_id}
+        )
 
         self.consumer = Consumer(consumer_settings)
         if privileged:
             privileged_prefix = f"{prefix}_privileged"
         else:  # do not attempt to subscribe to privileged topics
             privileged_prefix = f"{prefix}"
         existing_topics = [
```

### Comparing `swh.journal-1.3.1/swh/journal/pytest_plugin.py` & `swh.journal-1.3.2/swh/journal/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/serializers.py` & `swh.journal-1.3.2/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/journal_data.py` & `swh.journal-1.3.2/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_client.py` & `swh.journal-1.3.2/swh/journal/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,54 +110,75 @@
         prefix=kafka_prefix,
         on_eof=EofBehavior.STOP,
     )
     client.statsd._socket = FakeSocket()
     worker_fn = MagicMock()
     client.process(worker_fn)
 
+    group_tag = f"#group:{kafka_consumer_group}"
+
     worker_fn.assert_called_once_with({"revision": [REV]})
     assert client.statsd.namespace == "swh_journal_client"
     # check at least initialization of the status gauge is ok
-    assert client.statsd.socket.recv() == "swh_journal_client.status:0|g|#status:idle"
     assert (
         client.statsd.socket.recv()
-        == "swh_journal_client.status:0|g|#status:processing"
+        == f"swh_journal_client.status:0|g|{group_tag},status:idle"
     )
     assert (
-        client.statsd.socket.recv() == "swh_journal_client.status:0|g|#status:waiting"
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:0|g|{group_tag},status:processing"
+    )
+    assert (
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:0|g|{group_tag},status:waiting"
     )
     # processing the batch with only one message
-    assert client.statsd.socket.recv() == "swh_journal_client.status:1|g|#status:idle"
-    assert client.statsd.socket.recv() == "swh_journal_client.status:0|g|#status:idle"
     assert (
-        client.statsd.socket.recv() == "swh_journal_client.status:1|g|#status:waiting"
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:1|g|{group_tag},status:idle"
+    )
+    assert (
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:0|g|{group_tag},status:idle"
+    )
+    assert (
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:1|g|{group_tag},status:waiting"
     )
     assert (
-        client.statsd.socket.recv() == "swh_journal_client.status:0|g|#status:waiting"
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:0|g|{group_tag},status:waiting"
     )
     assert (
         client.statsd.socket.recv()
-        == "swh_journal_client.status:1|g|#status:processing"
+        == f"swh_journal_client.status:1|g|{group_tag},status:processing"
     )
     assert (
         client.statsd.socket.recv()
-        == "swh_journal_client.status:0|g|#status:processing"
+        == f"swh_journal_client.status:0|g|{group_tag},status:processing"
+    )
+    assert (
+        client.statsd.socket.recv()
+        == f"swh_journal_client.status:1|g|{group_tag},status:idle"
     )
-    assert client.statsd.socket.recv() == "swh_journal_client.status:1|g|#status:idle"
     # from there, status messages can be mixed with a few other ones...
     assert (
-        b"swh_journal_client.handle_message_total:1|c" in client.statsd.socket.payloads
+        f"swh_journal_client.handle_message_total:1|c|{group_tag}".encode()
+        in client.statsd.socket.payloads
+    )
+    assert (
+        f"swh_journal_client.stop_total:1|c|{group_tag}".encode()
+        in client.statsd.socket.payloads
     )
-    assert b"swh_journal_client.stop_total:1|c" in client.statsd.socket.payloads
     # and some waiting/idle forth and back may have happened, so only check the
     # last 3 messages resetting the status gauges)
     assert list(client.statsd.socket.payloads)[-3:] == [
-        b"swh_journal_client.status:0|g|#status:idle",
-        b"swh_journal_client.status:0|g|#status:processing",
-        b"swh_journal_client.status:0|g|#status:waiting",
+        f"swh_journal_client.status:0|g|{group_tag},status:idle".encode(),
+        f"swh_journal_client.status:0|g|{group_tag},status:processing".encode(),
+        f"swh_journal_client.status:0|g|{group_tag},status:waiting".encode(),
     ]
 
 
 @pytest.mark.parametrize(
     "count,legacy_eof", [(1, True), (2, True), (1, False), (2, False)]
 )
 def test_client_stop_after_objects(
```

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_inmemory.py` & `swh.journal-1.3.2/swh/journal/tests/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_kafka_writer.py` & `swh.journal-1.3.2/swh/journal/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_pytest_plugin.py` & `swh.journal-1.3.2/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_serializers.py` & `swh.journal-1.3.2/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/tests/test_stream.py` & `swh.journal-1.3.2/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/writer/__init__.py` & `swh.journal-1.3.2/swh/journal/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/writer/inmemory.py` & `swh.journal-1.3.2/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/writer/interface.py` & `swh.journal-1.3.2/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/writer/kafka.py` & `swh.journal-1.3.2/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh/journal/writer/stream.py` & `swh.journal-1.3.2/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/swh.journal.egg-info/PKG-INFO` & `swh.journal-1.3.2/swh.journal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.1
+Version: 1.3.2
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.1/swh.journal.egg-info/SOURCES.txt` & `swh.journal-1.3.2/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.1/tox.ini` & `swh.journal-1.3.2/tox.ini`

 * *Files identical despite different names*

