# Comparing `tmp/audiostretchy-1.0.8.tar.gz` & `tmp/audiostretchy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.0.8.tar", last modified: Mon May  1 00:47:24 2023, max compression
+gzip compressed data, was "audiostretchy-1.1.2.tar", last modified: Wed May  3 22:33:50 2023, max compression
```

## Comparing `audiostretchy-1.0.8.tar` & `audiostretchy-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.960883 audiostretchy-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.952883 audiostretchy-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.github/workflows/compile-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.github/workflows/compile-mac.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.github/workflows/compile-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 00:47:24.960883 audiostretchy-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-01 00:47:24.960883 audiostretchy-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.952883 audiostretchy-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/interface/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.956883 audiostretchy-1.0.8/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 00:47:24.000000 audiostretchy-1.0.8/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:47:24.960883 audiostretchy-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 00:47:09.000000 audiostretchy-1.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.375921 audiostretchy-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.379922 audiostretchy-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.375921 audiostretchy-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:49.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    98429 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1022110 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio_c.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1030216 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio_py.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/conftest.py
```

### Comparing `audiostretchy-1.0.8/.coveragerc` & `audiostretchy-1.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/.gitignore` & `audiostretchy-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/.pre-commit-config.yaml` & `audiostretchy-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/.readthedocs.yml` & `audiostretchy-1.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/LICENSE.txt` & `audiostretchy-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/PKG-INFO` & `audiostretchy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.0.8
+Version: 1.1.2
 Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -15,15 +15,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.8
+Version: 1.1.2
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.8/README.md` & `audiostretchy-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.8
+Version: 1.1.2
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.8/docs/Makefile` & `audiostretchy-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/docs/conf.py` & `audiostretchy-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/docs/index.md` & `audiostretchy-1.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/setup.cfg` & `audiostretchy-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/setup.py` & `audiostretchy-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/src/audiostretchy/__init__.py` & `audiostretchy-1.1.2/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.1.2/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.1.2/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.8/src/audiostretchy/interface/stretch.py` & `audiostretchy-1.1.2/src/audiostretchy/interface/tdhs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     lib_path = Path(__file__).parent / 'linux' / '_stretch.so'
 else:
     raise NotImplementedError("This platform is not supported.")
 
 stretch_lib = ctypes.cdll.LoadLibrary(str(lib_path))
 
 
-class Stretch:
+class TDHSAudioStretch:
     """
     The Stretch class is a Python binding for the _stretch library, providing an interface
     to time-stretch audio signals without changing their pitch.
     """
-
+    STRETCH_FAST_FLAG = 0x1
+    STRETCH_DUAL_FLAG = 0x2
+    
     def __init__(self, shortest_period: int, longest_period: int, num_chans: int, flags: int) -> None:
         """
         Initialize the stretching context with the given parameters.
 
         :param shortest_period: The shortest period, affecting frequency handling.
         :param longest_period: The longest period, affecting frequency handling.
         :param num_chans: The number of audio channels.
@@ -97,15 +99,15 @@
 
         :param max_num_samples: The maximum number of samples.
         :param max_ratio: The maximum stretching ratio.
         :return: The number of samples to reserve in the output array.
         """
         return self.stretch_output_capacity(self.handle, max_num_samples, max_ratio)
 
-    def samples(self, samples: np.ndarray, num_samples: int, output: np.ndarray, ratio: float) -> int:
+    def process_samples(self, samples: np.ndarray, num_samples: int, output: np.ndarray, ratio: float) -> int:
         """
         Process the samples with a specified ratio.
 
         :param samples: The input audio samples.
         :param num_samples: The number of samples.
         :param output: The output audio samples.
         :param ratio: The stretching ratio.
```

### Comparing `audiostretchy-1.0.8/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.1.2/src/audiostretchy/interface/win/_stretch.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800014d4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  1 00:37:04 2023
+Time/Date		Wed May  3 21:36:53 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000da00
 SizeOfInitializedData	000000000000ce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000014d4
@@ -30758,17 +30758,17 @@
    18001691d:	add    %al,(%rax)
    18001691f:	add    %dh,-0xe(%rax)
    180016922:	add    %al,0x1(%rax)
    180016928:	js     0x18001691c
    18001692a:	add    %al,0x1(%rax)
    180016930:	add    %al,(%rax)
    180016932:	add    %al,(%rax)
-   180016934:	mov    $0x9,%al
-   180016936:	rex.WRXB
-   180016937:	add    %al,%fs:(%rax)
+   180016934:	cmc
+   180016935:	rcll   %cl,0x64(%rdx)
+   180016938:	add    %al,(%rax)
    18001693a:	add    %al,(%rax)
    18001693c:	or     $0xb8000000,%eax
    180016941:	add    (%rax),%al
    180016943:	add    %ch,%al
    180016945:	insb   (%dx),%es:(%rdi)
    180016946:	add    %eax,(%rax)
    180016948:	call   0x180016aa7
```

### Comparing `audiostretchy-1.0.8/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.1.2/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.0.8
+Version: 1.1.2
 Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -15,15 +15,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.8
+Version: 1.1.2
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.8/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.1.2/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 .readthedocs.yml
 AUTHORS.md
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-.github/workflows/compile-linux.yaml
-.github/workflows/compile-mac.yaml
-.github/workflows/compile-windows.yaml
-.github/workflows/publish.yaml
+.github/workflows/ci.yaml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/license.md
@@ -30,12 +27,16 @@
 src/audiostretchy.egg-info/PKG-INFO
 src/audiostretchy.egg-info/SOURCES.txt
 src/audiostretchy.egg-info/dependency_links.txt
 src/audiostretchy.egg-info/entry_points.txt
 src/audiostretchy.egg-info/not-zip-safe
 src/audiostretchy.egg-info/requires.txt
 src/audiostretchy.egg-info/top_level.txt
-src/audiostretchy/interface/stretch.py
+src/audiostretchy/interface/tdhs.py
 src/audiostretchy/interface/linux/_stretch.so
 src/audiostretchy/interface/mac/_stretch.dylib
 src/audiostretchy/interface/win/_stretch.dll
+tests/audio.mp3
+tests/audio.wav
+tests/audio_c.wav
+tests/audio_py.wav
 tests/conftest.py
```

