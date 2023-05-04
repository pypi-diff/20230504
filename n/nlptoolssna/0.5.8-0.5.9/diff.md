# Comparing `tmp/nlptoolssna-0.5.8.tar.gz` & `tmp/nlptoolssna-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.5.8.tar", last modified: Thu May  4 13:56:08 2023, max compression
+gzip compressed data, was "nlptoolssna-0.5.9.tar", last modified: Thu May  4 20:10:07 2023, max compression
```

## Comparing `nlptoolssna-0.5.8.tar` & `nlptoolssna-0.5.9.tar`

### file list

```diff
@@ -1,81 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.995191 nlptoolssna-0.5.8/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-04 13:56:07.995191 nlptoolssna-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.877324 nlptoolssna-0.5.8/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.839612 nlptoolssna-0.5.8/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.840857 nlptoolssna-0.5.8/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.879321 nlptoolssna-0.5.8/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.8/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.890273 nlptoolssna-0.5.8/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.8/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.8/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.8/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.8/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.913625 nlptoolssna-0.5.8/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.916603 nlptoolssna-0.5.8/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.8/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.923331 nlptoolssna-0.5.8/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.926153 nlptoolssna-0.5.8/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.8/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.8/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.928151 nlptoolssna-0.5.8/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.8/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.8/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.8/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.8/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.8/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.8/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.8/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.933669 nlptoolssna-0.5.8/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.939436 nlptoolssna-0.5.8/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.8/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.8/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.951373 nlptoolssna-0.5.8/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.8/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.8/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.8/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.8/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.8/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.8/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.954567 nlptoolssna-0.5.8/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.8/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.959568 nlptoolssna-0.5.8/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.8/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.8/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.969180 nlptoolssna-0.5.8/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.8/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.8/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     7950 2023-05-04 08:27:31.000000 nlptoolssna-0.5.8/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.8/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.8/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.974186 nlptoolssna-0.5.8/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.8/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.8/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.979183 nlptoolssna-0.5.8/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.8/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.8/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.8/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.992187 nlptoolssna-0.5.8/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 13:56:07.000000 nlptoolssna-0.5.8/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-04 13:56:07.997760 nlptoolssna-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     2099 2023-05-04 13:53:33.000000 nlptoolssna-0.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:56:07.994186 nlptoolssna-0.5.8/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.8/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.554300 nlptoolssna-0.5.9/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-04 20:10:07.554300 nlptoolssna-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.440723 nlptoolssna-0.5.9/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.407172 nlptoolssna-0.5.9/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.408180 nlptoolssna-0.5.9/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.442698 nlptoolssna-0.5.9/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.9/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.451665 nlptoolssna-0.5.9/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.9/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.9/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.9/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.9/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.464500 nlptoolssna-0.5.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.466445 nlptoolssna-0.5.9/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.9/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.472877 nlptoolssna-0.5.9/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.475361 nlptoolssna-0.5.9/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.9/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.9/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.477315 nlptoolssna-0.5.9/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.9/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.9/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.483372 nlptoolssna-0.5.9/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.5.9/docs/source/api/utils/implication.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.485328 nlptoolssna-0.5.9/docs/source/api/utils/jaccard/
+-rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.5.9/docs/source/api/utils/jaccard/jaccardFunction.rst
+-rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.5.9/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.5.9/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.5.9/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.5.9/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.9/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.5.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.9/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.491222 nlptoolssna-0.5.9/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.495191 nlptoolssna-0.5.9/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.9/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.9/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.509384 nlptoolssna-0.5.9/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.9/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.9/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.9/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.9/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.9/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.9/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.511337 nlptoolssna-0.5.9/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.9/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.523126 nlptoolssna-0.5.9/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.9/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.9/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     7950 2023-05-04 19:24:11.000000 nlptoolssna-0.5.9/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.9/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.9/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.528912 nlptoolssna-0.5.9/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.9/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.9/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.9/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.533793 nlptoolssna-0.5.9/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.9/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    20611 2023-05-04 16:11:55.000000 nlptoolssna-0.5.9/nlptools/utils/implication.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.535748 nlptoolssna-0.5.9/nlptools/utils/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.9/nlptools/utils/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-05-04 19:22:43.000000 nlptoolssna-0.5.9/nlptools/utils/jaccard/jaccardFunction.py
+-rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.5.9/nlptools/utils/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.548441 nlptoolssna-0.5.9/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1841 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 20:10:07.000000 nlptoolssna-0.5.9/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-04 20:10:07.557231 nlptoolssna-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:10:07.553326 nlptoolssna-0.5.9/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.9/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.5.8/CONTRIBUTING.rst` & `nlptoolssna-0.5.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/LICENSE` & `nlptoolssna-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/PKG-INFO` & `nlptoolssna-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.8/README.rst` & `nlptoolssna-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/Makefile` & `nlptoolssna-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/build/html/_images/download.png` & `nlptoolssna-0.5.9/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/build/html/_static/download.png` & `nlptoolssna-0.5.9/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/make.bat` & `nlptoolssna-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/source/_static/download.png` & `nlptoolssna-0.5.9/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/source/conf.py` & `nlptoolssna-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/docs/source/installation.rst` & `nlptoolssna-0.5.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.5.9/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/arabiner/data.py` & `nlptoolssna-0.5.9/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/arabiner/datasets.py` & `nlptoolssna-0.5.9/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/arabiner/helpers.py` & `nlptoolssna-0.5.9/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/arabiner/infer.py` & `nlptoolssna-0.5.9/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/arabiner/transforms.py` & `nlptoolssna-0.5.9/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/data/my_data.pickle` & `nlptoolssna-0.5.9/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.5.9/nlptools/utils/jaccard/jaccardFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Dec  1 14:22:26 2021
 
 @author: Tymaa
 """
 
-from nlptools.parse.parser import arStrip
-from nlptools.salma.implication import Implication
+from nlptools.utlis.parser import arStrip
+from nlptools.utlis.implication import Implication
 
 
 def normalizeWord(word, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic):
     if ignoreAllDiacriticsButNotShadda:
         word = arStrip(word, True, True, False, False, False, False) # Remove diacs and smallDiacs 
         
     if ignoreShaddaDiacritic:
```

### Comparing `nlptoolssna-0.5.8/nlptools/morphology/charsets.py` & `nlptoolssna-0.5.9/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.5.9/nlptools/morphology/morph_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 from nlptools.morphology import settings 
 import re
 from nlptools.morphology.tokenizers_words import simple_word_tokenize
-from nlptools.parse.parser import arStrip
+from nlptools.utlis.parser import arStrip
 import os.path
 from nlptools.DataDownload import downloader
 from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
 import copy
 # def load_ALMA_dic():
 #    # Open the Pickle file in binary mode
 #     filename = 'ALMA27012000.pickle'
```

### Comparing `nlptoolssna-0.5.8/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.5.9/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/salma/implication.py` & `nlptoolssna-0.5.9/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.5.9/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.5.9/nlptoolssna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.8/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.5.9/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,46 @@
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/readme.rst
 docs/source/_static/download.png
 docs/source/api/DataDownload.rst
 docs/source/api/morphology.rst
+docs/source/api/utils.rst
 docs/source/api/DataDownload/downloader.rst
 docs/source/api/morphology/morph_analyzer.rst
+docs/source/api/utils/implication.rst
+docs/source/api/utils/jaccard.rst
+docs/source/api/utils/parser.rst
+docs/source/api/utils/jaccard/jaccardFunction.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
 nlptools/arabiner/datasets.py
 nlptools/arabiner/helpers.py
 nlptools/arabiner/infer.py
 nlptools/arabiner/transforms.py
 nlptools/data/my_data.pickle
-nlptools/jaccard/__init__.py
-nlptools/jaccard/jaccardFunction.py
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
-nlptools/parse/__init__.py
-nlptools/parse/parser.py
 nlptools/salma/__init__.py
 nlptools/salma/implication.py
 nlptools/salma/tokenizers_words.py
+nlptools/utils/__init__.py
+nlptools/utils/implication.py
+nlptools/utils/parser.py
+nlptools/utils/jaccard/__init__.py
+nlptools/utils/jaccard/jaccardFunction.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
 nlptoolssna.egg-info/requires.txt
 nlptoolssna.egg-info/top_level.txt
```

### Comparing `nlptoolssna-0.5.8/setup.cfg` & `nlptoolssna-0.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.8/setup.py` & `nlptoolssna-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     'pathlib',
     'torch==1.13.0',
     'transformers==4.24.0',
     'torchtext==0.14.0',
     'torchvision==0.14.0',
     'torchdata==0.5.1',
     'seqeval==1.2.2'
-
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
     author_email='alaa.omer2009@gmail.com',
```

