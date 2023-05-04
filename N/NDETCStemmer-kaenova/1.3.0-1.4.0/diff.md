# Comparing `tmp/NDETCStemmer_kaenova-1.3.0.tar.gz` & `tmp/NDETCStemmer_kaenova-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NDETCStemmer_kaenova-1.3.0.tar", last modified: Tue May  2 11:38:21 2023, max compression
+gzip compressed data, was "NDETCStemmer_kaenova-1.4.0.tar", last modified: Thu May  4 06:29:56 2023, max compression
```

## Comparing `NDETCStemmer_kaenova-1.3.0.tar` & `NDETCStemmer_kaenova-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.854830 NDETCStemmer_kaenova-1.3.0/
--rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/LICENSE
--rw-rw-rw-   0        0        0       32 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.796830 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/
--rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/BestWordSelector.py
--rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/CandidateGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.801829 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/
--rw-rw-rw-   0        0        0      962 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/compound_word.txt
--rw-rw-rw-   0        0        0      927 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/rare_word.txt
--rw-rw-rw-   0        0        0   267067 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/root_word.txt
--rw-rw-rw-   0        0        0     7203 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/stopword.txt
--rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/ListRules.py
--rw-rw-rw-   0        0        0     3833 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/ModelDownloader.py
--rw-rw-rw-   0        0        0     2681 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/NDETCStemmer.py
--rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/NDETCStemmerAbstract.py
--rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/RulesGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.806831 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/
--rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/__init__.py
--rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/generator_initiator.py
--rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/normalizer.py
--rw-rw-rw-   0        0        0      116 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.824830 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/
--rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/__init__.py
--rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/infixrule.py
--rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/particlerule.py
--rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/possessivepronounrule.py
--rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix10rule.py
--rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix1rule.py
--rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix20rule.py
--rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix39rule.py
--rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix6rule.py
--rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/reduplicationrule.py
--rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/simulfixrule.py
--rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/suffix2rule_v2.py
--rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/validsuffixprefix.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:38:21.852831 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/
--rw-rw-rw-   0        0        0     7504 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1339 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 11:38:21.000000 NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7504 2023-05-02 11:38:21.854830 NDETCStemmer_kaenova-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6956 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 11:38:21.854830 NDETCStemmer_kaenova-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-02 11:37:31.000000 NDETCStemmer_kaenova-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.212973 NDETCStemmer_kaenova-1.4.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.115974 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/
+-rw-rw-rw-   0        0        0     4608 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/BestWordSelector.py
+-rw-rw-rw-   0        0        0    17347 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/CandidateGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.119975 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/
+-rw-rw-rw-   0        0        0      962 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/compound_word.txt
+-rw-rw-rw-   0        0        0      927 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/rare_word.txt
+-rw-rw-rw-   0        0        0   267067 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/root_word.txt
+-rw-rw-rw-   0        0        0     7203 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/stopword.txt
+-rw-rw-rw-   0        0        0     1030 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/ListRules.py
+-rw-rw-rw-   0        0        0     6293 2023-05-04 06:18:43.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/ModelDownloader.py
+-rw-rw-rw-   0        0        0     2507 2023-05-04 05:41:32.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/NDETCStemmer.py
+-rw-rw-rw-   0        0        0     1517 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/NDETCStemmerAbstract.py
+-rw-rw-rw-   0        0        0      764 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/RulesGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.122973 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.125974 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/__pycache__/
+-rw-rw-rw-   0        0        0      169 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2116 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/__pycache__/generator_initiator.cpython-310.pyc
+-rw-rw-rw-   0        0        0      649 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/__pycache__/normalizer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1974 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/generator_initiator.py
+-rw-rw-rw-   0        0        0      516 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/normalizer.py
+-rw-rw-rw-   0        0        0      226 2023-05-04 05:57:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.135974 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/
+-rw-rw-rw-   0        0        0     3357 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/BestWordSelector.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7270 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/CandidateGenerator.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1605 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/ListRules.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5859 2023-05-04 06:18:45.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/ModelDownloader.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2517 2023-05-04 05:51:34.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/NDETCStemmer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3216 2023-05-04 05:51:35.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/NDETCStemmerAbstract.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1553 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/RulesGenerator.cpython-310.pyc
+-rw-rw-rw-   0        0        0      409 2023-05-04 05:57:44.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.150977 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/
+-rw-rw-rw-   0        0        0      364 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.165973 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/
+-rw-rw-rw-   0        0        0      481 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      907 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/infixrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0      539 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/particlerule.cpython-310.pyc
+-rw-rw-rw-   0        0        0      552 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/possessivepronounrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3177 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/prefix10rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1918 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/prefix1rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3809 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/prefix20rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1494 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/prefix39rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1272 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/prefix6rule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1534 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/reduplicationrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1082 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/simulfixrule.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1860 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/suffix2rule_v2.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1286 2023-05-04 05:51:37.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/__pycache__/validsuffixprefix.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4769 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/infixrule.py
+-rw-rw-rw-   0        0        0      913 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/particlerule.py
+-rw-rw-rw-   0        0        0      840 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/possessivepronounrule.py
+-rw-rw-rw-   0        0        0    11618 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix10rule.py
+-rw-rw-rw-   0        0        0     5080 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix1rule.py
+-rw-rw-rw-   0        0        0    14238 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix20rule.py
+-rw-rw-rw-   0        0        0     3108 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix39rule.py
+-rw-rw-rw-   0        0        0     3135 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix6rule.py
+-rw-rw-rw-   0        0        0     4023 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/reduplicationrule.py
+-rw-rw-rw-   0        0        0     3292 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/simulfixrule.py
+-rw-rw-rw-   0        0        0     4850 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/suffix2rule_v2.py
+-rw-rw-rw-   0        0        0     2381 2023-05-02 11:36:00.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/validsuffixprefix.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:29:56.211972 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/
+-rw-rw-rw-   0        0        0     6825 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2831 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 06:29:56.000000 NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6825 2023-05-04 06:29:56.212973 NDETCStemmer_kaenova-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6277 2023-05-04 06:20:47.000000 NDETCStemmer_kaenova-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 06:29:56.212973 NDETCStemmer_kaenova-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      915 2023-05-04 05:55:48.000000 NDETCStemmer_kaenova-1.4.0/setup.py
```

### Comparing `NDETCStemmer_kaenova-1.3.0/LICENSE` & `NDETCStemmer_kaenova-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/BestWordSelector.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/BestWordSelector.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/CandidateGenerator.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/CandidateGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/compound_word.txt` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/compound_word.txt`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/rare_word.txt` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/rare_word.txt`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/root_word.txt` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/root_word.txt`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/DictFile/stopword.txt` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/DictFile/stopword.txt`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/ListRules.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/ListRules.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/NDETCStemmer.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/NDETCStemmer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
-from NDETCStemmer.NDETCStemmerAbstract import NDETCStemmerAbstract
-from NDETCStemmer.Utility import normalizer
-from NDETCStemmer.BestWordSelector import BestWordSelector
-from NDETCStemmer.CandidateGenerator import CandidateGenerator 
-from NDETCStemmer.ModelDownloader import ModelDownloader
-from NDETCStemmer.ModelDownloader import CustomModelDownloader
+from .NDETCStemmerAbstract import NDETCStemmerAbstract
+from .Utility import normalizer
+from .BestWordSelector import BestWordSelector
+from .CandidateGenerator import CandidateGenerator 
+from .ModelDownloader import ModelDownloaderAbstract, HuggingfaceModelDownloader
 from typing import Optional
 import os
 
 class NDETCStemmer(NDETCStemmerAbstract):
