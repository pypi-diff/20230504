# Comparing `tmp/japyconjugator-1.0.2.tar.gz` & `tmp/japyconjugator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japyconjugator-1.0.2.tar", last modified: Mon Apr 17 13:16:48 2023, max compression
+gzip compressed data, was "japyconjugator-1.1.0.tar", last modified: Thu May  4 06:59:29 2023, max compression
```

## Comparing `japyconjugator-1.0.2.tar` & `japyconjugator-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1166 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/README.md
--rw-rw-rw-   0        0        0      547 2023-04-17 13:16:33.000000 japyconjugator-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.822004 japyconjugator-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator/
--rw-rw-rw-   0        0        0        0 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator/adjectives/
--rw-rw-rw-   0        0        0       24 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/__init__.py
--rw-rw-rw-   0        0        0      625 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugate.py
--rw-rw-rw-   0        0        0      911 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugation_helpers.py
--rw-rw-rw-   0        0        0     1239 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/conjugators.py
--rw-rw-rw-   0        0        0      241 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/adjectives/defs.py
--rw-rw-rw-   0        0        0      103 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/defs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.853253 japyconjugator-1.0.2/src/japyconjugator/verbs/
--rw-rw-rw-   0        0        0       24 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/__init__.py
--rw-rw-rw-   0        0        0      635 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugate.py
--rw-rw-rw-   0        0        0     2677 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugation_helpers.py
--rw-rw-rw-   0        0        0     1607 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/conjugators.py
--rw-rw-rw-   0        0        0      233 2023-04-17 13:14:24.000000 japyconjugator-1.0.2/src/japyconjugator/verbs/defs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:16:48.837629 japyconjugator-1.0.2/src/japyconjugator.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 13:16:48.000000 japyconjugator-1.0.2/src/japyconjugator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.774403 japyconjugator-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-17 13:14:24.000000 japyconjugator-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1166 2023-05-04 06:59:29.774403 japyconjugator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-04-17 13:14:24.000000 japyconjugator-1.1.0/README.md
+-rw-rw-rw-   0        0        0      547 2023-05-04 06:58:39.000000 japyconjugator-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 06:59:29.774403 japyconjugator-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.750402 japyconjugator-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.754405 japyconjugator-1.1.0/src/japyconjugator/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:53:53.000000 japyconjugator-1.1.0/src/japyconjugator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.770402 japyconjugator-1.1.0/src/japyconjugator/adjectives/
+-rw-rw-rw-   0        0        0       26 2023-05-04 06:49:07.000000 japyconjugator-1.1.0/src/japyconjugator/adjectives/__init__.py
+-rw-rw-rw-   0        0        0      440 2023-04-18 15:58:15.000000 japyconjugator-1.1.0/src/japyconjugator/adjectives/conjugation_helpers.py
+-rw-rw-rw-   0        0        0     1660 2023-05-04 06:56:02.000000 japyconjugator-1.1.0/src/japyconjugator/adjectives/conjugators.py
+-rw-rw-rw-   0        0        0       74 2023-04-18 15:57:22.000000 japyconjugator-1.1.0/src/japyconjugator/adjectives/defs.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.770402 japyconjugator-1.1.0/src/japyconjugator/verbs/
+-rw-rw-rw-   0        0        0       26 2023-05-04 06:49:00.000000 japyconjugator-1.1.0/src/japyconjugator/verbs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 06:52:54.000000 japyconjugator-1.1.0/src/japyconjugator/verbs/conjugation_helpers.py
+-rw-rw-rw-   0        0        0     1889 2023-05-04 06:43:53.000000 japyconjugator-1.1.0/src/japyconjugator/verbs/conjugators.py
+-rw-rw-rw-   0        0        0       87 2023-04-18 15:56:55.000000 japyconjugator-1.1.0/src/japyconjugator/verbs/defs.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:59:29.766402 japyconjugator-1.1.0/src/japyconjugator.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-05-04 06:59:29.000000 japyconjugator-1.1.0/src/japyconjugator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-05-04 06:59:29.000000 japyconjugator-1.1.0/src/japyconjugator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 06:59:29.000000 japyconjugator-1.1.0/src/japyconjugator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 06:59:29.000000 japyconjugator-1.1.0/src/japyconjugator.egg-info/top_level.txt
```

### Comparing `japyconjugator-1.0.2/LICENSE` & `japyconjugator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.2/PKG-INFO` & `japyconjugator-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japyconjugator
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python package for conjugating verbs in the Japanese language.
 Author: Simone Bondi
 Project-URL: Repository, https://github.com/Shibodd/japyconjugator
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `japyconjugator-1.0.2/README.md` & `japyconjugator-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `japyconjugator-1.0.2/pyproject.toml` & `japyconjugator-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "japyconjugator"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
     { name = "Simone Bondi" },
 ]
 description = "A python package for conjugating verbs in the Japanese language."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `japyconjugator-1.0.2/src/japyconjugator.egg-info/PKG-INFO` & `japyconjugator-1.1.0/src/japyconjugator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japyconjugator
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python package for conjugating verbs in the Japanese language.
 Author: Simone Bondi
 Project-URL: Repository, https://github.com/Shibodd/japyconjugator
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `japyconjugator-1.0.2/src/japyconjugator.egg-info/SOURCES.txt` & `japyconjugator-1.1.0/src/japyconjugator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 src/japyconjugator/__init__.py
-src/japyconjugator/defs.py
 src/japyconjugator.egg-info/PKG-INFO
 src/japyconjugator.egg-info/SOURCES.txt
 src/japyconjugator.egg-info/dependency_links.txt
 src/japyconjugator.egg-info/top_level.txt
 src/japyconjugator/adjectives/__init__.py
-src/japyconjugator/adjectives/conjugate.py
 src/japyconjugator/adjectives/conjugation_helpers.py
 src/japyconjugator/adjectives/conjugators.py
 src/japyconjugator/adjectives/defs.py
 src/japyconjugator/verbs/__init__.py
-src/japyconjugator/verbs/conjugate.py
 src/japyconjugator/verbs/conjugation_helpers.py
 src/japyconjugator/verbs/conjugators.py
 src/japyconjugator/verbs/defs.py
```

