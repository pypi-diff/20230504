# Comparing `tmp/z3c.jbot-1.1.1.tar.gz` & `tmp/z3c.jbot-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z3c.jbot-1.1.1.tar", last modified: Wed Aug 18 08:34:24 2021, max compression
+gzip compressed data, was "z3c.jbot-2.0.tar", last modified: Thu May  4 14:37:49 2023, max compression
```

## Comparing `z3c.jbot-1.1.1.tar` & `z3c.jbot-2.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/
--rw-r--r--   0 laurent    (501) staff       (20)     6501 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/bootstrap.py
--rw-r--r--   0 laurent    (501) staff       (20)     7530 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)       70 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/constraints.txt
--rw-r--r--   0 laurent    (501) staff       (20)       88 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)       32 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/COPYRIGHT.rst
--rw-r--r--   0 laurent    (501) staff       (20)      210 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/buildout.cfg
--rw-r--r--   0 laurent    (501) staff       (20)      132 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     1651 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/setup.py
--rw-r--r--   0 laurent    (501) staff       (20)      182 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/tox.ini
--rw-r--r--   0 laurent    (501) staff       (20)     2070 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/LICENSE.rst
--rw-r--r--   0 laurent    (501) staff       (20)      207 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     1647 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/README.rst
--rw-r--r--   0 laurent    (501) staff       (20)     3296 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/CHANGES.rst
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/
--rw-r--r--   0 laurent    (501) staff       (20)      200 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/
--rw-r--r--   0 laurent    (501) staff       (20)      179 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/interfaces.py
--rw-r--r--   0 laurent    (501) staff       (20)      261 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1569 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/utility.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/https/
--rw-r--r--   0 laurent    (501) staff       (20)       23 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/https/z3c.jbot.tests.templates.example.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/interface/
--rw-r--r--   0 laurent    (501) staff       (20)       27 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/interface/z3c.jbot.tests.templates.example.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/resources/
--rw-r--r--   0 laurent    (501) staff       (20)        9 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/resources/z3c.jbot.tests.resources.test.txt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/http/
--rw-r--r--   0 laurent    (501) staff       (20)       22 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/http/z3c.jbot.tests.templates.example.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/request/
--rw-r--r--   0 laurent    (501) staff       (20)       25 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/overrides/request/z3c.jbot.tests.templates.example.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1084 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/test_doctests.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/resources/
--rw-r--r--   0 laurent    (501) staff       (20)        9 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/resources/test.txt
--rw-r--r--   0 laurent    (501) staff       (20)     3178 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/test_five.py
--rw-r--r--   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      784 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/common.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/templates/
--rw-r--r--   0 laurent    (501) staff       (20)       64 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/tests/templates/example.pt
--rw-r--r--   0 laurent    (501) staff       (20)       31 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1030 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/browser.py
--rw-r--r--   0 laurent    (501) staff       (20)     4059 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/patches.py
--rw-r--r--   0 laurent    (501) staff       (20)      533 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/metadirectives.py
--rw-r--r--   0 laurent    (501) staff       (20)     1817 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/metaconfigure.py
--rw-r--r--   0 laurent    (501) staff       (20)      584 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/meta.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     7685 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/README.rst
--rw-r--r--   0 laurent    (501) staff       (20)     5318 2021-08-18 08:34:23.000000 z3c.jbot-1.1.1/src/z3c/jbot/manager.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     7530 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)        1 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/not-zip-safe
--rw-r--r--   0 laurent    (501) staff       (20)        4 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/namespace_packages.txt
--rw-r--r--   0 laurent    (501) staff       (20)     1316 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)       53 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      164 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        4 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2021-08-18 08:34:24.000000 z3c.jbot-1.1.1/src/z3c.jbot.egg-info/dependency_links.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.897944 z3c.jbot-2.0/
+-rw-r--r--   0 mac        (513) staff       (20)     3417 2023-05-04 14:37:47.000000 z3c.jbot-2.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-04 14:37:47.000000 z3c.jbot-2.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-04 14:37:47.000000 z3c.jbot-2.0/COPYRIGHT.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-04 14:37:47.000000 z3c.jbot-2.0/LICENSE.rst
+-rw-r--r--   0 mac        (513) staff       (20)      308 2023-05-04 14:37:47.000000 z3c.jbot-2.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     5910 2023-05-04 14:37:49.898220 z3c.jbot-2.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1647 2023-05-04 14:37:47.000000 z3c.jbot-2.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      418 2023-05-04 14:37:49.900898 z3c.jbot-2.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1615 2023-05-04 14:37:47.000000 z3c.jbot-2.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.831645 z3c.jbot-2.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.848778 z3c.jbot-2.0/src/z3c/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.878096 z3c.jbot-2.0/src/z3c/jbot/
+-rw-r--r--   0 mac        (513) staff       (20)     7683 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1048 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/browser.py
+-rw-r--r--   0 mac        (513) staff       (20)      261 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      179 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     5313 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/manager.py
+-rw-r--r--   0 mac        (513) staff       (20)      584 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/meta.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1815 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/metaconfigure.py
+-rw-r--r--   0 mac        (513) staff       (20)      530 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/metadirectives.py
+-rw-r--r--   0 mac        (513) staff       (20)     4054 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/patches.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.887652 z3c.jbot-2.0/src/z3c/jbot/tests/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      784 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/common.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.840346 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.889393 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/http/
+-rw-r--r--   0 mac        (513) staff       (20)       22 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/http/z3c.jbot.tests.templates.example.pt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.890825 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/https/
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/https/z3c.jbot.tests.templates.example.pt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.893277 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/interface/
+-rw-r--r--   0 mac        (513) staff       (20)       27 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/interface/z3c.jbot.tests.templates.example.pt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.894375 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/request/
+-rw-r--r--   0 mac        (513) staff       (20)       25 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/request/z3c.jbot.tests.templates.example.pt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.895133 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/resources/
+-rw-r--r--   0 mac        (513) staff       (20)        9 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/overrides/resources/z3c.jbot.tests.resources.test.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.895927 z3c.jbot-2.0/src/z3c/jbot/tests/resources/
+-rw-r--r--   0 mac        (513) staff       (20)        9 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/resources/test.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.897278 z3c.jbot-2.0/src/z3c/jbot/tests/templates/
+-rw-r--r--   0 mac        (513) staff       (20)       64 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/templates/example.pt
+-rw-r--r--   0 mac        (513) staff       (20)      567 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/test_doctests.py
+-rw-r--r--   0 mac        (513) staff       (20)     3152 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/tests/test_five.py
+-rw-r--r--   0 mac        (513) staff       (20)     1574 2023-05-04 14:37:47.000000 z3c.jbot-2.0/src/z3c/jbot/utility.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 14:37:49.862938 z3c.jbot-2.0/src/z3c.jbot.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     5910 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1273 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)       40 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (513) staff       (20)        4 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      159 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        4 2023-05-04 14:37:49.000000 z3c.jbot-2.0/src/z3c.jbot.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1417 2023-05-04 14:37:47.000000 z3c.jbot-2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `z3c.jbot-1.1.1/setup.py` & `z3c.jbot-2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-__version__ = '1.1.1'
 
 setup(
     name='z3c.jbot',
-    version=__version__,
+    version='2.0',
     description="Drop-in template overrides.",
     long_description=(open('README.rst').read() + "\n" +
                       open('CHANGES.rst').read()),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Zope',
-        'Framework :: Zope2',
-        'Framework :: Zope :: 2',
-        'Framework :: Zope3',
         'Framework :: Zope :: 3',
-        'Framework :: Zope :: 4',
+        'Framework :: Zope :: 5',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='page template override',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     url='https://github.com/zopefoundation/z3c.jbot',
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['z3c'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
-        'six',
         'zope.pagetemplate',
         'zope.component',
         'zope.configuration',
         'zope.security',
         'zope.publisher',
     ],
     extras_require={
         'test': [
-            'Zope2',
+            'Zope',
             'Products.BTreeFolder2',
             'Products.CMFCore',
             'plone.resource',
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
```

