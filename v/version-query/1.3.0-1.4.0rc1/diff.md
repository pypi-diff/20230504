# Comparing `tmp/version-query-1.3.0.tar.gz` & `tmp/version-query-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "version-query-1.3.0.tar", last modified: Fri Mar 17 09:47:27 2023, max compression
+gzip compressed data, was "version-query-1.4.0rc1.tar", last modified: Thu May  4 13:13:35 2023, max compression
```

## Comparing `version-query-1.3.0.tar` & `version-query-1.4.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:47:27.533331 version-query-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-17 09:47:17.000000 version-query-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-17 09:47:17.000000 version-query-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-17 09:47:17.000000 version-query-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-03-17 09:47:27.533331 version-query-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-03-17 09:47:17.000000 version-query-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-17 09:47:17.000000 version-query-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-17 09:47:17.000000 version-query-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-17 09:47:17.000000 version-query-1.3.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 09:47:27.533331 version-query-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-17 09:47:17.000000 version-query-1.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-03-17 09:47:17.000000 version-query-1.3.0/setup_boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:47:27.533331 version-query-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-17 09:47:17.000000 version-query-1.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-03-17 09:47:17.000000 version-query-1.3.0/test/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-03-17 09:47:17.000000 version-query-1.3.0/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-03-17 09:47:17.000000 version-query-1.3.0/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-03-17 09:47:17.000000 version-query-1.3.0/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-03-17 09:47:17.000000 version-query-1.3.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-17 09:47:17.000000 version-query-1.3.0/test/test_with_git_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:47:27.533331 version-query-1.3.0/version_query/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/git_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/py_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-03-17 09:47:17.000000 version-query-1.3.0/version_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:47:27.533331 version-query-1.3.0/version_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-03-17 09:47:27.000000 version-query-1.3.0/version_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-17 09:47:27.000000 version-query-1.3.0/version_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 09:47:27.000000 version-query-1.3.0/version_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-17 09:47:27.000000 version-query-1.3.0/version_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-17 09:47:27.000000 version-query-1.3.0/version_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/setup_boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_with_git_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/version_query/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/git_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/py_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/version_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/top_level.txt
```

### Comparing `version-query-1.3.0/LICENSE` & `version-query-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/NOTICE` & `version-query-1.4.0rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/PKG-INFO` & `version-query-1.4.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: version-query
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Zero-overhead package versioning for Python.
 Home-page: https://github.com/mbdevpl/version-query
 Download-URL: 
 Author: Mateusz Bysiek, John Vandenberg
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -58,15 +58,15 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/437ab82bd6324530847fe8ed833f8d78
     :target: https://app.codacy.com/gh/mbdevpl/version-query
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/version-query.svg
-    :target: https://github.com/mbdevpl/version-query/blob/v1.3.0/NOTICE
+    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/NOTICE
     :alt: license
 
 Package versioning toolkit for Python which relies on git tags, git history traversal
 and status of git repository to generate a very fine-grained version number.
 
 Aren't you tired hardcoding the version numbers when maintaining a Python package?!
 
@@ -468,12 +468,12 @@
 
 
 Requirements
 ============
 
 Python version 3.9 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.3.0/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.3.0/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements_test.txt>`_.
 
 Tested on Linux, OS X and Windows.
```

