# Comparing `tmp/gpt4all-0.0.1.tar.gz` & `tmp/gpt4all-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-0.0.1.tar", last modified: Thu May  4 13:08:28 2023, max compression
+gzip compressed data, was "gpt4all-0.1.0.tar", last modified: Thu May  4 16:16:37 2023, max compression
```

## Comparing `gpt4all-0.0.1.tar` & `gpt4all-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,21 @@
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 13:08:28.006927 gpt4all-0.0.1/
--rw-r--r--   0 richardguo   (501) staff       (20)      470 2023-05-04 13:08:28.006804 gpt4all-0.0.1/PKG-INFO
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 13:08:28.006669 gpt4all-0.0.1/gpt4all.egg-info/
--rw-r--r--   0 richardguo   (501) staff       (20)      470 2023-05-04 13:08:28.000000 gpt4all-0.0.1/gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      138 2023-05-04 13:08:28.000000 gpt4all-0.0.1/gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 13:08:28.000000 gpt4all-0.0.1/gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 13:08:28.000000 gpt4all-0.0.1/gpt4all.egg-info/top_level.txt
--rw-r--r--   0 richardguo   (501) staff       (20)      566 2023-05-04 13:07:44.000000 gpt4all-0.0.1/pyproject.toml
--rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-04 13:08:28.006965 gpt4all-0.0.1/setup.cfg
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.578034 gpt4all-0.1.0/
+-rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.0/LICENSE.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:16:37.577922 gpt4all-0.1.0/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.0/README.md
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.575790 gpt4all-0.1.0/gpt4all/
+-rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.0/gpt4all/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.0/gpt4all/gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)   285208 2023-05-04 16:13:44.000000 gpt4all-0.1.0/gpt4all/pyllmodel.c
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.577257 gpt4all-0.1.0/gpt4all.egg-info/
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      322 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/requires.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-04 16:16:37.000000 gpt4all-0.1.0/gpt4all.egg-info/top_level.txt
+-rw-------   0 richardguo   (501) staff       (20)      534 2023-05-04 16:15:51.000000 gpt4all-0.1.0/pyproject.toml
+-rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-04 16:16:37.578071 gpt4all-0.1.0/setup.cfg
+-rw-r--r--   0 richardguo   (501) staff       (20)      940 2023-05-04 16:12:20.000000 gpt4all-0.1.0/setup.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 16:16:37.577654 gpt4all-0.1.0/tests/
+-rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.0/tests/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.0/tests/test_gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.0/tests/test_pyllmodel.py
```

### Comparing `gpt4all-0.0.1/pyproject.toml` & `gpt4all-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=58.1.0", "wheel", "Cython==0.29.34"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt4all"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Richard Guo", email="richard@nomic.ai" },
 ]
-description = "A small example package"
+description = "Python bindings for GPT4All"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://pypi.org/project/gpt4all/"
```

