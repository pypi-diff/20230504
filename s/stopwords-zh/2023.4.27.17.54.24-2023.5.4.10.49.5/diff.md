# Comparing `tmp/stopwords-zh-2023.4.27.17.54.24.tar.gz` & `tmp/stopwords-zh-2023.5.4.10.49.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords-zh-2023.4.27.17.54.24.tar", last modified: Thu Apr 27 09:54:24 2023, max compression
+gzip compressed data, was "stopwords-zh-2023.5.4.10.49.5.tar", last modified: Thu May  4 02:49:06 2023, max compression
```

## Comparing `stopwords-zh-2023.4.27.17.54.24.tar` & `stopwords-zh-2023.5.4.10.49.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.865401 stopwords-zh-2023.4.27.17.54.24/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.859736 stopwords-zh-2023.4.27.17.54.24/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      323 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)     3590 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-27 09:53:36.000000 stopwords-zh-2023.4.27.17.54.24/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1071 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      325 2023-04-18 10:05:52.000000 stopwords-zh-2023.4.27.17.54.24/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2235 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1769 2023-04-27 09:54:24.865235 stopwords-zh-2023.4.27.17.54.24/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1056 2023-04-27 09:52:41.000000 stopwords-zh-2023.4.27.17.54.24/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.861535 stopwords-zh-2023.4.27.17.54.24/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      613 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-04-18 10:20:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4843 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      309 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1162 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      810 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       79 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      201 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-18 10:02:26.000000 stopwords-zh-2023.4.27.17.54.24/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-18 10:14:19.000000 stopwords-zh-2023.4.27.17.54.24/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 09:54:24.865452 stopwords-zh-2023.4.27.17.54.24/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1543 2023-04-27 09:54:23.000000 stopwords-zh-2023.4.27.17.54.24/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.861789 stopwords-zh-2023.4.27.17.54.24/stopwords/
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-04-27 09:51:45.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1423 2023-04-27 09:51:21.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/_stopwords.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.862175 stopwords-zh-2023.4.27.17.54.24/stopwords/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      574 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.863758 stopwords-zh-2023.4.27.17.54.24/stopwords/data/
--rw-r--r--   0 betterme   (501) staff       (20)    18313 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.all.txt
--rw-r--r--   0 betterme   (501) staff       (20)     9243 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.baidu.txt
--rw-r--r--   0 betterme   (501) staff       (20)     4717 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.cn.txt
--rw-r--r--   0 betterme   (501) staff       (20)     5273 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.hit.txt
--rw-r--r--   0 betterme   (501) staff       (20)     8115 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.ict.txt
--rw-r--r--   0 betterme   (501) staff       (20)     4961 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.iso.txt
--rw-r--r--   0 betterme   (501) staff       (20)     2553 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.marimo.txt
--rw-r--r--   0 betterme   (501) staff       (20)     7597 2023-04-18 09:26:36.000000 stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.scu.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.864687 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1769 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1036 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-27 09:54:24.000000 stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 09:54:24.864987 stopwords-zh-2023.4.27.17.54.24/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       42 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      887 2023-04-18 09:32:21.000000 stopwords-zh-2023.4.27.17.54.24/tests/test_stopwords-zh.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.152488 stopwords-zh-2023.5.4.10.49.5/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.146528 stopwords-zh-2023.5.4.10.49.5/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      323 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)     3590 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-27 09:53:36.000000 stopwords-zh-2023.5.4.10.49.5/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1071 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      325 2023-04-18 10:05:52.000000 stopwords-zh-2023.5.4.10.49.5/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2235 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-05-04 02:49:06.152359 stopwords-zh-2023.5.4.10.49.5/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1056 2023-04-27 09:52:41.000000 stopwords-zh-2023.5.4.10.49.5/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.148799 stopwords-zh-2023.5.4.10.49.5/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      613 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-04-18 10:20:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4843 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      309 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1162 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      810 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       79 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      215 2023-04-27 09:56:06.000000 stopwords-zh-2023.5.4.10.49.5/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-18 10:02:26.000000 stopwords-zh-2023.5.4.10.49.5/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-18 10:14:19.000000 stopwords-zh-2023.5.4.10.49.5/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 02:49:06.152533 stopwords-zh-2023.5.4.10.49.5/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1543 2023-04-27 09:54:23.000000 stopwords-zh-2023.5.4.10.49.5/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.149190 stopwords-zh-2023.5.4.10.49.5/stopwords/
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-04-27 09:51:45.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1438 2023-05-04 02:48:46.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/_stopwords.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.149630 stopwords-zh-2023.5.4.10.49.5/stopwords/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      574 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.151151 stopwords-zh-2023.5.4.10.49.5/stopwords/data/
+-rw-r--r--   0 betterme   (501) staff       (20)    18313 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.all.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     9243 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.baidu.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     4717 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.cn.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     5273 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.hit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     8115 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.ict.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     4961 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.iso.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     2553 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.marimo.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     7597 2023-04-18 09:26:36.000000 stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.scu.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.151873 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1036 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-05-04 02:49:06.000000 stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:49:06.152129 stopwords-zh-2023.5.4.10.49.5/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       42 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      887 2023-04-18 09:32:21.000000 stopwords-zh-2023.5.4.10.49.5/tests/test_stopwords-zh.py
```

### Comparing `stopwords-zh-2023.4.27.17.54.24/.gitignore` & `stopwords-zh-2023.5.4.10.49.5/.gitignore`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/CONTRIBUTING.rst` & `stopwords-zh-2023.5.4.10.49.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/LICENSE` & `stopwords-zh-2023.5.4.10.49.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/Makefile` & `stopwords-zh-2023.5.4.10.49.5/Makefile`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/PKG-INFO` & `stopwords-zh-2023.5.4.10.49.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords-zh
-Version: 2023.4.27.17.54.24
+Version: 2023.5.4.10.49.5
 Summary: stopwords-zh
 Home-page: https://github.com/yuanjie-ai/stopwords-zh
 Author: stopwords-zh
 Author-email: yuanjie@example.com
 License: MIT license
 Keywords: stopwords-zh
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `stopwords-zh-2023.4.27.17.54.24/README.md` & `stopwords-zh-2023.5.4.10.49.5/README.md`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/docs/Makefile` & `stopwords-zh-2023.5.4.10.49.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/docs/README.md` & `stopwords-zh-2023.5.4.10.49.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/docs/conf.py` & `stopwords-zh-2023.5.4.10.49.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/docs/installation.rst` & `stopwords-zh-2023.5.4.10.49.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/docs/make.bat` & `stopwords-zh-2023.5.4.10.49.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/setup.py` & `stopwords-zh-2023.5.4.10.49.5/setup.py`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/_stopwords.py` & `stopwords-zh-2023.5.4.10.49.5/stopwords/_stopwords.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Return:
         a set, 停用词表集合
     """
 
     supported_source = ["cn", "baidu", "hit", "scu", "marimo", "ict", "iso", "all"]
     if source not in supported_source:
         raise NotImplementedError("请求了未知来源，请使用`help(stopwords)`查看支持的来源")
-    return set(get_resolve_path(f"./data/stopwords.zh.{source}.txt").read_text().strip().split())
+    return set(get_resolve_path(f"./data/stopwords.zh.{source}.txt").read_text(encoding='utf8').strip().split())
 
 
 def filter_stopwords(words, source='all'):
     sw = stopwords(source)
     return [w for w in words if w not in sw]
```

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/clis/cli.py` & `stopwords-zh-2023.5.4.10.49.5/stopwords/clis/cli.py`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.all.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.all.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.baidu.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.baidu.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.cn.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.cn.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.hit.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.hit.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.ict.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.ict.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.iso.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.iso.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.marimo.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.marimo.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords/data/stopwords.zh.scu.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords/data/stopwords.zh.scu.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/PKG-INFO` & `stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords-zh
-Version: 2023.4.27.17.54.24
+Version: 2023.5.4.10.49.5
 Summary: stopwords-zh
 Home-page: https://github.com/yuanjie-ai/stopwords-zh
 Author: stopwords-zh
 Author-email: yuanjie@example.com
 License: MIT license
 Keywords: stopwords-zh
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `stopwords-zh-2023.4.27.17.54.24/stopwords_zh.egg-info/SOURCES.txt` & `stopwords-zh-2023.5.4.10.49.5/stopwords_zh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stopwords-zh-2023.4.27.17.54.24/tests/test_stopwords-zh.py` & `stopwords-zh-2023.5.4.10.49.5/tests/test_stopwords-zh.py`

 * *Files identical despite different names*

