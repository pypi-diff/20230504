# Comparing `tmp/eis1600-0.8.7.tar.gz` & `tmp/eis1600-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.7.tar", last modified: Fri Apr 28 07:47:20 2023, max compression
+gzip compressed data, was "eis1600-0.8.9.tar", last modified: Thu May  4 09:07:22 2023, max compression
```

## Comparing `eis1600-0.8.7.tar` & `eis1600-0.8.9.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.684525 eis1600-0.8.7/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.7/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-28 07:47:20.684525 eis1600-0.8.7/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.7/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.672525 eis1600-0.8.7/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.7/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.672525 eis1600-0.8.7/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.7/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.7/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.7/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.7/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.672525 eis1600-0.8.7/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.7/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5529 2023-04-27 07:28:56.000000 eis1600-0.8.7/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.7/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.676524 eis1600-0.8.7/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.7/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.8.7/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.8.7/eis1600/gazetteers/data/regions_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.8.7/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.8.7/eis1600/gazetteers/data/toponyms.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.676524 eis1600-0.8.7/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.8.7/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.8.7/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.7/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.7/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.676524 eis1600-0.8.7/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.7/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.8.7/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.7/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.7/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.7/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.7/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.7/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-26 15:08:00.000000 eis1600-0.8.7/eis1600/helper/my_json_ecoder.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.7/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.8.7/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1356 2023-04-24 07:56:45.000000 eis1600-0.8.7/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.7/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.7/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.7/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13077 2023-04-19 15:21:14.000000 eis1600-0.8.7/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.7/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.7/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.7/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7477 2023-04-27 07:58:47.000000 eis1600-0.8.7/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.7/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.7/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.7/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.7/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7231 2023-04-27 07:35:56.000000 eis1600-0.8.7/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.7/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.7/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.7/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.7/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.7/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1596 2023-04-28 07:44:42.000000 eis1600-0.8.7/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10535 2023-04-24 09:53:23.000000 eis1600-0.8.7/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.7/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.7/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.7/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.8.7/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.680525 eis1600-0.8.7/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.7/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.7/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.7/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-28 07:47:20.672525 eis1600-0.8.7/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1992 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       72 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-28 07:47:20.000000 eis1600-0.8.7/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-28 07:47:20.684525 eis1600-0.8.7/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2269 2023-04-28 07:46:35.000000 eis1600-0.8.7/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.9/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-05-04 09:07:22.117847 eis1600-0.8.9/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.9/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.9/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.9/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.9/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.9/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.9/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5679 2023-05-04 09:06:11.000000 eis1600-0.8.9/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.9/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.109847 eis1600-0.8.9/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.8.9/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.8.9/eis1600/gazetteers/data/regions_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.8.9/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.8.9/eis1600/gazetteers/data/toponyms.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.109847 eis1600-0.8.9/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.8.9/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.8.9/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.9/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.9/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.9/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.8.9/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.9/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.9/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.9/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.9/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.9/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.9/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.8.9/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1291 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.9/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.9/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.8.9/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.9/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.9/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8773 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.9/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.9/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.9/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.9/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6985 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.9/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.9/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.9/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.9/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.9/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1596 2023-04-28 07:44:42.000000 eis1600-0.8.9/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10489 2023-05-04 08:54:08.000000 eis1600-0.8.9/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.9/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.9/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.8.9/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.9/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.9/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.9/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-04 09:07:22.117847 eis1600-0.8.9/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2297 2023-05-04 09:04:19.000000 eis1600-0.8.9/setup.py
```

### Comparing `eis1600-0.8.7/LICENSE` & `eis1600-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/PKG-INFO` & `eis1600-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.7
+Version: 0.8.9
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.7/README.md` & `eis1600-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/dates/Date.py` & `eis1600-0.8.9/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/dates/date_patterns.py` & `eis1600-0.8.9/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/dates/methods.py` & `eis1600-0.8.9/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/gazetteers/Onomastics.py` & `eis1600-0.8.9/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/gazetteers/Toponyms.py` & `eis1600-0.8.9/eis1600/gazetteers/Toponyms.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 file_path = files('eis1600.gazetteers.data')
 thurayya_path = file_path.joinpath('toponyms.csv')
 regions_path = file_path.joinpath('regions_gazetteer.csv')
 
 
 def toponyms_from_rows(row: pd.Series) -> YAMLToponym:
     toponym = {
-            'name': row['uri'],
+            'uri': row['uri'],
+            'label': row['placeLabel'],
             'geometry': {
                     'type': row['geometry_type'],
                     'coordinates': row['geometry_coords']
             }
     }
     return YAMLToponym(toponym)
 
 
 class YAMLToponym:
     def __init__(self, attr: Dict):
