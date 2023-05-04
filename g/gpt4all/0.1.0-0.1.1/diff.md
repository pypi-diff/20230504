# Comparing `tmp/gpt4all-0.1.0.tar.gz` & `tmp/gpt4all-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-0.1.0.tar", last modified: Thu May  4 16:16:37 2023, max compression
+gzip compressed data, was "gpt4all-0.1.1.tar", last modified: Thu May  4 16:48:06 2023, max compression
```

## Comparing `gpt4all-0.1.0.tar` & `gpt4all-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.578034 gpt4all-0.1.0/
--rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.0/LICENSE.txt
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:16:37.577922 gpt4all-0.1.0/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.0/README.md
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.575790 gpt4all-0.1.0/gpt4all/
--rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.0/gpt4all/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.0/gpt4all/gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)   285208 2023-05-04 16:13:44.000000 gpt4all-0.1.0/gpt4all/pyllmodel.c
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.577257 gpt4all-0.1.0/gpt4all.egg-info/
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      322 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/requires.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/top_level.txt
--rw-------   0 richardguo   (501) staff       (20)      534 2023-05-04 16:15:51.000000 gpt4all-0.1.0/pyproject.toml
--rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-04 16:16:37.578071 gpt4all-0.1.0/setup.cfg
--rw-r--r--   0 richardguo   (501) staff       (20)      940 2023-05-04 16:12:20.000000 gpt4all-0.1.0/setup.py
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.577654 gpt4all-0.1.0/tests/
--rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.0/tests/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.0/tests/test_gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.0/tests/test_pyllmodel.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:48:06.089160 gpt4all-0.1.1/
+-rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.1/LICENSE.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       61 2023-05-04 16:46:09.000000 gpt4all-0.1.1/MANIFEST.in
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:48:06.089035 gpt4all-0.1.1/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.1/README.md
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:48:06.086818 gpt4all-0.1.1/gpt4all/
+-rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.1/gpt4all/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.1/gpt4all/gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)   285208 2023-05-04 16:13:44.000000 gpt4all-0.1.1/gpt4all/pyllmodel.c
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:48:06.088298 gpt4all-0.1.1/gpt4all.egg-info/
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:48:06.000000 gpt4all-0.1.1/gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      476 2023-05-04 16:48:06.000000 gpt4all-0.1.1/gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 16:48:06.000000 gpt4all-0.1.1/gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-04 16:48:06.000000 gpt4all-0.1.1/gpt4all.egg-info/requires.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-04 16:48:06.000000 gpt4all-0.1.1/gpt4all.egg-info/top_level.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-04 16:48:06.089200 gpt4all-0.1.1/setup.cfg
+-rw-r--r--   0 richardguo   (501) staff       (20)      941 2023-05-04 16:47:00.000000 gpt4all-0.1.1/setup.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:48:06.088761 gpt4all-0.1.1/tests/
+-rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.1/tests/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.1/tests/test_gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.1/tests/test_pyllmodel.py
```

### Comparing `gpt4all-0.1.0/LICENSE.txt` & `gpt4all-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.0/README.md` & `gpt4all-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.0/gpt4all/gpt4all.py` & `gpt4all-0.1.1/gpt4all/gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.0/gpt4all/pyllmodel.c` & `gpt4all-0.1.1/gpt4all/pyllmodel.c`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.0/setup.py` & `gpt4all-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     extra_link_args=['-Wl,-rpath,../../llmodel/build'],
 )
 
 ext_modules = cythonize([llmodel_extension])
 
 setup(
     name="gpt4all",
-    version="0.1.0",
+    version="0.1.1",
     description="Python bindings for GPT4All",
     author="Richard Guo",
     author_email="richard@nomic.ai",
     url="https://pypi.org/project/gpt4all/",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     packages=find_packages(),
     install_requires=[
         "Cython==0.29.34",
         "pytest==7.3.1"],
-    ext_modules=ext_modules
+    ext_modules=ext_modules,
 )
```

### Comparing `gpt4all-0.1.0/tests/test_gpt4all.py` & `gpt4all-0.1.1/tests/test_gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.0/tests/test_pyllmodel.py` & `gpt4all-0.1.1/tests/test_pyllmodel.py`

 * *Files identical despite different names*