### Comparing `z3c.jbot-1.1.1/LICENSE.rst` & `z3c.jbot-2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `z3c.jbot-1.1.1/README.rst` & `z3c.jbot-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.jbot-1.1.1/CHANGES.rst` & `z3c.jbot-2.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+2.0 (2023-05-04)
+----------------
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 1.1.1 (2021-08-18)
 ------------------
 
 - Fix error in find_zope2_product: "TypeError: expected str, bytes or os.PathLike object, not list".
   [jensens]
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/utility.py` & `z3c.jbot-2.0/src/z3c/jbot/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from z3c.jbot.interfaces import ITemplateManager
+import zope.security.interfaces
+import zope.security.management
 from zope.component import getGlobalSiteManager
 from zope.component.hooks import getSite
 from zope.interface import Interface
 from zope.interface import providedBy
 from zope.publisher.interfaces import IRequest
-import zope.security.interfaces
-import zope.security.management
+
+from z3c.jbot.interfaces import ITemplateManager
 
 
 try:
     import Acquisition  # noqa
-    ZOPE_2 = True
+    ZOPE_3 = False
 except ImportError:
-    ZOPE_2 = False
+    ZOPE_3 = True
 
 
 def getRequest():
-    if ZOPE_2:
+    if not ZOPE_3:
         # get request by acquisition
         site = getSite()
         if site is not None:
             try:
                 return site.request
             except AttributeError:
                 return site.REQUEST
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/tests/test_five.py` & `z3c.jbot-2.0/src/z3c/jbot/tests/test_five.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,43 +4,42 @@
 
 from . import common
 
 
 class FiveTests(ZopeTestCase):
     def setUp(self):
         common.setUp(self)
