# Comparing `tmp/langSrc-0.0.6.tar.gz` & `tmp/langsrc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langSrc-0.0.6.tar", last modified: Sun Jan 15 11:14:10 2023, max compression
+gzip compressed data, was "langsrc-0.0.8.tar", max compression
```

## Comparing `langSrc-0.0.6.tar` & `langsrc-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2023-01-15 11:14:10.796094 langSrc-0.0.6/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      392 2023-01-15 11:14:10.795973 langSrc-0.0.6/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      750 2022-11-13 13:41:41.000000 langSrc-0.0.6/README.md
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2023-01-15 11:14:10.795064 langSrc-0.0.6/langSrc/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2829 2022-11-13 13:55:11.000000 langSrc-0.0.6/langSrc/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2023-01-15 11:14:10.795687 langSrc-0.0.6/langSrc.egg-info/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      392 2023-01-15 11:14:10.000000 langSrc-0.0.6/langSrc.egg-info/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      188 2023-01-15 11:14:10.000000 langSrc-0.0.6/langSrc.egg-info/SOURCES.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2023-01-15 11:14:10.000000 langSrc-0.0.6/langSrc.egg-info/dependency_links.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        8 2023-01-15 11:14:10.000000 langSrc-0.0.6/langSrc.egg-info/top_level.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-11-13 11:48:52.000000 langSrc-0.0.6/langSrc.egg-info/zip-safe
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       38 2023-01-15 11:14:10.796128 langSrc-0.0.6/setup.cfg
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      642 2023-01-15 11:14:10.000000 langSrc-0.0.6/setup.py
+-rw-r--r--   0        0        0      750 2022-11-13 13:41:41.935206 langsrc-0.0.8/README.md
+-rw-r--r--   0        0        0     2975 2023-05-04 09:38:23.352918 langsrc-0.0.8/langsrc/__init__.py
+-rw-r--r--   0        0        0      309 2023-05-04 09:40:11.721198 langsrc-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 langsrc-0.0.8/setup.py
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 langsrc-0.0.8/PKG-INFO
```

### Comparing `langSrc-0.0.6/README.md` & `langsrc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `langSrc-0.0.6/langSrc/__init__.py` & `langsrc-0.0.8/langsrc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 name = "langSrc"
 
 
 class LanguageDetector:
-    def __init__(self, lang, srcPath, auto_translate=None):
+    def __init__(self, lang, srcPath, auto_translate=None, native_lang=None):
         """
         :param lang: 语言 | Language
         :param srcPath: 语言源文件路径 | Language source file path
         :param auto_translate: 自动翻译函数 | Auto translate function: func(text, lang) -> str
+        :param native_lang: 本地语言 | Native language
         """
+        self._native_lang = native_lang
         self._default_lang = lang.lower()
         self._srcPath = srcPath
         self._save_flag = 0
         self._load()
         self._save_flag = 1
         self._translate = auto_translate
 
@@ -66,15 +68,15 @@
             "slo": "Jezik",
             "swe": "Språk",
             "hu": "Nyelv",
             "vie": "Ngôn ngữ"
         }
         """
         if not hasattr(self, name):
-            setattr(self, name, word.get(self._default_lang, None))
+            setattr(self, name, word.get(self._default_lang, word.get(self._native_lang, None)))
             if self._save_flag > 0:
                 self._src[name] = word
                 self._save_flag = 2
         else:
             raise ValueError("The word has been registered")
 
     def __getitem__(self, item):
```

