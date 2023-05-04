# Comparing `tmp/NDETCStemmer_kaenova-1.4.2.tar.gz` & `tmp/NDETCStemmer_kaenova-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NDETCStemmer_kaenova-1.4.2.tar", last modified: Thu May  4 07:03:16 2023, max compression
+gzip compressed data, was "NDETCStemmer_kaenova-1.4.3.tar", last modified: Thu May  4 08:20:18 2023, max compression
```

## Comparing `NDETCStemmer_kaenova-1.4.2.tar` & `NDETCStemmer_kaenova-1.4.3.tar`

### file list

```diff
@@ -1,42 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.275256 NDETCStemmer_kaenova-1.4.2/
--rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/LICENSE
--rw-rw-rw-   0        0        0       32 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6825 2023-05-04 07:03:16.274255 NDETCStemmer_kaenova-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6277 2023-05-04 06:20:47.000000 NDETCStemmer_kaenova-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 07:03:16.276255 NDETCStemmer_kaenova-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-05-04 07:03:04.000000 NDETCStemmer_kaenova-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.233257 NDETCStemmer_kaenova-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.247256 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/
--rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/BestWordSelector.py
--rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/CandidateGenerator.py
--rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ListRules.py
--rw-rw-rw-   0        0        0     6293 2023-05-04 06:18:43.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ModelDownloader.py
--rw-rw-rw-   0        0        0     2507 2023-05-04 05:41:32.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmer.py
--rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmerAbstract.py
--rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/RulesGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.250257 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/
--rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/__init__.py
--rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/generator_initiator.py
--rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/normalizer.py
--rw-rw-rw-   0        0        0      226 2023-05-04 05:57:37.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.264256 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/
--rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/__init__.py
--rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/infixrule.py
--rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/particlerule.py
--rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/possessivepronounrule.py
--rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix10rule.py
--rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix1rule.py
--rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix20rule.py
--rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix39rule.py
--rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix6rule.py
--rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/reduplicationrule.py
--rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/simulfixrule.py
--rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/suffix2rule_v2.py
--rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/validsuffixprefix.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:16.273257 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/
--rw-rw-rw-   0        0        0     6825 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 07:01:37.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 07:03:16.000000 NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:18.002522 NDETCStemmer_kaenova-1.4.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-05-04 08:16:55.000000 NDETCStemmer_kaenova-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6825 2023-05-04 08:20:18.001522 NDETCStemmer_kaenova-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6277 2023-05-04 06:20:47.000000 NDETCStemmer_kaenova-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 08:20:18.003523 NDETCStemmer_kaenova-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-05-04 08:20:06.000000 NDETCStemmer_kaenova-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.923525 NDETCStemmer_kaenova-1.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.936525 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/
+-rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/BestWordSelector.py
+-rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/CandidateGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.942524 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/
+-rw-rw-rw-   0        0        0        0 2023-05-04 08:15:57.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/compound_word.txt
+-rw-rw-rw-   0        0        0      927 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/rare_word.txt
+-rw-rw-rw-   0        0        0   267067 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/root_word.txt
+-rw-rw-rw-   0        0        0     7203 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/DictFile/stopword.txt
+-rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/ListRules.py
+-rw-rw-rw-   0        0        0     6293 2023-05-04 08:18:20.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/ModelDownloader.py
+-rw-rw-rw-   0        0        0     3072 2023-05-04 08:17:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/NDETCStemmer.py
+-rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/NDETCStemmerAbstract.py
+-rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/RulesGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.944524 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.948523 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/__pycache__/
+-rw-rw-rw-   0        0        0      169 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2116 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/__pycache__/generator_initiator.cpython-310.pyc
+-rw-rw-rw-   0        0        0      649 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/__pycache__/normalizer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/generator_initiator.py
+-rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/normalizer.py
+-rw-rw-rw-   0        0        0      226 2023-05-04 05:57:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.959523 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/
+-rw-rw-rw-   0        0        0     3357 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/BestWordSelector.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7270 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/CandidateGenerator.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1605 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/ListRules.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5859 2023-05-04 06:18:45.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/ModelDownloader.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2517 2023-05-04 05:51:34.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/NDETCStemmer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3216 2023-05-04 05:51:35.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/NDETCStemmerAbstract.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1553 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/RulesGenerator.cpython-310.pyc
+-rw-rw-rw-   0        0        0      409 2023-05-04 05:57:44.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.972524 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/
+-rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:17.987523 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/
+-rw-rw-rw-   0        0        0      481 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      907 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/infixrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0      539 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/particlerule.cpython-310.pyc
+-rw-rw-rw-   0        0        0      552 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/possessivepronounrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3177 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/prefix10rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1918 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/prefix1rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3809 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/prefix20rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1494 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/prefix39rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1272 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/prefix6rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1534 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/reduplicationrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1082 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/simulfixrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1860 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/suffix2rule_v2.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1286 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/__pycache__/validsuffixprefix.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/infixrule.py
+-rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/particlerule.py
+-rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/possessivepronounrule.py
+-rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix10rule.py
+-rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix1rule.py
+-rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix20rule.py
+-rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix39rule.py
+-rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix6rule.py
+-rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/reduplicationrule.py
+-rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/simulfixrule.py
+-rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/suffix2rule_v2.py
+-rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/validsuffixprefix.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:20:18.001522 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/
+-rw-rw-rw-   0        0        0     6825 2023-05-04 08:20:17.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3101 2023-05-04 08:20:17.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 08:20:17.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:01:37.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-05-04 08:20:17.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 08:20:17.000000 NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/top_level.txt
```

### Comparing `NDETCStemmer_kaenova-1.4.2/LICENSE` & `NDETCStemmer_kaenova-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/PKG-INFO` & `NDETCStemmer_kaenova-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NDETCStemmer_kaenova
-Version: 1.4.2
+Version: 1.4.3
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
-Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.4.2 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.4.3 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
 LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