-	def __init__(self,weight=1, left_context=1, right_context=1, parent=True, custom_downloader: Optional[CustomModelDownloader] = None):
+	def __init__(self,weight=1, left_context=1, right_context=1, parent=True, downloader: Optional[ModelDownloaderAbstract] = HuggingfaceModelDownloader()):
 		"""
 		# weight               weight similarity  
 		# left_context          maximum left context to eval
 		# right_context         maximum right context to eval
 		# parent=True/False     True means that parent of ambiguous word include in the evaluation, otherwise excluding
 		"""
 		self._model=None
@@ -22,20 +21,17 @@
 		self._compound_word_file=None
 		self._stopword_file=None
 		self._weight=weight
 		self._left_context=left_context
 		self._right_context=right_context
 		self._parent=parent
 		
-		downloader = ModelDownloader()
-		if custom_downloader is not None:
-			downloader = custom_downloader
-		downloader.run()
+		model_path = downloader.download_model()
 		self.path=os.path.dirname(__file__) 
-		self.model=os.path.join(self.path,'Model','w2vec_wiki_id_case')
+		self.model=model_path.w2vec_wiki_id_case
 		self.rootWord=os.path.join(self.path,'DictFile','root_word.txt')
 		self.rareWord=os.path.join(self.path,'DictFile','rare_word.txt')
 		self.compoundWord=os.path.join(self.path,'DictFile','compound_word.txt')
 		self.stopWord=os.path.join(self.path,'DictFile','stopword.txt')
