# Comparing `tmp/aij-webcam-1.0.2.tar.gz` & `tmp/aij-webcam-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.2.tar", last modified: Thu May  4 09:42:19 2023, max compression
+gzip compressed data, was "aij-webcam-1.0.3.tar", last modified: Thu May  4 10:01:31 2023, max compression
```

## Comparing `aij-webcam-1.0.2.tar` & `aij-webcam-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.2/README.md
--rw-rw-rw-   0        0        0     6310 2023-05-04 09:42:04.000000 aij-webcam-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/webcam/
--rw-rw-rw-   0        0        0     9656 2023-05-04 09:41:56.000000 aij-webcam-1.0.2/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.3/README.md
+-rw-rw-rw-   0        0        0     6452 2023-05-04 10:01:16.000000 aij-webcam-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:01:32.000000 aij-webcam-1.0.3/src/webcam/
+-rw-rw-rw-   0        0        0    11221 2023-05-04 09:56:16.000000 aij-webcam-1.0.3/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.2/LICENSE.txt` & `aij-webcam-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.2/PKG-INFO` & `aij-webcam-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.2/README.md` & `aij-webcam-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.2/pyproject.toml` & `aij-webcam-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.2"
+version = "1.0.3"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -102,14 +102,23 @@
 # import cv2
 # import mediapipe as mp
 # import pandas as pd
 # import threading
 # from gtts import gTTS
 # from pygame import mixer
 dependencies = [
+    "requests",
+    "setuptools",
+    "wheel",
+    "pipenv",
+    "pylint",
+    "autopep8",
+    "pyinstaller",
+    "pytest",
+    "pytest-cov",
     "opencv-python",
     "mediapipe",
     "pandas",
     "gtts",
     "pygame"
 ]
```

### Comparing `aij-webcam-1.0.2/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.0.3/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.2/src/webcam/__init__.py` & `aij-webcam-1.0.3/src/webcam/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import time
+
+import requests
 import cv2
 import mediapipe as mp
 import cvzone
 import numpy as np
 import screeninfo
 
 import pandas as pd
@@ -11,26 +13,78 @@
 import pika
 import threading
 
 import openai
 from gtts import gTTS
 from pygame import mixer
 
+# build the required setup to run AIJ
+# make a directory in the user profile named '.aij' 
+# and create a file named 'config.json' in it
+
+def build_setup():
+    """
+    Build the required setup to run AIJ
+    """
+    # get the user profile path
+    user_profile = os.environ['USERPROFILE']
+
+    # create a directory named '.aij' in the user profile
+    os.mkdir(user_profile + '/.aij')
+
+    # create a file named 'config.json' in the directory
+    with open(user_profile + '/.aij/config.json', 'w', encoding="utf-8") as f:
+        f.write('{}')
+
+    # create a folder named 'data' to store audio files
+    os.mkdir(user_profile + '/.aij/data')
+        
+
+# build the required setup to run AIJ
+build_setup()
+
 # Using OpenCV to display the image
 cap = cv2.VideoCapture(0)
 
 cap.set(cv2.CAP_PROP_FRAME_WIDTH, 1280)
 cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 1024)
 cap.set(cv2.CAP_PROP_FPS, 60)
 
 # initialize dataframe
 df_url = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/news.csv"
-df = pd.read_csv(df_url, encoding='utf-8')
-df = df.dropna()
-df = df.reset_index(drop=True)
+
+# download the csv file to userprofile/.aij/news/news.csv
+def download_news_csv():
+    """
+    Download the news.csv file to userprofile/.aij/news/news.csv
+    """
+    # get the user profile path
+    user_profile = os.environ['USERPROFILE']
+
+    # create a directory named 'news' in the user profile
+    os.mkdir(user_profile + '/.aij/news')
+
+    # download the csv file
+    csv_remote_response = requests.get(df_url, allow_redirects=True, stream=True, timeout=10)
+
+    # save the csv file
+    with open(user_profile + '/.aij/news/news.csv', 'wb') as csv_file:
+        csv_file.write(csv_remote_response.content)
+
+
+def map_csv_to_df():
+    """
+    Read the csv file to a dataframe
+    """
+    _df = pd.read_csv(os.environ['USERPROFILE'] + '/.aij/news/news.csv', encoding='utf-8')
+    _df = _df.dropna()
+    _df = _df.reset_index(drop=True)
+    return _df
+
+df = map_csv_to_df()
 
 # text as one line string
 titles = ' '.join(df['title'].tolist())
 
 # add '###' between each title
 titles = ' ... | '.join(df['title'].tolist())
```

