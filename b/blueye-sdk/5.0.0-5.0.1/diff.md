# Comparing `tmp/blueye.sdk-5.0.0.tar.gz` & `tmp/blueye.sdk-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueye.sdk-5.0.0.tar", last modified: Thu Feb 27 08:43:49 2020, max compression
+gzip compressed data, was "blueye.sdk-5.0.1.tar", last modified: Thu Feb 27 12:12:01 2020, max compression
```

## Comparing `blueye.sdk-5.0.0.tar` & `blueye.sdk-5.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     7652 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/LICENSE
--rw-r--r--   0        0        0     2636 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/README.md
--rw-r--r--   0        0        0      128 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/blueye/__init__.py
--rw-r--r--   0        0        0      111 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/blueye/sdk/__init__.py
--rw-r--r--   0        0        0     7971 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/blueye/sdk/camera.py
--rw-r--r--   0        0        0      210 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/blueye/sdk/constants.py
--rw-r--r--   0        0        0     5233 2020-02-27 08:41:45.281460 blueye.sdk-5.0.0/blueye/sdk/logs.py
--rw-r--r--   0        0        0     7897 2020-02-27 08:41:45.285459 blueye.sdk-5.0.0/blueye/sdk/motion.py
--rwxr-xr-x   0        0        0    10120 2020-02-27 08:41:45.285459 blueye.sdk-5.0.0/blueye/sdk/pioneer.py
--rw-r--r--   0        0        0      532 2020-02-27 08:41:45.285459 blueye.sdk-5.0.0/blueye/sdk/utils.py
--rw-r--r--   0        0        0    15258 2020-02-27 08:43:48.767517 blueye.sdk-5.0.0/blueye.sdk_docs/404.html
--rw-r--r--   0        0        0     7652 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/LICENSE
--rw-r--r--   0        0        0    21070 2020-02-27 08:43:48.791517 blueye.sdk-5.0.0/blueye.sdk_docs/README.html
--rw-r--r--   0        0        0    30721 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/font-awesome.css
--rw-r--r--   0        0        0      873 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/material-icons.css
--rw-r--r--   0        0        0   165548 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.ttf
--rw-r--r--   0        0        0    98024 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff
--rw-r--r--   0        0        0    77160 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff2
--rw-r--r--   0        0        0   128180 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.ttf
--rw-r--r--   0        0        0    57620 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff
--rw-r--r--   0        0        0    44300 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff2
--rw-r--r--   0        0        0      521 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/favicon.png
--rw-r--r--   0        0        0     1230 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/bitbucket.1b09e088.svg
--rw-r--r--   0        0        0      993 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/github.f0b8504a.svg
--rw-r--r--   0        0        0     1138 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/gitlab.6dd19c00.svg
--rw-r--r--   0        0        0    79589 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/application.c33a9706.js
--rw-r--r--   0        0        0    17538 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ar.js
--rw-r--r--   0        0        0     4610 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.da.js
--rw-r--r--   0        0        0     6087 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.de.js
--rw-r--r--   0        0        0     6167 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.du.js
--rw-r--r--   0        0        0    11424 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.es.js
--rw-r--r--   0        0        0     9222 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.fi.js
--rw-r--r--   0        0        0    10593 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.fr.js
--rw-r--r--   0        0        0     9379 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.hu.js
--rw-r--r--   0        0        0    11091 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.it.js
--rw-r--r--   0        0        0     2629 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ja.js
--rw-r--r--   0        0        0       36 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.jp.js
--rw-r--r--   0        0        0      817 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.multi.js
--rw-r--r--   0        0        0     5985 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.nl.js
--rw-r--r--   0        0        0     4694 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.no.js
--rw-r--r--   0        0        0    10083 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.pt.js
--rw-r--r--   0        0        0    10851 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ro.js
--rw-r--r--   0        0        0    10160 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ru.js
--rw-r--r--   0        0        0     3808 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.stemmer.support.js
--rw-r--r--   0        0        0     4481 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.sv.js
--rw-r--r--   0        0        0     1381 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.th.js
--rw-r--r--   0        0        0    14113 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.tr.js
--rw-r--r--   0        0        0     1142 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.vi.js
--rw-r--r--   0        0        0    18278 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   555307 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0     7296 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/modernizr.86422ebf.js
--rw-r--r--   0        0        0    38773 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/stylesheets/application-palette.a8b3c06d.css
--rw-r--r--   0        0        0    76332 2020-02-27 08:43:48.619517 blueye.sdk-5.0.0/blueye.sdk_docs/assets/stylesheets/application.adb8469c.css
--rw-r--r--   0        0        0    19605 2020-02-27 08:43:48.799517 blueye.sdk-5.0.0/blueye.sdk_docs/contributing.html
--rw-r--r--   0        0        0    25283 2020-02-27 08:43:48.811517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/configuration.html
--rw-r--r--   0        0        0  1039497 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/http-api.html
--rw-r--r--   0        0        0    24327 2020-02-27 08:43:48.839517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/listing-and-downloading.html
--rw-r--r--   0        0        0    25567 2020-02-27 08:43:48.851517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/log-file-format.html
--rw-r--r--   0        0        0    22254 2020-02-27 08:43:48.863517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/plotting.html
--rw-r--r--   0        0        0     1607 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/media/blueye_b.svg
--rw-r--r--   0        0        0    35460 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/media/depth_plot.svg
--rw-r--r--   0        0        0    18795 2020-02-27 08:43:48.871517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/movement/from-the-CLI.html
--rw-r--r--   0        0        0    30730 2020-02-27 08:43:48.895517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/movement/with-a-gamepad.html
--rw-r--r--   0        0        0    32374 2020-02-27 08:43:48.827517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/quick_start.html
--rw-r--r--   0        0        0    23508 2020-02-27 08:43:48.907517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/video/downloading.html
--rw-r--r--   0        0        0    22904 2020-02-27 08:43:48.915517 blueye.sdk-5.0.0/blueye.sdk_docs/docs/video/gstreamer-for-video-streaming.html
--rw-r--r--   0        0        0    23406 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/http-api.yml
--rw-r--r--   0        0        0    82322 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/poetry.lock
--rw-r--r--   0        0        0     3387 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/pyproject.toml
--rw-r--r--   0        0        0      215 2020-02-27 08:43:48.615517 blueye.sdk-5.0.0/blueye.sdk_docs/pytest.ini
--rw-r--r--   0        0        0    45163 2020-02-27 08:43:48.939517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/camera.html
--rw-r--r--   0        0        0    20855 2020-02-27 08:43:48.947517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/constants.html
--rw-r--r--   0        0        0    19018 2020-02-27 08:43:48.923517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/index.html
--rw-r--r--   0        0        0    36628 2020-02-27 08:43:48.959517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/logs.html
--rw-r--r--   0        0        0    43676 2020-02-27 08:43:48.971517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/motion.html
--rw-r--r--   0        0        0    51876 2020-02-27 08:43:48.987517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/pioneer.html
--rw-r--r--   0        0        0    20016 2020-02-27 08:43:48.995517 blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/utils.html
--rw-r--r--   0        0        0   198948 2020-02-27 08:43:48.995517 blueye.sdk-5.0.0/blueye.sdk_docs/search/search_index.json
--rw-r--r--   0        0        0     2053 2020-02-27 08:43:48.627517 blueye.sdk-5.0.0/blueye.sdk_docs/sitemap.xml
--rw-r--r--   0        0        0      205 2020-02-27 08:43:48.627517 blueye.sdk-5.0.0/blueye.sdk_docs/sitemap.xml.gz
--rw-r--r--   0        0        0     3387 2020-02-27 08:43:12.115604 blueye.sdk-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 blueye.sdk-5.0.0/setup.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 blueye.sdk-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/LICENSE
+-rw-r--r--   0        0        0     2636 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/README.md
+-rw-r--r--   0        0        0      128 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/__init__.py
+-rw-r--r--   0        0        0     7971 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/camera.py
+-rw-r--r--   0        0        0      210 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/constants.py
+-rw-r--r--   0        0        0     5233 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/logs.py
+-rw-r--r--   0        0        0     7897 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/motion.py
+-rwxr-xr-x   0        0        0    10120 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/pioneer.py
+-rw-r--r--   0        0        0      532 2020-02-27 12:10:27.351340 blueye.sdk-5.0.1/blueye/sdk/utils.py
+-rw-r--r--   0        0        0    15258 2020-02-27 12:12:00.989467 blueye.sdk-5.0.1/blueye.sdk_docs/404.html
+-rw-r--r--   0        0        0     7652 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/LICENSE
+-rw-r--r--   0        0        0    21070 2020-02-27 12:12:01.009468 blueye.sdk-5.0.1/blueye.sdk_docs/README.html
+-rw-r--r--   0        0        0    30721 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/font-awesome.css
+-rw-r--r--   0        0        0      873 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/material-icons.css
+-rw-r--r--   0        0        0   165548 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.ttf
+-rw-r--r--   0        0        0    98024 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff
+-rw-r--r--   0        0        0    77160 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff2
+-rw-r--r--   0        0        0   128180 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.ttf
+-rw-r--r--   0        0        0    57620 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff
+-rw-r--r--   0        0        0    44300 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff2
+-rw-r--r--   0        0        0      521 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/favicon.png
+-rw-r--r--   0        0        0     1230 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/bitbucket.1b09e088.svg
+-rw-r--r--   0        0        0      993 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/github.f0b8504a.svg
+-rw-r--r--   0        0        0     1138 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/gitlab.6dd19c00.svg
+-rw-r--r--   0        0        0    79589 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/application.c33a9706.js
+-rw-r--r--   0        0        0    17538 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ar.js
+-rw-r--r--   0        0        0     4610 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.da.js
+-rw-r--r--   0        0        0     6087 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.de.js
+-rw-r--r--   0        0        0     6167 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.du.js
+-rw-r--r--   0        0        0    11424 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.es.js
+-rw-r--r--   0        0        0     9222 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.fi.js
+-rw-r--r--   0        0        0    10593 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.fr.js
+-rw-r--r--   0        0        0     9379 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.hu.js
+-rw-r--r--   0        0        0    11091 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.it.js
+-rw-r--r--   0        0        0     2629 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ja.js
+-rw-r--r--   0        0        0       36 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.jp.js
+-rw-r--r--   0        0        0      817 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.multi.js
+-rw-r--r--   0        0        0     5985 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.nl.js
+-rw-r--r--   0        0        0     4694 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.no.js
+-rw-r--r--   0        0        0    10083 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.pt.js
+-rw-r--r--   0        0        0    10851 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ro.js
+-rw-r--r--   0        0        0    10160 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ru.js
+-rw-r--r--   0        0        0     3808 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.stemmer.support.js
+-rw-r--r--   0        0        0     4481 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.sv.js
+-rw-r--r--   0        0        0     1381 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.th.js
+-rw-r--r--   0        0        0    14113 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.tr.js
+-rw-r--r--   0        0        0     1142 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.vi.js
+-rw-r--r--   0        0        0    18278 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   555307 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0     7296 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/modernizr.86422ebf.js
+-rw-r--r--   0        0        0    38773 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/stylesheets/application-palette.a8b3c06d.css
+-rw-r--r--   0        0        0    76332 2020-02-27 12:12:00.869460 blueye.sdk-5.0.1/blueye.sdk_docs/assets/stylesheets/application.adb8469c.css
+-rw-r--r--   0        0        0    19605 2020-02-27 12:12:01.013468 blueye.sdk-5.0.1/blueye.sdk_docs/contributing.html
+-rw-r--r--   0        0        0    25283 2020-02-27 12:12:01.025469 blueye.sdk-5.0.1/blueye.sdk_docs/docs/configuration.html
+-rw-r--r--   0        0        0  1039497 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/docs/http-api.html
+-rw-r--r--   0        0        0    24327 2020-02-27 12:12:01.045470 blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/listing-and-downloading.html
+-rw-r--r--   0        0        0    25567 2020-02-27 12:12:01.057471 blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/log-file-format.html
+-rw-r--r--   0        0        0    22254 2020-02-27 12:12:01.069471 blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/plotting.html
+-rw-r--r--   0        0        0     1607 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/docs/media/blueye_b.svg
+-rw-r--r--   0        0        0    35460 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/docs/media/depth_plot.svg
+-rw-r--r--   0        0        0    18795 2020-02-27 12:12:01.073472 blueye.sdk-5.0.1/blueye.sdk_docs/docs/movement/from-the-CLI.html
+-rw-r--r--   0        0        0    30730 2020-02-27 12:12:01.093473 blueye.sdk-5.0.1/blueye.sdk_docs/docs/movement/with-a-gamepad.html
+-rw-r--r--   0        0        0    32374 2020-02-27 12:12:01.037470 blueye.sdk-5.0.1/blueye.sdk_docs/docs/quick_start.html
+-rw-r--r--   0        0        0    23508 2020-02-27 12:12:01.101473 blueye.sdk-5.0.1/blueye.sdk_docs/docs/video/downloading.html
+-rw-r--r--   0        0        0    22904 2020-02-27 12:12:01.109474 blueye.sdk-5.0.1/blueye.sdk_docs/docs/video/gstreamer-for-video-streaming.html
+-rw-r--r--   0        0        0    23406 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/http-api.yml
+-rw-r--r--   0        0        0    82322 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/poetry.lock
+-rw-r--r--   0        0        0     3387 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/pyproject.toml
+-rw-r--r--   0        0        0      215 2020-02-27 12:12:00.865460 blueye.sdk-5.0.1/blueye.sdk_docs/pytest.ini
+-rw-r--r--   0        0        0    45163 2020-02-27 12:12:01.129475 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/camera.html
+-rw-r--r--   0        0        0    20855 2020-02-27 12:12:01.133475 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/constants.html
+-rw-r--r--   0        0        0    19018 2020-02-27 12:12:01.113474 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/index.html
+-rw-r--r--   0        0        0    36628 2020-02-27 12:12:01.145475 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/logs.html
+-rw-r--r--   0        0        0    43676 2020-02-27 12:12:01.153476 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/motion.html
+-rw-r--r--   0        0        0    51876 2020-02-27 12:12:01.169477 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/pioneer.html
+-rw-r--r--   0        0        0    20016 2020-02-27 12:12:01.177477 blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/utils.html
+-rw-r--r--   0        0        0   198948 2020-02-27 12:12:01.177477 blueye.sdk-5.0.1/blueye.sdk_docs/search/search_index.json
+-rw-r--r--   0        0        0     2053 2020-02-27 12:12:00.877461 blueye.sdk-5.0.1/blueye.sdk_docs/sitemap.xml
+-rw-r--r--   0        0        0      205 2020-02-27 12:12:00.877461 blueye.sdk-5.0.1/blueye.sdk_docs/sitemap.xml.gz
+-rw-r--r--   0        0        0     3387 2020-02-27 12:11:36.671747 blueye.sdk-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 blueye.sdk-5.0.1/setup.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 blueye.sdk-5.0.1/PKG-INFO
```

### Comparing `blueye.sdk-5.0.0/LICENSE` & `blueye.sdk-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/README.md` & `blueye.sdk-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye/sdk/camera.py` & `blueye.sdk-5.0.1/blueye/sdk/camera.py`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye/sdk/logs.py` & `blueye.sdk-5.0.1/blueye/sdk/logs.py`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye/sdk/motion.py` & `blueye.sdk-5.0.1/blueye/sdk/motion.py`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye/sdk/pioneer.py` & `blueye.sdk-5.0.1/blueye/sdk/pioneer.py`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye/sdk/utils.py` & `blueye.sdk-5.0.1/blueye/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/404.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/404.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/LICENSE` & `blueye.sdk-5.0.1/blueye.sdk_docs/LICENSE`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/README.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/README.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/font-awesome.css` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/material-icons.css` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/material-icons.css`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.ttf` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.ttf`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff2` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/FontAwesome.woff2`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.ttf` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff2` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/fonts/specimen/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/favicon.png` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/bitbucket.1b09e088.svg` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/bitbucket.1b09e088.svg`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/github.f0b8504a.svg` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/github.f0b8504a.svg`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/images/icons/gitlab.6dd19c00.svg` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/images/icons/gitlab.6dd19c00.svg`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/application.c33a9706.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/application.c33a9706.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ar.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ar.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.da.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.da.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.de.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.de.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.du.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.du.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.es.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.es.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.fi.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.fr.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.hu.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.it.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.it.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ja.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.multi.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.nl.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.no.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.no.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.pt.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ro.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.ru.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.stemmer.support.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.sv.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.th.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.th.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.tr.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/lunr.vi.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/tinyseg.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/lunr/wordcut.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/javascripts/modernizr.86422ebf.js` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/javascripts/modernizr.86422ebf.js`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/stylesheets/application-palette.a8b3c06d.css` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/stylesheets/application-palette.a8b3c06d.css`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/assets/stylesheets/application.adb8469c.css` & `blueye.sdk-5.0.1/blueye.sdk_docs/assets/stylesheets/application.adb8469c.css`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/contributing.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/contributing.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/configuration.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/configuration.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/http-api.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/http-api.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/listing-and-downloading.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/listing-and-downloading.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/log-file-format.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/log-file-format.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/logs/plotting.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/logs/plotting.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/media/blueye_b.svg` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/media/blueye_b.svg`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/media/depth_plot.svg` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/media/depth_plot.svg`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/movement/from-the-CLI.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/movement/from-the-CLI.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/movement/with-a-gamepad.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/movement/with-a-gamepad.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/quick_start.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/quick_start.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/video/downloading.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/video/downloading.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/docs/video/gstreamer-for-video-streaming.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/docs/video/gstreamer-for-video-streaming.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/http-api.yml` & `blueye.sdk-5.0.1/blueye.sdk_docs/http-api.yml`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/poetry.lock` & `blueye.sdk-5.0.1/blueye.sdk_docs/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 [[package]]
 category = "main"
 description = "Python protocol definition for the Blueye Pioneer"
 name = "blueye.protocol"
 optional = false
 python-versions = ">=3.7,<4.0"
-version = "1.2.1"
+version = "1.2.2"
 
 [package.dependencies]
 numpy = ">=1.17,<2.0"
 setuptools = ">=40"
 
 [[package]]
 category = "main"
@@ -982,15 +982,15 @@
 docs = ["sphinx", "jaraco.packaging (>=3.2)", "rst.linker (>=1.9)"]
 testing = ["jaraco.itertools", "func-timeout"]
 
 [extras]
 examples = ["inputs", "asciimatics", "pandas", "matplotlib", "webdavclient3"]
 
 [metadata]
-content-hash = "3f9f7e4bf39dc715a1ab4858d7b6acb21c392c0bb0c688bd42b9c3a56e5b33e4"
+content-hash = "6d37c463dee0b404e2010f4026b34ed0e3818a3b03f9d9bebefccaae7c7fc0c8"
 python-versions = "^3.7"
 
 [metadata.files]
 appdirs = [
     {file = "appdirs-1.4.3-py2.py3-none-any.whl", hash = "sha256:d8b24664561d0d34ddfaec54636d502d7cea6e29c3eaf68f3df6180863e2166e"},
     {file = "appdirs-1.4.3.tar.gz", hash = "sha256:9e5896d1372858f8dd3344faf4e5014d21849c756c8d5701f78f8a103b372d92"},
 ]
@@ -1015,16 +1015,16 @@
     {file = "attrs-19.3.0.tar.gz", hash = "sha256:f7b7ce16570fe9965acd6d30101a28f62fb4a7f9e926b3bbc9b61f8b04247e72"},
 ]
 black = [
     {file = "black-19.10b0-py36-none-any.whl", hash = "sha256:1b30e59be925fafc1ee4565e5e08abef6b03fe455102883820fe5ee2e4734e0b"},
     {file = "black-19.10b0.tar.gz", hash = "sha256:c2edb73a08e9e0e6f65a0e6af18b059b8b1cdd5bef997d7a0b181df93dc81539"},
 ]
 "blueye.protocol" = [
-    {file = "blueye.protocol-1.2.1-py3-none-any.whl", hash = "sha256:92bdff1196127b78d45767d3675531cc0f074080064c1950cf0f63ffaf2170b5"},
-    {file = "blueye.protocol-1.2.1.tar.gz", hash = "sha256:07a13fbd7ad873f759a03147c525952ed4c0d2f90a0c757e138628865547f2c9"},
+    {file = "blueye.protocol-1.2.2-py3-none-any.whl", hash = "sha256:de456805eefe96e39a0291aeb60eb43ebe8426e6cc66922d862f1c6186281b97"},
+    {file = "blueye.protocol-1.2.2.tar.gz", hash = "sha256:29fac9a48589c44eefe7d4786fa74d27aa6d6da42f8700d26edcdbf7c6712afa"},
 ]
 certifi = [
     {file = "certifi-2019.11.28-py2.py3-none-any.whl", hash = "sha256:017c25db2a153ce562900032d5bc68e9f191e44e9a0f762f373977de9df1fbb3"},
     {file = "certifi-2019.11.28.tar.gz", hash = "sha256:25b64c7da4cd7479594d035c08c2d809eb4aab3a26e5a990ea98cc450c320f1f"},
 ]
 cfgv = [
     {file = "cfgv-3.1.0-py2.py3-none-any.whl", hash = "sha256:1ccf53320421aeeb915275a196e23b3b8ae87dea8ac6698b1638001d4a486d53"},
```

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/pyproject.toml` & `blueye.sdk-5.0.1/blueye.sdk_docs/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blueye.sdk"
-version = "5.0.0"
+version = "5.0.1"
 description = "SDK for controlling a Blueye Pioneer"
 authors = ["Sindre Hansen <sindre.hansen@blueye.no>",
            "Aksel Lenes <aksel.lenes@blueye.no"]
 packages = [
   { include = "blueye" }
 ]
 
