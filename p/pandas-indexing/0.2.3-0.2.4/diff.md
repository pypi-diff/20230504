# Comparing `tmp/pandas-indexing-0.2.3.tar.gz` & `tmp/pandas-indexing-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.3.tar", last modified: Wed May  3 21:24:02 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.4.tar", last modified: Wed May  3 22:26:06 2023, max compression
```

## Comparing `pandas-indexing-0.2.3.tar` & `pandas-indexing-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.156448 pandas-indexing-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.156448 pandas-indexing-0.2.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.152447 pandas-indexing-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.160447 pandas-indexing-0.2.3/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.160447 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.410071 pandas-indexing-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.410071 pandas-indexing-0.2.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.402071 pandas-indexing-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.414072 pandas-indexing-0.2.4/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.3/CHANGELOG.rst` & `pandas-indexing-0.2.4/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.4 (2023-05-03)
+------------------------------------------------------------
+
+* Paper-bag release: Fix new accessors :py:func:`~accessors.IndexIdxAccessor.unique` and
+  :py:func:`~accessors.IndexIdxAccessor.__repr__` and improve tests to catch trivial
+  errors like these earlier :pull:`10`
+
 v0.2.3 (2023-05-03)
 ------------------------------------------------------------
+
 * :py:func:`~core.uniquelevel` or ``.idx.unique`` returns the unique values of one
   or multiple levels. :pull:`8`
 * :py:func:`~core.summarylevel` creates a string summarizing the index levels and their
   values. Can also be accessed as ``df.idx`` or ``index.idx`` :pull:`9`
 
 v0.2.2 (2023-05-02)
 ------------------------------------------------------------
+
 * :py:func:`~core.assignlevel` takes labels from an optional positional dataframe :pull:`5`
 * Add :py:func:`~core.dropnalevel` to remove missing index entries :pull:`4`, :pull:`6`
 
 v0.2.1 (2023-04-08)
 ------------------------------------------------------------
 
 * Restore compatibility with python 3.8
```

### Comparing `pandas-indexing-0.2.3/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/CONTRIBUTING.rst` & `pandas-indexing-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/LICENSE` & `pandas-indexing-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/PKG-INFO` & `pandas-indexing-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.3
+Version: 0.2.4
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.3/README.rst` & `pandas-indexing-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/docs/api.rst` & `pandas-indexing-0.2.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/docs/conf.py` & `pandas-indexing-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.4/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/pyproject.toml` & `pandas-indexing-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.4/src/pandas_indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.4/src/pandas_indexing/accessors.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Convenience accessor for accessing `pandas-indexing` functions.
     """
 
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
     def __repr__(self):
-        return summarylevel(self.obj)
+        return summarylevel(self._obj)
 
     def assign(
         self,
         frame: Optional[Data] = None,
         order: bool = False,
         axis: int = 0,
         **labels: Any,
@@ -86,15 +86,15 @@
         -------
         unique_index : Index
 
         See also
         --------
         pandas.Index.unique
         """
-        return uniquelevel(self.obj, levels=levels, axis=axis)
+        return uniquelevel(self._obj, levels=levels, axis=axis)
 
     def project(
         self,
         levels: Sequence[str],
         axis: Union[int, str] = 0,
     ) -> Union[DataFrame, Series, Index]:
         """
```

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.4/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/core.py` & `pandas-indexing-0.2.4/src/pandas_indexing/core.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.4/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.4/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.4/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.4/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.4/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.3
+Version: 0.2.4
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.3/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.4/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

