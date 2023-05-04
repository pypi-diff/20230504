# Comparing `tmp/hurry.query-3.2.tar.gz` & `tmp/hurry.query-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hurry.query-3.2.tar", last modified: Mon Nov 16 16:07:23 2020, max compression
+gzip compressed data, was "hurry.query-4.0.tar", last modified: Thu May  4 06:27:30 2023, max compression
```

## Comparing `hurry.query-3.2.tar` & `hurry.query-4.0.tar`

### file list

```diff
@@ -1,41 +1,36 @@
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.406184 hurry.query-3.2/
--rw-r--r--   0 sylvain    (501) staff       (20)      170 2020-11-16 16:07:22.000000 hurry.query-3.2/.gitignore
--rw-r--r--   0 sylvain    (501) staff       (20)      368 2020-11-16 16:07:22.000000 hurry.query-3.2/.travis.yml
--rw-r--r--   0 sylvain    (501) staff       (20)     5172 2020-11-16 16:07:22.000000 hurry.query-3.2/CHANGES.txt
--rw-r--r--   0 sylvain    (501) staff       (20)       32 2020-11-16 16:07:22.000000 hurry.query-3.2/COPYRIGHT.txt
--rw-r--r--   0 sylvain    (501) staff       (20)      249 2020-11-16 16:07:22.000000 hurry.query-3.2/CREDITS.txt
--rw-r--r--   0 sylvain    (501) staff       (20)      264 2020-11-16 16:07:22.000000 hurry.query-3.2/INSTALL.txt
--rw-r--r--   0 sylvain    (501) staff       (20)     2070 2020-11-16 16:07:22.000000 hurry.query-3.2/LICENSE.txt
--rw-r--r--   0 sylvain    (501) staff       (20)       57 2020-11-16 16:07:22.000000 hurry.query-3.2/MANIFEST.in
--rw-r--r--   0 sylvain    (501) staff       (20)     8482 2020-11-16 16:07:23.405783 hurry.query-3.2/PKG-INFO
--rw-r--r--   0 sylvain    (501) staff       (20)      336 2020-11-16 16:07:22.000000 hurry.query-3.2/README.txt
--rw-r--r--   0 sylvain    (501) staff       (20)     2179 2020-11-16 16:07:22.000000 hurry.query-3.2/ZopePublicLicense.txt
--rw-r--r--   0 sylvain    (501) staff       (20)     2516 2020-11-16 16:07:22.000000 hurry.query-3.2/bootstrap.py
--rw-r--r--   0 sylvain    (501) staff       (20)      247 2020-11-16 16:07:22.000000 hurry.query-3.2/buildout.cfg
--rw-r--r--   0 sylvain    (501) staff       (20)      124 2020-11-16 16:07:22.000000 hurry.query-3.2/requirements.txt
--rw-r--r--   0 sylvain    (501) staff       (20)       38 2020-11-16 16:07:23.406264 hurry.query-3.2/setup.cfg
--rw-r--r--   0 sylvain    (501) staff       (20)     3045 2020-11-16 16:07:22.000000 hurry.query-3.2/setup.py
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.396338 hurry.query-3.2/src/
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.400799 hurry.query-3.2/src/hurry/
--rw-r--r--   0 sylvain    (501) staff       (20)       56 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/__init__.py
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.404614 hurry.query-3.2/src/hurry/query/
--rw-r--r--   0 sylvain    (501) staff       (20)      831 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/__init__.py
--rw-r--r--   0 sylvain    (501) staff       (20)      152 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/configure.zcml
--rw-r--r--   0 sylvain    (501) staff       (20)     3023 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/interfaces.py
--rw-r--r--   0 sylvain    (501) staff       (20)    17096 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/query.py
--rw-r--r--   0 sylvain    (501) staff       (20)    22502 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/query.txt
--rw-r--r--   0 sylvain    (501) staff       (20)     3072 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/set.py
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.405431 hurry.query-3.2/src/hurry/query/tests/
--rw-r--r--   0 sylvain    (501) staff       (20)      826 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/tests/__init__.py
--rw-r--r--   0 sylvain    (501) staff       (20)      140 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/tests/test_doctests.py
--rw-r--r--   0 sylvain    (501) staff       (20)    13942 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/tests/test_query.py
--rw-r--r--   0 sylvain    (501) staff       (20)     4145 2020-11-16 16:07:22.000000 hurry.query-3.2/src/hurry/query/value.py
-drwxr-xr-x   0 sylvain    (501) staff       (20)        0 2020-11-16 16:07:23.402870 hurry.query-3.2/src/hurry.query.egg-info/
--rw-r--r--   0 sylvain    (501) staff       (20)     8482 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/PKG-INFO
--rw-r--r--   0 sylvain    (501) staff       (20)      788 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/SOURCES.txt
--rw-r--r--   0 sylvain    (501) staff       (20)        1 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/dependency_links.txt
--rw-r--r--   0 sylvain    (501) staff       (20)        6 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/namespace_packages.txt
--rw-r--r--   0 sylvain    (501) staff       (20)        1 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/not-zip-safe
--rw-r--r--   0 sylvain    (501) staff       (20)      182 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/requires.txt
--rw-r--r--   0 sylvain    (501) staff       (20)        6 2020-11-16 16:07:23.000000 hurry.query-3.2/src/hurry.query.egg-info/top_level.txt
--rw-r--r--   0 sylvain    (501) staff       (20)      638 2020-11-16 16:07:22.000000 hurry.query-3.2/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.977653 hurry.query-4.0/
+-rw-r--r--   0 mac        (513) staff       (20)     5293 2023-05-04 06:27:30.000000 hurry.query-4.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-04 06:27:30.000000 hurry.query-4.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-04 06:27:30.000000 hurry.query-4.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)      249 2023-05-04 06:27:30.000000 hurry.query-4.0/CREDITS.rst
+-rw-r--r--   0 mac        (513) staff       (20)      264 2023-05-04 06:27:30.000000 hurry.query-4.0/INSTALL.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-04 06:27:30.000000 hurry.query-4.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      224 2023-05-04 06:27:30.000000 hurry.query-4.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     6901 2023-05-04 06:27:30.977780 hurry.query-4.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      336 2023-05-04 06:27:30.000000 hurry.query-4.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      514 2023-05-04 06:27:30.978342 hurry.query-4.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2822 2023-05-04 06:27:30.000000 hurry.query-4.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.966962 hurry.query-4.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.971640 hurry.query-4.0/src/hurry/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.976370 hurry.query-4.0/src/hurry/query/
+-rw-r--r--   0 mac        (513) staff       (20)     1137 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      152 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     3049 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)    17003 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/query.py
+-rw-r--r--   0 mac        (513) staff       (20)    22502 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/query.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2990 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/set.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.977354 hurry.query-4.0/src/hurry/query/tests/
+-rw-r--r--   0 mac        (513) staff       (20)     1103 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       83 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/tests/test_doctests.py
+-rw-r--r--   0 mac        (513) staff       (20)    13996 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/tests/test_query.py
+-rw-r--r--   0 mac        (513) staff       (20)     4043 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry/query/value.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:27:30.974004 hurry.query-4.0/src/hurry.query.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     6901 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      726 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        6 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      178 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        6 2023-05-04 06:27:30.000000 hurry.query-4.0/src/hurry.query.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1432 2023-05-04 06:27:30.000000 hurry.query-4.0/tox.ini
```

### Comparing `hurry.query-3.2/CHANGES.txt` & `hurry.query-4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+4.0 (2023-05-04)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
 3.2 (2020-11-16)
 ----------------
 
 - Add support for Python 3.7.
 
 - Add support for Python 3.8.