-        self.name = ''
+        self.uri = ''
+        self.label = ''
         self.geometry = {
                 'type': '',
                 'coordinates': [0, 0]
         }
 
         for key, val in attr.items():
             self.__setattr__(key, val)
@@ -39,22 +41,25 @@
     @property
     def attribute(self):
         return self._attribute
 
     def coords(self) -> List[float, float]:
         return self.geometry['coordinates']
 
+    def to_json(self) -> Dict:
+        return self.__dict__
+
     def __repr__(self) -> str:
         return str(type(self)) + str(self.__dict__)
 
     def __str__(self) -> str:
         return str(self.__dict__)
 
     def __hash__(self):
-        return hash(self.name + str(self.geometry.get('coordinates')))
+        return hash(self.uri + str(self.geometry.get('coordinates')))
 
 
 @Singleton
 class Toponyms:
     """
     Gazetteer
 
@@ -121,15 +126,16 @@
 
         :param str uri: URI of the province to look up attributes
         :return:
         """
         # TODO lookup provinces from provinces gazetteer
         # TODO toponyms_from_rows(row)
         province = {
-                'name': uri,
+                'uri': uri,
+                'label': '',
                 'geometry': {
                         'type': 'point',
                         'coordinates': [0, 0]
                 }
         }
 
         return YAMLToponym(province)