```

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/NDETCStemmerAbstract.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/NDETCStemmerAbstract.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/RulesGenerator.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/RulesGenerator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/generator_initiator.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/generator_initiator.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/Utility/normalizer.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/Utility/normalizer.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/infixrule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/infixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/particlerule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/particlerule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/possessivepronounrule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/possessivepronounrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix10rule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix10rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix1rule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix1rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix20rule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix20rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix39rule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix39rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/prefix6rule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/prefix6rule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/reduplicationrule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/reduplicationrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/simulfixrule.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/simulfixrule.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/suffix2rule_v2.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/suffix2rule_v2.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer/morphology/validsuffixprefix.py` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer/morphology/validsuffixprefix.py`

 * *Files identical despite different names*

### Comparing `NDETCStemmer_kaenova-1.3.0/NDETCStemmer_kaenova.egg-info/PKG-INFO` & `NDETCStemmer_kaenova-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
-Name: NDETCStemmer-kaenova
-Version: 1.3.0
+Name: NDETCStemmer_kaenova
+Version: 1.4.0
 Summary: Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context
 Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nondeterministic Context (NDETC) Stemmer
 
+**This is Kaenova's maintained NDETCStemmer, a fork from the [original](https://github.com/alifadwitiyap/NDETCStemmer). I upload the model to Huggingface for model reliability.**
+
 Nondeterministic Context (NDETC) Stemmer adalah library yang mengimplementasikan metode stemming nondeterministic berbasis context untuk memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam bahasa Indonesia.
 
 ## Installation
 Untuk menginstall library ini diperlukan pip python yang dapat anda download dengan mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
 Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
 ```bash
-pip install git+https://github.com/kaenova/NDETCStemmer.git@master
+pip install NDETCStemmer-kaenova
 ```
     
 ## Usage
 Setelah menginstall library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python
 #import NDETCStemmer library
 from NDETCStemmer import NDETCStemmer
