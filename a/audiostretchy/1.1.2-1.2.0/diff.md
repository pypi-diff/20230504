# Comparing `tmp/audiostretchy-1.1.2.tar.gz` & `tmp/audiostretchy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.1.2.tar", last modified: Wed May  3 22:33:50 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.0.tar", last modified: Thu May  4 02:29:01 2023, max compression
```

## Comparing `audiostretchy-1.1.2.tar` & `audiostretchy-1.2.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.375921 audiostretchy-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.379922 audiostretchy-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.375921 audiostretchy-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.387921 audiostretchy-1.1.2/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.383921 audiostretchy-1.1.2/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:49.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 22:33:50.000000 audiostretchy-1.1.2/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:50.391921 audiostretchy-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    98429 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1022110 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio_c.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1030216 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/audio_py.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-03 22:33:34.000000 audiostretchy-1.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.157647 audiostretchy-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.165648 audiostretchy-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-04 02:29:01.185648 audiostretchy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.157647 audiostretchy-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:29:00.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    99491 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/temp.mp3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/conftest.py
```

### Comparing `audiostretchy-1.1.2/.coveragerc` & `audiostretchy-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/.github/workflows/ci.yaml` & `audiostretchy-1.2.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/.gitignore` & `audiostretchy-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/.pre-commit-config.yaml` & `audiostretchy-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/.readthedocs.yml` & `audiostretchy-1.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/LICENSE.txt` & `audiostretchy-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/PKG-INFO` & `audiostretchy-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.1.2
+Version: 1.2.0
 Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.1.2
+Version: 1.2.0
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
-- Supports WAV files
+- Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
+- Optional resampling
 
-Adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
 
 Time-domain harmonic scaling (TDHS) is a method for time-scale
 modification of speech (or other audio signals), allowing the apparent
 rate of speech articulation to be changed without affecting the
 pitch-contour and the time-evolution of the formant structure. TDHS
 differs from other time-scale modification algorithms in that
 time-scaling operations are performed in the time domain (not the
@@ -58,84 +60,89 @@
 Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
 non-standard sampling rates will probably result. Many programs will still
 properly play these files, and audio editing programs will likely import
 them correctly (by resampling), but it is possible that some applications
 will barf on them. They can also be resampled to a standard rate using
 [audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
 
-The Python package does not expose all command-line options of the original library. 
+_Note: The Python package does not expose all command-line options of the original library._
 
 ## Installation
 
-Install AudioStretchy using pip:
+### Simple installation
+
+To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
 
 ```
-python3 -m pip install audiostretchy
+pip install audiostretchy[all]
 ```
 
-or
+### Efficient installation
+
+To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
+
 
 ```
-python3 -m pip install git+https://github.com/twardoch/audiostretchy
+pip install audiostretchy
+```
+
+### Development installation
+
+To install the development version, use:
+
+```
+python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
 ## Usage
 
 ### CLI
 
 ```
-audiostretchy INFILENAME OUTFILENAME <flags>
+audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INFILENAME
-        The path to the input WAV file.
-    OUTFILENAME
-        The path to the output WAV file.
+    INPUT_WAV
+    OUTPUT_WAV
 
 FLAGS
     -r, --ratio=RATIO
-        Type: float
         Default: 1.0
-        The ratio to use for processing. Defaults to 1.0.
-    -s, --silence_ratio=SILENCE_RATIO
-        Type: float
+    -g, --gap_ratio=GAP_RATIO
         Default: 0.0
-        The silence ratio to use for processing if different from ratio
+    -u, --upper_freq=UPPER_FREQ
+        Default: 333
+    -l, --lower_freq=LOWER_FREQ
+        Default: 55
+    -b, --buffer_ms=BUFFER_MS
+        Default: 25
+    -t, --threshold_gap_db=THRESHOLD_GAP_DB
+        Default: -40
+    -d, --dual_force=DUAL_FORCE
+        Default: False
+    -f, --fast_detection=FAST_DETECTION
+        Default: False
+    -n, --normal_detection=NORMAL_DETECTION
+        Default: False
+    -s, --sample_rate=SAMPLE_RATE
+        Default: 0
 ```
 
 ### Python
 
 ```python
-from audiostretchy.stretch import process_audio
-
-input_file = "input.wav"
-output_file = "output.wav"
-stretch_ratio = 1.1
+from audiostretchy.stretch import stretch_audio
 
-process_audio(input_file, output_file, ratio=stretch_ratio)
+stretch_audio("input.wav", "output.wav", ratio=ratio)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-## API
-
-The main function to use in AudioStretchy is `process_audio` in `audiostretchy.stretch`:
-
-```python
-process_audio(
-    infilename: Union[str, Path],
-    outfilename: Union[str, Path],
-    ratio: float = 1.0,
-    silence_ratio: float = 0.0,
-)
-```
+For advanced usage, you can use the `AudioStretch` class (docs to be provided).
 
-- `infilename`: The path to the input audio file (WAV format).
-- `outfilename`: The path to the output audio file (WAV format).
-- `ratio`: The stretching ratio. Must be between 0.25 and 4.0. Defaults to 1.0 (no stretching).
-- `silence_ratio`: The silence ratio to use for processing. Must be between 0.25 and 4.0. Defaults to 0.0 (use the same ratio as `ratio`).
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
+- Written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `audiostretchy-1.1.2/README.md` & `audiostretchy-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.1.2
+Version: 1.2.0
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
-- Supports WAV files
+- Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
+- Optional resampling
 
-Adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
 
 Time-domain harmonic scaling (TDHS) is a method for time-scale
 modification of speech (or other audio signals), allowing the apparent
 rate of speech articulation to be changed without affecting the
 pitch-contour and the time-evolution of the formant structure. TDHS
 differs from other time-scale modification algorithms in that
 time-scaling operations are performed in the time domain (not the
@@ -41,84 +42,89 @@
 Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
 non-standard sampling rates will probably result. Many programs will still
 properly play these files, and audio editing programs will likely import
 them correctly (by resampling), but it is possible that some applications
 will barf on them. They can also be resampled to a standard rate using
 [audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
 
-The Python package does not expose all command-line options of the original library. 
+_Note: The Python package does not expose all command-line options of the original library._
 
 ## Installation
 
-Install AudioStretchy using pip:
+### Simple installation
+
+To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
 
 ```
-python3 -m pip install audiostretchy
+pip install audiostretchy[all]
 ```
 
-or
+### Efficient installation
+
+To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
+
 
 ```
-python3 -m pip install git+https://github.com/twardoch/audiostretchy
+pip install audiostretchy
+```
+
+### Development installation
+
+To install the development version, use:
+
+```
+python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
 ## Usage
 
 ### CLI
 
 ```
-audiostretchy INFILENAME OUTFILENAME <flags>
+audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INFILENAME
-        The path to the input WAV file.
-    OUTFILENAME
-        The path to the output WAV file.
+    INPUT_WAV
+    OUTPUT_WAV
 
 FLAGS
     -r, --ratio=RATIO
-        Type: float
         Default: 1.0
-        The ratio to use for processing. Defaults to 1.0.
-    -s, --silence_ratio=SILENCE_RATIO
-        Type: float
+    -g, --gap_ratio=GAP_RATIO
         Default: 0.0
-        The silence ratio to use for processing if different from ratio
+    -u, --upper_freq=UPPER_FREQ
+        Default: 333
+    -l, --lower_freq=LOWER_FREQ
+        Default: 55
+    -b, --buffer_ms=BUFFER_MS
+        Default: 25
+    -t, --threshold_gap_db=THRESHOLD_GAP_DB
+        Default: -40
+    -d, --dual_force=DUAL_FORCE
+        Default: False
+    -f, --fast_detection=FAST_DETECTION
+        Default: False
+    -n, --normal_detection=NORMAL_DETECTION
+        Default: False
+    -s, --sample_rate=SAMPLE_RATE
+        Default: 0
 ```
 
 ### Python
 
 ```python
-from audiostretchy.stretch import process_audio
-
-input_file = "input.wav"
-output_file = "output.wav"
-stretch_ratio = 1.1
+from audiostretchy.stretch import stretch_audio
 
-process_audio(input_file, output_file, ratio=stretch_ratio)
+stretch_audio("input.wav", "output.wav", ratio=ratio)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-## API
-
-The main function to use in AudioStretchy is `process_audio` in `audiostretchy.stretch`:
-
-```python
-process_audio(
-    infilename: Union[str, Path],
-    outfilename: Union[str, Path],
-    ratio: float = 1.0,
-    silence_ratio: float = 0.0,
-)
-```
+For advanced usage, you can use the `AudioStretch` class (docs to be provided).
 
-- `infilename`: The path to the input audio file (WAV format).
-- `outfilename`: The path to the output audio file (WAV format).
-- `ratio`: The stretching ratio. Must be between 0.25 and 4.0. Defaults to 1.0 (no stretching).
-- `silence_ratio`: The silence ratio to use for processing. Must be between 0.25 and 4.0. Defaults to 0.0 (use the same ratio as `ratio`).
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
+- Written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `audiostretchy-1.1.2/docs/Makefile` & `audiostretchy-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/docs/conf.py` & `audiostretchy-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/docs/index.md` & `audiostretchy-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/setup.cfg` & `audiostretchy-1.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 exclude = 
 	tests
 
 [options.package_data]
 * = *.dll, *.so, *.dylib
 
 [options.extras_require]
+all = 
+	pydub>=0.25.1; sys_platform == 'darwin'
+	pymp3>=0.1.9; sys_platform == 'win32' or sys_platform == 'linux'
+	soxr>=0.3.5
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts =
```

### Comparing `audiostretchy-1.1.2/setup.py` & `audiostretchy-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy/__init__.py` & `audiostretchy-1.2.0/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.0/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.0/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.0/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.0/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.1.2/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.0/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.1.2
+Version: 1.2.0
 Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.1.2
+Version: 1.2.0
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
-- Supports WAV files
+- Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
+- Optional resampling
 
-Adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
 
 Time-domain harmonic scaling (TDHS) is a method for time-scale
 modification of speech (or other audio signals), allowing the apparent
 rate of speech articulation to be changed without affecting the
 pitch-contour and the time-evolution of the formant structure. TDHS
 differs from other time-scale modification algorithms in that
 time-scaling operations are performed in the time domain (not the
@@ -58,84 +60,89 @@
 Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
 non-standard sampling rates will probably result. Many programs will still
 properly play these files, and audio editing programs will likely import
 them correctly (by resampling), but it is possible that some applications
 will barf on them. They can also be resampled to a standard rate using
 [audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
 
-The Python package does not expose all command-line options of the original library. 
+_Note: The Python package does not expose all command-line options of the original library._
 
 ## Installation
 
-Install AudioStretchy using pip:
+### Simple installation
+
+To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
 
 ```
-python3 -m pip install audiostretchy
+pip install audiostretchy[all]
 ```
 
-or
+### Efficient installation
+
+To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
+
 
 ```
-python3 -m pip install git+https://github.com/twardoch/audiostretchy
+pip install audiostretchy
+```
+
+### Development installation
+
+To install the development version, use:
+
+```
+python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
 ## Usage
 
 ### CLI
 
 ```
-audiostretchy INFILENAME OUTFILENAME <flags>
+audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INFILENAME
-        The path to the input WAV file.
-    OUTFILENAME
-        The path to the output WAV file.
+    INPUT_WAV
+    OUTPUT_WAV
 
 FLAGS
     -r, --ratio=RATIO
-        Type: float
         Default: 1.0
-        The ratio to use for processing. Defaults to 1.0.
-    -s, --silence_ratio=SILENCE_RATIO
-        Type: float
+    -g, --gap_ratio=GAP_RATIO
         Default: 0.0
-        The silence ratio to use for processing if different from ratio
+    -u, --upper_freq=UPPER_FREQ
+        Default: 333
+    -l, --lower_freq=LOWER_FREQ
+        Default: 55
+    -b, --buffer_ms=BUFFER_MS
+        Default: 25
+    -t, --threshold_gap_db=THRESHOLD_GAP_DB
+        Default: -40
+    -d, --dual_force=DUAL_FORCE
+        Default: False
+    -f, --fast_detection=FAST_DETECTION
+        Default: False
+    -n, --normal_detection=NORMAL_DETECTION
+        Default: False
+    -s, --sample_rate=SAMPLE_RATE
+        Default: 0
 ```
 
 ### Python
 
 ```python
-from audiostretchy.stretch import process_audio
-
-input_file = "input.wav"
-output_file = "output.wav"
-stretch_ratio = 1.1
+from audiostretchy.stretch import stretch_audio
 
-process_audio(input_file, output_file, ratio=stretch_ratio)
+stretch_audio("input.wav", "output.wav", ratio=ratio)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-## API
-
-The main function to use in AudioStretchy is `process_audio` in `audiostretchy.stretch`:
-
-```python
-process_audio(
-    infilename: Union[str, Path],
-    outfilename: Union[str, Path],
-    ratio: float = 1.0,
-    silence_ratio: float = 0.0,
-)
-```
+For advanced usage, you can use the `AudioStretch` class (docs to be provided).
 
-- `infilename`: The path to the input audio file (WAV format).
-- `outfilename`: The path to the output audio file (WAV format).
-- `ratio`: The stretching ratio. Must be between 0.25 and 4.0. Defaults to 1.0 (no stretching).
-- `silence_ratio`: The silence ratio to use for processing. Must be between 0.25 and 4.0. Defaults to 0.0 (use the same ratio as `ratio`).
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
+- Written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `audiostretchy-1.1.2/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.0/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 .readthedocs.yml
 AUTHORS.md
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+temp.mp3
 .github/workflows/ci.yaml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
@@ -31,12 +32,12 @@
 src/audiostretchy.egg-info/not-zip-safe
 src/audiostretchy.egg-info/requires.txt
 src/audiostretchy.egg-info/top_level.txt
 src/audiostretchy/interface/tdhs.py
 src/audiostretchy/interface/linux/_stretch.so
 src/audiostretchy/interface/mac/_stretch.dylib
 src/audiostretchy/interface/win/_stretch.dll
+tests/audio-1.2.mp3
+tests/audio-1.2.wav
 tests/audio.mp3
 tests/audio.wav
-tests/audio_c.wav
-tests/audio_py.wav
 tests/conftest.py
```

### Comparing `audiostretchy-1.1.2/tests/audio.wav` & `audiostretchy-1.2.0/tests/audio.wav`

 * *Files identical despite different names*

