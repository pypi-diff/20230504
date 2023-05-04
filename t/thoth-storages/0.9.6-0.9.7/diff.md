# Comparing `tmp/thoth-storages-0.9.6.tar.gz` & `tmp/thoth-storages-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thoth-storages-0.9.6.tar", last modified: Thu Feb 14 06:27:07 2019, max compression
+gzip compressed data, was "dist/thoth-storages-0.9.7.tar", last modified: Wed Mar 20 09:57:17 2019, max compression
```

## Comparing `thoth-storages-0.9.6.tar` & `thoth-storages-0.9.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       56 2018-12-03 14:32:17.000000 thoth-storages-0.9.6/MANIFEST.in
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1571 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/PKG-INFO
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1057 2019-01-09 13:09:37.000000 thoth-storages-0.9.6/README.rst
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       47 2018-11-13 08:55:05.000000 thoth-storages-0.9.6/requirements-test.txt
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      129 2018-12-03 13:25:12.000000 thoth-storages-0.9.6/requirements.txt
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       38 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/setup.cfg
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1945 2019-02-01 15:39:40.000000 thoth-storages-0.9.6/setup.py
-drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth/
-drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth/storages/
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1609 2019-02-14 06:27:02.000000 thoth-storages-0.9.6/thoth/storages/__init__.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      965 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/advisers.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      984 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/advisers_cache.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      961 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/analyses.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1258 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/analyses_by_digest.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1187 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/analyses_cache.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1078 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/base.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2819 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/buildlogs.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     6726 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/ceph.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1545 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/ceph_cache.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1238 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/dependency_monkey_reports.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1212 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/exceptions.py
-drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth/storages/graph/
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      551 2019-02-07 10:46:17.000000 thoth-storages-0.9.6/thoth/storages/graph/__init__.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1669 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/graph/cache.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)    73601 2019-02-14 06:27:02.000000 thoth-storages-0.9.6/thoth/storages/graph/janusgraph.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)    11950 2019-02-11 14:21:51.000000 thoth-storages-0.9.6/thoth/storages/graph/models.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     4121 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/graph/models_base.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     6586 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/graph/utils.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1156 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/inspections.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      958 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/observations.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      954 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/provenance.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1011 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/provenance_cache.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     4280 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/result_base.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2393 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/result_schema.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      961 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/solvers.py
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     8673 2019-02-11 08:51:33.000000 thoth-storages-0.9.6/thoth/storages/sync.py
-drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1571 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/PKG-INFO
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1087 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/SOURCES.txt
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        1 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/dependency_links.txt
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        1 2018-11-20 09:33:58.000000 thoth-storages-0.9.6/thoth_storages.egg-info/not-zip-safe
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      129 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/requires.txt
--rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        6 2019-02-14 06:27:07.000000 thoth-storages-0.9.6/thoth_storages.egg-info/top_level.txt
+drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       56 2018-12-03 14:32:17.000000 thoth-storages-0.9.7/MANIFEST.in
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     3318 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/PKG-INFO
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2492 2019-03-15 09:39:38.000000 thoth-storages-0.9.7/README.rst
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       47 2018-11-13 08:55:05.000000 thoth-storages-0.9.7/requirements-test.txt
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      129 2018-12-03 13:25:12.000000 thoth-storages-0.9.7/requirements.txt
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)       38 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/setup.cfg
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2072 2019-03-15 09:39:38.000000 thoth-storages-0.9.7/setup.py
+drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth/
+drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth/storages/
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1661 2019-03-18 10:09:30.000000 thoth-storages-0.9.7/thoth/storages/__init__.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      965 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/advisers.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      984 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/advisers_cache.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      961 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/analyses.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1258 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/analyses_by_digest.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1187 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/analyses_cache.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1078 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/base.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2819 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/buildlogs.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     6726 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/ceph.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1545 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/ceph_cache.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1238 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/dependency_monkey_reports.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1212 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/exceptions.py
+drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth/storages/graph/
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      551 2019-02-07 10:46:17.000000 thoth-storages-0.9.7/thoth/storages/graph/__init__.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1669 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/graph/cache.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)    79820 2019-03-20 09:56:45.000000 thoth-storages-0.9.7/thoth/storages/graph/janusgraph.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)    13113 2019-03-18 14:23:59.000000 thoth-storages-0.9.7/thoth/storages/graph/models.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     4121 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/graph/models_base.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     6586 2019-03-16 12:26:21.000000 thoth-storages-0.9.7/thoth/storages/graph/utils.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1156 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/inspections.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      958 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/observations.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      954 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/provenance.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1011 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/provenance_cache.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     4280 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/result_base.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     2393 2019-02-11 08:51:33.000000 thoth-storages-0.9.7/thoth/storages/result_schema.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1177 2019-02-20 10:14:20.000000 thoth-storages-0.9.7/thoth/storages/solvers.py
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)    10191 2019-02-20 07:08:28.000000 thoth-storages-0.9.7/thoth/storages/sync.py
+drwxrwxr-x   0 fpokorny (20905) fpokorny (20905)        0 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     3318 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/PKG-INFO
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)     1087 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/SOURCES.txt
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        1 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/dependency_links.txt
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        1 2019-03-16 15:25:59.000000 thoth-storages-0.9.7/thoth_storages.egg-info/not-zip-safe
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)      129 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/requires.txt
+-rw-rw-r--   0 fpokorny (20905) fpokorny (20905)        6 2019-03-20 09:57:17.000000 thoth-storages-0.9.7/thoth_storages.egg-info/top_level.txt
```

### Comparing `thoth-storages-0.9.6/PKG-INFO` & `thoth-storages-0.9.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,82 @@
 Metadata-Version: 1.0
 Name: thoth-storages
-Version: 0.9.6
+Version: 0.9.7
 Summary: Storage and database adapters available in project Thoth
 Home-page: UNKNOWN
 Author: Fridolin Pokorny
 Author-email: fridolin@redhat.com
 License: GPLv3+
-Description: thoth-storages
+Description: Thoth Storages
         --------------
-        This repo provides a library called
-        `thoth-storages <https://pypi.org/project/thoth-storages>`_.
-        The library exposes core queries and methods for JanusGraph database as well
-        as adapters for manipulating with Ceph via its S3 compatible API.
+        
+        This library provides a library called `thoth-storages
+        <https://pypi.org/project/thoth-storages>`_ used in project `Thoth
+        <https://thoth-station.ninja>`_.  The library exposes core queries and methods
+        for JanusGraph database as well as adapters for manipulating with Ceph via its
+        S3 compatible API.
         
         Installation and Usage
         ======================
         
-        The library can be installed via pip or pipenv:
+        The library can be installed via pip or Pipenv from
+        `PyPI <https://pypi.org/project/thoth-storages>`_:
         
         .. code-block:: console
         
            pipenv install thoth-storages
         
         The library does not provide any CLI, it is rather a low level library
         supporting other parts of Thoth.
         
         You can run prepared testsuite via the following command:
         
         .. code-block:: console
         
-            pipenv install --dev
-            pipenv run python3 setup.py test
+          pipenv install --dev
+          pipenv run python3 setup.py test
+        
+          # To generate docs:
+          pipenv run python3 setup.py build_sphinx
+        
+        Automatically generate schema for Graph database
+        ================================================
+        
+        To automatically generate schema for the graph database from models defined in
+        this module, run:
+        
+        .. code-block:: console
+        
+           # Install dev dependencies which include goblinoid:
+           pipenv install --dev
+        
+           # From root of this repository:
+           PYTHONPATH=. pipenv run goblinoid -m thoth.storages.graph.models -i ALL_MODELS
         
+           # Or to directly adjust used schema:
+           export PYTHONPATH=.
+           # Or export also ../goblinoid to have the most recent Goblinoid version (devel from master).
+           export PYTHONPATH=.:../goblinoid
+           pipenv run goblinoid -m thoth.storages.graph.models -i ALL_MODELS --output-file ../janusgraph-thoth-config/scripts/init.groovy --index-file ../janusgraph-thoth-config/scripts/indexes.groovy.template
+        
+        After running this command, there will be present file called `init.groovy`
+        which is generated automatically from models stated in `ALL_MODELS` (see file
+        thoth/storages/graph/models.py) as well as with indexes as configured in the
+        indexes.groovy.template (placed into a single file to run it in one
+        transaction).
+        
+        See `goblinoid <https://github.com/thoth-station/goblinoid>`_ for more info
+        on how to configure models generation.
         
         Known Issues
         ============
         
         - Gremlin queries are hanging:
         
-           When using :code:`aiogremlin==3.3.1` (despite being not part of our specification, it might happen that another library overrides that dependency), gremlin queries might _hang indeffinitely_ without throwing any error in Jupyter Notebooks. Make sure to check that correct version of :code:`aiogremlin` is installed.
+           When using :code:`aiogremlin==3.3.1` (despite being not part of our
+           specification, it might happen that another library overrides that
+           dependency), gremlin queries might hang indeffinitely without throwing any
+           error in Jupyter Notebooks. Make sure to check that correct version of
+           :code:`aiogremlin` is installed.
+        
         
 Platform: UNKNOWN