@@ -12,15 +12,15 @@
 readme = "README.md"
 repository="https://github.com/blueye-robotics/blueye.sdk"
 homepage ="https://www.blueyerobotics.com"
 keywords = ["Blueye", "Pioneer", "Robotics", "SDK", "Software Development Kit"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-"blueye.protocol" = "^1.2.1"
+"blueye.protocol" = "^1.2.2"
 asciimatics = {version = "^1.11.0", optional = true}
 inputs = {version = "^0.5", optional = true}
 pandas = {version = "^0.25.2", optional = true}
 matplotlib = {version = "^3.1.1", optional = true}
 webdavclient3 = {version = "^0.12", optional = true}
 requests = "^2.22.0"
 tabulate = "^0.8.5"
```

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/camera.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/camera.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/constants.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/constants.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/index.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/index.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/logs.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/logs.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/motion.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/motion.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/pioneer.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/pioneer.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/reference/blueye/sdk/utils.html` & `blueye.sdk-5.0.1/blueye.sdk_docs/reference/blueye/sdk/utils.html`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/search/search_index.json` & `blueye.sdk-5.0.1/blueye.sdk_docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/blueye.sdk_docs/sitemap.xml` & `blueye.sdk-5.0.1/blueye.sdk_docs/sitemap.xml`

 * *Files identical despite different names*

### Comparing `blueye.sdk-5.0.0/pyproject.toml` & `blueye.sdk-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blueye.sdk"
-version = "5.0.0"
+version = "5.0.1"
 description = "SDK for controlling a Blueye Pioneer"
 authors = ["Sindre Hansen <sindre.hansen@blueye.no>",
            "Aksel Lenes <aksel.lenes@blueye.no"]
 packages = [
   { include = "blueye" }
 ]
 
@@ -12,15 +12,15 @@
 readme = "README.md"
 repository="https://github.com/blueye-robotics/blueye.sdk"
 homepage ="https://www.blueyerobotics.com"
 keywords = ["Blueye", "Pioneer", "Robotics", "SDK", "Software Development Kit"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-"blueye.protocol" = "^1.2.1"
+"blueye.protocol" = "^1.2.2"
 asciimatics = {version = "^1.11.0", optional = true}
 inputs = {version = "^0.5", optional = true}
 pandas = {version = "^0.25.2", optional = true}
 matplotlib = {version = "^3.1.1", optional = true}
 webdavclient3 = {version = "^0.12", optional = true}
 requests = "^2.22.0"
 tabulate = "^0.8.5"
```

### Comparing `blueye.sdk-5.0.0/setup.py` & `blueye.sdk-5.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 packages = \
 ['blueye', 'blueye.sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['blueye.protocol>=1.2.1,<2.0.0',
+['blueye.protocol>=1.2.2,<2.0.0',
  'packaging>=20.1,<21.0',
  'requests>=2.22.0,<3.0.0',
  'tabulate>=0.8.5,<0.9.0']
 
 extras_require = \
 {'examples': ['asciimatics>=1.11.0,<2.0.0',
               'inputs>=0.5,<0.6',
               'pandas>=0.25.2,<0.26.0',
               'matplotlib>=3.1.1,<4.0.0',
               'webdavclient3>=0.12,<0.13']}
 
 setup_kwargs = {
     'name': 'blueye.sdk',
-    'version': '5.0.0',
+    'version': '5.0.1',
     'description': 'SDK for controlling a Blueye Pioneer',
     'long_description': '# blueye.sdk\n[![Tests](https://github.com/BluEye-Robotics/blueye.sdk/workflows/Tests/badge.svg)](https://github.com/BluEye-Robotics/blueye.sdk/actions)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/BluEye-Robotics/blueye.sdk.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/BluEye-Robotics/blueye.sdk/context:python)\n[![codecov](https://codecov.io/gh/BluEye-Robotics/blueye.sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/BluEye-Robotics/blueye.sdk)\n[![PyPi-version](https://img.shields.io/pypi/v/blueye.sdk.svg?maxAge=3600)](https://pypi.org/project/blueye.sdk/)\n[![python-versions](https://img.shields.io/pypi/pyversions/blueye.sdk.svg?longCache=True)](https://pypi.org/project/blueye.sdk/)\n_________________\n\n[Read Latest Documentation](https://blueye-robotics.github.io/blueye.sdk/) - [Browse GitHub Code Repository](https://github.com/BluEye-Robotics/blueye.sdk)\n_________________\n\n**Note: This is a pre-release -- Please report any issues you might encounter**\n_________________\nA Python package for remote control of the Blueye Pioneer underwater drone.\n\n\n![SDK demo](https://user-images.githubusercontent.com/8504604/66751230-d05c7e00-ee8e-11e9-91cb-d46b433aafa5.gif)\n\n## About The Pioneer\nThe Blueye Pioneer is a underwater drone designed for inspections. It is produced and sold by the Norwegian company [`Blueye Robotics`](https://www.blueyerobotics.com/).\nHere is a Youtube video  that gives a overview of the system and its specifications.\n\n[![about the Pioneer video](https://img.youtube.com/vi/_-AEtr6xOP8/0.jpg)](https://www.youtube.com/watch?v=_-AEtr6xOP8)\n\n## This SDK and the Pioneer\nThe Pioneer is normally controlled via a mobile device through the Blueye App ([iOS](https://apps.apple.com/no/app/blueye/id1369714041)/[Android](https://play.google.com/store/apps/details?id=no.blueye.blueyeapp)). The mobile device\nis connected via WiFi to a surface unit, and the Pioneer is connected to the surface unit via a tether cable.\n\nThis python SDK exposes the functionality of the Blueye app through a Python object. The SDK enables remote control of the Pioneer as well as reading telemetry data and viewing video streams, it is not meant for executing code on the Pioneer.\nTo control the Pioneer you connect your laptop to the surface unit WiFi and run code that interfaces with the Pioneer through the Pioneer Python object.\n\n\nCheck out the [`Quick Start Guide`](https://blueye-robotics.github.io/blueye.sdk/docs/quick_start/) to get started with using the SDK.\n',
     'author': 'Sindre Hansen',
     'author_email': 'sindre.hansen@blueye.no',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.blueyerobotics.com',
```

### Comparing `blueye.sdk-5.0.0/PKG-INFO` & `blueye.sdk-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: blueye.sdk
-Version: 5.0.0
+Version: 5.0.1
 Summary: SDK for controlling a Blueye Pioneer
 Home-page: https://www.blueyerobotics.com
 Keywords: Blueye,Pioneer,Robotics,SDK,Software Development Kit
 Author: Sindre Hansen
 Author-email: sindre.hansen@blueye.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: examples
 Requires-Dist: asciimatics (>=1.11.0,<2.0.0); extra == "examples"
-Requires-Dist: blueye.protocol (>=1.2.1,<2.0.0)
+Requires-Dist: blueye.protocol (>=1.2.2,<2.0.0)
 Requires-Dist: inputs (>=0.5,<0.6); extra == "examples"
 Requires-Dist: matplotlib (>=3.1.1,<4.0.0); extra == "examples"
 Requires-Dist: packaging (>=20.1,<21.0)
 Requires-Dist: pandas (>=0.25.2,<0.26.0); extra == "examples"
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Requires-Dist: tabulate (>=0.8.5,<0.9.0)
 Requires-Dist: webdavclient3 (>=0.12,<0.13); extra == "examples"
```