```

### Comparing `hurry.query-3.2/LICENSE.txt` & `hurry.query-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hurry.query-3.2/setup.py` & `hurry.query-4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,89 +7,80 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-"""Setup
-
-$Id$
-"""
+import html
 import os
-import sys
-from setuptools import setup, find_packages
 
-if sys.version_info.major > 2:
-    import html
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
-    text = open(os.path.join(os.path.dirname(__file__), *rnames)).read()
-    if sys.version_info.major == 2:
-        text = unicode(text, 'utf-8').encode('ascii', 'xmlcharrefreplace')
-    else:
-        text = html.escape(text)
-    return text
+    with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
+        text = f.read()
+    return html.escape(text)
 
 
 tests_require = [
     'testfixtures',
     'zope.container',
     ]
 
 setup(
     name="hurry.query",
-    version='3.2',
+    version='4.0',
     author='Infrae',
-    author_email='faassen@startifact.com',
-    description="Higher level query system for the zope.catalog",
-    long_description=(read('README.txt') +
+    author_email='zope-dev@zope.dev',
+    description="Higher level query system for zope.catalog.",
+    long_description=(read('README.rst') +
                       '\n\n' +
-                      read('CHANGES.txt')),
+                      read('CHANGES.rst')),
     license='ZPL 2.1',
     keywords="zope zope3 catalog index query",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
-        'Framework :: Zope :: 3'],
-    url='http://pypi.python.org/pypi/hurry.query',
+        'Framework :: Zope :: 3',
+    ],
+    url='https://github.com/zopefoundation/hurry.query',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['hurry'],
     package_data={
         '': ['*.txt', '*.zcml'],
     },
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
         'BTrees',