-        super(FiveTests, self).setUp()
-
-        from Products.Five.browser.pagetemplatefile import (
-            ZopeTwoPageTemplateFile as Template
-        )
+        super().setUp()
 
         from Products.Five.browser import BrowserView
+        from Products.Five.browser.pagetemplatefile import \
+            ZopeTwoPageTemplateFile as Template
 
         class MockView(BrowserView):
             template = Template("templates/example.pt")
             interface_override = Template(
                 "overrides/interface/z3c.jbot.tests.templates.example.pt"
             )
             http_override = Template(
                 "overrides/http/z3c.jbot.tests.templates.example.pt"
             )
             https_override = Template(
                 "overrides/https/z3c.jbot.tests.templates.example.pt"
             )
 
         # set up mock site and request
-        from zope.publisher.browser import TestRequest
         from zope import component
+        from zope.publisher.browser import TestRequest
 
-        class MockSite(object):
+        class MockSite:
             REQUEST = TestRequest("en")
             getSiteManager = component.getSiteManager
 
-        from zope.component.hooks import setHooks, setSite
+        from zope.component.hooks import setHooks
+        from zope.component.hooks import setSite
 
         setHooks()
         setSite(MockSite())
         self._request = MockSite.REQUEST
 
         # render templates for later comparison
         view = self._view = MockView(self.folder, MockSite.REQUEST)
@@ -55,25 +54,27 @@
 
     def tearDown(self):
         import zope.component.testing
 
         zope.component.testing.tearDown(self)
 
     def test_override_for_interface(self):
-        from z3c.jbot.metaconfigure import handler
         from zope import interface
 
+        from z3c.jbot.metaconfigure import handler
+
         handler("%s/overrides/interface" % self._tests, interface.Interface)
         self.assertEqual(self._view.template(), self._interface_override)
 
     def test_override_for_httprequest(self):
-        from z3c.jbot.metaconfigure import handler
         from zope import interface
         from zope.publisher.interfaces.browser import IHTTPRequest
 
+        from z3c.jbot.metaconfigure import handler
+
         class IHTTPSRequest(IHTTPRequest):
             pass
 
         # register handlers
         handler("%s/overrides/interface" % self._tests, interface.Interface)
         handler("%s/overrides/https" % self._tests, IHTTPSRequest)
 
@@ -90,12 +91,9 @@
         from zope.interface import noLongerProvides
 
         noLongerProvides(self._request, IHTTPSRequest)
         self.assertEqual(self._view.template(), self._interface_override)
 
 
 def test_suite():