```

### Comparing `thoth-storages-0.9.6/setup.py` & `thoth-storages-0.9.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,25 +43,30 @@
         self.test_args = []
         self.test_suite = True
 
     def run_tests(self):
         import pytest
         sys.exit(pytest.main(self.pytest_args))
 
-
+VERSION = get_version()
 setup(
     name='thoth-storages',
-    version=get_version(),
+    version=VERSION,
     description='Storage and database adapters available in project Thoth',
     long_description=Path('README.rst').read_text(),
     author='Fridolin Pokorny',
     author_email='fridolin@redhat.com',
     license='GPLv3+',
     packages=[
         'thoth.storages',
         'thoth.storages.graph'
     ],
     zip_safe=False,
     install_requires=get_install_requires(),
     tests_require=get_test_requires(),
     cmdclass={'test': Test},
+    command_options={
+        'build_sphinx': {
+            'version': ('setup.py', VERSION),
+        }
+    }
 )
```

### Comparing `thoth-storages-0.9.6/thoth/storages/__init__.py` & `thoth-storages-0.9.7/thoth/storages/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 from .provenance_cache import ProvenanceCacheStore
 from .result_schema import RESULT_SCHEMA
 from .solvers import SolverResultsStore
 from .sync import sync_adviser_documents
 from .sync import sync_analysis_documents
 from .sync import sync_solver_documents
 from .sync import sync_inspection_documents
+from .sync import sync_provenance_checker_documents
 from .analyses_by_digest import AnalysisByDigest
 
 
 __name__ = "thoth-storages"
-__version__ = "0.9.6"
+__version__ = "0.9.7"
```

### Comparing `thoth-storages-0.9.6/thoth/storages/advisers.py` & `thoth-storages-0.9.7/thoth/storages/advisers.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/advisers_cache.py` & `thoth-storages-0.9.7/thoth/storages/advisers_cache.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/analyses.py` & `thoth-storages-0.9.7/thoth/storages/analyses.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/analyses_by_digest.py` & `thoth-storages-0.9.7/thoth/storages/analyses_by_digest.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/analyses_cache.py` & `thoth-storages-0.9.7/thoth/storages/analyses_cache.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/base.py` & `thoth-storages-0.9.7/thoth/storages/base.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/buildlogs.py` & `thoth-storages-0.9.7/thoth/storages/buildlogs.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/ceph.py` & `thoth-storages-0.9.7/thoth/storages/ceph.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/ceph_cache.py` & `thoth-storages-0.9.7/thoth/storages/ceph_cache.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/dependency_monkey_reports.py` & `thoth-storages-0.9.7/thoth/storages/dependency_monkey_reports.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/exceptions.py` & `thoth-storages-0.9.7/thoth/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/__init__.py` & `thoth-storages-0.9.7/thoth/storages/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/cache.py` & `thoth-storages-0.9.7/thoth/storages/graph/cache.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/janusgraph.py` & `thoth-storages-0.9.7/thoth/storages/graph/janusgraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 from itertools import chain
 from collections import ChainMap
 
 import uvloop
 from aiogremlin.process.graph_traversal import AsyncGraphTraversal
 from gremlin_python.process.traversal import Order
 from gremlin_python.process.traversal import without
+from gremlin_python.process.traversal import within
 from gremlin_python.process.traversal import gt
 from gremlin_python.process.graph_traversal import inE
 from gremlin_python.process.graph_traversal import id as id_
 from gremlin_python.process.graph_traversal import outE
 from gremlin_python.process.graph_traversal import constant
-from gremlin_python.process.graph_traversal import flatMap
+from gremlin_python.process.graph_traversal import valueMap
 from goblin import Goblin
 
 from thoth.common import datetime_str2timestamp
 from thoth.common import timestamp2datetime
 from thoth.common import OpenShift
 
 from ..base import StorageBase
@@ -61,30 +62,33 @@
 from .models import PythonPackageVersion
 from .models import Requires
 from .models import RunsIn
 from .models import PythonPackageIndex
 from .models import RunsOn
 from .models import BuildsIn
 from .models import BuildsOn
-from .models import BuildtimeEnvironment
 from .models import RPMPackageVersion
 from .models import RPMRequirement
-from .models import RuntimeEnvironment
+from .models import EnvironmentBase
+from .models import RuntimeEnvironment as RuntimeEnvironmentModel
+from .models import BuildtimeEnvironment as BuildtimeEnvironmentModel
 from .models import HardwareInformation
 from .models import Solved
 from .models import AdviserSoftwareStack
+from .models import Advised
 from .models import InspectionSoftwareStack
 from .models import UserSoftwareStack
 from .models import SoftwareStackBase
 from .models import CreatesStack
 
 # from .utils import enable_edge_cache
 from .utils import enable_vertex_cache
 from ..advisers import AdvisersResultsStore
 from ..analyses import AnalysisResultsStore
+from ..provenance import ProvenanceResultsStore
 from ..solvers import SolverResultsStore
 
 _LOGGER = logging.getLogger(__name__)
 
 # http://goblin.readthedocs.io/en/latest/performance.html#use-uvloop
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
@@ -206,48 +210,38 @@
         if not result:
             raise NotFoundError(f"Analysis with analysis document if {analysis_document_id} was not found")
 
         result["analysis_datetime"] = timestamp2datetime(result["analysis_datetime"])
 
         return result
 