```

### Comparing `NDETCStemmer_kaenova-1.4.2/README.md` & `NDETCStemmer_kaenova-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/setup.py` & `NDETCStemmer_kaenova-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="NDETCStemmer_kaenova",
-    version="1.4.2",
+    version="1.4.3",
     py_modules=["NDETCStemmer"],
     description="Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaenova/NDETCStemmer",
     include_package_data=True,
     zip_safe=False,
```

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/BestWordSelector.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/BestWordSelector.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/CandidateGenerator.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/CandidateGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ListRules.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/ListRules.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/ModelDownloader.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/ModelDownloader.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmer.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/NDETCStemmer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,81 @@
-
 from .NDETCStemmerAbstract import NDETCStemmerAbstract
 from .Utility import normalizer
 from .BestWordSelector import BestWordSelector
-from .CandidateGenerator import CandidateGenerator 
+from .CandidateGenerator import CandidateGenerator
 from .ModelDownloader import ModelDownloaderAbstract, HuggingfaceModelDownloader
 from typing import Optional
 import os
 
-class NDETCStemmer(NDETCStemmerAbstract):
-	def __init__(self,weight=1, left_context=1, right_context=1, parent=True, downloader: Optional[ModelDownloaderAbstract] = HuggingfaceModelDownloader()):
-		"""
-		# weight               weight similarity  
-		# left_context          maximum left context to eval
-		# right_context         maximum right context to eval
-		# parent=True/False     True means that parent of ambiguous word include in the evaluation, otherwise excluding
-		"""
-		self._model=None
-		self._root_word_file=None
-		self._rare_word_file=None
-		self._compound_word_file=None
-		self._stopword_file=None
-		self._weight=weight
-		self._left_context=left_context
-		self._right_context=right_context
-		self._parent=parent
-		
-		model_path = downloader.download_model()
-		self.path=os.path.dirname(__file__) 
-		self.model=model_path.w2vec_wiki_id_case
-		self.rootWord=os.path.join(self.path,'DictFile','root_word.txt')
-		self.rareWord=os.path.join(self.path,'DictFile','rare_word.txt')
-		self.compoundWord=os.path.join(self.path,'DictFile','compound_word.txt')
-		self.stopWord=os.path.join(self.path,'DictFile','stopword.txt')
-
-
 
-	def stem(self,stemmer_input,from_file=False,stopword=False,):
-		"""
-		# stemmer_input         input string
-		# from_file=True/False  True means that input word will be read from file, otherwise input word will be string
-		# stopword=True/False  True means that input word will be remove words which exist in the list of stop word
-		"""
-		stemmer_input=normalizer.normalize(stemmer_input,from_file=from_file,stopword=stopword,stopword_file=self._stopword_file)
-		word_candidate=CandidateGenerator(stemmer_input).generate()
-		selector=BestWordSelector(stemmer_input=stemmer_input,model=self._model,root_word=self.rootWord,rare_word=self.rareWord,compound_word=self.compoundWord,weight=self._weight,left_context=self._left_context,right_context=self._right_context,parent=self._parent)
-		best_word=selector.select(word_candidate)
-
-		# # for test only 
-		# return best_word
-
-		output = ''
-		for candidate_keys in range(len(best_word)):
-			output += best_word[candidate_keys][0] + ' '
-
-		return output
-
-		
-
-		
+class NDETCStemmer(NDETCStemmerAbstract):
+    def __init__(
+        self,
+        weight=1,
+        left_context=1,
+        right_context=1,
+        parent=True,
+        downloader: Optional[ModelDownloaderAbstract] = HuggingfaceModelDownloader(),
+    ):
+        """
+        # weight               weight similarity
+        # left_context          maximum left context to eval
+        # right_context         maximum right context to eval
+        # parent=True/False     True means that parent of ambiguous word include in the evaluation, otherwise excluding
+        """
+        self._model = None
+        self._root_word_file = None
+        self._rare_word_file = None
+        self._compound_word_file = None
+        self._stopword_file = None
+        self._weight = weight
+        self._left_context = left_context
+        self._right_context = right_context
+        self._parent = parent
+
+        model_path = downloader.download_model()
+        self.path = os.path.dirname(__file__)
+        self.model = model_path.w2vec_wiki_id_case
+        self.rootWord = os.path.join(self.path, "DictFile", "root_word.txt")
+        self.rareWord = os.path.join(self.path, "DictFile", "rare_word.txt")
+        self.compoundWord = os.path.join(self.path, "DictFile", "compound_word.txt")
+        self.stopWord = os.path.join(self.path, "DictFile", "stopword.txt")
+
+    def stem(
+        self,
+        stemmer_input,
+        from_file=False,
+        stopword=False,
+    ):
+        """
+        # stemmer_input         input string
+        # from_file=True/False  True means that input word will be read from file, otherwise input word will be string
+        # stopword=True/False  True means that input word will be remove words which exist in the list of stop word
+        """
+        stemmer_input = normalizer.normalize(
+            stemmer_input,
+            from_file=from_file,
+            stopword=stopword,
+            stopword_file=self._stopword_file,
+        )
+        word_candidate = CandidateGenerator(stemmer_input).generate()
+        selector = BestWordSelector(
+            stemmer_input=stemmer_input,
+            model=self._model,
+            root_word=self.rootWord,
+            rare_word=self.rareWord,
+            compound_word=self.compoundWord,
+            weight=self._weight,
+            left_context=self._left_context,
+            right_context=self._right_context,
+            parent=self._parent,
+        )
+        best_word = selector.select(word_candidate)
+
+        # # for test only
+        # return best_word
+
+        output = ""
+        for candidate_keys in range(len(best_word)):
+            output += best_word[candidate_keys][0] + " "
 
+        return output
```

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/NDETCStemmerAbstract.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/NDETCStemmerAbstract.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/RulesGenerator.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/RulesGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/generator_initiator.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/generator_initiator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/Utility/normalizer.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/Utility/normalizer.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/infixrule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/infixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/particlerule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/particlerule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/possessivepronounrule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/possessivepronounrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix10rule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix10rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix1rule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix1rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix20rule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix20rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix39rule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix39rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/prefix6rule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/prefix6rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/reduplicationrule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/reduplicationrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/simulfixrule.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/simulfixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/suffix2rule_v2.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/suffix2rule_v2.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer/morphology/validsuffixprefix.py` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer/morphology/validsuffixprefix.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.4.2/src/NDETCStemmer_kaenova.egg-info/PKG-INFO` & `NDETCStemmer_kaenova-1.4.3/src/NDETCStemmer_kaenova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NDETCStemmer-kaenova
-Version: 1.4.2
+Version: 1.4.3
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
-Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.4.2 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.4.3 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
 LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
```