-    return unittest.TestSuite((unittest.makeSuite(FiveTests),))
-
-
-if __name__ == '__main__':
-    unittest.main(defaultTest='test_suite')
+    return unittest.TestSuite(
+        (unittest.defaultTestLoader.loadTestsFromTestCase(FiveTests),))
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/tests/common.py` & `z3c.jbot-2.0/src/z3c/jbot/tests/common.py`

 * *Files identical despite different names*

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/browser.py` & `z3c.jbot-2.0/src/z3c/jbot/browser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from zope.interface import implementer, providedBy
+from zope.interface import implementer
+from zope.interface import providedBy
 from zope.publisher.interfaces.browser import IBrowserPublisher
 
+
 try:
     from plone.resource.file import FilesystemFile
     HAS_PLONE_RESOURCE = True
 except ImportError:
     HAS_PLONE_RESOURCE = False
 
 from .utility import getManagers
 
 
 @implementer(IBrowserPublisher)
-class FilesystemFileResourceBrowserPublisher(object):
+class FilesystemFileResourceBrowserPublisher:
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def browserDefault(self, request):
         assert HAS_PLONE_RESOURCE
         layer = providedBy(request)
@@ -29,8 +31,7 @@
                     self.context.__name__,
                 )
                 break
         else:
             resource = self.context
 
         return resource, ()
-
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/patches.py` & `z3c.jbot-2.0/src/z3c/jbot/patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 from zope.pagetemplate.pagetemplatefile import PageTemplateFile
 
 from . import utility
 
+
 try:
     from Acquisition.interfaces import IAcquirer
 except ImportError:
     IAcquirer = None
 
 
 logger = logging.getLogger('jbot')
@@ -68,17 +69,16 @@
     logger.debug(repr(pt_class))
 
     del pt_class
 
 # Zope 2.12 ViewPageTemplateFile; note that we import
 # ``BoundPageTemplate`` to provoke an import-error on Zope 2.10.
 try:
-    from Products.Five.browser.pagetemplatefile import (
+    from Products.Five.browser.pagetemplatefile import \
         ViewPageTemplateFile as pt_class
-    )
     zope_bind = pt_class.__get__
 except ImportError:
     pass
 except AttributeError:
     pass
 else:
     def five_get_and_bind(template, view=None, cls=None):
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/metadirectives.py` & `z3c.jbot-2.0/src/z3c/jbot/metadirectives.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from zope.interface import Interface
 
 
 class ITemplateOverridesDirective(Interface):
     """Directive which registers a directory with template overrides."""
 
     directory = fields.Path(
-        title=u"Path to directory",
+        title="Path to directory",
         required=True,
     )
 
     layer = GlobalObject(
-        title=u"The layer the overrides should be enabled for",
-        description=u"By default overrides are used for all layers.",
+        title="The layer the overrides should be enabled for",
+        description="By default overrides are used for all layers.",
         required=False,
     )
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/metaconfigure.py` & `z3c.jbot-2.0/src/z3c/jbot/metaconfigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from zope import component
 from zope import interface
 from zope.publisher.interfaces.browser import IBrowserPublisher
 
+
 try:
     from plone.resource.file import FilesystemFile
     HAS_PLONE_RESOURCE = True
 except ImportError:
     HAS_PLONE_RESOURCE = False
 
+from . import browser
 from . import interfaces
 from . import manager
-from . import browser
 
 
 def handler(directory, layer):
     lookup_all = component.getGlobalSiteManager().adapters.lookupAll
 
     # check if a template manager already exists
-    factories = set(
+    factories = {
         factory
         for name, factory in lookup_all((layer,), interfaces.ITemplateManager)
-    )
+    }
 
     # this might yield several factories (template managers); we check
     # if one is registered for exactly our layer
     base_factories = set()
     if layer is not interface.Interface:
         for base in layer.__bases__:
             for name, factory in lookup_all(
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/meta.zcml` & `z3c.jbot-2.0/src/z3c/jbot/meta.zcml`

 * *Files identical despite different names*

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/README.rst` & `z3c.jbot-2.0/src/z3c/jbot/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 Using ZCML
 ----------
 
 First we load the metadirectives of the package. This will allow us
 to register template overrides directories in configuration files.
 