-    def register_python_package_index(
-        self, url: str, *, warehouse_api_url: str = None, verify_ssl: bool = True, warehouse: bool = False
-    ) -> typing.Tuple[PythonPackageIndex, bool]:
-        """Return a list of available Python package indexes."""
-        python_package_index = PythonPackageIndex.from_properties(
-            url=url, warehouse_api_url=warehouse_api_url, verify_ssl=verify_ssl, warehouse=warehouse
-        )
-        existed = python_package_index.get_or_create(self.g)
-        return python_package_index, existed
-
     def runtime_environment_listing(self, start_offset: int = 0, count: int = 100) -> list:
         """Get listing of runtime environments available."""
         query = (
             self.g.V()
-            .has("__label__", RuntimeEnvironment.__label__)
+            .has("__label__", RuntimeEnvironmentModel.__label__)
             .has("__type__", "vertex")
-            .values("runtime_environment_name")
+            .values("environment_name")
             .dedup()
             .order()
             .range(start_offset, start_offset + count)
             .toList()
         )
 
         return asyncio.get_event_loop().run_until_complete(query)
 
     def runtime_environment_analyses_listing(
         self, runtime_environment_name: str, start_offset: int = 0, count: int = 100
     ) -> list:
         """Get listing of analyses available for the given environment."""
         query = (
             self.g.V()
-            .has("__label__", RuntimeEnvironment.__label__)
+            .has("__label__", RuntimeEnvironmentModel.__label__)
             .has("__type__", "vertex")
-            .has("runtime_environment_name", runtime_environment_name)
+            .has("environment_name", runtime_environment_name)
             .inE()
             .has("__label__", IsPartOf.__label__)
             .has("__type__", "edge")
             .order()
             .by("analysis_datetime", Order.decr)
             .project("analysis_datetime", "analysis_document_id", "analyzer_name", "analyzer_version")
             .by("analysis_datetime")
@@ -261,17 +255,17 @@
 
         entries = asyncio.get_event_loop().run_until_complete(query)
 
         if not entries:
             # TODO: we could optimize this into a single query
             query = (
                 self.g.V()
-                .has("__label__", RuntimeEnvironment.__label__)
+                .has("__label__", RuntimeEnvironmentModel.__label__)
                 .has("__type__", "vertex")
-                .has("runtime_environment_name", runtime_environment_name)
+                .has("environment_name", runtime_environment_name)
                 .count()
                 .next()
             )
 
             count = asyncio.get_event_loop().run_until_complete(query)
             if not count:
                 raise NotFoundError(f"No analyses found for runtime environment {runtime_environment_name!r}")
@@ -287,17 +281,17 @@
         Select the newest analysis if no document id is present.
         """
         loop = asyncio.get_event_loop()
 
         if not analysis_document_id:
             analysis_document_id = loop.run_until_complete(
                 self.g.V()
-                .has("__label__", RuntimeEnvironment.__label__)
+                .has("__label__", RuntimeEnvironmentModel.__label__)
                 .has("__type__", "vertex")
-                .has("runtime_environment_name", runtime_environment_name)
+                .has("environment_name", runtime_environment_name)
                 .inE()
                 .has("__label__", IsPartOf.__label__)
                 .order()
                 .by("analysis_datetime", Order.decr)
                 .range(0, 1)
                 .valueMap()
                 .select("analysis_document_id")
@@ -305,17 +299,17 @@
             )
 
             if not analysis_document_id:
                 raise NotFoundError(f"No entries for runtime environment {runtime_environment_name!r} found")
 
         query = (
             self.g.V()
-            .has("__label__", RuntimeEnvironment.__label__)
+            .has("__label__", RuntimeEnvironmentModel.__label__)
             .has("__type__", "vertex")
-            .has("runtime_environment_name", runtime_environment_name)
+            .has("environment_name", runtime_environment_name)
             .coalesce(
                 inE().has("__label__", IsPartOf.__label__).has("analysis_document_id", analysis_document_id).outV(),
                 constant(False),
             )
             .toList()
         )
 
@@ -380,121 +374,137 @@
         # present at the same time. The query continues for all N packages giving
         # back all software stacks where all N packages are present (note there can
         # be also other packages).
         if len(packages) == 0:
             raise ValueError("Cannot query for a stack with no packages.")
 
         package_name, package_version, index_url = packages[0]
-        query = self.g.V().has('__type__', 'vertex') \
-            .has('__label__', 'python_package_version') \
-            .has('ecosystem', 'pypi') \
-            .has('package_version', package_version) \
-            .has('package_name', package_name) \
-            .has('index_url', index_url) \
-            .outE() \
-            .has('__type__', 'edge') \
-            .has('__label__', 'creates_stack') \
-            .inV().has('__type__', 'vertex').has('__label__', 'software_stack')
+        query = (
+            self.g.V()
+            .has("__type__", "vertex")
+            .has("__label__", "python_package_version")
+            .has("ecosystem", "pypi")
+            .has("package_version", package_version)
+            .has("package_name", package_name)
+            .has("index_url", index_url)
+            .outE()
+            .has("__type__", "edge")
+            .has("__label__", "creates_stack")
+            .inV()
+            .has("__type__", "vertex")
+            .has("__label__", InspectionSoftwareStack.__label__)
+        )
 
         for package_name, package_version, index_url in packages[1:]:
-            query = query.inE() \
-                .has('__type__', 'edge').has('__label__', 'creates_stack') \
-                .outV() \
-                .has('__type__', 'vertex') \
-                .has('__label__', 'python_package_version') \
-                .has('ecosystem', 'pypi') \
-                .has('package_version', package_version) \
-                .has('package_name', package_name) \
-                .has('index_url', index_url) \
-                .outE() \
-                .has('__type__', 'edge') \
-                .has('__label__', 'creates_stack') \
-                .inV().has('__type__', 'vertex').has('__label__', 'software_stack')
+            query = (
+                query.inE()
+                .has("__type__", "edge")
+                .has("__label__", "creates_stack")
+                .outV()
+                .has("__type__", "vertex")
+                .has("__label__", "python_package_version")
+                .has("ecosystem", "pypi")
+                .has("package_version", package_version)
+                .has("package_name", package_name)
+                .has("index_url", index_url)
+                .outE()
+                .has("__type__", "edge")
+                .has("__label__", "creates_stack")
+                .inV()
+                .has("__type__", "vertex")
+                .has("__label__", InspectionSoftwareStack.__label__)
+            )
 
         return query
 
     def get_software_stacks(self, packages: typing.List[tuple]) -> typing.List[SoftwareStackBase]:
         """Get all stacks that include the given set of packages.
 
         Packages in stacks returned are superset of packages in the original set of
         packages given in parameters - meaning a returned stack has packages as
         provided in the parameter, but can also have additional packages.
         """
         query = self._get_stack(packages)
         return asyncio.get_event_loop().run_until_complete(query.toList())
 
-    @staticmethod
-    def _compute_python_package_version_avg_performance_on_hw(
-        query, hardware_specs: dict, runtime_environment_name: str
-    ) -> float:
-        """Extend the avg performance query so that there is taken into account hardware we run on."""
-        query = query.inV().has("__label__", RuntimeEnvironment.__label__)
-
-        if runtime_environment_name:
-            query = query.has("runtime_environment_name", runtime_environment_name)
-
-        query = query.outE().has("__label__", RunsOn.__label__).inV().has("__label__", HardwareInformation.__label__)
-
-        for attribute_name, attribute_value in hardware_specs.items():
-            query = query.has(attribute_name, attribute_value)
-
-        query = query.inE().has("__label__", "runs_on").values("performance_index").mean().next()
-
-        return asyncio.get_event_loop().run_until_complete(query)
-
     def compute_python_package_version_avg_performance(
-        self,
-        packages: typing.List[tuple],
-        *,
-        runtime_environment_name: str = None,
-        hardware_specs: dict = None,
-    ) -> float:
-        """Get average performance of Python packages on the given runtime environment.
+        self, packages: typing.List[tuple], *, runtime_environment: dict = None, hardware_specs: dict = None
+    ) -> typing.Optional[float]:
+        """Get average performance of Python packages on the given runtime environment with hardware specs.
 
         We derive this average performance based on software stacks we have
         evaluated on the given runtime environment including the given
         package in specified version. There are also included stacks that
         failed for some reason that have negative performance impact on the overall value.
 
         There are considered software stacks that include packages listed,
         they can however include also other packages.
 
         Optional parameters additionally slice results - e.g. if runtime_environment is set,
-        it picks only resutls that match the given parameters criteria.
+        it picks only results that match the given parameters criteria.
         """
         query = self._get_stack(packages)
-        query = query.outE().has("__label__", RunsIn.__label__)
+        software_stack_ids = asyncio.get_event_loop().run_until_complete(query.id().toList())
+
+        if not software_stack_ids:
+            # No software stacks for the given package set found.
+            return None
+
+        query = None
+        if hardware_specs:
+            query = self.g.V().has("__label__", HardwareInformation.__label__).has("__type__", "vertex")
+            for key, value in hardware_specs.items():
+                query = query.has(key, value)
 
-        if runtime_environment_name and not hardware_specs:
             query = (
-                query.inV()
-                .has("__label__", RuntimeEnvironment.__label__)
-                .has("runtime_environment_name", runtime_environment_name)
+                query
                 .inE()
-                .has("__label__", RunsIn.__label__)
+                .has("__label__", "runs_on")
+                .has("__type__", "edge")
+                .outV()
+                .has("__label__", RuntimeEnvironmentModel.__label__)
+                .has("__type__", "vertex")
             )
 
-        if hardware_specs:
-            # We pass runtime environment name to optimize traversal (no need to go back).
-            return self._compute_python_package_version_avg_performance_on_hw(
-                query, hardware_specs, runtime_environment_name
-            )
+        if not query:
+            # No hardware specs supplied, start in a runtime environment.
+            query = self.g.V().has("__label__", RuntimeEnvironmentModel.__label__).has("__type__", "vertex")
+
+        if runtime_environment:
+            # We have a specific runtime environment, add attributes of it to the query.
+            for key, value in runtime_environment.items():
+                query = query.has(key, value)
+
+        query = (
+            query
+            .inE()
+            .has("__label__", "runs_in")
+            .has("__type__", "edge")
+            .as_("runs_in_edge")
+            .has("performance_index")
+            .outV()
+            .has("__label__", InspectionSoftwareStack.__label__)
+            .has("__type__", "vertex")
+            .id().is_(within(software_stack_ids))
+            .select("runs_in_edge")
+            .dedup()
+            .values("performance_index").mean().next()
+        )
 
-        query = query.values("performance_index").mean().next()
         return asyncio.get_event_loop().run_until_complete(query)
 
     def get_all_versions_python_package(
-            self,
-            package_name: str,
-            index_url: str = None,
-            *,
-            os_name: str = None,
-            os_version: str = None,
-            python_version: str = None,
-            without_error: bool = False,
+        self,
+        package_name: str,
+        index_url: str = None,
+        *,
+        os_name: str = None,
+        os_version: str = None,
+        python_version: str = None,
+        without_error: bool = False,
     ) -> typing.List[tuple]:
         """Get all versions available for a Python package."""
         package_name = self.normalize_python_package_name(package_name)
 
         query = self.g.E().has("__label__", "solved").has("__type__", "edge")
 
         if os_name:
@@ -525,24 +535,38 @@
         result = []
         query_result = asyncio.get_event_loop().run_until_complete(query)
         for item in query_result:
             result.append((item["package_version"][0], item["index_url"][0]))
 
         return result
 
-    def retrieve_unsolved_pypi_packages(self) -> dict:
-        """Retrieve a dictionary mapping package names to versions that dependencies were not yet resolved."""
+    def retrieve_unsolved_pypi_packages(self, solver_name: str = None) -> dict:
+        """Retrieve a dictionary mapping package names to versions that dependencies were not yet resolved.
+
+        If solver_name argument is provided the given solver, query narrows down to packages that were
+        not resolved by the given solver.
+        """
+        edge_query = inE().has("__label__", Solved.__label__).has("__type__", "edge")
+
+        if not solver_name:
+            solver_info = self.parse_python_solver_name(solver_name)
+            edge_query = (
+                edge_query.has("os_version", solver_info["os_version"])
+                .has("os_name", solver_info["os_name"])
+                .has("python_version", solver_info["python_version"])
+            )
+
         query = (
             self.g.V()
             .has("__label__", "python_package_version")
             .has("__type__", "vertex")
             .has("ecosystem", "pypi")
             .has("package_name")
             .has("package_version")
-            .not_(inE().has("__label__", Solved.__label__).has("__type__", "edge"))
+            .not_(edge_query)
             .group()
             .by("package_name")
             .by("package_version")
             .next()
         )
 
         return asyncio.get_event_loop().run_until_complete(query)
