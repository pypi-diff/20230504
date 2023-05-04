# Comparing `tmp/aacommons-0.2.5.tar.gz` & `tmp/aacommons-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommons-0.2.5.tar", last modified: Thu May  4 12:24:39 2023, max compression
+gzip compressed data, was "aacommons-0.2.7.tar", last modified: Thu May  4 12:37:50 2023, max compression
```

## Comparing `aacommons-0.2.5.tar` & `aacommons-0.2.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/
--rw-rw-r--   0 apang     (1000) apang     (1000)      623 2021-11-13 04:56:04.000000 aacommons-0.2.5/LICENSE
--rw-rw-r--   0 apang     (1000) apang     (1000)       16 2021-11-13 04:56:04.000000 aacommons-0.2.5/MANIFEST.in
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/NOTICE
--rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:24:39.416583 aacommons-0.2.5/PKG-INFO
--rw-rw-r--   0 apang     (1000) apang     (1000)      102 2021-11-13 04:56:04.000000 aacommons-0.2.5/README.rst
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.412583 aacommons-0.2.5/aacommons/
--rw-rw-r--   0 apang     (1000) apang     (1000)      686 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.412583 aacommons-0.2.5/aacommons/contentprovider/
--rw-rw-r--   0 apang     (1000) apang     (1000)    13694 2021-11-22 11:50:54.000000 aacommons-0.2.5/aacommons/contentprovider/ContentProvider.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5107 2023-05-04 12:24:06.000000 aacommons-0.2.5/aacommons/contentprovider/RedisStore.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      877 2021-11-22 09:25:18.000000 aacommons-0.2.5/aacommons/contentprovider/__init__.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      955 2021-11-13 07:54:13.000000 aacommons-0.2.5/aacommons/contentprovider/util.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.412583 aacommons-0.2.5/aacommons/dataparser/
--rwxrwxr-x   0 apang     (1000) apang     (1000)     8951 2021-11-13 08:30:24.000000 aacommons-0.2.5/aacommons/dataparser/AirRecorder.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/aacommons/dataparser/cli/
--rw-rw-r--   0 apang     (1000) apang     (1000)     5632 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/AbstractTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1268 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/CliParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1174 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/CliParserBase.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2339 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/GenericJsonCsvTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     7230 2022-02-11 08:47:35.000000 aacommons-0.2.5/aacommons/dataparser/cli/GenericRegexTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     3541 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5710 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     4455 2022-09-26 06:48:33.000000 aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5310 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosStd.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     7891 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/TableHelpers.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/aacommons/dataparser/cli/arcli/
--rw-rw-r--   0 apang     (1000) apang     (1000)     7506 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliContentProvider.py
--rwxrwxr-x   0 apang     (1000) apang     (1000)     5566 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliContext.py
--rw-rw-r--   0 apang     (1000) apang     (1000)    19680 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliDocuments.py
--rwxrwxr-x   0 apang     (1000) apang     (1000)    54577 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2778 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliParserRequest.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1288 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliResult.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5016 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/dataparser/cli/arcli/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/aacommons/helpers/
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/helpers/__init__.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2122 2021-11-13 08:32:41.000000 aacommons-0.2.5/aacommons/helpers/get_my_ip.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2938 2023-02-23 00:48:58.000000 aacommons-0.2.5/aacommons/helpers/jstyleson_lint.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/aacommons/misc/
--rw-rw-r--   0 apang     (1000) apang     (1000)    23940 2021-11-30 08:07:06.000000 aacommons-0.2.5/aacommons/misc/Stats.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.5/aacommons/misc/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.412583 aacommons-0.2.5/aacommons.egg-info/
--rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:24:39.000000 aacommons-0.2.5/aacommons.egg-info/PKG-INFO
--rw-rw-r--   0 apang     (1000) apang     (1000)     1621 2023-05-04 12:24:39.000000 aacommons-0.2.5/aacommons.egg-info/SOURCES.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)        1 2023-05-04 12:24:39.000000 aacommons-0.2.5/aacommons.egg-info/dependency_links.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       54 2023-05-04 12:24:39.000000 aacommons-0.2.5/aacommons.egg-info/requires.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       10 2023-05-04 12:24:39.000000 aacommons-0.2.5/aacommons.egg-info/top_level.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       38 2023-05-04 12:24:39.416583 aacommons-0.2.5/setup.cfg
--rwxrwxr-x   0 apang     (1000) apang     (1000)      611 2023-02-23 00:48:58.000000 aacommons-0.2.5/setup.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:24:39.416583 aacommons-0.2.5/tests/
--rw-rw-r--   0 apang     (1000) apang     (1000)     3197 2021-11-13 04:56:04.000000 aacommons-0.2.5/tests/test_dataparser_airrecorder.py
--rw-rw-r--   0 apang     (1000) apang     (1000)    24217 2023-02-23 00:48:58.000000 aacommons-0.2.5/tests/test_dataparser_cli.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     3611 2022-02-11 08:47:35.000000 aacommons-0.2.5/tests/test_table_helpers.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/
+-rw-rw-r--   0 apang     (1000) apang     (1000)      623 2021-11-13 04:56:04.000000 aacommons-0.2.7/LICENSE
+-rw-rw-r--   0 apang     (1000) apang     (1000)       16 2021-11-13 04:56:04.000000 aacommons-0.2.7/MANIFEST.in
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/NOTICE
+-rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:37:50.313813 aacommons-0.2.7/PKG-INFO
+-rw-rw-r--   0 apang     (1000) apang     (1000)      102 2021-11-13 04:56:04.000000 aacommons-0.2.7/README.rst
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/
+-rw-rw-r--   0 apang     (1000) apang     (1000)      686 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/__init__.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/contentprovider/
+-rw-rw-r--   0 apang     (1000) apang     (1000)    13694 2021-11-22 11:50:54.000000 aacommons-0.2.7/aacommons/contentprovider/ContentProvider.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     5107 2023-05-04 12:24:06.000000 aacommons-0.2.7/aacommons/contentprovider/RedisStore.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      877 2021-11-22 09:25:18.000000 aacommons-0.2.7/aacommons/contentprovider/__init__.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      955 2021-11-13 07:54:13.000000 aacommons-0.2.7/aacommons/contentprovider/util.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/dataparser/
+-rwxrwxr-x   0 apang     (1000) apang     (1000)     8951 2021-11-13 08:30:24.000000 aacommons-0.2.7/aacommons/dataparser/AirRecorder.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/__init__.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/dataparser/cli/
+-rw-rw-r--   0 apang     (1000) apang     (1000)     5632 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/AbstractTableParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     1268 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/CliParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     1174 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/CliParserBase.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     2339 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/GenericJsonCsvTableParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     7230 2022-02-11 08:47:35.000000 aacommons-0.2.7/aacommons/dataparser/cli/GenericRegexTableParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     3541 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     5710 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     4455 2022-09-26 06:48:33.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     5561 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosStd.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     8061 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/TableHelpers.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/__init__.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/dataparser/cli/arcli/
+-rw-rw-r--   0 apang     (1000) apang     (1000)     7506 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContentProvider.py
+-rwxrwxr-x   0 apang     (1000) apang     (1000)     5566 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContext.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)    19680 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliDocuments.py
+-rwxrwxr-x   0 apang     (1000) apang     (1000)    55157 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParser.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     2778 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParserRequest.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     1288 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliResult.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     8585 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/__init__.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/helpers/
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/helpers/__init__.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     2122 2021-11-13 08:32:41.000000 aacommons-0.2.7/aacommons/helpers/get_my_ip.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     2938 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/helpers/jstyleson_lint.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/misc/
+-rw-rw-r--   0 apang     (1000) apang     (1000)    23940 2021-11-30 08:07:06.000000 aacommons-0.2.7/aacommons/misc/Stats.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/misc/__init__.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons.egg-info/
+-rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/PKG-INFO
+-rw-rw-r--   0 apang     (1000) apang     (1000)     1621 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 apang     (1000) apang     (1000)        1 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 apang     (1000) apang     (1000)       54 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/requires.txt
+-rw-rw-r--   0 apang     (1000) apang     (1000)       10 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/top_level.txt
+-rw-rw-r--   0 apang     (1000) apang     (1000)       38 2023-05-04 12:37:50.313813 aacommons-0.2.7/setup.cfg
+-rwxrwxr-x   0 apang     (1000) apang     (1000)      611 2023-05-04 12:36:47.000000 aacommons-0.2.7/setup.py
+drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/tests/
+-rw-rw-r--   0 apang     (1000) apang     (1000)     3197 2021-11-13 04:56:04.000000 aacommons-0.2.7/tests/test_dataparser_airrecorder.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)    24217 2023-02-23 00:48:58.000000 aacommons-0.2.7/tests/test_dataparser_cli.py
+-rw-rw-r--   0 apang     (1000) apang     (1000)     3611 2022-02-11 08:47:35.000000 aacommons-0.2.7/tests/test_table_helpers.py
```

### Comparing `aacommons-0.2.5/LICENSE` & `aacommons-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/NOTICE` & `aacommons-0.2.7/NOTICE`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/__init__.py` & `aacommons-0.2.7/aacommons/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/contentprovider/ContentProvider.py` & `aacommons-0.2.7/aacommons/contentprovider/ContentProvider.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/contentprovider/RedisStore.py` & `aacommons-0.2.7/aacommons/contentprovider/RedisStore.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/contentprovider/__init__.py` & `aacommons-0.2.7/aacommons/contentprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/contentprovider/util.py` & `aacommons-0.2.7/aacommons/contentprovider/util.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/AirRecorder.py` & `aacommons-0.2.7/aacommons/dataparser/AirRecorder.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/__init__.py` & `aacommons-0.2.7/aacommons/dataparser/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/AbstractTableParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/AbstractTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/CliParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/CliParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/CliParserBase.py` & `aacommons-0.2.7/aacommons/dataparser/cli/CliParserBase.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/GenericJsonCsvTableParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/GenericJsonCsvTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/GenericRegexTableParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/GenericRegexTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py` & `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py` & `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/RowColumnTableParserAosStd.py` & `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosStd.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,26 +41,28 @@
 class RowColumnTableParserAosStd(AbstractTableParser):
     def __init__(self, source, marker=None, tableOptions=None):
         super().__init__()
         self.source = source
         self.marker = marker
         self.tableOptions = tableOptions
         self.markerSearchLines = 10
+        self.markerTableOffset = 2
         if tableOptions is not None:
             self.markerSearchLines = tableOptions.get("marker.search.lines", self.markerSearchLines)
+            self.markerTableOffset = tableOptions.get("marker.table.offset", self.markerTableOffset)
 
     def readContent(self):
         if type(self.source) == list:
             self.contentLines = self.source
         else:
             self.contentLines = self.source.splitlines()
 
     def parse(self):
         # Process structure
-        log.debug("marker [%s]" % str(self.marker))
+        log.debug("marker [%s], marker.table.offset: %d" % (str(self.marker), self.markerTableOffset))
         if self.marker is None:
             # No marker was given, find out from first self.markerSearchLines lines
             currentLineNo = 0
             for currentLine in self.contentLines:
                 if currentLineNo > self.markerSearchLines:
                     break
                 if len(currentLine) > 0 and ((currentLineNo + 1) < len(self.contentLines)):
@@ -84,15 +86,15 @@
                         break
                 currentLineNo += 1
             if self.marker is None:
                 raise Exception("marker not found in %d lines" % (self.markerSearchLines))
 
         # Update main table
         self.tables[0]['name'] = self.marker
-        log.debug("processing table [%s]" % str(self.marker))
+        log.debug("processing table [%s], content len: %d" % (str(self.marker), len(self.contentLines)))
 
         markerLine = -1
         currentPage = None
         currentLineNo = 0
         rows = []
         for currentLine in self.contentLines:
             # Begin page
@@ -108,15 +110,15 @@
                 log.debug("end page [%s] at [%d]" % (str(self.marker), currentLineNo))
                 markerLine = -1
                 currentPage = None
                 currentLineNo += 1
                 continue
 
             # Skip information content between begin page and actual data
-            if (currentPage is None) and (markerLine >= 0) and (currentLineNo > (markerLine + 2)):
+            if (currentPage is None) and (markerLine >= 0) and (currentLineNo > (markerLine + self.markerTableOffset)):
                 if currentLine.startswith("-"):
                     currentPage = self.createPage(self.tables[0],
                                                   self.contentLines[currentLineNo],
                                                   self.contentLines[currentLineNo - 1])
                     log.debug("new page [%s] at [%d]" % (currentPage, currentLineNo))
                     if not 'header' in self.tables[0]:
                         self.tables[0]['header'] = currentPage
```

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/TableHelpers.py` & `aacommons-0.2.7/aacommons/dataparser/cli/TableHelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
                 Default: None
 - "data.trim": true|false. When true, all table values have beginning and ending white-spaces trimmed.
                Default: true
 
 aos-std TABLE PARSER OPTIONS
 ----------------------------
 - "marker.search.lines": "<# lines to search>". Provide number of lines to search for marker. Default 10.