-  >>> from six import StringIO
+  >>> from io import StringIO
   >>> from zope.configuration import xmlconfig
   >>> xmlconfig.XMLConfig('meta.zcml', z3c.jbot)()
 
 Let's try registering the directory again::
 
   >>> xmlconfig.xmlconfig(StringIO("""
   ... <configure xmlns="http://namespaces.zope.org/browser">
@@ -264,8 +264,7 @@
   >>> from zope.component import getMultiAdapter
   >>> from zope.publisher.interfaces.browser import IBrowserPublisher
   >>> publisher = getMultiAdapter((resource, interface.Interface), IBrowserPublisher)
   >>> resource, _ = publisher.browserDefault(None)
   >>> with open(resource.path) as f:
   ...     f.read()
   'Override\n'
-
```

### Comparing `z3c.jbot-1.1.1/src/z3c/jbot/manager.py` & `z3c.jbot-2.0/src/z3c/jbot/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-import tempfile
 
 from zope.interface import implementer
 
 from . import interfaces
 from . import utility
 
 
@@ -25,84 +24,86 @@
 def sort_by_path(path, paths):
     return sorted(
         paths, key=lambda syspath: root_length(syspath, path), reverse=True
     )
 
 
 def find_zope2_product(path):
-    """Check the Zope2 magic Products semi-namespace to see if the
+    """Check the Zope 5 magic Products semi-namespace to see if the
     path is part of a Product."""
     _syspaths = sort_by_path(
-        path, 
+        path,
         [normalize(path) for path in sys.modules["Products"].__path__],
     )
     syspath = _syspaths[0]
 
     if not path.startswith(syspath):
         return
 
-    product = path[len(syspath) + 1 :].split(os.path.sep, 2)[0]
+    product = path[len(syspath) + 1:].split(os.path.sep, 2)[0]
 
     return normalize("Products." + product)
 
 
 def find_package(syspaths, path):
     """Determine the Python-package where path is located.  If the path is
     not located within the Python sys-path, return ``None``.
     The returned path is already 'normcase'. """
 
     _syspaths = sort_by_path(path, syspaths)
     syspath = _syspaths[0]
 
     if not path.startswith(syspath):
-        if utility.ZOPE_2:
+        if not utility.ZOPE_3:
             return find_zope2_product(path)
         return None
 
-    path = path[len(syspath) :]
+    path = path[len(syspath):]
 
     # convert path to dotted filename
     if path.startswith(os.path.sep):
         path = path[1:]
     return path
 
 
-class ResourceManagerFactory(object):
+class ResourceManagerFactory:
     def __init__(self, name):
         self.manager = TemplateManager(name)
 
     def __call__(self, layer):
         return self.manager
 
 
-class TemplateManagerFactory(object):
+class TemplateManagerFactory:
     def __init__(self, name):
         self.manager = TemplateManager(name)
 
     def __call__(self, layer):
         return self.manager
 
 
 @implementer(interfaces.ITemplateManager)
-class TemplateManager(object):
+class TemplateManager:
     def __init__(self, name):
         self.syspaths = {normalize(p) for p in sys.path}
         self.resources = {}
         self.templates = {}
         self.paths = {}
         self.directories = set()
         self.name = name
 
     def registerDirectory(self, directory):
         directory = normalize(directory)
         self.directories.add(directory)
 
         for filename in os.listdir(directory):
             filename = os.path.normcase(filename)
-            self.paths[filename] = normalize("%s%s%s" % (directory, os.path.sep, filename))
+            self.paths[filename] = normalize(
+                "%s%s%s" %
+                (directory, os.path.sep, filename))
 
         for template, filename in list(self.templates.items()):
             if filename is IGNORE:
                 del self.templates[template]
 
     def unregisterDirectory(self, directory):
         directory = normalize(directory)
```

### Comparing `z3c.jbot-1.1.1/src/z3c.jbot.egg-info/SOURCES.txt` & `z3c.jbot-2.0/src/z3c.jbot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-bootstrap.py
-buildout.cfg
-constraints.txt
-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 src/z3c/__init__.py
 src/z3c.jbot.egg-info/PKG-INFO
 src/z3c.jbot.egg-info/SOURCES.txt
 src/z3c.jbot.egg-info/dependency_links.txt
```