@@ -697,15 +721,15 @@
         return asyncio.get_event_loop().run_until_complete(query)
 
     def get_analyzer_documents_count(self) -> int:
         """Get number of image analysis documents synced into graph."""
         query = (
             self.g.E()
             .has("__type__", "edge")
-            .has("__type__", Requires.__label__)
+            .has("__label__", Requires.__label__)
             .has("analysis_datetime")
             .has("analysis_document_id")
             .has("analyzer_name")
             .has("analyzer_version")
             .valueMap()
             .select("analysis_document_id")
             .dedup()
@@ -754,15 +778,18 @@
 
         return asyncio.get_event_loop().run_until_complete(query)
 
     async def get_python_package_tuple(self, python_package_node_id: int) -> typing.Dict[int, tuple]:
         """Get Python's package name, package version, package index tuple for the given package id."""
         session = await self.app.session()
         result = (
-            await session.g.V(python_package_node_id).valueMap().select("package_name", "package_version", "index_url").next()
+            await session.g.V(python_package_node_id)
+            .valueMap()
+            .select("package_name", "package_version", "index_url")
+            .next()
         )
 
         return {
             python_package_node_id: (result["package_name"][0], result["package_version"][0], result["index_url"][0])
         }
 
     def get_python_package_tuples(self, python_package_node_ids: typing.Set[int]) -> typing.Dict[int, tuple]:
@@ -782,22 +809,22 @@
 
         loop = asyncio.get_event_loop()
         results = loop.run_until_complete(asyncio.gather(*tasks))
         results_dict = list(chain(results))
         return dict(ChainMap(*results_dict))
 
     def retrieve_transitive_dependencies_python(
-            self,
-            package_name: str,
-            package_version: str,
-            index_url: str,
-            *,
-            os_name: str = None,
-            os_version: str = None,
-            python_version: str = None,
+        self,
+        package_name: str,
+        package_version: str,
+        index_url: str,
+        *,
+        os_name: str = None,
+        os_version: str = None,
+        python_version: str = None,
     ) -> list:
         """Get all transitive dependencies for the given package by traversing dependency graph.
 
         It's much faster to retrieve just dependencies for the transitive
         dependencies as most of the time is otherwise spent in serialization
         and deserialization of query results.
         """
@@ -829,30 +856,24 @@
                 query_start = query_start.has("python_version", python_version)
 
             query_start.inV()
         else:
             query_start = self.g.V()
 
         query_start = (
-            query_start
-            .has("__type__", "vertex")
+            query_start.has("__type__", "vertex")
             .has("__label__", "python_package_version")
             .has("ecosystem", "pypi")
             .has("package_version", package_version)
             .has("package_name", package_name)
             .has("index_url", index_url)
         )
 
         query = (
-            query_start
-            .repeat(flatMap(inner_query.inV()))
-            .emit()
-            .path()
-            .by(id_())
-            .toList()
+            query_start.repeat(inner_query.inV()).emit().path().by(id_()).by(valueMap().select("solver_error")).toList()
         )
 
         return asyncio.get_event_loop().run_until_complete(query)
 
     def solver_records_exist(self, solver_document: dict) -> bool:
         """Check if the given solver document record exists."""
         loop = asyncio.get_event_loop()
@@ -926,72 +947,30 @@
 
         return bool(loop.run_until_complete(query))
 
     @staticmethod
     def _get_hardware_information(specs: dict) -> HardwareInformation:
         """Get hardware information based on requests provided."""
         hardware = specs.get("hardware") or {}
+        ram_size = OpenShift.parse_memory_spec(specs["memory"]) if specs.get("memory") else None
+        if ram_size is not None:
+            # Convert bytes to GiB, we need float number for Gremlin/JanusGraph serialization
+            ram_size = ram_size / (1024**3)
+
         return HardwareInformation.from_properties(
             cpu_family=hardware.get("cpu_family"),
             cpu_model=hardware.get("cpu_model"),
             cpu_physical_cpus=hardware.get("physical_cpus"),
             cpu_model_name=hardware.get("processor"),
             cpu_cores=OpenShift.parse_cpu_spec(specs["cpu"]) if specs.get("cpu") else None,
-            ram_size=OpenShift.parse_memory_spec(specs["memory"]) if specs.get("memory") else None,
+            ram_size=ram_size
         )
 
-    def create_software_stack_pipfile(
-            self,
-            pipfile_locked: dict,
-            document_id: str,
-            *,
-            is_user_stack: bool,
-            is_adviser_stack: bool,
-            is_inspection_stack: bool,
-            adviser_stack_index: int = None
-    ) -> SoftwareStackBase:  # Ignore PyDocStyleBear
-        """Create a software stack inside graph database from a Pipfile.lock."""
-        only_one_stated = sum((
-            int(is_user_stack),
-            int(is_adviser_stack),
-            int(is_inspection_stack),
-        ))
-
-        if not only_one_stated:
-            raise ValueError("Only one of type is_user_stack, is_adviser_stack, is_inspection_stack allowed")
-
-        if adviser_stack_index is not None and not is_adviser_stack:
-            raise ValueError(
-                "Index of adviser stack is allowed only for adviser stacks (is_adviser_stack should be set to True)"
-            )
-
-        software_stack_properties = {
-            "document_id": document_id
-        }
-        software_stack_class = None
-
-        if is_adviser_stack is True:
-            if adviser_stack_index is None:
-                raise ValueError(
-                    "Adviser stack index has to be set in case of adviser stacks"
-                )
-
-            software_stack_class = AdviserSoftwareStack
-            software_stack_properties["adviser_stack_index"] = adviser_stack_index
-
-        if is_user_stack:
-            # TODO: state origin in software stack properties.
-            software_stack_class = UserSoftwareStack
-
-        if is_inspection_stack:
-            software_stack_class = InspectionSoftwareStack
-
-        if software_stack_class is None:
-            raise ValueError("Unknown software stack type - should be at least one of user, inspection, adviser")
-
+    def create_python_packages_pipfile(self, pipfile_locked: dict) -> typing.List[PythonPackageVersion]:
+        """Create Python packages from Pipfile.lock entries and return them."""
         def get_index_url(index_name: str):
             for source_index in pipfile_locked["_meta"]["sources"]:
                 if source_index["name"] == index_name:
                     return source_index["url"]
 
             raise ValueError(f"Index with name {index_name!r} not found in Pipfile.lock metadata")
 
@@ -1002,42 +981,76 @@
                 _LOGGER.error(
                     "Package %r in version %r in the Pipfile.lock was not pinned to a specific version correctly",
                     package_name,
                     package_info["version"],
                 )
                 package_version = package_info["version"]
             else:
-                package_version = package_info["version"][len("==") :]  # Ignore PycodestyleBear (E203)
+                package_version = package_info["version"][len("=="):]  # Ignore PycodestyleBear (E203)
 
             index_url = get_index_url(package_info["index"])
 
             existed, _, v, python_package_version = self.create_pypi_package_version(
                 package_name, package_version, index_url=index_url
             )
             python_packages.append(python_package_version)
 
-        software_stack = software_stack_class.from_properties(**software_stack_properties)
-        software_stack.get_or_create(self.g)
+        return python_packages
 
-        for python_package_version in python_packages:
+    def _python_packages_create_stack(
+        self, python_package_versions: typing.Iterable[PythonPackageVersion], software_stack: SoftwareStackBase
+    ) -> None:
+        """Assign the given set of packages to the stack."""
+        for python_package_version in python_package_versions:
             CreatesStack.from_properties(source=python_package_version, target=software_stack).get_or_create(self.g)
 
+    def create_user_software_stack_pipfile(
+        self, document_id: str, pipfile_locked: dict, *, origin: str = None
+    ) -> UserSoftwareStack:
+        """Create a user software stack entry from Pipfile.lock."""
+        python_package_versions = self.create_python_packages_pipfile(pipfile_locked)
+        software_stack = UserSoftwareStack.from_properties(document_id=document_id, origin=origin)
+        software_stack.get_or_create(self.g)
+        self._python_packages_create_stack(python_package_versions, software_stack)
+        return software_stack
+
+    def create_inspection_software_stack_pipfile(
+        self, document_id: str, pipfile_locked: dict
+    ) -> InspectionSoftwareStack:
+        """Create an inspection software stack entry from Pipfile.lock."""
+        python_package_versions = self.create_python_packages_pipfile(pipfile_locked)
+        software_stack = InspectionSoftwareStack.from_properties(document_id=document_id)
+        software_stack.get_or_create(self.g)
+        self._python_packages_create_stack(python_package_versions, software_stack)
+        return software_stack
+
+    def create_adviser_software_stack_pipfile(
+        self, document_id: str, pipfile_locked: dict, *, adviser_stack_index: int
+    ) -> AdviserSoftwareStack:
+        """Create an inspection software stack entry from Pipfile.lock."""
+        python_package_versions = self.create_python_packages_pipfile(pipfile_locked)
+        software_stack = AdviserSoftwareStack.from_properties(
+            document_id=document_id, adviser_stack_index=adviser_stack_index
+        )
+        software_stack.get_or_create(self.g)
+        self._python_packages_create_stack(python_package_versions, software_stack)
         return software_stack
 
     def sync_inspection_result(self, document) -> None:
         """Sync the given inspection document into the graph database."""
-        software_stack = None
+        software_stack, python_version, os_name, os_version = None, None, None, None
         if document["specification"].get("python"):
-            software_stack = self.create_software_stack_pipfile(
-                document["specification"]["python"]["requirements_locked"],
-                document["inspection_id"],
-                is_user_stack=False,
-                is_adviser_stack=False,
-                is_inspection_stack=True,
+            software_stack = self.create_inspection_software_stack_pipfile(
+                document["inspection_id"], document["specification"]["python"]["requirements_locked"]
             )
+            python_version = document["specification"]["python"]["requirements"].get("requires", {}).get("python_version")
+
+        if ":" in document["specification"]["base"]:
+            # TODO: we should capture os info in inspection report directly.
+            os_name, os_version = document["specification"]["base"].split(":")
 
         environment_name = document["inspection_id"]
         if document["job_log"] is not None:
             performance_index = None
             if document["status"]["job"]["exit_code"] != 0:
                 # Negative performance index - the application does not run.
                 performance_index = -1.0
@@ -1051,57 +1064,62 @@
                 _LOGGER.warning("No performance index found in document for inspection %r", document["inspection_id"])
 
             if not document["specification"].get("packages"):
                 # Use the base image as an environment name if there were not
                 # installed any native packages.
                 environment_name = document["specification"]["base"]
 
-            runtime_environment = RuntimeEnvironment.from_properties(runtime_environment_name=environment_name)
+            runtime_environment = RuntimeEnvironmentModel.from_properties(
+                environment_name=environment_name,
+                python_version=python_version,
+                os_name=os_name,
+                os_version=os_version,
+            )
             runtime_environment.get_or_create(self.g)
 
             runtime_hardware = self._get_hardware_information(document["specification"]["run"]["requests"])
             runtime_hardware.get_or_create(self.g)
 
             run_error = document["status"]["job"]["exit_code"] == 0
 
             if software_stack:
                 if performance_index is not None:
                     RunsIn.from_properties(
                         source=software_stack,
                         target=runtime_environment,
-                        inspection_document_id=document["inspection_id"],
+                        document_id=document["inspection_id"],
                         run_error=run_error,
                         performance_index=performance_index,
                     ).get_or_create(self.g)
                 else:
                     # We cannot pass performance_index as None as goblin will complain.
                     RunsIn.from_properties(
                         source=software_stack,
                         target=runtime_environment,
-                        inspection_document_id=document["inspection_id"],
+                        document_id=document["inspection_id"],
                         run_error=run_error,
                     ).get_or_create(self.g)
 
             if performance_index is not None:
                 RunsOn.from_properties(
                     source=runtime_environment,
                     target=runtime_hardware,
-                    inspection_document_id=document["inspection_id"],
+                    document_id=document["inspection_id"],
                     run_error=run_error,
                     performance_index=performance_index,
                 ).get_or_create(self.g)
             else:
                 RunsOn.from_properties(
                     source=runtime_environment,
                     target=runtime_hardware,
-                    inspection_document_id=document["inspection_id"],
+                    document_id=document["inspection_id"],
                     run_error=run_error,
                 ).get_or_create(self.g)
 
-        buildtime_environment = BuildtimeEnvironment.from_properties(buildtime_environment_name=environment_name)
+        buildtime_environment = BuildtimeEnvironmentModel.from_properties(environment_name=environment_name)
         buildtime_environment.get_or_create(self.g)
 
         buildtime_hardware = self._get_hardware_information(document["specification"]["build"]["requests"])
         buildtime_hardware.get_or_create(self.g)
 
         build_error = document["status"]["build"]["exit_code"] == 0
 
@@ -1173,14 +1191,15 @@
 
     def unsolved_runtime_environments(self, package_name: str, package_version: str) -> list:
         """Get unsolved runtime environment which are not connected and attached to python package version."""
         package_name = self.normalize_python_package_name(package_name)
         query = (
             self.g.V()
             .has("__label__", "python_package_version")
+            .has("__type__", "vertex")
             .has("package_name", package_name)
             .has("package_version", package_version)
             .inE()
             .has("__label__", "solved")
             .outV()
             .dedup()
             .aggregate("solvers_solved_python_package_version")
@@ -1194,63 +1213,139 @@
 
         return asyncio.get_event_loop().run_until_complete(query)
 
     @enable_vertex_cache
     def sync_adviser_result(self, document: dict) -> None:
         """Sync adviser result into graph database."""
         adviser_document_id = AdvisersResultsStore.get_document_id(document)
+        origin = (document["metadata"]["arguments"]["thoth-adviser"].get("metadata") or {}).get("origin")
 
+        if not origin:
+            _LOGGER.warning("No origin stated in the adviser result %r", adviser_document_id)
+
+        user_software_stack = None
         if document["result"]["input"]["requirements_locked"]:
             # User provided a Pipfile.lock, we can sync it.
-            self.create_software_stack_pipfile(
-                document["result"]["input"]["requirements_locked"],
-                document_id=adviser_document_id,
-                is_user_stack=True,
-                is_adviser_stack=False,
-                is_inspection_stack=False,
+            user_software_stack = self.create_user_software_stack_pipfile(
+                adviser_document_id, document["result"]["input"]["requirements_locked"], origin=origin
             )
 
+        runtime_info = document["result"]["parameters"]["runtime_environment"]
+
+        hardware_info = runtime_info.pop("hardware", {})
+        hardware_information = HardwareInformation.from_properties(**hardware_info)
+        hardware_information.get_or_create(self.g)
+
+        operating_system = runtime_info.pop("operating_system", {})
+        # TODO: we should derive name from image sha to have exact match.
+        runtime_info.pop("name", None)  # We do not rely on user's input here, it can be anything...
+        runtime_environment_name = (
+            operating_system.get("name", "unknown") + ":" + operating_system.get("version", "unknown")
+        )
+        runtime_environment = RuntimeEnvironmentModel.from_properties(
+            environment_name=runtime_environment_name,
+            os_name=operating_system.get("name"),
+            os_version=operating_system.get("version"),
+            **runtime_info,
+        )
+        runtime_environment.get_or_create(self.g)
+
+        RunsOn.from_properties(
+            source=runtime_environment, target=hardware_information, document_id=adviser_document_id
+        ).get_or_create(self.g)
+
+        RunsIn.from_properties(
+            source=user_software_stack, target=runtime_environment, document_id=adviser_document_id
+        ).get_or_create(self.g)
+
+        adviser_datetime = datetime_str2timestamp(document["metadata"]["datetime"])
+        adviser_version = document["analyzer"]["version"]
         for idx, result in enumerate(document["result"]["report"]):
             if len(result) != 2:
                 _LOGGER.debug("Omitting stack as no output Pipfile.lock was provided - was the report error report?")
                 continue
 
             # result[0] is score report
             # result[1]["requirements"] is Pipfile
             # result[1]["requirements_locked"] is Pipfile.lock
-            if result[1] and "requirements_locked" in result[1]:
-                self.create_software_stack_pipfile(
-                    result[1]["requirements_locked"],
-                    document_id=adviser_document_id,
-                    is_user_stack=False,
-                    is_adviser_stack=True,
-                    is_inspection_stack=False,
-                    adviser_stack_index=idx
+            if result[1] and result[1].get("requirements_locked"):
+                adviser_software_stack = self.create_adviser_software_stack_pipfile(
+                    adviser_document_id, result[1]["requirements_locked"], adviser_stack_index=idx
                 )
 
+                # The linkage to hardware information is already done when user software stack was created.
+                RunsIn.from_properties(
+                    source=adviser_software_stack, target=runtime_environment, document_id=adviser_document_id
+                ).get_or_create(self.g)
+
+                if user_software_stack:
+                    Advised.from_properties(
+                        source=user_software_stack,
+                        target=adviser_software_stack,
+                        adviser_document_id=adviser_document_id,
+                        adviser_version=adviser_version,
+                        adviser_datetime=adviser_datetime,
+                    ).get_or_create(self.g)
+
+    def provenance_checker_document_id_exist(self, provenance_checker_document_id: str) -> bool:
+        """Check if there is a provenance-checker document record with the given id."""
+        loop = asyncio.get_event_loop()
+
+        query = self.g.V().has("document_id", provenance_checker_document_id).count().is_(gt(0)).next()
+
+        return bool(loop.run_until_complete(query))
+
+    @enable_vertex_cache
+    def sync_provenance_checker_result(self, document: dict) -> None:
+        """Sync provenance checker results into graph database."""
+        provenance_checker_document_id = ProvenanceResultsStore.get_document_id(document)
+        origin = (document["metadata"]["arguments"]["thoth-adviser"].get("metadata") or {}).get("origin")
+
+        if not origin:
+            _LOGGER.warning("No origin stated in the provenance-checker result %r", provenance_checker_document_id)
+
+        user_input = document["result"]["input"]
+        if user_input.get("requirements_locked"):
+            self.create_user_software_stack_pipfile(
+                provenance_checker_document_id, user_input["requirements_locked"], origin=origin
+            )
+
     # @enable_edge_cache
     @enable_vertex_cache
     def sync_solver_result(self, document: dict) -> None:
         """Sync the given solver result to the graph database."""
-        solver_name = document["metadata"]["analyzer"]
+        solver_document_id = SolverResultsStore.get_document_id(document)
+        solver_name = SolverResultsStore.get_solver_name_from_document_id(solver_document_id)
         solver_info = self.parse_python_solver_name(solver_name)
 
+        errors = {}
+        for error_info in document["result"]["errors"]:
+            package_name = error_info.get("package_name") or error_info["package"]
+            package_version = error_info["version"]
+            index_url = error_info["index"]
+
+            if package_name not in errors:
+                errors[package_name] = {}
+
+            if package_version not in errors[package_name]:
+                errors[package_name][package_version] = {}
+
+            if index_url not in errors[package_name][package_version]:
+                errors[package_name][package_version][index_url] = True
+
         ecosystem_solver = EcosystemSolver.from_properties(
             solver_name=solver_name,
             solver_version=document["metadata"]["analyzer_version"],
             os_name=solver_info["os_name"],
             os_version=solver_info["os_version"],
-            python_version=solver_info["python_version"]
+            python_version=solver_info["python_version"],
         )
 
         ecosystem_solver.get_or_create(self.g)
-
-        solver_document_id = SolverResultsStore.get_document_id(document)
         solver_datetime = datetime_str2timestamp(document["metadata"]["datetime"])
-
         for python_package_info in document["result"]["tree"]:
             try:
                 existed, python_package, _, python_package_version = self.create_pypi_package_version(
                     python_package_info["package_name"],
                     python_package_info["package_version"],
                     python_package_info["index_url"],
                     hashes=python_package_info["sha256"],
@@ -1292,23 +1387,30 @@
                                 solver_error_unsolvable=False,
                                 solver_error_unparsable=False,
                                 os_name=solver_info["os_name"],
                                 os_version=solver_info["os_version"],
                                 python_version=solver_info["python_version"],
                             ).get_or_create(self.g)
 
+                            solver_error = (
+                                errors.get(python_package_version_dependency.package_name.value, {})
+                                .get(python_package_version_dependency.package_version.value, {})
+                                .get(python_package_version_dependency.index_url.value, False)
+                            )
+
                             # TODO: mark extras
                             DependsOn.from_properties(
                                 source=python_package_version,
                                 target=python_package_version_dependency,
                                 package_name=python_package_version_dependency.package_name.value,
                                 version_range=dependency["required_version"] or "*",
                                 os_name=solver_info["os_name"],
                                 os_version=solver_info["os_version"],
                                 python_version=solver_info["python_version"],
+                                solver_error=solver_error,
                             ).get_or_create(self.g)
                 except Exception:  # pylint: disable=broad-except
                     _LOGGER.exception(
                         f"Failed to sync Python package {python_package_version.to_dict()}" f"dependency: {dependency}"
                     )
 
         for error_info in document["result"]["errors"]:
@@ -1341,15 +1443,15 @@
                 # packages in ecosystem that we cannot find (e.g. not configured private index
                 # or removed package).
                 _LOGGER.warning(
                     f"Cannot sync unsolvable package {unsolvable} as package is not locked to as specific version"
                 )
                 continue
 
-            package_version = unsolvable["version_spec"][len("==") :]  # Ignore PycodestyleBear (E203)
+            package_version = unsolvable["version_spec"][len("=="):]
             try:
                 existed, python_package, _, python_package_version = self.create_pypi_package_version(
                     package_name=unsolvable["package_name"],
                     package_version=package_version,
                     index_url=unsolvable["index"],
                 )
 
@@ -1395,15 +1497,15 @@
                     os_version=solver_info["os_version"],
                     python_version=solver_info["python_version"],
                 ).get_or_create(self.g)
             except Exception:  # pylint: disable=broad-except
                 _LOGGER.exception("Failed to sync unparsed Python package, error is not fatal: %r", unparsed)
 
     def _deb_sync_analysis_result(
-        self, document_id: str, document: dict, runtime_environment: RuntimeEnvironment
+        self, document_id: str, document: dict, environment: EnvironmentBase
     ) -> None:
         """Sync results of deb packages found in the given container image."""
         for deb_package_info in document["result"]["deb-dependencies"]:
             try:
                 deb_package_version = DebPackageVersion.from_properties(
                     ecosystem="deb",
                     package_name=deb_package_info["name"],
@@ -1418,15 +1520,15 @@
                 )
                 deb_package.get_or_create(self.g)
 
                 HasVersion.from_properties(source=deb_package, target=deb_package_version).get_or_create(self.g)
 
                 IsPartOf.from_properties(
                     source=deb_package_version,
-                    target=runtime_environment,
+                    target=environment,
                     analysis_datetime=datetime_str2timestamp(document["metadata"]["datetime"]),
                     analysis_document_id=document_id,
                     analyzer_name=document["metadata"]["analyzer"],
                     analyzer_version=document["metadata"]["analyzer_version"],
                 ).get_or_create(self.g)
 
                 # These three can be grouped with a zip, but that is not that readable...
@@ -1453,15 +1555,15 @@
                     DebReplaces.from_properties(
                         source=deb_package_version, target=package, version_range=replaces.get("version")
                     ).get_or_create(self.g)
             except Exception:
                 _LOGGER.exception("Failed to sync debian package, error is not fatal: %r", deb_package_info)
 
     def _rpm_sync_analysis_result(
-        self, document_id: str, document: dict, runtime_environment: RuntimeEnvironment
+        self, document_id: str, document: dict, environment: EnvironmentBase
     ) -> None:
         """Sync results of RPMs found in the given container image."""
         for rpm_package_info in document["result"]["rpm-dependencies"]:
             try:
                 rpm_package_version = RPMPackageVersion.from_properties(
                     ecosystem="rpm",
                     package_name=rpm_package_info["name"],
@@ -1479,15 +1581,15 @@
                 )
                 rpm_package.get_or_create(self.g)
 
                 HasVersion.from_properties(source=rpm_package, target=rpm_package_version).get_or_create(self.g)
 
                 IsPartOf.from_properties(
                     source=rpm_package_version,
-                    target=runtime_environment,
+                    target=environment,
                     analysis_datetime=datetime_str2timestamp(document["metadata"]["datetime"]),
                     analysis_document_id=document_id,
                     analyzer_name=document["metadata"]["analyzer"],
                     analyzer_version=document["metadata"]["analyzer_version"],
                 ).get_or_create(self.g)
 
             except Exception:  # pylint: disable=broad-except
@@ -1509,15 +1611,15 @@
                     ).get_or_create(self.g)
                 except Exception:  # pylint: disable=broad-except
                     _LOGGER.exception(
                         f"Failed to sync dependencies for " f"RPM {rpm_package_version.to_dict()}: {dependency!r}"
                     )
 
     def _python_sync_analysis_result(
-        self, document_id: str, document: dict, runtime_environment: RuntimeEnvironment
+        self, document_id: str, document: dict, environment: EnvironmentBase
     ) -> None:
         """Sync results of Python packages found in the given container image."""
         # or [] should go to analyzer to be consistent
         for python_package_info in document["result"]["mercator"] or []:
             if python_package_info["ecosystem"] == "Python-RequirementsTXT":
                 # We don't want to sync found requirement.txt artifacts as
                 # they do not carry any valuable information for us.
@@ -1538,15 +1640,15 @@
                     package_name=python_package_info["result"]["name"],
                     package_version=python_package_info["result"]["version"],
                     index_url=None,
                 )
 
                 IsPartOf.from_properties(
                     source=python_package_version,
-                    target=runtime_environment,
+                    target=environment,
                     analysis_datetime=datetime_str2timestamp(document["metadata"]["datetime"]),
                     analysis_document_id=document_id,
                     analyzer_name=document["metadata"]["analyzer"],
                     analyzer_version=document["metadata"]["analyzer_version"],
                 ).get_or_create(self.g)
             except Exception:  # pylint: disable=broad-exception
                 _LOGGER.exception(f"Failed to sync Python package, error is not fatal: {python_package_info!r}")
@@ -1586,36 +1688,42 @@
 
     def get_python_cve_records(self, package_name: str, package_version: str) -> typing.List[dict]:
         """Get known vulnerabilities for the given package-version."""
         package_name = self.normalize_python_package_name(package_name)
         query = (
             self.g.V()
             .has("__label__", "python_package_version")
+            .has("__type__", "vertex")
             .has("package_name", package_name)
             .has("package_version", package_version)
+            .has("ecosystem", "pypi")
             .outE()
             .has("__label__", "has_vulnerability")
             .has("__type__", "edge")
             .inV()
             .has("__label__", "cve")
             .has("__type__", "vertex")
-            .project("cve_id", "advisory", "version_range").by("cve_id").by("advisory").by("version_range")
+            .project("cve_id", "advisory", "version_range", "cve_name")
+            .by("cve_id")
+            .by("advisory")
+            .by("version_range")
+            .by("cve_name")
             .toList()
         )
 
-        # TODO: add cve_name to the projected result once we re-create janusgraph instance.
         return asyncio.get_event_loop().run_until_complete(query)
 
     def get_python_package_version_hashes_sha256(
         self, package_name: str, package_version: str, index_url: str
     ) -> typing.List[str]:
         """Get hashes for a Python package in specified version."""
         query = (
             self.g.V()
             .has("__label__", "python_package_version")
+            .has("__type__", "vertex")
             .has("package_name", package_name)
             .has("package_version", package_version)
             .has("index_url", index_url)
             .outE()
             .has("__label__", "has_artifact")
             .inV()
             .valueMap()
@@ -1626,14 +1734,15 @@
         return list(chain(*asyncio.get_event_loop().run_until_complete(query)))
 
     def get_all_python_package_version_hashes_sha256(self, package_name: str, package_version: str) -> list:
         """Get hashes for a Python package per index."""
         query = (
             self.g.V()
             .has("__label__", "python_package_version")
+            .has("__type__", "vertex")
             .has("package_name", package_name)
             .has("package_version", package_version)
             .flatMap(outE().inV())
             .has("__label__", "python_artifact")
             .has("__type__", "vertex")
             .path()
             .by("index_url")
@@ -1643,22 +1752,33 @@
 
         return asyncio.get_event_loop().run_until_complete(query)
 
     # @enable_edge_cache
     @enable_vertex_cache
     def sync_analysis_result(self, document: dict) -> None:
         """Sync the given analysis result to the graph database."""
-        runtime_environment = RuntimeEnvironment.from_properties(
-            runtime_environment_name=document["metadata"]["arguments"]["extract-image"]["image"]
-        )
-        runtime_environment.get_or_create(self.g)
+        environment_type = document["metadata"]["arguments"]["thoth-package-extract"]["metadata"]["environment_type"]
+        # TODO: we should sync also origin of analysed images
+        if environment_type == "runtime":
+            environment = RuntimeEnvironmentModel.from_properties(
+                environment_name=document["metadata"]["arguments"]["extract-image"]["image"]
+            )
+            environment.get_or_create(self.g)
+        elif environment_type == "buildtime":
+            environment = BuildtimeEnvironmentModel.from_properties(
+                environment_name=document["metadata"]["arguments"]["extract-image"]["image"]
+            )
+            environment.get_or_create(self.g)
+        else:
+            raise ValueError("Unknown environment type %r, should be buildtime or runtime" % environment_type)
+
         document_id = AnalysisResultsStore.get_document_id(document)
-        self._rpm_sync_analysis_result(document_id, document, runtime_environment)
-        self._deb_sync_analysis_result(document_id, document, runtime_environment)
-        self._python_sync_analysis_result(document_id, document, runtime_environment)
+        self._rpm_sync_analysis_result(document_id, document, environment)
+        self._deb_sync_analysis_result(document_id, document, environment)
+        self._python_sync_analysis_result(document_id, document, environment)
 
     def register_python_package_index(self, url: str, warehouse_api_url: str = None, verify_ssl: bool = True):
         """Register the given Python package index in the graph database."""
         package_index = PythonPackageIndex.from_properties(
             url=url, warehouse_api_url=warehouse_api_url, verify_ssl=verify_ssl
         )
         package_index.get_or_create(self.g)
@@ -1702,32 +1822,29 @@
         )
 
         return set(chain(*asyncio.get_event_loop().run_until_complete(query)))
 
     @staticmethod
     def parse_python_solver_name(solver_name: str) -> dict:
         """Parse os and Python identifiers encoded into solver name."""
-        if solver_name.startswith('solver-'):
-            solver_identifiers = solver_name[len('solver-'):]
+        if solver_name.startswith("solver-"):
+            solver_identifiers = solver_name[len("solver-"):]
         else:
             raise ValueError("Solver name has to start with 'solver-' prefix")
 
-        parts = solver_identifiers.split('-')
+        parts = solver_identifiers.split("-")
         if len(parts) != 3:
             raise ValueError(
                 "Solver should be in a form of 'solver-<os_name>-<os_version>-<python_version>, "
                 f"solver name {solver_name} does not correspond to this naming schema"
             )
 
         python_version = parts[2]
-        if python_version.startswith('py'):
-            python_version = python_version[len('py'):]
+        if python_version.startswith("py"):
+            python_version = python_version[len("py"):]
         else:
             raise ValueError(
                 f"Python version encoded into Python solver name does not start with 'py' prefix: {solver_name}"
             )
 
-        return {
-            "os_name": parts[0],
-            "os_version": parts[1],
-            "python_version": python_version
-        }
+        python_version = ".".join(list(python_version))
+        return {"os_name": parts[0], "os_version": parts[1], "python_version": python_version}
```

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/models.py` & `thoth-storages-0.9.7/thoth/storages/graph/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,58 +91,82 @@
 class PythonArtifact(VertexBase):
     """A Python artifact as placed on a source package index."""
 
     # artifact_name = VertexProperty(properties.String)
     artifact_hash_sha256 = VertexProperty(properties.String)
 
 
-class RuntimeEnvironment(VertexBase):
-    """Environment such as container image which consists of various packages."""
+class EnvironmentBase(VertexBase):
+    """A base class for environment types."""
+
+    environment_name = VertexProperty(properties.String)
+    python_version = VertexProperty(properties.String, default=None)
 
-    runtime_environment_name = VertexProperty(properties.String)
     # TODO: capture hashes of layers to be precise?
 
 
-class BuildtimeEnvironment(VertexBase):
+class RuntimeEnvironment(EnvironmentBase):
     """Environment such as container image which consists of various packages."""
 
-    buildtime_environment_name = VertexProperty(properties.String)
-    # TODO: capture hashes of layers to be precise?
+    os_name = VertexProperty(properties.String, default=None)
+    os_version = VertexProperty(properties.String, default=None)
+    python_version = VertexProperty(properties.String, default=None)
+    cuda_version = VertexProperty(properties.String, default=None)
+
+
+class BuildtimeEnvironment(EnvironmentBase):
+    """Environment such as container image which consists of various packages."""
 
 
 class SoftwareStackBase(VertexBase):
     """A software stack crated by packages in specific versions.
 
     This is just a base class for creating software stack instances inside graph database.
     See specific software stack types for specific software stacks we are interested in.
     """
+
     # If a user stack, document id points to adviser document that introduced the stack.
     # If an adviser stack, document_id points to adviser document that introduced the stack.
     # If an inspection stack, document_id points to inspection document that introduced the stack.
+
     document_id = VertexProperty(properties.String)
 
 
 class AdviserSoftwareStack(SoftwareStackBase):
     """A software stack as produced by adviser (the output of recommendation engine)."""
+
     # As adviser can output multiple stacks, this property states the index in
     # the resulting adviser document if is_adviser stack is set to True.
+
     adviser_stack_index = VertexProperty(properties.Integer, default=None)
 
 
 class UserSoftwareStack(SoftwareStackBase):
     """A software stack as used by a user (input for the recommendation engine)."""
 
     # Origin of the software stack.
     origin = VertexProperty(properties.String, default=None)
+    # Holds True/False if there was an error during advises in adviser.
+    # Holds None if user stack came from provenance-checks.
+    adviser_error = VertexProperty(properties.Boolean, default=None)
 
 
 class InspectionSoftwareStack(SoftwareStackBase):
     """A software stack which was used on Amun during inspection runs (e.g. as produced by dependency-monkey)."""
 
 
+class Advised(EdgeBase):
+    """A relationship between user software stack and the advised software stack by Thoth's adviser."""
+
+    adviser_version = Property(properties.String)
+    adviser_document_id = Property(properties.String)
+    adviser_datetime = Property(properties.Integer)
+    recommendation_type = Property(properties.String)
+
+
 class SoftwareStackObservation(VertexBase):
     """Observations we have about the given stack based on run on a specific hardware."""
 
     performance_index = VertexProperty(properties.Float)
     inspection_document_id = VertexProperty(properties.String, db_name="document_id")
 
 
@@ -164,15 +188,17 @@
 
     # TODO: provide once we will have them available from Amun.
     # gpu_vendor = VertexProperty(properties.String)
     # gpu_model_name = VertexProperty(properties.String)
     # gpu_cores = VertexProperty(properties.Integer)
     # gpu_memory_size = VertexProperty(properties.Integer)
 
-    ram_size = VertexProperty(properties.Integer)
+    # We use float here as using Integer can lead to serialization/deserialization
+    # issues on Graph database side. JanusGraph treats Integer in fixed size of int32.
+    ram_size = VertexProperty(properties.Float)
 
 
 class EcosystemSolver(VertexBase):
     """Solver used to resolve dependencies within ecosystem."""
 
     solver_name = VertexProperty(properties.String)
     solver_version = VertexProperty(properties.String)
@@ -186,14 +212,19 @@
 class DependsOn(EdgeBase):
     """Dependency between packages modeling based on ecosystem specification."""
 
     version_range = Property(properties.String, default="*")
     package_name = Property(properties.String)
     extras = Property(properties.String)
 
+    os_name = Property(properties.String)
+    os_version = Property(properties.String)
+    python_version = Property(properties.String)
+    solver_error = Property(properties.Boolean, default=False)
+
 
 class Observed(EdgeBase):
     """Information about observations gathered on run."""
 
     inspection_document_id = Property(properties.String)
 
 
@@ -254,49 +285,45 @@
 class HasVersion(EdgeBase):
     """The given package has a specific version."""
 
 
 class RunsIn(EdgeBase):
     """The given software stack runs in a runtime environment."""
 
-    inspection_document_id = Property(properties.String)
-    run_error = Property(properties.Boolean)
-    performance_index = Property(properties.Float)
+    document_id = Property(properties.String)
+    run_error = Property(properties.Boolean, default=None)
+    performance_index = Property(properties.Float, default=None)
 
 
 class RunsOn(EdgeBase):
     """The given software stack runs on the given hardware."""
 
-    inspection_document_id = Property(properties.String)
-    run_error = Property(properties.Boolean)
-    performance_index = Property(properties.Float)
+    document_id = Property(properties.String)
+    run_error = Property(properties.Boolean, default=None)
+    performance_index = Property(properties.Float, default=None)
 
 
 class BuildsIn(EdgeBase):
     """The given software stack builds in a build environment."""
 
-    inspection_document_id = Property(properties.String)
+    document_id = Property(properties.String)
     build_error = Property(properties.Boolean)
 
 
 class BuildsOn(EdgeBase):
     """The given software stack builds on the given hardware."""
 
-    inspection_document_id = Property(properties.String)
+    document_id = Property(properties.String)
     build_error = Property(properties.Boolean)
 
 
 class HasVulnerability(EdgeBase):
     """The given package version has a vulnerability."""
 
 
-class HasArtifact(EdgeBase):
-    """The given package-version has an artifact."""
-
-
 class Requires(PackageExtractNativeBase):
     """Requirement edge of an RPM package."""
 
 
 class DebDepends(PackageExtractNativeBase):
     """Depending edge of a deb package."""
 
@@ -325,14 +352,15 @@
         CVE,
         DebDepends,
         DebPackageVersion,
         DebPreDepends,
         DebReplaces,
         DependsOn,
         EcosystemSolver,
+        HasArtifact,
         HasVersion,
         HasVulnerability,
         IsPartOf,
         Package,
         PythonArtifact,
         PythonPackageIndex,
         PythonPackageVersion,
```

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/models_base.py` & `thoth-storages-0.9.7/thoth/storages/graph/models_base.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/graph/utils.py` & `thoth-storages-0.9.7/thoth/storages/graph/utils.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/inspections.py` & `thoth-storages-0.9.7/thoth/storages/inspections.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/observations.py` & `thoth-storages-0.9.7/thoth/storages/observations.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/provenance.py` & `thoth-storages-0.9.7/thoth/storages/provenance.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/provenance_cache.py` & `thoth-storages-0.9.7/thoth/storages/provenance_cache.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/result_base.py` & `thoth-storages-0.9.7/thoth/storages/result_base.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/result_schema.py` & `thoth-storages-0.9.7/thoth/storages/result_schema.py`

 * *Files identical despite different names*

### Comparing `thoth-storages-0.9.6/thoth/storages/solvers.py` & `thoth-storages-0.9.7/thoth/storages/solvers.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,7 +20,12 @@
 from .result_base import ResultStorageBase
 
 
 class SolverResultsStore(ResultStorageBase):
     """Adapter for persisting solver results."""
 
     RESULT_TYPE = "solver"
+
+    @staticmethod
+    def get_solver_name_from_document_id(solver_document_id: str) -> str:
+        """Retrieve solver name from solver's document id."""
+        return solver_document_id.rsplit("-", maxsplit=1)[0]
```

### Comparing `thoth-storages-0.9.6/thoth/storages/sync.py` & `thoth-storages-0.9.7/thoth/storages/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from amun import is_inspection_finished
 from amun import has_inspection_job
 
 from .solvers import SolverResultsStore
 from .analyses import AnalysisResultsStore
 from .advisers import AdvisersResultsStore
 from .inspections import InspectionResultsStore
+from .provenance import ProvenanceResultsStore
 from .dependency_monkey_reports import DependencyMonkeyReportsStore
 from .graph import GraphDatabase
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def sync_adviser_documents(
@@ -154,14 +155,55 @@
         else:
             _LOGGER.info(f"Sync of analysis document with id {document_id!r} skipped - already synced")
             skipped += 1
 
     return processed, synced, skipped, failed
 
 
+def sync_provenance_checker_documents(
+        document_ids: list = None,
+        force: bool = False,
+        graceful: bool = False,
+        graph: GraphDatabase = None,
+) -> tuple:
+    """Sync provenance check documents into graph."""
+    if not graph:
+        graph = GraphDatabase()
+        graph.connect()
+
+    provenance_check_store = ProvenanceResultsStore()
+    provenance_check_store.connect()
+
+    processed, synced, skipped, failed = 0, 0, 0, 0
+    for document_id in document_ids or provenance_check_store.get_document_listing():
+        processed += 1
+
+        if force or not graph.provenance_checker_document_id_exist(document_id):
+            _LOGGER.info(
+                f"Syncing provenance-checker document from {provenance_check_store.ceph.host} "
+                f"with id {document_id!r} to graph {graph.hosts}"
+            )
+
+            try:
+                document = provenance_check_store.retrieve_document(document_id)
+                graph.sync_provenance_checker_result(document)
+                synced += 1
+            except Exception:
+                if not graceful:
+                    raise
+
+                _LOGGER.exception("Failed to sync provenance-checker result with document id %r", document_id)
+                failed += 1
+        else:
+            _LOGGER.info(f"Sync of provenance-checker document with id {document_id!r} skipped - already synced")
+            skipped += 1
+
+    return processed, synced, skipped, failed
+
+
 def sync_inspection_documents(
     amun_api_url: str,
     document_ids: list = None,
     *,
     force_sync: bool = False,
     graceful: bool = False,
     only_graph_sync: bool = False,
```

### Comparing `thoth-storages-0.9.6/thoth_storages.egg-info/PKG-INFO` & `thoth-storages-0.9.7/thoth_storages.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,82 @@
 Metadata-Version: 1.0
 Name: thoth-storages
-Version: 0.9.6
+Version: 0.9.7
 Summary: Storage and database adapters available in project Thoth
 Home-page: UNKNOWN
 Author: Fridolin Pokorny
 Author-email: fridolin@redhat.com
 License: GPLv3+
-Description: thoth-storages
+Description: Thoth Storages
         --------------
-        This repo provides a library called
-        `thoth-storages <https://pypi.org/project/thoth-storages>`_.
-        The library exposes core queries and methods for JanusGraph database as well
-        as adapters for manipulating with Ceph via its S3 compatible API.
+        
+        This library provides a library called `thoth-storages
+        <https://pypi.org/project/thoth-storages>`_ used in project `Thoth
+        <https://thoth-station.ninja>`_.  The library exposes core queries and methods
+        for JanusGraph database as well as adapters for manipulating with Ceph via its
+        S3 compatible API.
         
         Installation and Usage
         ======================
         
-        The library can be installed via pip or pipenv:
+        The library can be installed via pip or Pipenv from
+        `PyPI <https://pypi.org/project/thoth-storages>`_:
         
         .. code-block:: console
         
            pipenv install thoth-storages
         
         The library does not provide any CLI, it is rather a low level library
         supporting other parts of Thoth.
         
         You can run prepared testsuite via the following command:
         
         .. code-block:: console
         
-            pipenv install --dev
-            pipenv run python3 setup.py test
+          pipenv install --dev
+          pipenv run python3 setup.py test
+        
+          # To generate docs:
+          pipenv run python3 setup.py build_sphinx
+        
+        Automatically generate schema for Graph database
+        ================================================
+        
+        To automatically generate schema for the graph database from models defined in
+        this module, run:
+        
+        .. code-block:: console
+        
+           # Install dev dependencies which include goblinoid:
+           pipenv install --dev
+        
+           # From root of this repository:
+           PYTHONPATH=. pipenv run goblinoid -m thoth.storages.graph.models -i ALL_MODELS
         
+           # Or to directly adjust used schema:
+           export PYTHONPATH=.
+           # Or export also ../goblinoid to have the most recent Goblinoid version (devel from master).
+           export PYTHONPATH=.:../goblinoid
+           pipenv run goblinoid -m thoth.storages.graph.models -i ALL_MODELS --output-file ../janusgraph-thoth-config/scripts/init.groovy --index-file ../janusgraph-thoth-config/scripts/indexes.groovy.template
+        
+        After running this command, there will be present file called `init.groovy`
+        which is generated automatically from models stated in `ALL_MODELS` (see file
+        thoth/storages/graph/models.py) as well as with indexes as configured in the
+        indexes.groovy.template (placed into a single file to run it in one
+        transaction).
+        
+        See `goblinoid <https://github.com/thoth-station/goblinoid>`_ for more info
+        on how to configure models generation.
         
         Known Issues
         ============
         
         - Gremlin queries are hanging:
         
-           When using :code:`aiogremlin==3.3.1` (despite being not part of our specification, it might happen that another library overrides that dependency), gremlin queries might _hang indeffinitely_ without throwing any error in Jupyter Notebooks. Make sure to check that correct version of :code:`aiogremlin` is installed.
+           When using :code:`aiogremlin==3.3.1` (despite being not part of our
+           specification, it might happen that another library overrides that
+           dependency), gremlin queries might hang indeffinitely without throwing any
+           error in Jupyter Notebooks. Make sure to check that correct version of
+           :code:`aiogremlin` is installed.
+        
         
 Platform: UNKNOWN
```

### Comparing `thoth-storages-0.9.6/thoth_storages.egg-info/SOURCES.txt` & `thoth-storages-0.9.7/thoth_storages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

