# Comparing `tmp/nlptoolssna-0.5.6.tar.gz` & `tmp/nlptoolssna-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.5.6.tar", last modified: Wed May  3 19:33:06 2023, max compression
+gzip compressed data, was "nlptoolssna-0.5.7.tar", last modified: Thu May  4 08:28:53 2023, max compression
```

## Comparing `nlptoolssna-0.5.6.tar` & `nlptoolssna-0.5.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.052841 nlptoolssna-0.5.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-03 19:33:06.053758 nlptoolssna-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.939455 nlptoolssna-0.5.6/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.898846 nlptoolssna-0.5.6/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.900850 nlptoolssna-0.5.6/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.941449 nlptoolssna-0.5.6/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.6/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.947476 nlptoolssna-0.5.6/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.6/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.6/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.6/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.6/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.961362 nlptoolssna-0.5.6/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.963364 nlptoolssna-0.5.6/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.6/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.967559 nlptoolssna-0.5.6/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.971114 nlptoolssna-0.5.6/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.6/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.6/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.974114 nlptoolssna-0.5.6/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.6/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.6/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.6/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.6/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.6/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.6/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.980172 nlptoolssna-0.5.6/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.983523 nlptoolssna-0.5.6/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.6/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.6/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.996578 nlptoolssna-0.5.6/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.6/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.6/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.6/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.6/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.6/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.6/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:05.999047 nlptoolssna-0.5.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.004066 nlptoolssna-0.5.6/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.6/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.6/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.016792 nlptoolssna-0.5.6/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.6/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.6/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     8214 2023-05-03 19:32:57.000000 nlptoolssna-0.5.6/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.6/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.6/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.021793 nlptoolssna-0.5.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.029340 nlptoolssna-0.5.6/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.6/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.6/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.6/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.045814 nlptoolssna-0.5.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 19:33:05.000000 nlptoolssna-0.5.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-03 19:33:06.055809 nlptoolssna-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:33:06.050755 nlptoolssna-0.5.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.709983 nlptoolssna-0.5.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-04 08:28:53.709983 nlptoolssna-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.564154 nlptoolssna-0.5.7/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.515480 nlptoolssna-0.5.7/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.516864 nlptoolssna-0.5.7/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.571649 nlptoolssna-0.5.7/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.7/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.594155 nlptoolssna-0.5.7/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.7/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.7/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.7/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.7/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.617845 nlptoolssna-0.5.7/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.626633 nlptoolssna-0.5.7/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.7/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.635144 nlptoolssna-0.5.7/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.639986 nlptoolssna-0.5.7/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.7/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.7/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.641986 nlptoolssna-0.5.7/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.7/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.7/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.7/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.7/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.7/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.646983 nlptoolssna-0.5.7/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.650538 nlptoolssna-0.5.7/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.7/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.7/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.661769 nlptoolssna-0.5.7/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.7/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.7/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.7/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.7/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.7/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.7/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.666652 nlptoolssna-0.5.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.670664 nlptoolssna-0.5.7/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.7/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.7/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.680549 nlptoolssna-0.5.7/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.7/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.7/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     7950 2023-05-04 08:27:31.000000 nlptoolssna-0.5.7/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.7/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.7/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.685646 nlptoolssna-0.5.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.691645 nlptoolssna-0.5.7/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.7/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.7/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.7/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.705337 nlptoolssna-0.5.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 08:28:53.000000 nlptoolssna-0.5.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-04 08:28:53.711988 nlptoolssna-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:28:53.708983 nlptoolssna-0.5.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.5.6/CONTRIBUTING.rst` & `nlptoolssna-0.5.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/LICENSE` & `nlptoolssna-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/PKG-INFO` & `nlptoolssna-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.6/README.rst` & `nlptoolssna-0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/Makefile` & `nlptoolssna-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/build/html/_images/download.png` & `nlptoolssna-0.5.7/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/build/html/_static/download.png` & `nlptoolssna-0.5.7/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/make.bat` & `nlptoolssna-0.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/source/_static/download.png` & `nlptoolssna-0.5.7/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/source/conf.py` & `nlptoolssna-0.5.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/docs/source/installation.rst` & `nlptoolssna-0.5.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.5.7/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/arabiner/data.py` & `nlptoolssna-0.5.7/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/arabiner/datasets.py` & `nlptoolssna-0.5.7/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/arabiner/helpers.py` & `nlptoolssna-0.5.7/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/arabiner/infer.py` & `nlptoolssna-0.5.7/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/arabiner/transforms.py` & `nlptoolssna-0.5.7/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.5.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.5.7/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/morphology/charsets.py` & `nlptoolssna-0.5.7/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.5.7/nlptools/morphology/morph_analyzer.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,22 +33,16 @@
         list (:obj:`list`): A list of [token, lemma, pos], where:
             - token: the original input token
             - lemma: the lemma of the token 
             - pos: the part-of-speech of the token 
             If no sloution is found for this token, an empty list is returned.
     """
     if token in settings.div_dic.keys():
-        soluation =settings.div_dic[token]
-        if task =='full' :          
-            return  [token, soluation[0], soluation[1]]               
-        elif  task == 'pos':                       
-            return  [token, soluation[1]]
-        elif  task == 'lemmatizer':                       
-            return  [token, soluation[0]]       
-        return []
+        soluation = settings.div_dic[token]
+        return  [token, soluation[0], soluation[1]]               
     else:
         return []
 
 def analyze(text, language ='MSA', task ='full'):
    """
     This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
     if:
@@ -123,14 +117,15 @@
                output_list.append(result_token)
          else:
             # if no solution is found
             output_list.append(solution)
         
    return filter_results(task, output_list)
 
+
 def filter_results(task, lst):
     if task == 'lemmatizer':
         return remove_items_by_index(lst, [2])
     elif task == 'pos':
         return remove_items_by_index(lst, [1])
     else: 
         return lst
```

### Comparing `nlptoolssna-0.5.6/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.5.7/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/parse/parser.py` & `nlptoolssna-0.5.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/salma/implication.py` & `nlptoolssna-0.5.7/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.5.7/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.5.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.5.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/setup.cfg` & `nlptoolssna-0.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.6/setup.py` & `nlptoolssna-0.5.7/setup.py`

 * *Files identical despite different names*

