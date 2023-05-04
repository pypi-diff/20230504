# Comparing `tmp/tootstagram-0.0.4.tar.gz` & `tmp/tootstagram-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstagram-0.0.4.tar", last modified: Sun Apr 30 18:02:39 2023, max compression
+gzip compressed data, was "tootstagram-0.0.5.tar", last modified: Thu May  4 11:18:07 2023, max compression
```

## Comparing `tootstagram-0.0.4.tar` & `tootstagram-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-29 17:31:28.000000 tootstagram-0.0.4/LICENSE.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 18:02:39.678214 tootstagram-0.0.4/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1513 2023-04-30 17:52:39.000000 tootstagram-0.0.4/README.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      697 2023-04-30 18:02:30.000000 tootstagram-0.0.4/pyproject.toml
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-04-30 18:02:39.678214 tootstagram-0.0.4/setup.cfg
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/tootstagram/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/__init__.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-04-30 17:30:14.000000 tootstagram-0.0.4/tootstagram/database.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2339 2023-04-30 17:42:14.000000 tootstagram-0.0.4/tootstagram/instagram.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2078 2023-04-30 18:01:40.000000 tootstagram-0.0.4/tootstagram/main.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/mastodon.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-29 17:31:28.000000 tootstagram-0.0.4/tootstagram/utils.py
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-04-30 18:02:39.678214 tootstagram-0.0.4/tootstagram.egg-info/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/SOURCES.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/dependency_links.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/entry_points.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/requires.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-04-30 18:02:39.000000 tootstagram-0.0.4/tootstagram.egg-info/top_level.txt
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-04 11:18:07.515234 tootstagram-0.0.5/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-26 13:26:59.000000 tootstagram-0.0.5/LICENSE.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-05-04 11:18:07.515234 tootstagram-0.0.5/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1513 2023-05-01 06:26:22.000000 tootstagram-0.0.5/README.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      710 2023-05-04 11:13:48.000000 tootstagram-0.0.5/pyproject.toml
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-05-04 11:18:07.515234 tootstagram-0.0.5/setup.cfg
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-04 11:18:07.515234 tootstagram-0.0.5/tootstagram/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-27 06:40:20.000000 tootstagram-0.0.5/tootstagram/__init__.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-05-01 06:26:22.000000 tootstagram-0.0.5/tootstagram/database.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2531 2023-05-04 11:11:47.000000 tootstagram-0.0.5/tootstagram/instagram.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2078 2023-05-01 06:26:22.000000 tootstagram-0.0.5/tootstagram/main.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-27 11:25:42.000000 tootstagram-0.0.5/tootstagram/mastodon.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-27 06:40:20.000000 tootstagram-0.0.5/tootstagram/utils.py
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-04 11:18:07.515234 tootstagram-0.0.5/tootstagram.egg-info/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2084 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/entry_points.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       48 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/requires.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-05-04 11:18:07.000000 tootstagram-0.0.5/tootstagram.egg-info/top_level.txt
```

### Comparing `tootstagram-0.0.4/LICENSE.md` & `tootstagram-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.4/PKG-INFO` & `tootstagram-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.4
+Version: 0.0.5
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
-Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
-Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
+Project-URL: Homepage, https://cvs.sonologic.net/gmc/nlgenerator
+Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/nlgenerator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `tootstagram-0.0.4/README.md` & `tootstagram-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.4/pyproject.toml` & `tootstagram-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tootstagram"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Koen Martens", email="kmartens@sonologic.se" },
 ]
 description = "Duplicate posted images from Mastodon to Instagram"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,16 +14,16 @@
     "Environment :: Console",
 ]
 dependencies = [
     "instagrapi",
     "Pillow>=8.1.1",
     "toml",
     "feedparser",
+    "Pillow",
 ]
 
-
 [project.scripts]
 tootstagram = "tootstagram.main:main"
 
 [project.urls]
-"Homepage" = "https://cvs.sonologic.net/gmc/tootstagram"
-"Bug Tracker" = "https://cvs.sonologic.net/gmc/tootstagram/-/issues"
+"Homepage" = "https://cvs.sonologic.net/gmc/nlgenerator"
+"Bug Tracker" = "https://cvs.sonologic.net/gmc/nlgenerator/-/issues"
```

### Comparing `tootstagram-0.0.4/tootstagram/database.py` & `tootstagram-0.0.5/tootstagram/database.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.4/tootstagram/instagram.py` & `tootstagram-0.0.5/tootstagram/instagram.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 https://firstdonoharm.dev/version/3/0/bds-cl-eco-extr-ffd-media-my-soc-sv-tal-xuar.md
 
 """
 import os
 from tempfile import TemporaryDirectory
 
 import instagrapi
+from PIL import Image
 from instagrapi.exceptions import LoginRequired
 
 from tootstagram.utils import download_file
 
 
 class InstagramClient:
     def __init__(self, username: str, password: str, session_file_path: str) -> None:
@@ -54,13 +55,17 @@
         if alt_text:
             extra_data['custom_accessibility_caption'] = alt_text
 
         extension = os.path.splitext(os.path.basename(image_url))[1][1:]
         with TemporaryDirectory() as temp_dir:
             image_path = os.path.join(temp_dir, f'image.{extension}')
             download_file(image_url, image_path)
+            image = Image.open(image_path)
+            if image.format != 'JPEG':
+                image_path = f"{image_path}.jpg"
+                image.save(image_path)
             self._client.photo_upload(
                 image_path,
                 description,
                 extra_data=extra_data
             )
```

### Comparing `tootstagram-0.0.4/tootstagram/main.py` & `tootstagram-0.0.5/tootstagram/main.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.4/tootstagram/mastodon.py` & `tootstagram-0.0.5/tootstagram/mastodon.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.4/tootstagram.egg-info/PKG-INFO` & `tootstagram-0.0.5/tootstagram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.4
+Version: 0.0.5
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
-Project-URL: Homepage, https://cvs.sonologic.net/gmc/tootstagram
-Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/tootstagram/-/issues
+Project-URL: Homepage, https://cvs.sonologic.net/gmc/nlgenerator
+Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/nlgenerator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