-        'six',
         'setuptools',
         'transaction',
         'zc.catalog',
         'zope.cachedescriptors',
         'zope.catalog',
         'zope.component',
         'zope.index',
         'zope.interface',
         'zope.intid',
         'zope.location',
     ],
-    tests_require=tests_require,
     extras_require={'test': tests_require},
     )
```

### Comparing `hurry.query-3.2/src/hurry/query/__init__.py` & `hurry.query-4.0/src/hurry/query/tests/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,13 +7,20 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-"""
-$Id$
-"""
-from hurry.query.query import All, And, Or, Eq, NotEq, Difference, Objects, Ids
-from hurry.query.query import Between, In, Ge, Le, Text
+from hurry.query.query import All
+from hurry.query.query import And
+from hurry.query.query import Between
+from hurry.query.query import Difference
+from hurry.query.query import Eq
+from hurry.query.query import Ge
+from hurry.query.query import In
+from hurry.query.query import Le
+from hurry.query.query import NotEq
+from hurry.query.query import Objects
+from hurry.query.query import Or
+from hurry.query.query import Text
 from hurry.query.query import no_results
```

### Comparing `hurry.query-3.2/src/hurry/query/interfaces.py` & `hurry.query-4.0/src/hurry/query/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Query interfaces
 """
 
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
 
 
 class IQuery(Interface):
 
     def searchResults(
             query, context=None, sort_field=None, limit=None, reverse=False,
             start=0, caching=False):
```

### Comparing `hurry.query-3.2/src/hurry/query/query.py` & `hurry.query-4.0/src/hurry/query/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,66 +12,67 @@
 #
 ##############################################################################
 """Basic query implementation
 
 This module contains an IQuery utility implementation, basic query term
 implementations and concrete term implementations for zope.catalog indexes.
 
