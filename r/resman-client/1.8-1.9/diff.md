# Comparing `tmp/resman-client-1.8.tar.gz` & `tmp/resman-client-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resman-client-1.8.tar", last modified: Thu Oct 13 10:00:49 2022, max compression
+gzip compressed data, was "resman-client-1.9.tar", last modified: Fri Oct 21 14:56:31 2022, max compression
```

## Comparing `resman-client-1.8.tar` & `resman-client-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:00:49.883673 resman-client-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-13 10:00:37.000000 resman-client-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-10-13 10:00:49.883673 resman-client-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-10-13 10:00:37.000000 resman-client-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-13 10:00:37.000000 resman-client-1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:00:49.879672 resman-client-1.8/resman_client/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-13 10:00:37.000000 resman-client-1.8/resman_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13426 2022-10-13 10:00:37.000000 resman-client-1.8/resman_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-10-13 10:00:37.000000 resman-client-1.8/resman_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-13 10:00:37.000000 resman-client-1.8/resman_client/ffmpeg_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:00:49.883673 resman-client-1.8/resman_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-13 10:00:49.000000 resman-client-1.8/resman_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-13 10:00:49.883673 resman-client-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-10-13 10:00:37.000000 resman-client-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:56:31.060979 resman-client-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-21 14:56:23.000000 resman-client-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-10-21 14:56:31.060979 resman-client-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-10-21 14:56:23.000000 resman-client-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-21 14:56:23.000000 resman-client-1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:56:31.056979 resman-client-1.9/resman_client/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-21 14:56:23.000000 resman-client-1.9/resman_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13486 2022-10-21 14:56:23.000000 resman-client-1.9/resman_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-10-21 14:56:23.000000 resman-client-1.9/resman_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-21 14:56:23.000000 resman-client-1.9/resman_client/ffmpeg_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:56:31.060979 resman-client-1.9/resman_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-10-21 14:56:30.000000 resman-client-1.9/resman_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-21 14:56:31.000000 resman-client-1.9/resman_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 14:56:30.000000 resman-client-1.9/resman_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-21 14:56:30.000000 resman-client-1.9/resman_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-21 14:56:30.000000 resman-client-1.9/resman_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-21 14:56:30.000000 resman-client-1.9/resman_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 14:56:31.060979 resman-client-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-10-21 14:56:23.000000 resman-client-1.9/setup.py
```

### Comparing `resman-client-1.8/LICENSE` & `resman-client-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `resman-client-1.8/PKG-INFO` & `resman-client-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resman-client
-Version: 1.8
+Version: 1.9
 Summary: Python client of Resman
 Home-page: https://github.com/TsingJyujing/DataSpider
 Author: Tsing Jyujing
 Author-email: nigel434@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `resman-client-1.8/README.md` & `resman-client-1.9/README.md`

 * *Files identical despite different names*

### Comparing `resman-client-1.8/pyproject.toml` & `resman-client-1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `resman-client-1.8/resman_client/cli.py` & `resman-client-1.9/resman_client/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from resman_client.ffmpeg_util import convert_video_to_h264
 
 log = logging.getLogger("Resman Client")
 
 use_qsv: bool = int(os.environ.get("USE_QSV", "0")) > 0
 force_convert: bool = int(os.environ.get("FORCE_CONVERT", "0")) > 0
 
+VIDEO_SUFFIX_SET = {".mp4", ".avi", ".mkv", ".wmv", ".3gp", ".mdf", ".rm", ".rmvb", ".mpg"}
 
 def pretty_size(size_in_bytes: int, to: str = None, bsize: int = 1024):
     """
     Modified from https://gist.github.com/shawnbutts/3906915
     """
     a = {'k': 1, 'm': 2, 'g': 3, 't': 4, 'p': 5, 'e': 6}
     if to is None:
@@ -121,15 +122,15 @@
         description: str,
         like: bool,
         path: str,
         y: bool
 ):
     path = path or click.prompt("Input path of the file(s)")
 
-    video_files = search_file_in_path(path, {".mp4", ".avi", ".mkv", ".wmv", ".3gp", ".mdf"})
+    video_files = search_file_in_path(path, VIDEO_SUFFIX_SET)
     if len(video_files) <= 0:
         raise Exception(f"Can't find file in path {path}")
     video_files = sorted(video_files)
 
     print(f"Title: {title}\nDescription: {description}\nSet Like: {like}")
     print("Files:")
     sum_size = 0
```

### Comparing `resman-client-1.8/resman_client/client.py` & `resman-client-1.9/resman_client/client.py`

 * *Files identical despite different names*

### Comparing `resman-client-1.8/resman_client/ffmpeg_util.py` & `resman-client-1.9/resman_client/ffmpeg_util.py`

 * *Files identical despite different names*

### Comparing `resman-client-1.8/resman_client.egg-info/PKG-INFO` & `resman-client-1.9/resman_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resman-client
-Version: 1.8
+Version: 1.9
 Summary: Python client of Resman
 Home-page: https://github.com/TsingJyujing/DataSpider
 Author: Tsing Jyujing
 Author-email: nigel434@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `resman-client-1.8/setup.py` & `resman-client-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open("resman_client/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="resman-client",
-    version="1.8",
+    version="1.9",
     author="Tsing Jyujing",
     author_email="nigel434@gmail.com",
     description="Python client of Resman",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TsingJyujing/DataSpider",
     packages=[
```

