# Comparing `tmp/NDETCStemmer_kaenova-1.4.1.tar.gz` & `tmp/NDETCStemmer_kaenova-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NDETCStemmer_kaenova-1.4.1.tar", last modified: Thu May  4 06:53:45 2023, max compression
+gzip compressed data, was "NDETCStemmer_kaenova-1.4.2.tar", last modified: Thu May  4 07:03:16 2023, max compression
```

## Comparing `NDETCStemmer_kaenova-1.4.1.tar` & `NDETCStemmer_kaenova-1.4.2.tar`

### file list

```diff
@@ -1,73 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:45.034190 NDETCStemmer_kaenova-1.4.1/
--rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/LICENSE
--rw-rw-rw-   0        0        0       32 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:44.971191 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/
--rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/BestWordSelector.py
--rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/CandidateGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:44.975190 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/DictFile/
--rw-rw-rw-   0        0        0      962 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/DictFile/compound_word.txt
--rw-rw-rw-   0        0        0      927 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/DictFile/rare_word.txt
--rw-rw-rw-   0        0        0   267067 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/DictFile/root_word.txt
--rw-rw-rw-   0        0        0     7203 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/DictFile/stopword.txt
--rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/ListRules.py
--rw-rw-rw-   0        0        0     6293 2023-05-04 06:18:43.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/ModelDownloader.py
--rw-rw-rw-   0        0        0     2507 2023-05-04 05:41:32.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/NDETCStemmer.py
--rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/NDETCStemmerAbstract.py
--rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/RulesGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:44.978190 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/
--rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:44.982191 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/__pycache__/
--rw-rw-rw-   0        0        0      169 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2116 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/__pycache__/generator_initiator.cpython-310.pyc
--rw-rw-rw-   0        0        0      649 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/__pycache__/normalizer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/generator_initiator.py
--rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/normalizer.py
--rw-rw-rw-   0        0        0      226 2023-05-04 05:57:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:44.991189 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/
--rw-rw-rw-   0        0        0     3357 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/BestWordSelector.cpython-310.pyc
--rw-rw-rw-   0        0        0     7270 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/CandidateGenerator.cpython-310.pyc
--rw-rw-rw-   0        0        0     1605 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/ListRules.cpython-310.pyc
--rw-rw-rw-   0        0        0     5859 2023-05-04 06:18:45.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/ModelDownloader.cpython-310.pyc
--rw-rw-rw-   0        0        0     2517 2023-05-04 05:51:34.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/NDETCStemmer.cpython-310.pyc
--rw-rw-rw-   0        0        0     3216 2023-05-04 05:51:35.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/NDETCStemmerAbstract.cpython-310.pyc
--rw-rw-rw-   0        0        0     1553 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/RulesGenerator.cpython-310.pyc
--rw-rw-rw-   0        0        0      409 2023-05-04 05:57:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:45.004189 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/
--rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:45.020191 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/
--rw-rw-rw-   0        0        0      481 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      907 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/infixrule.cpython-310.pyc
--rw-rw-rw-   0        0        0      539 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/particlerule.cpython-310.pyc
--rw-rw-rw-   0        0        0      552 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/possessivepronounrule.cpython-310.pyc
--rw-rw-rw-   0        0        0     3177 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/prefix10rule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1918 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/prefix1rule.cpython-310.pyc
--rw-rw-rw-   0        0        0     3809 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/prefix20rule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1494 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/prefix39rule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1272 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/prefix6rule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1534 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/reduplicationrule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1082 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/simulfixrule.cpython-310.pyc
--rw-rw-rw-   0        0        0     1860 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/suffix2rule_v2.cpython-310.pyc
--rw-rw-rw-   0        0        0     1286 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/__pycache__/validsuffixprefix.cpython-310.pyc
--rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/infixrule.py
--rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/particlerule.py
--rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/possessivepronounrule.py
--rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix10rule.py
--rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix1rule.py
--rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix20rule.py
--rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix39rule.py
--rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix6rule.py
--rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/reduplicationrule.py
--rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/simulfixrule.py
--rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/suffix2rule_v2.py
--rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/validsuffixprefix.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:53:45.033191 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/
--rw-rw-rw-   0        0        0     6825 2023-05-04 06:53:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2831 2023-05-04 06:53:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 06:53:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 06:52:15.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-05-04 06:53:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 06:53:44.000000 NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6825 2023-05-04 06:53:45.034190 NDETCStemmer_kaenova-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6277 2023-05-04 06:20:47.000000 NDETCStemmer_kaenova-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 06:53:45.035191 NDETCStemmer_kaenova-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      915 2023-05-04 06:52:46.000000 NDETCStemmer_kaenova-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.275256 NDETCStemmer_kaenova-1.4.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6825 2023-05-04 07:03:16.274255 NDETCStemmer_kaenova-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6277 2023-05-04 06:20:47.000000 NDETCStemmer_kaenova-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:03:16.276255 NDETCStemmer_kaenova-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-05-04 07:03:04.000000 NDETCStemmer_kaenova-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.233257 NDETCStemmer_kaenova-1.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.247256 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/
+-rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/BestWordSelector.py
+-rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/CandidateGenerator.py
+-rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ListRules.py
+-rw-rw-rw-   0        0        0     6293 2023-05-04 06:18:43.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ModelDownloader.py
+-rw-rw-rw-   0        0        0     2507 2023-05-04 05:41:32.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmer.py
+-rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmerAbstract.py
+-rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/RulesGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.250257 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/__init__.py
+-rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/generator_initiator.py
+-rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/normalizer.py
+-rw-rw-rw-   0        0        0      226 2023-05-04 05:57:37.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.264256 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/
+-rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/__init__.py
+-rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/infixrule.py
+-rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/particlerule.py
+-rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/possessivepronounrule.py
+-rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix10rule.py
+-rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix1rule.py
+-rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix20rule.py
+-rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix39rule.py
+-rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix6rule.py
+-rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/reduplicationrule.py
+-rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/simulfixrule.py
+-rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/suffix2rule_v2.py
+-rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/validsuffixprefix.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.273257 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/
+-rw-rw-rw-   0        0        0     6825 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:01:37.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/top_level.txt
```

### Comparing `NDETCStemmer_kaenova-1.4.1/LICENSE` & `NDETCStemmer_kaenova-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/BestWordSelector.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/BestWordSelector.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/CandidateGenerator.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/CandidateGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/ListRules.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ListRules.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/ModelDownloader.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ModelDownloader.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/NDETCStemmer.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmer.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/NDETCStemmerAbstract.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmerAbstract.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/RulesGenerator.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/RulesGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/generator_initiator.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/generator_initiator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/Utility/normalizer.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/normalizer.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/infixrule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/infixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/particlerule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/particlerule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/possessivepronounrule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/possessivepronounrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix10rule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix10rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix1rule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix1rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix20rule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix20rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix39rule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix39rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/prefix6rule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix6rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/reduplicationrule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/reduplicationrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/simulfixrule.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/simulfixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/suffix2rule_v2.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/suffix2rule_v2.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer/morphology/validsuffixprefix.py` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/validsuffixprefix.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.1/NDETCStemmer_kaenova.egg-info/PKG-INFO` & `NDETCStemmer_kaenova-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: NDETCStemmer-kaenova
-Version: 1.4.1
+Name: NDETCStemmer_kaenova
+Version: 1.4.2
 Summary: Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context
 Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.4.2 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
 LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
```

### Comparing `NDETCStemmer_kaenova-1.4.1/PKG-INFO` & `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: NDETCStemmer_kaenova
-Version: 1.4.1
+Name: NDETCStemmer-kaenova
+Version: 1.4.2
 Summary: Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context
 Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.4.2 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
 LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
```

### Comparing `NDETCStemmer_kaenova-1.4.1/README.md` & `NDETCStemmer_kaenova-1.4.2/README.md`

 * *Files identical despite different names*