+- "marker.table.offset": "<# lines>". Number of lines between marker and start of a table header (row of -----). Default 2.
 
 aos-dp-std TABLE PARSER OPTIONS
 -------------------------------
 - "marker.search.lines": "<# lines to search>". Provide number of lines to search for marker. Default 10.
 
 aos-smart TABLE PARSER OPTIONS
 ------------------------------
@@ -175,17 +176,17 @@
 
 
 '''
 #
 # Parse content as parameter value list
 #
 '''
-def contentAsParameterValueList(content, marker=None):
+def contentAsParameterValueList(content, marker=None, tableOptions=None):
     source = content
-    parser = RowColumnTableParser(source, marker=marker)
+    parser = RowColumnTableParser(source, marker=marker, tableOptions=tableOptions)
     parser.process()
     parsedTable = parser.getTables()[0]
     # Data
     parameterValueList = dict()
     for row in parsedTable['rows']:
         parameterValueList[row[0].strip()] = row[1].strip()
     return parameterValueList
```

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/__init__.py` & `aacommons-0.2.7/aacommons/dataparser/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliContentProvider.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContentProvider.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliContext.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContext.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliDocuments.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliDocuments.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliParser.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,25 +202,31 @@
 
 
 def arCliProcessRecordExtractCommand(command, r_options, m, r_text):
     # Last resort
     r_suffix_default = '_'
     # By default we suffix original command with new derived command
     r_prefix = command + ":"
-    if not r_options.get('prefix', True):
-        r_prefix = ""
+    ropt_prefix = r_options.get('prefix', True)
+    if isinstance(ropt_prefix, bool):
+        if not ropt_prefix:
+            r_prefix = ""
+    elif isinstance(ropt_prefix, str):
+        r_prefix = command + ropt_prefix
+    else:
+        raise Exception("roptions prefix must be true, false or string")
     if len(m.groups()) > 0:
         # Groups available
         ropt_command = r_options.get("command", None)
         if ropt_command is None:
             # Use first group by default
             r_suffix = m.groups(r_suffix_default)[0]
         elif isinstance(ropt_command, str):
             # Use specified named group
-            r_suffix = m.groupdict(r_suffix_default).get(ropt_command, r_suffix_default)
+            r_suffix = m.groupdict(r_suffix_default).get(ropt_command, ropt_command)
         elif isinstance(ropt_command, int):
             # Use specified unnamed group
             try:
                 r_suffix = m.groups(r_suffix_default)[ropt_command]
             except IndexError:
                 r_suffix = r_suffix_default
         else:
@@ -367,15 +373,16 @@
                     rows = nrows
                     logAr.debug("parsed table(transposed): %s, rows: %d" % (name, len(rows)))
             else:
                 rows = contentAsListOfDict(ttext, marker=marker, tableOptions=tableOptions)
                 logAr.debug("parsed table: %s, rows: %d" % (name, len(rows)))
         else:
             # KVP
-            _rows = contentAsParameterValueList(ttext, marker=marker)
+            tableOptions=table['toptions']
+            _rows = contentAsParameterValueList(ttext, marker=marker, tableOptions=tableOptions)
             rows = [ _rows ]
             logAr.debug("parsed kvp: %s, columns: %d" % (name, len(rows)))
         T.append((table, rows))
 
 
 # AOS smart output parsing
 aosSmartTypesMapping = {
@@ -700,14 +707,18 @@
                 if m != None:
                     cliCommandDef = _cliCommandDef
                     P.update(m.groupdict())
                     break
             if cliCommandDef is None:
                 self._log.info("[%s] [%s] [%s] drop - no cliCommandDef" % \
                     (parserRequest['Source'], parserRequest['Label'], command))
+                if parserRequest.get('_raiseOnNocliCommandDef', False):
+                    # make noise for debugging
+                    raise Exception("label [%s] is missing command [%s]" % \
+                        (parserRequest['Label'], command))
                 return
 
         # Records
         records = cliCommandDef['records']
         if len(records) > 0:
             # Preprocess CLI output for records
             precords = arCliProcessRecords(records, command, parserRequest['Stdout'], P)
@@ -816,15 +827,15 @@
         # Process tables
         result.addType(ArCliResult.TYPE_TABLES)
         if len(T) > 0:
             savedP = P
             for (tableDef, rows) in T:
                 name = tableDef['name']
                 tableDocType = tableDef.get('document', doc_type)
-                logAr.debug('processing tables rows: %s' % (name))
+                logAr.debug('processing tables rows: %s, len: %d' % (name, len(rows)))
                 messages = result.addSection(ArCliResult.TYPE_TABLES, name)
                 for C in rows:
                     body = {}
                     P = dict()
                     P.update(savedP)
                     # Add row content as fields
                     for (k, v) in C.items():
```

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliParserRequest.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParserRequest.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/ArCliResult.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliResult.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/dataparser/cli/arcli/__init__.py` & `aacommons-0.2.7/aacommons/dataparser/cli/arcli/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/helpers/__init__.py` & `aacommons-0.2.7/aacommons/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/helpers/get_my_ip.py` & `aacommons-0.2.7/aacommons/helpers/get_my_ip.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/helpers/jstyleson_lint.py` & `aacommons-0.2.7/aacommons/helpers/jstyleson_lint.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/misc/Stats.py` & `aacommons-0.2.7/aacommons/misc/Stats.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons/misc/__init__.py` & `aacommons-0.2.7/aacommons/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/aacommons.egg-info/SOURCES.txt` & `aacommons-0.2.7/aacommons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/setup.py` & `aacommons-0.2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open('README.rst', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='aacommons',
-    version='0.2.5',
+    version='0.2.7',
     description='aacommons',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Thomas Bastian, Jeffrey Goff, Albert Pang',
     url='',
     test_suite="tests",
     packages=find_packages(exclude=('tests', 'docs')),
```

### Comparing `aacommons-0.2.5/tests/test_dataparser_airrecorder.py` & `aacommons-0.2.7/tests/test_dataparser_airrecorder.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/tests/test_dataparser_cli.py` & `aacommons-0.2.7/tests/test_dataparser_cli.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.5/tests/test_table_helpers.py` & `aacommons-0.2.7/tests/test_table_helpers.py`

 * *Files identical despite different names*