```

### Comparing `eis1600-0.8.7/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.8.9/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.8.9/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/gazetteers/data/toponyms.csv` & `eis1600-0.8.9/eis1600/gazetteers/data/toponyms.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/EntityTags.py` & `eis1600-0.8.9/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/Singleton.py` & `eis1600-0.8.9/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/ar_normalization.py` & `eis1600-0.8.9/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.8.9/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/markdown_methods.py` & `eis1600-0.8.9/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/markdown_patterns.py` & `eis1600-0.8.9/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/miu_random_revisions.py` & `eis1600-0.8.9/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/repo.py` & `eis1600-0.8.9/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/yml_methods.py` & `eis1600-0.8.9/eis1600/helper/yml_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/helper/yml_to_json.py` & `eis1600-0.8.9/eis1600/helper/yml_to_json.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import json
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from pathlib import Path
-
-from eis1600.helper.my_json_ecoder import MyJSONEncoder
+import jsonpickle
 from p_tqdm import p_uimap
 
 from eis1600.processing.preprocessing import get_yml
 
 
 def main():
     arg_parser = ArgumentParser(
@@ -30,14 +28,14 @@
             print(file)
             res.append(get_yml(file))
     else:
         res = p_uimap(get_yml, infiles)
 
     yml_dict = {}
     for path, yml in res:
-        yml_dict[path] = yml
+        yml_dict[path] = yml.to_json()
 
-    # TODO: Where shall that file be?
-    with open('OpenITI_EIS1600_MIUs/gold_standard_yml.json', 'w', encoding='utf-8') as fh:
-        json.dump(yml_dict, fh, cls=MyJSONEncoder, indent='\t', ensure_ascii=False)
+    with open('MasterChronicle/masterchronicleapp/src/data.json', 'w', encoding='utf-8') as fh:
+        json_str = jsonpickle.encode(yml_dict, unpicklable=False)
+        fh.write(json_str)
 
     print('Done')
```

### Comparing `eis1600-0.8.7/eis1600/markdown/UIDs.py` & `eis1600-0.8.9/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.8.9/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/markdown/insert_uids.py` & `eis1600-0.8.9/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/markdown/methods.py` & `eis1600-0.8.9/eis1600/markdown/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                 page_tag = PAGE_TAG_PATTERN.match(paragraph).group('page_tag')
                 if PAGE_TAG_SPLITTING_PARAGRAPH_PATTERN.search('\n\n'.join([prev_p, paragraph, next_p])):
                     if text_updated:
                         if text_updated[-1][-1] == ' ':
                             text_updated[-1] += page_tag + ' ' + next_p
                         else:
                             text_updated[-1] += ' ' + page_tag + ' ' + next_p
-                        prev_p = paragraph
                         paragraph = next_p
                         next_p = next(text_iter, None)
                 elif text_updated:
                     text_updated[-1] += ' ' + page_tag
                 # else:
                 # Remove PageV00P000 at the beginning in an individual paragraph
                 # text_updated.append(paragraph)
@@ -293,15 +292,14 @@
                 if PAGE_TAG_IN_BETWEEN_PATTERN.search('\n\n'.join([prev_p, paragraph, next_p])):
                     if text_updated:
                         next_p_text = next_p.split('::UNDEFINED:: ~\n')[1]
                         if text_updated[-1][-1] == ' ':
                             text_updated[-1] += page_tag + ' ' + next_p_text
                         else:
                             text_updated[-1] += ' ' + page_tag + ' ' + next_p_text
-                        prev_p = paragraph
                         paragraph = next_p
                         next_p = next(text_iter, None)
                 elif text_updated:
                     text_updated[-1] += ' ' + page_tag
                 # else:
                 # Remove PageV00P000 at the beginning in an individual paragraph
                 # text_updated.append(paragraph)
```

### Comparing `eis1600-0.8.7/eis1600/markdown/update_uids.py` & `eis1600-0.8.9/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.8.9/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/miu/HeadingTracker.py` & `eis1600-0.8.9/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/miu/YAMLHandler.py` & `eis1600-0.8.9/eis1600/miu/YAMLHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from ast import literal_eval
 from typing import Any, Dict, Optional
 
+
 from eis1600.gazetteers.Toponyms import YAMLToponym
 from eis1600.helper.markdown_patterns import MIU_HEADER
 from eis1600.helper.yml_methods import dict_to_yaml
 from eis1600.miu.HeadingTracker import HeadingTracker
 
 
 class YAMLHandler:
@@ -24,17 +25,19 @@
     """
     # Only attributes named in the following list are allowed to be added to the YAMLHeader - add any new attribute
     # to that list
     __attr_from_annotation = ['dates', 'ages', 'onomastics', 'ambigious_toponyms', 'toponyms', 'places', 'provinces',
                               'edges_places', 'edges_provinces']
 
     @staticmethod
-    def __parse_yml_val(val: str) -> Any:
+    def __parse_yml_val(val: str, key: Optional[str] = None) -> Any:
         if val.isdigit():
             return int(val)
+        if len(val.split('.')) == 2 and val.split('.')[0].isdigit() and val.split('.')[1].isdigit():
+            return float(val)
         elif val == 'True':
             return True
         elif val == 'False':
             return False
         elif val == 'None' or val == '':
             return None
         elif val.startswith(('\'', '"')):
@@ -45,18 +48,23 @@
             if raw_val_list.startswith('(') and raw_val_list.endswith(')'):
                 # List of tuples
                 val_list = raw_val_list.strip('()').split('), (')
                 values = []
                 for v in val_list:
                     t = v.split(', ')
                     values.append((YAMLHandler.__parse_yml_val(t[0]), YAMLHandler.__parse_yml_val(t[1])))
-            elif raw_val_list.startswith('['):
+            elif raw_val_list.startswith('[') or raw_val_list.startswith('{'):
                 # Nested lists
                 nested_lists = literal_eval(val)
-                values = nested_lists
+                if key == 'places' or key == 'provinces':
+                    values = [YAMLToponym(toponym) for toponym in nested_lists]
+                elif key.startswith('edges'):
+                    values = [[YAMLToponym(edge[0]), YAMLToponym(edge[1])] for edge in nested_lists]
+                else:
+                    values = nested_lists
             else:
                 # List of other values
                 val_list = raw_val_list.split(', ')
                 values = [YAMLHandler.__parse_yml_val(v) for v in val_list]
             return values
         else:
             return val
@@ -81,21 +89,21 @@
                     else:
                         yml[dict_key] = dict_val
                     level.pop()
 
                 if intend and intend == len(level) and val != '':
                     # Stay on level and add key, val to the respective dict
                     curr_dict = level[-1][1]
-                    curr_dict[key] = YAMLHandler.__parse_yml_val(val)
+                    curr_dict[key] = YAMLHandler.__parse_yml_val(val, key)
                 elif val == '':
                     # Go one level deeper, add key and empty dict for that new level
                     level.append((key, {}))
                 else:
                     # Add key, val to the top level
-                    yml[key] = YAMLHandler.__parse_yml_val(val)
+                    yml[key] = YAMLHandler.__parse_yml_val(val, key)
 
         if len(level):
             dict_key = level[-1][0]
             dict_val = level[-1][1]
             yml[dict_key] = dict_val
 
         return yml
@@ -139,29 +147,41 @@
 
     def get_yamlfied(self) -> str:
         yaml_str = MIU_HEADER + 'Begin#\n\n'
         for key, val in vars(self).items():
             if val:
                 if key == 'category':
                     yaml_str += key + '    : \'' + val + '\'\n'
+                elif key == 'places' or key == 'provinces':
+                    yaml_str += f'{key}    : {[toponym.as_dict() for toponym in val]}\n'
+                elif key.startswith('edges'):
+                    yaml_str += f'{key}    : {[[edge[0].as_dict(), edge[1].as_dict()] for edge in val]}\n'
+                elif hasattr(val, 'get_yamlfied'):
+                    yaml_str += f'{key}    : {val.get_yamlfied()}\n'
                 elif isinstance(val, dict):
                     yaml_str += f'{key}    :\n{dict_to_yaml(val, 1)}\n'
-                elif isinstance(val, YAMLToponym):
-                    yaml_str += f'{key}    :\n{dict_to_yaml(val.as_dict(), 1)}\n'
                 else:
                     yaml_str += key + '    : ' + str(val) + '\n'
         yaml_str += '\n' + MIU_HEADER + 'End#\n\n'
 
         return yaml_str
 
     def to_json(self) -> Dict:
         json_dict = {}
         for key, val in vars(self).items():
-            if val:
-                json_dict[key] = val
+            if key != 'toponyms' and val:
+                # Toponym is only to control the entity and how it was identified
+                if key == 'places' or key == 'provinces':
+                    json_dict[key] = [elem.to_json() for elem in val]
+                elif key.startswith('edges'):
+                    json_dict[key] = [[edge[0].to_json(), edge[1].to_json()] for edge in val]
+                elif hasattr(val, 'to_json'):
+                    json_dict[key] = val.to_json()
+                else:
+                    json_dict[key] = val
         return json_dict
 
     def is_bio(self) -> bool:
         return self.category == '$' or self.category == '$$'
 
     def is_reviewed(self) -> bool:
         return self.reviewed.startswith('REVIEWED')
```

### Comparing `eis1600-0.8.7/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.8.9/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/miu/methods.py` & `eis1600-0.8.9/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.8.9/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/miu/yml_handling.py` & `eis1600-0.8.9/eis1600/miu/yml_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,31 +87,24 @@
             entities_dict[cat][tag] = [entity]
         elif isinstance(entity, list):
             entities_dict[cat] = entity
         else:
             entities_dict[cat] = [entity]
 
 
-def toponyms_list_to_dict(t_list: List[YAMLToponym]) -> Dict:
-    t_dict = {}
-    for t in t_list:
-        t_dict[t.name] = t.geometry
-
-    return t_dict
-
-
 def add_annotated_entities_to_yml(text_with_tags: str, yml_handler: YAMLHandler, filename: str) -> None:
     """Populates YAMLHeader with annotated entities.
 
     :param str text_with_tags: Text with inserted tags of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param str filename: Filename of the current MIU (used in error msg).
     """
     # We do not need to differentiate between automated and manual tags
     text_with_tags = text_with_tags.replace('Ü', '')
+    tg = Toponyms.instance()
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     nas_dict = {}
     toponyms_set: Set[YAMLToponym] = set()
     provinces_set: Set[YAMLToponym] = set()
     nas_counter = 0
 
@@ -126,15 +119,14 @@
             try:
                 val = get_yrs_tag_value(m.group(0))
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val})
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {filename}')
                 return
         elif cat == 'TOPONYM':
-            tg = Toponyms.instance()
             place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
             if len(list_of_uris) > 1:
                 yml_handler.set_ambigious_toponyms()
             toponyms_set.update(list_of_uris)
             provinces_set.update(list_of_provinces)
             add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uri})
         elif cat == 'ONOMASTIC':
@@ -157,13 +149,13 @@
             entities_dict['onomastics'] = {'nas': nas_dict}
 
     if 'onomastics' in entities_dict.keys():
         # Sort dict by keys
         entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
 
     if toponyms_set:
-        entities_dict['places'] = toponyms_list_to_dict(list(toponyms_set))
-        entities_dict['edges_places'] = [[a.coords(), b.coords()] for a, b in combinations(toponyms_set, 2)]
+        entities_dict['places'] = list(toponyms_set)
+        entities_dict['edges_places'] = [[a, b] for a, b in combinations(toponyms_set, 2)]
         provinces_set = set([tg.look_up_province(p) for p in provinces_set])
-        entities_dict['provinces'] = toponyms_list_to_dict(list(provinces_set))
-        entities_dict['edges_provinces'] = [[a.coords(), b.coords()] for a, b in combinations(provinces_set, 2)]
+        entities_dict['provinces'] = list(provinces_set)
+        entities_dict['edges_provinces'] = [[a, b] for a, b in combinations(provinces_set, 2)]
     yml_handler.add_tagged_entities(entities_dict)
```

### Comparing `eis1600-0.8.7/eis1600/nlp/cameltools.py` & `eis1600-0.8.9/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.8.9/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/nlp/utils.py` & `eis1600-0.8.9/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/onomastics/annotation.py` & `eis1600-0.8.9/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/onomastics/methods.py` & `eis1600-0.8.9/eis1600/onomastics/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from pathlib import Path
 from typing import Optional
 
 import pandas as pd
 from numpy import nan
 from pandas import Series
 
-from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.gazetteers.Onomastics import Onomastics
 from eis1600.gazetteers.Toponyms import Toponyms
-from eis1600.onomastics.re_pattern import ABU, ABI, BANU_BANI, CRF_PATTERN, IBN_IBNA, BN_BNT, SHR_PATTERN, SPELLING, UMM
-from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
+from eis1600.miu.YAMLHandler import YAMLHandler
+from eis1600.onomastics.re_pattern import ABI, ABU, BN_BNT, CRF_PATTERN, IBN_IBNA, SHR_PATTERN, SPELLING, UMM
 from eis1600.processing.postprocessing import reconstruct_miu_text_with_tags, write_updated_miu_to_file
+from eis1600.processing.preprocessing import get_tokens_and_tags, get_yml_and_miu_df
 
 
 def get_nas(text: str) -> str:
     """Add the list of forefathers to the YAMLHeader and return nasab part with tagged NAS and manipulated so it is
     ignored for further onomastic analysis (all elements which refere to ancestors are filtered here).
 
     :param str text: nasab str.
-    :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :return str: nasab str with tagged and manipulated nas elements.
     """
     og = Onomastics.instance()
 
     text_mnpld = ABU.sub(' ابو_', text)
     text_mnpld = UMM.sub(' ام_', text_mnpld)
     text_mnpld = ABI.sub(' ابي_', text_mnpld)
@@ -70,14 +69,15 @@
 
     return text_mnpld
 
 
 def tag_nasab(text: str, logger_nasab: Logger) -> str:
     """Annotate the nasab part of the MIU.
 
+    :param logger_nasab:
     :param str text: nasab part of the MIU as one single string with tagged and filtered NAS elements (NAS is
     connected with '_' and therefore does not match with the gazetteer).
     :return str: the nasab part pf the MIU which contains also the tags in front of the recognized elements,
     '_' are removed.
     """
     og = Onomastics.instance()
     tg = Toponyms.instance()
```

### Comparing `eis1600-0.8.7/eis1600/onomastics/re_pattern.py` & `eis1600-0.8.9/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/processing/postprocessing.py` & `eis1600-0.8.9/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/processing/preprocessing.py` & `eis1600-0.8.9/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/stats/methods.py` & `eis1600-0.8.9/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600/stats/miu_stats.py` & `eis1600-0.8.9/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/eis1600.egg-info/PKG-INFO` & `eis1600-0.8.9/eis1600.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.7
+Version: 0.8.9
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.7/eis1600.egg-info/SOURCES.txt` & `eis1600-0.8.9/eis1600.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
 eis1600/helper/miu_random_revisions.py
-eis1600/helper/my_json_ecoder.py
 eis1600/helper/repo.py
 eis1600/helper/yml_methods.py
 eis1600/helper/yml_to_json.py
 eis1600/helper/data/__init__.py
 eis1600/helper/data/entity_tags.csv
 eis1600/markdown/UIDs.py
 eis1600/markdown/__init__.py
```

### Comparing `eis1600-0.8.7/eis1600.egg-info/entry_points.txt` & `eis1600-0.8.9/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.7/setup.py` & `eis1600-0.8.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.7',
+      version='0.8.9',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
@@ -33,15 +33,16 @@
       python_requires='>=3.7, <3.9',
       install_requires=[
               'openiti',
               'pandas',
               'numpy',
               'tqdm',
               'p_tqdm',
-              'importlib_resources'
+              'importlib_resources',
+              'jsonpickle'
       ],
       extras_require={'NER': ['camel-tools']},
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent',
                    'Development Status :: 1 - Planning',
                    'Intended Audience :: Science/Research']
```