@@ -37,34 +39,14 @@
 print(output)
 #boleh saya perah lembu ini
 
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
 #bibir merah tangan jadi lengket madu
 
 ```
-Untuk menggunakan alamat download model dari luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti di bawah:
-```python
-from NDETCStemmer import NDETCStemmer, CustomModelDownloader
-
-downloader = CustomModelDownloader(
-    model_1="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-    model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.trainables.syn1neg.npy",
-    model_3="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy"
-)
-
-stemmer=NDETCStemmer(custom_downloader=downloader)
-
-# stemming process
-output=stemmer.stem('boleh saya memerah lembu ini')
-
-print(output)
-#boleh saya perah lembu ini
-
-print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
-```
 
 
 ## Cititation
 ```
 @INPROCEEDINGS{9617514,
   author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
   booktitle={2021 International Conference on Data Science and Its Applications (ICoDSA)},
```

#### html2text {}

```diff
@@ -1,62 +1,53 @@
-Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.4.0 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
-LICENSE # Nondeterministic Context (NDETC) Stemmer Nondeterministic Context
-(NDETC) Stemmer adalah library yang mengimplementasikan metode stemming
-nondeterministic berbasis context untuk memecahkan permasalahan kata-kata
-ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam
-bahasa Indonesia. ## Installation Untuk menginstall library ini diperlukan pip
-python yang dapat anda download dengan mengikuti link [berikut](https://
-pip.pypa.io/en/stable/installation/#). Kemudian anda dapat menjalankan kode
-berikut pada terminal yang anda gunakan ```bash pip install git+https://
-github.com/kaenova/NDETCStemmer.git@master ``` ## Usage Setelah menginstall
+LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
+maintained NDETCStemmer, a fork from the [original](https://github.com/
+alifadwitiyap/NDETCStemmer). I upload the model to Huggingface for model
+reliability.** Nondeterministic Context (NDETC) Stemmer adalah library yang
+mengimplementasikan metode stemming nondeterministic berbasis context untuk
+memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis
+pada proses stemming kata dalam bahasa Indonesia. ## Installation Untuk
+menginstall library ini diperlukan pip python yang dapat anda download dengan
+mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
+Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
+```bash pip install NDETCStemmer-kaenova ``` ## Usage Setelah menginstall
 library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder
 yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file
 NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python #import NDETCStemmer library from NDETCStemmer import NDETCStemmer
 #init stemmer stemmer=NDETCStemmer() # stemming process output=stemmer.stem
 ('boleh saya memerah lembu ini') print(output) #boleh saya perah lembu ini
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu')) #bibir
-merah tangan jadi lengket madu ``` Untuk menggunakan alamat download model dari
-luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti
-di bawah: ```python from NDETCStemmer import NDETCStemmer,
-CustomModelDownloader downloader = CustomModelDownloader( model_1="https://
-is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/
-w2vec_wiki_id_case.trainables.syn1neg.npy", model_3="https://is3.cloudhost.id/
-s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy" )
-stemmer=NDETCStemmer(custom_downloader=downloader) # stemming process
-output=stemmer.stem('boleh saya memerah lembu ini') print(output) #boleh saya
-perah lembu ini print(stemmer.stem('bibirnya memerah tangannya jadi selengket
-madu')) ``` ## Cititation ``` @INPROCEEDINGS{9617514, author={Bunyamin and
-Huda, Arief Fatchul and Suryani, Arie Ardiyanti}, booktitle={2021 International
-Conference on Data Science and Its Applications (ICoDSA)}, title={Indonesian
-Stemmer for Ambiguous Word based on Context}, year={2021}, volume={}, number=
-{}, pages={1-9}, doi={10.1109/ICoDSA53588.2021.9617514}} ``` ## Tentang
-Nondeterministic Context Stemmer Merupakan stemmer yang dikembangkan oleh
-Bunyamin_et_al. yang merupakan penelitian lanjutan dari pendekatan
-nondeterministic yang diusulkan oleh Purwarianti. Dalam penelitian Purwarianti,
-setiap kata tidak diperiksa menurut urutan aturan morfologi, tetapi diperiksa
-menggunakan semua aturan. Kemudian, hasilnya disimpan satu per satu dalam
-daftar kandidat kata. Kata akhir akan dipilih menggunakan beberapa aturan
-heuristik, yaitu ketersediaan kosakata dari kata dasar khusus dan panjang kata.
-Masalah yang dihadapi oleh metode nondeterministic yang dikembangkan
-Purwarianti ini dan stemmer deterministic (Andiani_et_al.) adalah masalah
-ambiguitas kata yang dihasilkan oleh stemmer. Misalkan kata "memalukan"
-mempunyai 2 kata dasar, yaitu âmaluâ dan âpaluâ , tergantung
-konteksnya. Pada pernyataan-pernyataan berikut âdia tidak ingin memalukan
-keluarganyaâ dan âtukang memalukan paku di tembokâ kata ambigu
-"memalukan" akan menghasilkan kata dasar "malu" secara terus-menerus.
-Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat pertama
-dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
+merah tangan jadi lengket madu ``` ## Cititation ``` @INPROCEEDINGS{9617514,
+author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
+booktitle={2021 International Conference on Data Science and Its Applications
+(ICoDSA)}, title={Indonesian Stemmer for Ambiguous Word based on Context},
+year={2021}, volume={}, number={}, pages={1-9}, doi={10.1109/
+ICoDSA53588.2021.9617514}} ``` ## Tentang Nondeterministic Context Stemmer
+Merupakan stemmer yang dikembangkan oleh Bunyamin_et_al. yang merupakan
+penelitian lanjutan dari pendekatan nondeterministic yang diusulkan oleh
+Purwarianti. Dalam penelitian Purwarianti, setiap kata tidak diperiksa menurut
+urutan aturan morfologi, tetapi diperiksa menggunakan semua aturan. Kemudian,
+hasilnya disimpan satu per satu dalam daftar kandidat kata. Kata akhir akan
+dipilih menggunakan beberapa aturan heuristik, yaitu ketersediaan kosakata dari
+kata dasar khusus dan panjang kata.  Masalah yang dihadapi oleh metode
+nondeterministic yang dikembangkan Purwarianti ini dan stemmer deterministic
+(Andiani_et_al.) adalah masalah ambiguitas kata yang dihasilkan oleh stemmer.
+Misalkan kata "memalukan" mempunyai 2 kata dasar, yaitu âmaluâ dan
+âpaluâ , tergantung konteksnya. Pada pernyataan-pernyataan berikut âdia
+tidak ingin memalukan keluarganyaâ dan âtukang memalukan paku di tembokâ
+kata ambigu "memalukan" akan menghasilkan kata dasar "malu" secara terus-
+menerus. Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat
+pertama dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
 menghasilkan beberapa alternatif kandidat kata dari kata-kata ambigu tersebut,
 tetapi memiliki kelemahan dalam memilih hasil yang tepat, karena ketiadaan
 konteks. Nondeterministic Context Stemmer memperbaiki pendekatan
 nondeterministik itu dengan menambahkan konteks dalam pemilihan kata terbaik.
 Dalam menyelesaikan masalah pemilihan kata terbaik untuk setiap masukan kata
 ambigu, diusulkan penggunaan model word2vec. Dengan cara ini stemmer akan lebih
 akurat dalam melakukan stemming dibandingkan dengan cara-cara sebelumnya. ####
```

### Comparing `NDETCStemmer_kaenova-1.3.0/PKG-INFO` & `NDETCStemmer_kaenova-1.4.0/NDETCStemmer_kaenova.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
-Name: NDETCStemmer_kaenova
-Version: 1.3.0
+Name: NDETCStemmer-kaenova
+Version: 1.4.0
 Summary: Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context
 Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nondeterministic Context (NDETC) Stemmer
 
+**This is Kaenova's maintained NDETCStemmer, a fork from the [original](https://github.com/alifadwitiyap/NDETCStemmer). I upload the model to Huggingface for model reliability.**
+
 Nondeterministic Context (NDETC) Stemmer adalah library yang mengimplementasikan metode stemming nondeterministic berbasis context untuk memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam bahasa Indonesia.
 
 ## Installation
 Untuk menginstall library ini diperlukan pip python yang dapat anda download dengan mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
 Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
 ```bash
-pip install git+https://github.com/kaenova/NDETCStemmer.git@master
+pip install NDETCStemmer-kaenova
 ```
     
 ## Usage
 Setelah menginstall library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python
 #import NDETCStemmer library
 from NDETCStemmer import NDETCStemmer
@@ -37,34 +39,14 @@
 print(output)
 #boleh saya perah lembu ini
 
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
 #bibir merah tangan jadi lengket madu
 
 ```
-Untuk menggunakan alamat download model dari luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti di bawah:
-```python
-from NDETCStemmer import NDETCStemmer, CustomModelDownloader
-
-downloader = CustomModelDownloader(
-    model_1="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-    model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.trainables.syn1neg.npy",
-    model_3="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy"
-)
-
-stemmer=NDETCStemmer(custom_downloader=downloader)
-
-# stemming process
-output=stemmer.stem('boleh saya memerah lembu ini')
-
-print(output)
-#boleh saya perah lembu ini
-
-print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
-```
 
 
 ## Cititation
 ```
 @INPROCEEDINGS{9617514,
   author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
   booktitle={2021 International Conference on Data Science and Its Applications (ICoDSA)},
```

#### html2text {}

```diff
@@ -1,62 +1,53 @@
-Metadata-Version: 2.1 Name: NDETCStemmer_kaenova Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: NDETCStemmer-kaenova Version: 1.4.0 Summary:
 Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode
 Nondeterministic Context Home-page: https://github.com/kaenova/NDETCStemmer
 Keywords: linguistic stemming indonesian bahasa Classifier: Programming
 Language :: Python :: 3 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: Topic :: Text
 Processing :: Linguistic Description-Content-Type: text/markdown License-File:
-LICENSE # Nondeterministic Context (NDETC) Stemmer Nondeterministic Context
-(NDETC) Stemmer adalah library yang mengimplementasikan metode stemming
-nondeterministic berbasis context untuk memecahkan permasalahan kata-kata
-ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam
-bahasa Indonesia. ## Installation Untuk menginstall library ini diperlukan pip
-python yang dapat anda download dengan mengikuti link [berikut](https://
-pip.pypa.io/en/stable/installation/#). Kemudian anda dapat menjalankan kode
-berikut pada terminal yang anda gunakan ```bash pip install git+https://
-github.com/kaenova/NDETCStemmer.git@master ``` ## Usage Setelah menginstall
+LICENSE # Nondeterministic Context (NDETC) Stemmer **This is Kaenova's
+maintained NDETCStemmer, a fork from the [original](https://github.com/
+alifadwitiyap/NDETCStemmer). I upload the model to Huggingface for model
+reliability.** Nondeterministic Context (NDETC) Stemmer adalah library yang
+mengimplementasikan metode stemming nondeterministic berbasis context untuk
+memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis
+pada proses stemming kata dalam bahasa Indonesia. ## Installation Untuk
+menginstall library ini diperlukan pip python yang dapat anda download dengan
+mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
+Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
+```bash pip install NDETCStemmer-kaenova ``` ## Usage Setelah menginstall
 library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder
 yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file
 NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python #import NDETCStemmer library from NDETCStemmer import NDETCStemmer
 #init stemmer stemmer=NDETCStemmer() # stemming process output=stemmer.stem
 ('boleh saya memerah lembu ini') print(output) #boleh saya perah lembu ini
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu')) #bibir
-merah tangan jadi lengket madu ``` Untuk menggunakan alamat download model dari
-luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti
-di bawah: ```python from NDETCStemmer import NDETCStemmer,
-CustomModelDownloader downloader = CustomModelDownloader( model_1="https://
-is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/
-w2vec_wiki_id_case.trainables.syn1neg.npy", model_3="https://is3.cloudhost.id/
-s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy" )
-stemmer=NDETCStemmer(custom_downloader=downloader) # stemming process
-output=stemmer.stem('boleh saya memerah lembu ini') print(output) #boleh saya
-perah lembu ini print(stemmer.stem('bibirnya memerah tangannya jadi selengket
-madu')) ``` ## Cititation ``` @INPROCEEDINGS{9617514, author={Bunyamin and
-Huda, Arief Fatchul and Suryani, Arie Ardiyanti}, booktitle={2021 International
-Conference on Data Science and Its Applications (ICoDSA)}, title={Indonesian
-Stemmer for Ambiguous Word based on Context}, year={2021}, volume={}, number=
-{}, pages={1-9}, doi={10.1109/ICoDSA53588.2021.9617514}} ``` ## Tentang
-Nondeterministic Context Stemmer Merupakan stemmer yang dikembangkan oleh
-Bunyamin_et_al. yang merupakan penelitian lanjutan dari pendekatan
-nondeterministic yang diusulkan oleh Purwarianti. Dalam penelitian Purwarianti,
-setiap kata tidak diperiksa menurut urutan aturan morfologi, tetapi diperiksa
-menggunakan semua aturan. Kemudian, hasilnya disimpan satu per satu dalam
-daftar kandidat kata. Kata akhir akan dipilih menggunakan beberapa aturan
-heuristik, yaitu ketersediaan kosakata dari kata dasar khusus dan panjang kata.
-Masalah yang dihadapi oleh metode nondeterministic yang dikembangkan
-Purwarianti ini dan stemmer deterministic (Andiani_et_al.) adalah masalah
-ambiguitas kata yang dihasilkan oleh stemmer. Misalkan kata "memalukan"
-mempunyai 2 kata dasar, yaitu âmaluâ dan âpaluâ , tergantung
-konteksnya. Pada pernyataan-pernyataan berikut âdia tidak ingin memalukan
-keluarganyaâ dan âtukang memalukan paku di tembokâ kata ambigu
-"memalukan" akan menghasilkan kata dasar "malu" secara terus-menerus.
-Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat pertama
-dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
+merah tangan jadi lengket madu ``` ## Cititation ``` @INPROCEEDINGS{9617514,
+author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
+booktitle={2021 International Conference on Data Science and Its Applications
+(ICoDSA)}, title={Indonesian Stemmer for Ambiguous Word based on Context},
+year={2021}, volume={}, number={}, pages={1-9}, doi={10.1109/
+ICoDSA53588.2021.9617514}} ``` ## Tentang Nondeterministic Context Stemmer
+Merupakan stemmer yang dikembangkan oleh Bunyamin_et_al. yang merupakan
+penelitian lanjutan dari pendekatan nondeterministic yang diusulkan oleh
+Purwarianti. Dalam penelitian Purwarianti, setiap kata tidak diperiksa menurut
+urutan aturan morfologi, tetapi diperiksa menggunakan semua aturan. Kemudian,
+hasilnya disimpan satu per satu dalam daftar kandidat kata. Kata akhir akan
+dipilih menggunakan beberapa aturan heuristik, yaitu ketersediaan kosakata dari
+kata dasar khusus dan panjang kata.  Masalah yang dihadapi oleh metode
+nondeterministic yang dikembangkan Purwarianti ini dan stemmer deterministic
+(Andiani_et_al.) adalah masalah ambiguitas kata yang dihasilkan oleh stemmer.
+Misalkan kata "memalukan" mempunyai 2 kata dasar, yaitu âmaluâ dan
+âpaluâ , tergantung konteksnya. Pada pernyataan-pernyataan berikut âdia
+tidak ingin memalukan keluarganyaâ dan âtukang memalukan paku di tembokâ
+kata ambigu "memalukan" akan menghasilkan kata dasar "malu" secara terus-
+menerus. Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat
+pertama dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
 menghasilkan beberapa alternatif kandidat kata dari kata-kata ambigu tersebut,
 tetapi memiliki kelemahan dalam memilih hasil yang tepat, karena ketiadaan
 konteks. Nondeterministic Context Stemmer memperbaiki pendekatan
 nondeterministik itu dengan menambahkan konteks dalam pemilihan kata terbaik.
 Dalam menyelesaikan masalah pemilihan kata terbaik untuk setiap masukan kata
 ambigu, diusulkan penggunaan model word2vec. Dengan cara ini stemmer akan lebih
 akurat dalam melakukan stemming dibandingkan dengan cara-cara sebelumnya. ####
```

### Comparing `NDETCStemmer_kaenova-1.3.0/README.md` & `NDETCStemmer_kaenova-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Nondeterministic Context (NDETC) Stemmer
 
+**This is Kaenova's maintained NDETCStemmer, a fork from the [original](https://github.com/alifadwitiyap/NDETCStemmer). I upload the model to Huggingface for model reliability.**
+
 Nondeterministic Context (NDETC) Stemmer adalah library yang mengimplementasikan metode stemming nondeterministic berbasis context untuk memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam bahasa Indonesia.
 
 ## Installation
 Untuk menginstall library ini diperlukan pip python yang dapat anda download dengan mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
 Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
 ```bash
-pip install git+https://github.com/kaenova/NDETCStemmer.git@master
+pip install NDETCStemmer-kaenova
 ```
     
 ## Usage
 Setelah menginstall library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python
 #import NDETCStemmer library
 from NDETCStemmer import NDETCStemmer
@@ -24,34 +26,14 @@
 print(output)
 #boleh saya perah lembu ini
 
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
 #bibir merah tangan jadi lengket madu
 
 ```
-Untuk menggunakan alamat download model dari luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti di bawah:
-```python
-from NDETCStemmer import NDETCStemmer, CustomModelDownloader
-
-downloader = CustomModelDownloader(
-    model_1="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-    model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.trainables.syn1neg.npy",
-    model_3="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy"
-)
-
-stemmer=NDETCStemmer(custom_downloader=downloader)
-
-# stemming process
-output=stemmer.stem('boleh saya memerah lembu ini')
-
-print(output)
-#boleh saya perah lembu ini
-
-print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu'))
-```
 
 
 ## Cititation
 ```
 @INPROCEEDINGS{9617514,
   author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
   booktitle={2021 International Conference on Data Science and Its Applications (ICoDSA)},
```

#### html2text {}

```diff
@@ -1,55 +1,46 @@
-# Nondeterministic Context (NDETC) Stemmer Nondeterministic Context (NDETC)
-Stemmer adalah library yang mengimplementasikan metode stemming
-nondeterministic berbasis context untuk memecahkan permasalahan kata-kata
-ambigu (bermakna lebih dari satu) morfologis pada proses stemming kata dalam
-bahasa Indonesia. ## Installation Untuk menginstall library ini diperlukan pip
-python yang dapat anda download dengan mengikuti link [berikut](https://
-pip.pypa.io/en/stable/installation/#). Kemudian anda dapat menjalankan kode
-berikut pada terminal yang anda gunakan ```bash pip install git+https://
-github.com/kaenova/NDETCStemmer.git@master ``` ## Usage Setelah menginstall
+# Nondeterministic Context (NDETC) Stemmer **This is Kaenova's maintained
+NDETCStemmer, a fork from the [original](https://github.com/alifadwitiyap/
+NDETCStemmer). I upload the model to Huggingface for model reliability.**
+Nondeterministic Context (NDETC) Stemmer adalah library yang
+mengimplementasikan metode stemming nondeterministic berbasis context untuk
+memecahkan permasalahan kata-kata ambigu (bermakna lebih dari satu) morfologis
+pada proses stemming kata dalam bahasa Indonesia. ## Installation Untuk
+menginstall library ini diperlukan pip python yang dapat anda download dengan
+mengikuti link [berikut](https://pip.pypa.io/en/stable/installation/#).
+Kemudian anda dapat menjalankan kode berikut pada terminal yang anda gunakan
+```bash pip install NDETCStemmer-kaenova ``` ## Usage Setelah menginstall
 library ini, anda dapat menggunakannya dengan membuat file baru di dalam folder
 yang sama dengan NDETCStemmer_IO.py atau dengan cara mengubah file
 NDETCStemmer_IO.py dengan mengikuti baris code berikut sebagai percobaan:
 ```python #import NDETCStemmer library from NDETCStemmer import NDETCStemmer
 #init stemmer stemmer=NDETCStemmer() # stemming process output=stemmer.stem
 ('boleh saya memerah lembu ini') print(output) #boleh saya perah lembu ini
 print(stemmer.stem('bibirnya memerah tangannya jadi selengket madu')) #bibir
-merah tangan jadi lengket madu ``` Untuk menggunakan alamat download model dari
-luar, silakan untuk menggunakan `CustomModelDownloader` dengan contoh seperti
-di bawah: ```python from NDETCStemmer import NDETCStemmer,
-CustomModelDownloader downloader = CustomModelDownloader( model_1="https://
-is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case",
-model_2="https://is3.cloudhost.id/s3.kaenova.my.id/NDETCStemmer/Model/
-w2vec_wiki_id_case.trainables.syn1neg.npy", model_3="https://is3.cloudhost.id/
-s3.kaenova.my.id/NDETCStemmer/Model/w2vec_wiki_id_case.wv.vectors.npy" )
-stemmer=NDETCStemmer(custom_downloader=downloader) # stemming process
-output=stemmer.stem('boleh saya memerah lembu ini') print(output) #boleh saya
-perah lembu ini print(stemmer.stem('bibirnya memerah tangannya jadi selengket
-madu')) ``` ## Cititation ``` @INPROCEEDINGS{9617514, author={Bunyamin and
-Huda, Arief Fatchul and Suryani, Arie Ardiyanti}, booktitle={2021 International
-Conference on Data Science and Its Applications (ICoDSA)}, title={Indonesian
-Stemmer for Ambiguous Word based on Context}, year={2021}, volume={}, number=
-{}, pages={1-9}, doi={10.1109/ICoDSA53588.2021.9617514}} ``` ## Tentang
-Nondeterministic Context Stemmer Merupakan stemmer yang dikembangkan oleh
-Bunyamin_et_al. yang merupakan penelitian lanjutan dari pendekatan
-nondeterministic yang diusulkan oleh Purwarianti. Dalam penelitian Purwarianti,
-setiap kata tidak diperiksa menurut urutan aturan morfologi, tetapi diperiksa
-menggunakan semua aturan. Kemudian, hasilnya disimpan satu per satu dalam
-daftar kandidat kata. Kata akhir akan dipilih menggunakan beberapa aturan
-heuristik, yaitu ketersediaan kosakata dari kata dasar khusus dan panjang kata.
-Masalah yang dihadapi oleh metode nondeterministic yang dikembangkan
-Purwarianti ini dan stemmer deterministic (Andiani_et_al.) adalah masalah
-ambiguitas kata yang dihasilkan oleh stemmer. Misalkan kata "memalukan"
-mempunyai 2 kata dasar, yaitu âmaluâ dan âpaluâ , tergantung
-konteksnya. Pada pernyataan-pernyataan berikut âdia tidak ingin memalukan
-keluarganyaâ dan âtukang memalukan paku di tembokâ kata ambigu
-"memalukan" akan menghasilkan kata dasar "malu" secara terus-menerus.
-Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat pertama
-dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
+merah tangan jadi lengket madu ``` ## Cititation ``` @INPROCEEDINGS{9617514,
+author={Bunyamin and Huda, Arief Fatchul and Suryani, Arie Ardiyanti},
+booktitle={2021 International Conference on Data Science and Its Applications
+(ICoDSA)}, title={Indonesian Stemmer for Ambiguous Word based on Context},
+year={2021}, volume={}, number={}, pages={1-9}, doi={10.1109/
+ICoDSA53588.2021.9617514}} ``` ## Tentang Nondeterministic Context Stemmer
+Merupakan stemmer yang dikembangkan oleh Bunyamin_et_al. yang merupakan
+penelitian lanjutan dari pendekatan nondeterministic yang diusulkan oleh
+Purwarianti. Dalam penelitian Purwarianti, setiap kata tidak diperiksa menurut
+urutan aturan morfologi, tetapi diperiksa menggunakan semua aturan. Kemudian,
+hasilnya disimpan satu per satu dalam daftar kandidat kata. Kata akhir akan
+dipilih menggunakan beberapa aturan heuristik, yaitu ketersediaan kosakata dari
+kata dasar khusus dan panjang kata.  Masalah yang dihadapi oleh metode
+nondeterministic yang dikembangkan Purwarianti ini dan stemmer deterministic
+(Andiani_et_al.) adalah masalah ambiguitas kata yang dihasilkan oleh stemmer.
+Misalkan kata "memalukan" mempunyai 2 kata dasar, yaitu âmaluâ dan
+âpaluâ , tergantung konteksnya. Pada pernyataan-pernyataan berikut âdia
+tidak ingin memalukan keluarganyaâ dan âtukang memalukan paku di tembokâ
+kata ambigu "memalukan" akan menghasilkan kata dasar "malu" secara terus-
+menerus. Berdasarkan konteksnya, hasilnya seharusnya menjadi "malu" di kalimat
+pertama dan "palu" di kalimat kedua. Nondeterministic stemmer dari Purwarianti
 menghasilkan beberapa alternatif kandidat kata dari kata-kata ambigu tersebut,
 tetapi memiliki kelemahan dalam memilih hasil yang tepat, karena ketiadaan
 konteks. Nondeterministic Context Stemmer memperbaiki pendekatan
 nondeterministik itu dengan menambahkan konteks dalam pemilihan kata terbaik.
 Dalam menyelesaikan masalah pemilihan kata terbaik untuk setiap masukan kata
 ambigu, diusulkan penggunaan model word2vec. Dengan cara ini stemmer akan lebih
 akurat dalam melakukan stemming dibandingkan dengan cara-cara sebelumnya. ####
```

### Comparing `NDETCStemmer_kaenova-1.3.0/setup.py` & `NDETCStemmer_kaenova-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
 name='NDETCStemmer_kaenova',  
-version='1.3.0',
+version='1.4.0',
 py_modules=['NDETCStemmer'] ,
 description="Library untuk stemming kata dalam Bahasa Indonesia menggunakan metode Nondeterministic Context",
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/kaenova/NDETCStemmer",
 packages=setuptools.find_packages(),
 include_package_data=True,
@@ -22,10 +22,11 @@
 ],
 # What does your project relate to?
 keywords='linguistic stemming indonesian bahasa',
 install_requires=[
 	'nltk',
 	'gensim',
 	'gdown',
-	'checksumdir'
+	'checksumdir',
+	'huggingface_hub'
 ]
 )
```

