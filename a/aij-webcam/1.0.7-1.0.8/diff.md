# Comparing `tmp/aij-webcam-1.0.7.tar.gz` & `tmp/aij-webcam-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.7.tar", last modified: Thu May  4 10:22:10 2023, max compression
+gzip compressed data, was "aij-webcam-1.0.8.tar", last modified: Thu May  4 10:27:27 2023, max compression
```

## Comparing `aij-webcam-1.0.7.tar` & `aij-webcam-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.7/README.md
--rw-rw-rw-   0        0        0     6452 2023-05-04 10:22:02.000000 aij-webcam-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/webcam/
--rw-rw-rw-   0        0        0    12135 2023-05-04 10:21:52.000000 aij-webcam-1.0.7/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.8/README.md
+-rw-rw-rw-   0        0        0     6452 2023-05-04 10:27:18.000000 aij-webcam-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/webcam/
+-rw-rw-rw-   0        0        0    11775 2023-05-04 10:26:14.000000 aij-webcam-1.0.8/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.7/LICENSE.txt` & `aij-webcam-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.7/PKG-INFO` & `aij-webcam-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.7
+Version: 1.0.8
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.7/README.md` & `aij-webcam-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.7/pyproject.toml` & `aij-webcam-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.7"
+version = "1.0.8"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.0.7/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.0.8/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.7
+Version: 1.0.8
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.7/src/webcam/__init__.py` & `aij-webcam-1.0.8/src/webcam/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import cv2
 import mediapipe as mp
 import cvzone
 import numpy as np
 import screeninfo
 
 import pandas as pd
+import json
+from pandas import DataFrame
 
 import pika
 import threading
 
 import openai
 from gtts import gTTS
 from pygame import mixer
@@ -55,15 +57,15 @@
 cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 1024)
 cap.set(cv2.CAP_PROP_FPS, 60)
 
 # initialize dataframe
 csv_url = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/news.csv"
 
 # download the csv file to userprofile/.aij/news/news.csv
-def download_news_csv():
+def download_news_csv() -> DataFrame:
     """
     Download the news.csv file to userprofile/.aij/news/news.csv
     """
     # get the user profile path
     user_profile = os.environ['USERPROFILE']
     _sep = os.path.sep
     csv_home = user_profile + _sep + '.aij' + _sep + 'news' + _sep + 'news.csv'
@@ -73,34 +75,22 @@
         os.mkdir(user_profile + _sep + '.aij' + _sep + 'news')
 
     # download the csv file
     csv_remote_response = requests.get(csv_url, allow_redirects=True, stream=True, timeout=10)
 
     # save the csv file if the response is ok and the file does not exist
     if csv_remote_response.status_code == 200 and not os.path.exists(csv_home):
-        with open(csv_home, 'wb') as csv_file:
-            csv_file.write(csv_remote_response.content)
+        # write the csv file using pandas
+        pd.read_csv(csv_url).to_csv(csv_home, index=False, encoding='utf-8')
 
+    # return the dataframe
+    return pd.read_csv(csv_home)
 
-def map_csv_to_df():
-    """
-    Read the csv file to a dataframe
-    """
-
-    user_profile = os.environ['USERPROFILE']
-    _sep = os.path.sep
-    if not os.path.exists(user_profile + _sep + '.aij' + _sep + 'news'):
-        os.mkdir(user_profile + _sep + '.aij' + _sep + 'news')
-    csv_home = user_profile + _sep + '.aij' + _sep + 'news' + _sep + 'news.csv'
-    _df = pd.read_csv(csv_home, encoding='utf-8')
-    _df = _df.dropna()
-    _df = _df.reset_index(drop=True)
-    return _df
 
-df = map_csv_to_df()
+df = download_news_csv()
 
 # text as one line string
 titles = ' '.join(df['title'].tolist())
 
 # add '###' between each title
 titles = ' ... | '.join(df['title'].tolist())
```