-$Id$
 """
 import itertools
 import logging
 import os
 import time
-import six
 
 from BTrees.IFBTree import IFSet
+from BTrees.IFBTree import difference
+from BTrees.IFBTree import intersection
+from BTrees.IFBTree import multiunion
 from BTrees.IFBTree import weightedIntersection
-from BTrees.IFBTree import multiunion, difference, intersection
 from zope.cachedescriptors.property import Lazy
 from zope.catalog.field import IFieldIndex
 from zope.catalog.interfaces import ICatalog
 from zope.catalog.text import ITextIndex
-from zope.component import getUtility, getSiteManager, IComponentLookup
-from zope.interface import implementer
-from zope.intid.interfaces import IIntIds
+from zope.component import IComponentLookup
+from zope.component import getSiteManager
+from zope.component import getUtility
 from zope.index.interfaces import IIndexSort
 from zope.index.text.parsetree import ParseError
-from zope.location.location import located, LocationProxy
+from zope.interface import implementer
+from zope.intid.interfaces import IIntIds
+from zope.location.location import LocationProxy
+from zope.location.location import located
+
 from hurry.query import interfaces
 
 
 logger = logging.getLogger('hurry.query')
 HURRY_QUERY_TIMING = 0.0  # log queries taking longer than this, in seconds
 if 'HURRY_QUERY_TIMING' in os.environ:
     try:
         HURRY_QUERY_TIMING = float(os.environ['HURRY_QUERY_TIMING'])
     except (ValueError, TypeError):
         pass
 
-if six.PY3:
-    _perf_counter = time.perf_counter
-else:
-    _perf_counter = time.clock
+_perf_counter = time.perf_counter
 
 
-class Locator(object):
+class Locator:
 
     def __init__(self, container, get):
         self.container = container
         self.get = get
 
     def __call__(self, oid):
         contained = self.get(oid)
         return located(
             LocationProxy(contained), self.container, contained.__name__)
 
 
 @implementer(interfaces.IResults)
-class Results(object):
+class Results:
 
     def __init__(self, context, all_results, selected_results,
                  wrapper=None, locate_to=None):
         self.context = context
         self.locate_to = locate_to
         self.wrapper = wrapper
         self.__all = all_results
@@ -103,15 +104,15 @@
 
     def __iter__(self):
         for uid in self.__selected:
             yield self.get(uid)
 
 
 @implementer(interfaces.IResults)
-class NoResults(object):
+class NoResults:
 
     count = 0
     total = 0
 
     def first(self):
         return None
 
@@ -121,15 +122,15 @@
     def __iter__(self):
         return iter([])
 
 
 no_results = NoResults()
 
 
-class Timing(object):
+class Timing:
 
     def __init__(self, key=None, order=0):
         self.key = key
         self.start = _perf_counter()
         self.start_order = order
         self.end = None
         self.end_order = None
@@ -141,15 +142,15 @@
     @property
     def total(self):
         if self.end is not None:
             return self.end - self.start
         return None
 
 
-class TimingAwareCache(object):
+class TimingAwareCache:
 
     def __init__(self, cache):
         self.cache = cache
         self.timing = {}
         self.count = 0
         self.post = None
 
@@ -186,26 +187,26 @@
         logger.info(
             'Catalog query took {:.4f}s for terms, {:.4f}s to finish.'.format(
                 total_terms, total_post))
         for timing in all_timing:
             if order == [] or timing.start_order < order[-1]:
                 indent += 4
                 order.append(timing.end_order)
-            total = timing.total and '{:.4f}s'.format(timing.total) or '?'
+            total = timing.total and f'{timing.total:.4f}s' or '?'
             logger.info(
                 '{} {}: {}.'.format(
                     ' ' * indent, total, str(timing.key)))
             if timing.end_order and len(order) \
                and timing.end_order > order[-1]:
                 indent -= 4
                 order.pop()
 
 
 @implementer(interfaces.IQuery)
-class Query(object):
+class Query:
 
     def searchResults(
             self, query, context=None, sort_field=None, limit=None,
             reverse=False, start=0, caching=None, timing=HURRY_QUERY_TIMING,
             wrapper=None, locate_to=None):
 
         if context is None:
@@ -280,15 +281,15 @@
             timer.report(over=timing)
 
         return Results(
             context, all_results, selected_results, wrapper, locate_to)
 
 
 @implementer(interfaces.ITerm)
-class Term(object):
+class Term:
 
     def key(self, context=None):
         raise NotImplementedError()
 
     def apply(self, cache, context=None):
         raise NotImplementedError()
 
@@ -474,61 +475,61 @@
         index = catalog[self.index_name]
         return index
 
 
 class Text(IndexTerm):
 
     def __init__(self, index_id, text):
-        super(Text, self).__init__(index_id)
+        super().__init__(index_id)
         self.text = text
 
     def getIndex(self, context):
-        index = super(Text, self).getIndex(context)
+        index = super().getIndex(context)
         assert ITextIndex.providedBy(index)
         return index
 
     def apply(self, cache, context=None):
         index = self.getIndex(context)
         try:
             return index.apply(self.text)
         except ParseError:
             logger.error(
-                'search text "{}" yielded a ParseError'.format(self.text))
+                f'search text "{self.text}" yielded a ParseError')
             return IFSet()
 
     def key(self, context=None):
         return ('text', self.catalog_name, self.index_name, self.text)
 
 
 class FieldTerm(IndexTerm):
 
     def getIndex(self, context):
-        index = super(FieldTerm, self).getIndex(context)
+        index = super().getIndex(context)
         assert IFieldIndex.providedBy(index)
         return index
 
 
 class Eq(FieldTerm):
 
     def __init__(self, index_id, value):
         assert value is not None
-        super(Eq, self).__init__(index_id)
+        super().__init__(index_id)
         self.value = value
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply((self.value, self.value))
 
     def key(self, context=None):
         return ('equal', self.catalog_name, self.index_name, self.value)
 
 
 class NotEq(FieldTerm):
 
     def __init__(self, index_id, value):
-        super(NotEq, self).__init__(index_id)
+        super().__init__(index_id)
         self.value = value
 
     def apply(self, cache, context=None):
         index = self.getIndex(context)
         values = index.apply((None, None))
         matches = index.apply((self.value, self.value))
         return difference(values, matches)
@@ -546,41 +547,41 @@
         return ('all', self.catalog_name, self.index_name)
 
 
 class Between(FieldTerm):
 
     def __init__(self, index_id,
                  minimum=None, maximum=None):
-        super(Between, self).__init__(index_id)
+        super().__init__(index_id)
         self.options = (minimum, maximum)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply(self.options)
 
     def key(self, context=None):
         return ('between', self.catalog_name, self.index_name, self.options)
 
 
 class Ge(Between):
 
     def __init__(self, index_id, min_value):
-        super(Ge, self).__init__(index_id, min_value, None)
+        super().__init__(index_id, min_value, None)
 
 
 class Le(Between):
 
     def __init__(self, index_id, max_value):
-        super(Le, self).__init__(index_id, None, max_value)
+        super().__init__(index_id, None, max_value)
 
 
 class In(FieldTerm):
 
     def __init__(self, index_id, values):
         assert None not in values
-        super(In, self).__init__(index_id)
+        super().__init__(index_id)
         self.values = tuple(values)
 
     def apply(self, cache, context=None):
         results = []
         index = self.getIndex(context)
         for value in self.values:
             r = index.apply((value, value))
```

### Comparing `hurry.query-3.2/src/hurry/query/query.txt` & `hurry.query-4.0/src/hurry/query/query.rst`

 * *Files identical despite different names*

### Comparing `hurry.query-3.2/src/hurry/query/set.py` & `hurry.query-4.0/src/hurry/query/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from hurry.query import query
 
 
 class SetTerm(query.IndexTerm):
 
     def getIndex(self, context):
-        index = super(SetTerm, self).getIndex(context)
+        index = super().getIndex(context)
         assert ISetIndex.providedBy(index)
         return index
 
 
 class All(SetTerm):
 
     def apply(self, cache, context=None):
@@ -36,65 +36,65 @@
     def key(self, context=None):
         return ('all', self.catalog_name, self.index_name)
 
 
 class AnyOf(SetTerm):
 
     def __init__(self, index_id, values):
-        super(AnyOf, self).__init__(index_id)
+        super().__init__(index_id)
         self.values = tuple(values)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'any_of': self.values})
 
     def key(self, context=None):
         return ('any of', self.catalog_name, self.index_name, self.values)
 
 
 class AllOf(SetTerm):
 
     def __init__(self, index_id, values):
-        super(AllOf, self).__init__(index_id)
+        super().__init__(index_id)
         self.values = tuple(values)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'all_of': self.values})
 
     def key(self, context=None):
         return ('all of', self.catalog_name, self.index_name, self.values)
 
 
 class SetBetween(SetTerm):
 
     def __init__(self, index_id,
                  minimum=None, maximum=None,
                  exclude_min=False, exclude_max=False):
-        super(SetBetween, self).__init__(index_id)
+        super().__init__(index_id)
         self.options = (minimum, maximum, exclude_min, exclude_max)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'between': self.options})
 
     def key(self, context=None):
         return ('between', self.catalog_name, self.index_name, self.options)
 
 
 class ExtentAny(SetTerm):
     """Any ids in the extent that are indexed by this index."""
 
     def __init__(self, index_id, extent):
-        super(ExtentAny, self).__init__(index_id)
+        super().__init__(index_id)
         self.extent = extent
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'any': self.extent})
 
 
 class ExtentNone(SetTerm):
     """Any ids in the extent that are not indexed by this index."""
 
     def __init__(self, index_id, extent):
-        super(ExtentNone, self).__init__(index_id)
+        super().__init__(index_id)
         self.extent = extent
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'none': self.extent})
```

### Comparing `hurry.query-3.2/src/hurry/query/tests/test_query.py` & `hurry.query-4.0/src/hurry/query/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import functools
 import time
 import unittest
+
 import zope.component.testing
 import zope.intid.interfaces
-
 from testfixtures import LogCapture
 from zope.catalog.catalog import Catalog
 from zope.catalog.field import FieldIndex
 from zope.catalog.interfaces import ICatalog
 from zope.catalog.text import TextIndex
-from zope.component import provideUtility, getUtility
+from zope.component import getUtility
+from zope.component import provideUtility
 from zope.container.contained import Contained
-from zope.interface import Interface, Attribute, implementer
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
 
 from hurry.query import query
 from hurry.query.interfaces import IQuery
 
 
 """Bring `query` testcoverage to 100% without polluting the doctest"""
 
@@ -45,19 +48,19 @@
     def __lt__(self, other):
         return self.id < other.id
 
     def __eq__(self, other):
         return self.id == other.id
 
     def __repr__(self):
-        return '<Content "{}">'.format(self.id)
+        return f'<Content "{self.id}">'
 
 
 @implementer(zope.intid.interfaces.IIntIds)
-class DummyIntId(object):
+class DummyIntId:
     MARKER = '__dummy_int_id__'
 
     def __init__(self):
         self.counter = 0
         self.data = {}
 
     def register(self, obj):
@@ -303,15 +306,15 @@
 
         self.assertTrue(records[2].msg.endswith('  ?: foobar.'))
 
 
 class QueryTest(QueryTestBase):
 
     def test_injected_caching(self):
-        class MockCaching(object):
+        class MockCaching:
             _cache = dict()
             _get = 0
             _set = 0
 
             def get(self, key):
                 self._get += 1
                 return self._cache.get(key)
```

### Comparing `hurry.query-3.2/src/hurry/query/value.py` & `hurry.query-4.0/src/hurry/query/value.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 
 from hurry.query import query
 
 
 class ValueTerm(query.IndexTerm):
 
     def getIndex(self, context):
-        index = super(ValueTerm, self).getIndex(context)
+        index = super().getIndex(context)
         assert IValueIndex.providedBy(index)
         return index
 
 
 class Eq(ValueTerm):
 
     def __init__(self, index_id, value):
         assert value is not None
-        super(Eq, self).__init__(index_id)
+        super().__init__(index_id)
         self.value = value
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'any_of': (self.value,)})
 
     def key(self, context=None):
         return ('equal', self.catalog_name, self.index_name, self.value)
 
 
 class NotEq(ValueTerm):
 
     def __init__(self, index_id, value):
-        super(NotEq, self).__init__(index_id)
+        super().__init__(index_id)
         self.value = value
 
     def apply(self, cache, context=None):
         index = self.getIndex(context)
         values = list(index.values())
         # the remove method produces a value error when the value to
         # be removed is not in the list in the first place.  Having a
@@ -74,63 +74,63 @@
         return ('all', self.catalog_name, self.index_name)
 
 
 class Between(ValueTerm):
 
     def __init__(self, index_id, min_value=None, max_value=None,
                  exclude_min=False, exclude_max=False):
-        super(Between, self).__init__(index_id)
+        super().__init__(index_id)
         self.options = (min_value, max_value, exclude_min, exclude_max)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'between': self.options})
 
     def key(self, context=None):
         return ('between', self.catalog_name, self.index_name, self.options)
 
 
 class Ge(Between):
 
     def __init__(self, index_id, min_value):
-        super(Ge, self).__init__(index_id, min_value=min_value)
+        super().__init__(index_id, min_value=min_value)
 
 
 class Le(Between):
 
     def __init__(self, index_id, max_value):
-        super(Le, self).__init__(index_id, max_value=max_value)
+        super().__init__(index_id, max_value=max_value)
 
 
 class In(ValueTerm):
 
     def __init__(self, index_id, values):
         assert None not in values
-        super(In, self).__init__(index_id)
+        super().__init__(index_id)
         self.values = tuple(values)
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'any_of': self.values})
 
     def key(self, context=None):
         return ('in', self.catalog_name, self.index_name, self.values)
 
 
 class ExtentAny(ValueTerm):
     """Any ids in the extent that are indexed by this index."""
 
     def __init__(self, index_id, extent):
-        super(ExtentAny, self).__init__(index_id)
+        super().__init__(index_id)
         self.extent = extent
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'any': self.extent})
 
 
 class ExtentNone(ValueTerm):
     """Any ids in the extent that are not indexed by this index."""
 
     def __init__(self, index_id, extent):
-        super(ExtentNone, self).__init__(index_id)
+        super().__init__(index_id)
         self.extent = extent
 
     def apply(self, cache, context=None):
         return self.getIndex(context).apply({'none': self.extent})
```

### Comparing `hurry.query-3.2/src/hurry.query.egg-info/SOURCES.txt` & `hurry.query-4.0/src/hurry.query.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-.gitignore
-.travis.yml
-CHANGES.txt
+CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
-CREDITS.txt
-INSTALL.txt
+CREDITS.rst
+INSTALL.rst
 LICENSE.txt
 MANIFEST.in
-README.txt
-ZopePublicLicense.txt
-bootstrap.py
-buildout.cfg
-requirements.txt
+README.rst
+setup.cfg
 setup.py
 tox.ini
 src/hurry/__init__.py
 src/hurry.query.egg-info/PKG-INFO
 src/hurry.query.egg-info/SOURCES.txt
 src/hurry.query.egg-info/dependency_links.txt
 src/hurry.query.egg-info/namespace_packages.txt
 src/hurry.query.egg-info/not-zip-safe
 src/hurry.query.egg-info/requires.txt
 src/hurry.query.egg-info/top_level.txt
 src/hurry/query/__init__.py
 src/hurry/query/configure.zcml
 src/hurry/query/interfaces.py
 src/hurry/query/query.py
-src/hurry/query/query.txt
+src/hurry/query/query.rst
 src/hurry/query/set.py
 src/hurry/query/value.py
 src/hurry/query/tests/__init__.py
 src/hurry/query/tests/test_doctests.py
 src/hurry/query/tests/test_query.py
```

