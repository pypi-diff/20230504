# Comparing `tmp/split_file_reader-0.1.3.tar.gz` & `tmp/split_file_reader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Xavier\PycharmProjects\SplitFileReaderProject\dist\.tmp-k06dp6dk\split_file_reader-0.1.3.tar", last modified: Thu May  4 01:03:52 2023, max compression
+gzip compressed data, was "C:\Users\Xavier\PycharmProjects\SplitFileReaderProject\dist\.tmp-i8bg66f8\split_file_reader-0.1.4.tar", last modified: Thu May  4 01:33:48 2023, max compression
```

## Comparing `split_file_reader-0.1.3.tar` & `split_file_reader-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/
--rw-rw-rw-   0        0        0    35769 2022-01-16 22:31:16.000000 split_file_reader-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      973 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9472 2023-05-01 03:05:10.000000 split_file_reader-0.1.3/README.md
--rw-rw-rw-   0        0        0     1841 2023-04-30 03:19:06.000000 split_file_reader-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/
--rw-rw-rw-   0        0        0     1095 2023-04-29 00:29:50.000000 split_file_reader-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0       88 2022-06-26 03:47:31.000000 split_file_reader-0.1.3/src/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/http_file_reader/
--rw-rw-rw-   0        0        0       46 2022-06-26 03:47:31.000000 split_file_reader-0.1.3/src/http_file_reader/__init__.py
--rw-rw-rw-   0        0        0    10366 2023-04-29 02:53:13.000000 split_file_reader-0.1.3/src/http_file_reader/http_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader/
--rw-rw-rw-   0        0        0       48 2023-04-28 21:33:13.000000 split_file_reader-0.1.3/src/split_file_reader/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-04-29 00:54:53.000000 split_file_reader-0.1.3/src/split_file_reader/__main__.py
--rw-rw-rw-   0        0        0    30939 2023-04-29 02:51:32.000000 split_file_reader-0.1.3/src/split_file_reader/split_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/
--rw-rw-rw-   0        0        0      973 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_writer/
--rw-rw-rw-   0        0        0       99 2023-04-29 00:29:50.000000 split_file_reader-0.1.3/src/split_file_writer/__init__.py
--rw-rw-rw-   0        0        0    11399 2023-04-29 02:34:33.000000 split_file_reader-0.1.3/src/split_file_writer/split_file_writer.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/
+-rw-rw-rw-   0        0        0    35769 2022-01-16 22:31:16.000000 split_file_reader-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    10490 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9472 2023-05-01 03:05:10.000000 split_file_reader-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1863 2023-05-04 01:32:57.000000 split_file_reader-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/
+-rw-rw-rw-   0        0        0     1095 2023-04-29 00:29:50.000000 split_file_reader-0.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0       88 2022-06-26 03:47:31.000000 split_file_reader-0.1.4/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/http_file_reader/
+-rw-rw-rw-   0        0        0       46 2022-06-26 03:47:31.000000 split_file_reader-0.1.4/src/http_file_reader/__init__.py
+-rw-rw-rw-   0        0        0    10366 2023-04-29 02:53:13.000000 split_file_reader-0.1.4/src/http_file_reader/http_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader/
+-rw-rw-rw-   0        0        0       48 2023-04-28 21:33:13.000000 split_file_reader-0.1.4/src/split_file_reader/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-04-29 00:54:53.000000 split_file_reader-0.1.4/src/split_file_reader/__main__.py
+-rw-rw-rw-   0        0        0    30939 2023-04-29 02:51:32.000000 split_file_reader-0.1.4/src/split_file_reader/split_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/
+-rw-rw-rw-   0        0        0    10490 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_reader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 01:33:48.000000 split_file_reader-0.1.4/src/split_file_writer/
+-rw-rw-rw-   0        0        0       99 2023-04-29 00:29:50.000000 split_file_reader-0.1.4/src/split_file_writer/__init__.py
+-rw-rw-rw-   0        0        0    11399 2023-04-29 02:34:33.000000 split_file_reader-0.1.4/src/split_file_writer/split_file_writer.py
```

### Comparing `split_file_reader-0.1.3/LICENSE` & `split_file_reader-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/README.md` & `split_file_reader-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/pyproject.toml` & `split_file_reader-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     'Programming Language :: Python :: Implementation :: CPython',
     'Programming Language :: Python :: Implementation :: PyPy',
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Topic :: System :: Filesystems",
 ]
 description="A package to read parted files on disk."
+readme = "README.md"
 name="split_file_reader"
-version="0.1.3"
+version="0.1.4"
 requires-python = ">=3.5"
 
 [project.scripts]
 split_file_reader = "split_file_reader.__main__:main"
 
 [build-system]
 requires = ["pip>=22", "setuptools", "wheel"]
```

### Comparing `split_file_reader-0.1.3/src/__init__.py` & `split_file_reader-0.1.4/src/__init__.py`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/src/http_file_reader/http_file_reader.py` & `split_file_reader-0.1.4/src/http_file_reader/http_file_reader.py`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/src/split_file_reader/__main__.py` & `split_file_reader-0.1.4/src/split_file_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/src/split_file_reader/split_file_reader.py` & `split_file_reader-0.1.4/src/split_file_reader/split_file_reader.py`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/src/split_file_reader.egg-info/SOURCES.txt` & `split_file_reader-0.1.4/src/split_file_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.3/src/split_file_writer/split_file_writer.py` & `split_file_reader-0.1.4/src/split_file_writer/split_file_writer.py`

 * *Files identical despite different names*

