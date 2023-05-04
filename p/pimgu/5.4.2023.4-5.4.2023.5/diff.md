# Comparing `tmp/pimgu-5.4.2023.4.tar.gz` & `tmp/pimgu-5.4.2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimgu-5.4.2023.4.tar", last modified: Thu May  4 20:54:24 2023, max compression
+gzip compressed data, was "pimgu-5.4.2023.5.tar", last modified: Thu May  4 20:56:37 2023, max compression
```

## Comparing `pimgu-5.4.2023.4.tar` & `pimgu-5.4.2023.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:54:24.067985 pimgu-5.4.2023.4/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     1067 2023-05-04 17:58:18.000000 pimgu-5.4.2023.4/LICENSE
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:54:24.067653 pimgu-5.4.2023.4/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)     3546 2023-05-04 20:41:55.000000 pimgu-5.4.2023.4/README.md
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:54:24.064846 pimgu-5.4.2023.4/pimgu/
--rw-r--r--   0 ianwilkey   (501) staff       (20)      425 2023-05-04 20:53:49.000000 pimgu-5.4.2023.4/pimgu/__init__.py
--rw-r--r--   0 ianwilkey   (501) staff       (20)     8989 2023-05-04 20:34:27.000000 pimgu-5.4.2023.4/pimgu/applet.py
--rw-r--r--   0 ianwilkey   (501) staff       (20)     2479 2023-05-04 20:29:19.000000 pimgu-5.4.2023.4/pimgu/pimgl.py
-drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:54:24.067035 pimgu-5.4.2023.4/pimgu.egg-info/
--rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:54:23.000000 pimgu-5.4.2023.4/pimgu.egg-info/PKG-INFO
--rw-r--r--   0 ianwilkey   (501) staff       (20)      219 2023-05-04 20:54:23.000000 pimgu-5.4.2023.4/pimgu.egg-info/SOURCES.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 20:54:23.000000 pimgu-5.4.2023.4/pimgu.egg-info/dependency_links.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 20:54:23.000000 pimgu-5.4.2023.4/pimgu.egg-info/requires.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 20:54:23.000000 pimgu-5.4.2023.4/pimgu.egg-info/top_level.txt
--rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 20:54:24.068117 pimgu-5.4.2023.4/setup.cfg
--rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 20:54:18.000000 pimgu-5.4.2023.4/setup.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.329893 pimgu-5.4.2023.5/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1067 2023-05-04 17:58:18.000000 pimgu-5.4.2023.5/LICENSE
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:56:37.329638 pimgu-5.4.2023.5/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     3546 2023-05-04 20:41:55.000000 pimgu-5.4.2023.5/README.md
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.327519 pimgu-5.4.2023.5/pimgu/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      404 2023-05-04 20:56:19.000000 pimgu-5.4.2023.5/pimgu/__init__.py
+-rw-r--r--   0 ianwilkey   (501) staff       (20)    10888 2023-05-04 20:56:09.000000 pimgu-5.4.2023.5/pimgu/applet.py
+drwxr-xr-x   0 ianwilkey   (501) staff       (20)        0 2023-05-04 20:56:37.329195 pimgu-5.4.2023.5/pimgu.egg-info/
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     4303 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/PKG-INFO
+-rw-r--r--   0 ianwilkey   (501) staff       (20)      204 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/SOURCES.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        1 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/dependency_links.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       28 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/requires.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)        6 2023-05-04 20:56:37.000000 pimgu-5.4.2023.5/pimgu.egg-info/top_level.txt
+-rw-r--r--   0 ianwilkey   (501) staff       (20)       38 2023-05-04 20:56:37.330002 pimgu-5.4.2023.5/setup.cfg
+-rw-r--r--   0 ianwilkey   (501) staff       (20)     1085 2023-05-04 20:56:24.000000 pimgu-5.4.2023.5/setup.py
```

### Comparing `pimgu-5.4.2023.4/LICENSE` & `pimgu-5.4.2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pimgu-5.4.2023.4/PKG-INFO` & `pimgu-5.4.2023.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.4
+Version: 5.4.2023.5
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pimgu-5.4.2023.4/README.md` & `pimgu-5.4.2023.5/README.md`

 * *Files identical despite different names*

### Comparing `pimgu-5.4.2023.4/pimgu.egg-info/PKG-INFO` & `pimgu-5.4.2023.5/pimgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimgu
-Version: 5.4.2023.4
+Version: 5.4.2023.5
 Summary: A simple framework for creating robust 2D GUI applications using Pygame and ImGui.
 Home-page: https://github.com/iwilkey/pimgu
 Author: Ian Wilkey
 Author-email: iwilkey@mail.bradley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pimgu-5.4.2023.4/setup.py` & `pimgu-5.4.2023.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pimgu',
-    version='v05.04.2023.4',
+    version='v05.04.2023.5',
     description='A simple framework for creating robust 2D GUI applications using Pygame and ImGui.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ian Wilkey',
     author_email='iwilkey@mail.bradley.edu',
     url='https://github.com/iwilkey/pimgu',
     packages=find_packages(),
```