### Comparing `version-query-1.3.0/README.rst` & `version-query-1.4.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/pyproject.toml` & `version-query-1.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/setup.py` & `version-query-1.4.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/setup_boilerplate.py` & `version-query-1.4.0rc1/setup_boilerplate.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/__init__.py` & `version-query-1.4.0rc1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/examples.py` & `version-query-1.4.0rc1/test/examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,18 @@
 
 KWARG_NAMES = ('major', 'minor', 'patch', 'pre_release', 'local')
 
 INIT_CASES: t.Dict[str, t.Tuple[tuple, dict]] = {
     '1': ((1,), {}),
     '1.0': ((1, 0), {}),
     '1.0.0': ((1, 0, 0), {}),
+    '1.0.0rc1': ((1, 0, 0, None, 'rc', 1), {}),
+    '1.0.0rc2': ((1, 0, 0, None, 'rc', 2), {}),
     '1.0.0.rc2': ((1, 0, 0, '.', 'rc', 2), {}),
+    '1.0.0rc3': ((1, 0, 0, None, 'rc', 3), {}),
     '1.0.0.rc3': ((1, 0, 0, ('.', 'rc', 3)), {}),
     '1.0.0.rc2+local': ((1, 0, 0, '.', 'rc', 2, 'local'), {}),
     '1.0.0.rc3+local': ((1, 0, 0, ('.', 'rc', 3), 'local'), {}),
     '1.0.0.rc4+local': ((1, 0, 0, ('.', 'rc', 4), ('local',)), {})}
 
 BAD_INIT_CASES: t.Dict[t.Tuple[tuple, tuple], t.Type[Exception]] = {
     (('spam',), ()): TypeError,
@@ -122,22 +125,24 @@
     '5.0+f753199e': ((5, 0, None), {'local': 'f753199e'}),
     '0.54.0': ((0, 54, 0), {}),
     '1.0.0': ((1, 0, 0), {}),
     '7.0.42+1d7b090a': ((7, 0, 42), {'local': '1d7b090a'}),
     '1.0.0.4': ((1, 0, 0, '.', None, 4), {}),
     '2.0.0.8+cc81cee': ((2, 0, 0, '.', None, 8, 'cc81cee'), {}),
     '4.5.0.dev1234': ((4, 5, 0, '.', 'dev', 1234), {}),
-    '1.0.0.rc3': ((1, 0, 0, '.', 'rc', 3), {}),
+    '1.0.0rc1': ((1, 0, 0, None, 'rc', 1), {}),
+    '1.0.0rc3': ((1, 0, 0, None, 'rc', 3), {}),
     '1.0.1.dev0': ((1, 0, 1, '.', 'dev', 0), {}),
     '0.4.4.dev5+84e1d430': ((0, 4, 4, '.', 'dev', 5, '84e1d430'), {}),
     '0.4.4.dev5+20171003.84e1d430': ((0, 4, 4, '.', 'dev', 5, '20171003', '.', '84e1d430'), {})}
 
 INCOMPATIBLE_STR_CASES: t.Dict[str, t.Tuple[tuple, dict]] = {
     '1.0.0-2': ((1, 0, 0, '-', None, 2), {}),
     # '1.0.0-0.2': ((1, 0, 0, '-', None, 0, '.', None, 2), {}),
+    '1.0.0.rc3': ((1, 0, 0, '.', 'rc', 3), {}),
     '4.5.0.dev': ((4, 5, 0, '.', 'dev', None), {})}
 
 STR_CASES = dict(itertools.chain(COMPATIBLE_STR_CASES.items(),
                                  INCOMPATIBLE_STR_CASES.items()))
 
 BAD_STR_CASES = {
     '-1.0.0': ValueError,
```

### Comparing `version-query-1.3.0/test/test_git.py` & `version-query-1.4.0rc1/test/test_git.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/test_query.py` & `version-query-1.4.0rc1/test/test_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/test_setup.py` & `version-query-1.4.0rc1/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/test_version.py` & `version-query-1.4.0rc1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/test/test_with_git_repo.py` & `version-query-1.4.0rc1/test/test_with_git_repo.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/version_query/git_query.py` & `version-query-1.4.0rc1/version_query/git_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/version_query/main.py` & `version-query-1.4.0rc1/version_query/main.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/version_query/py_query.py` & `version-query-1.4.0rc1/version_query/py_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/version_query/query.py` & `version-query-1.4.0rc1/version_query/query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.3.0/version_query/version.py` & `version-query-1.4.0rc1/version_query/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import typing as t
 
 import packaging.version
 import semver
 
 _LOG = logging.getLogger(__name__)
 
+PY_PRE_RELEASE_INDICATORS = {'a', 'b', 'c', 'rc'}
+
 
 @enum.unique
 class VersionComponent(enum.IntEnum):
     """Enumeration of standard version components."""
 
     Major = 1 << 1
     Minor = 1 << 2
@@ -164,16 +166,16 @@
         if pre_ver_present > 1:
             raise NotImplementedError(py_version)
         if ver.dev:
             pre_ver = ver.dev
         elif ver.pre:
             pre_ver = ver.pre
         if pre_ver:
-            pre_release = [('.', pre_ver[0] if len(pre_ver) > 0 else None,
-                            pre_ver[1] if len(pre_ver) > 1 else None)]
+            prefix_dot = None if pre_ver[0] in PY_PRE_RELEASE_INDICATORS else '.'
+            pre_release = [(prefix_dot, pre_ver[0], pre_ver[1] if len(pre_ver) > 1 else None)]
         if ver.local:
             local = tuple(itertools.chain.from_iterable(
                 (dot, str(_)) for dot, _ in zip('.' * len(ver.local), ver.local)))[1:]
         _LOG.debug('parsing %s %s', type(py_version), py_version)
         return cls(major, minor, patch, pre_release=pre_release, local=local)
 
     @classmethod
@@ -498,14 +500,16 @@
     def _pre_release_segment_to_str(self, segment: int) -> str:
         assert self._pre_release is not None
         version_tuple = self._pre_release[segment]
         if _version_tuple_checker(version_tuple, (True, True, False)):
             return '{}{}'.format(*version_tuple[:2])
         if _version_tuple_checker(version_tuple, (True, False, True)):
             return f'{version_tuple[0]}{version_tuple[2]}'
+        if _version_tuple_checker(version_tuple, (False, True, True)):
+            return '{}{}'.format(*version_tuple[1:])
         if _version_tuple_checker(version_tuple, (True, True, True)):
             return '{}{}{}'.format(*version_tuple)
         raise ValueError(f'cannot generate valid version string from {repr(self)}')
 
     def pre_release_to_str(self) -> str:
         if self._pre_release is None:
             return ''
```

### Comparing `version-query-1.3.0/version_query.egg-info/PKG-INFO` & `version-query-1.4.0rc1/version_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: version-query
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Zero-overhead package versioning for Python.
 Home-page: https://github.com/mbdevpl/version-query
 Download-URL: 
 Author: Mateusz Bysiek, John Vandenberg
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -58,15 +58,15 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/437ab82bd6324530847fe8ed833f8d78
     :target: https://app.codacy.com/gh/mbdevpl/version-query
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/version-query.svg
-    :target: https://github.com/mbdevpl/version-query/blob/v1.3.0/NOTICE
+    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/NOTICE
     :alt: license
 
 Package versioning toolkit for Python which relies on git tags, git history traversal
 and status of git repository to generate a very fine-grained version number.
 
 Aren't you tired hardcoding the version numbers when maintaining a Python package?!
 
@@ -468,12 +468,12 @@
 
 
 Requirements
 ============
 
 Python version 3.9 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.3.0/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.3.0/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements_test.txt>`_.
 
 Tested on Linux, OS X and Windows.
```

### Comparing `version-query-1.3.0/version_query.egg-info/SOURCES.txt` & `version-query-1.4.0rc1/version_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

