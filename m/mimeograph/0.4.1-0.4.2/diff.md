# Comparing `tmp/mimeograph-0.4.1.tar.gz` & `tmp/mimeograph-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.4.1.tar", last modified: Tue Apr 25 07:14:50 2023, max compression
+gzip compressed data, was "mimeograph-0.4.2.tar", last modified: Thu May  4 11:24:38 2023, max compression
```

## Comparing `mimeograph-0.4.1.tar` & `mimeograph-0.4.2.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.1/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.1/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-25 07:14:50.511719 mimeograph-0.4.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    20615 2023-04-24 13:03:27.000000 mimeograph-0.4.1/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2023-04-25 07:14:26.000000 mimeograph-0.4.1/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-25 07:14:50.511719 mimeograph-0.4.1/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-25 07:13:50.000000 mimeograph-0.4.1/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9574 2023-04-25 07:13:50.000000 mimeograph-0.4.1/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      553 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12842 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-20 08:22:52.000000 mimeograph-0.4.1/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/annotations.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6402 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)      194 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      165 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2101 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      860 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2128 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      101 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/exc.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-20 08:22:48.000000 mimeograph-0.4.1/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      680 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5677 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-20 08:22:47.000000 mimeograph-0.4.1/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-20 08:22:45.000000 mimeograph-0.4.1/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      458 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)      330 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8714 2023-04-25 07:12:18.000000 mimeograph-0.4.1/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7433 2023-04-25 07:12:18.000000 mimeograph-0.4.1/src/mimeo/utils/renderer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1774 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    31417 2023-04-24 13:03:27.000000 mimeograph-0.4.1/tests/test_mimeo_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.4.1/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.1/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.2/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.2/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22824 2023-05-04 11:24:38.404713 mimeograph-0.4.2/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20867 2023-05-04 11:08:55.000000 mimeograph-0.4.2/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1712 2023-05-04 11:24:30.000000 mimeograph-0.4.2/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-04 11:24:38.404713 mimeograph-0.4.2/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.396713 mimeograph-0.4.2/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1251 2023-05-04 11:24:30.000000 mimeograph-0.4.2/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      372 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      757 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1498 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4031 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17457 2023-05-04 11:24:30.000000 mimeograph-0.4.2/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      521 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2994 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    30070 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1232 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1240 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2152 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2997 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      825 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      932 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4047 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4717 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15071 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4786 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2752 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1344 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5026 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5307 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1966 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5111 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2045 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7578 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/mimeo_db.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      807 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2810 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11599 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1264 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1645 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      579 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3760 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      585 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      356 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-04 10:17:10.000000 mimeograph-0.4.2/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-04 10:17:10.000000 mimeograph-0.4.2/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      700 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-04 10:17:11.000000 mimeograph-0.4.2/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.2/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-04 10:17:13.000000 mimeograph-0.4.2/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1048 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1749 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1326 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23391 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19663 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22824 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1826 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1838 2023-05-04 11:08:55.000000 mimeograph-0.4.2/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.2/tests/test_tools.py
```

### Comparing `mimeograph-0.4.1/LICENSE` & `mimeograph-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/PKG-INFO` & `mimeograph-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,15 +39,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool generating custom data based on a template.
+**Mimeo** is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -82,20 +82,33 @@
       }
     }
   ]
 }
 ```
 _You can find more configuration examples in the `examples` folder._
 
-### Mimeo CLI
+### Mimeograph
+
+#### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
 ```
 
+#### Python library
+
+```python
+from mimeo import MimeoConfig, Mimeograph
+
+config = {
+    # Your configuration
+}
+mimeo_config = MimeoConfig(config)
+Mimeograph(mimeo_config).process()
+```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
@@ -154,17 +167,17 @@
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
 | Short option | Long option         | Description                                                                          |
 |:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-x`     | `--xml-declaration` | overwrite the `xml_declaration` property                                             |
-|     `-i`     | `--indent`          | overwrite the `indent` property                                                      |
 |     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
+|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
+|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
 |     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
 |     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
 |     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
 |     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
 |     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
 |     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
 |     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
@@ -182,36 +195,36 @@
 |              | `--debug`   | enable DEBUG mode |
 |              | `--fine`    | enable FINE mode  |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                             |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:--------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_format`                 |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details`                |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`      |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/directory_path` |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`      |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`         |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`       |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`           |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`           |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`           |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `indent`                        |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
+|:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
+| `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
```

### Comparing `mimeograph-0.4.1/README.md` & `mimeograph-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool generating custom data based on a template.
+**Mimeo** is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -40,20 +40,33 @@
       }
     }
   ]
 }
 ```
 _You can find more configuration examples in the `examples` folder._
 
-### Mimeo CLI
+### Mimeograph
+
+#### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
 ```
 
+#### Python library
+
+```python
+from mimeo import MimeoConfig, Mimeograph
+
+config = {
+    # Your configuration
+}
+mimeo_config = MimeoConfig(config)
+Mimeograph(mimeo_config).process()
+```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
@@ -112,17 +125,17 @@
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
 | Short option | Long option         | Description                                                                          |
 |:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-x`     | `--xml-declaration` | overwrite the `xml_declaration` property                                             |
-|     `-i`     | `--indent`          | overwrite the `indent` property                                                      |
 |     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
+|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
+|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
 |     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
 |     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
 |     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
 |     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
 |     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
 |     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
 |     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
@@ -140,36 +153,36 @@
 |              | `--debug`   | enable DEBUG mode |
 |              | `--fine`    | enable FINE mode  |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                             |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:--------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_format`                 |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details`                |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`      |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/directory_path` |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`      |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`         |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`       |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`           |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`           |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`           |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `indent`                        |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
+|:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
+| `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
```

### Comparing `mimeograph-0.4.1/pyproject.toml` & `mimeograph-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.4.1"
+version = "0.4.2"
 description = "Generate data based on a simple template"
 readme = "README.md"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -32,25 +32,25 @@
 [project.optional-dependencies]
 dev = ["bumpver", "build", "twine", "pylama", "isort", "pytest", "pytest-cov", "responses"]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.4.1"
+current_version = "0.4.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/mimeo/__init__.py" = ["{version}"]
-"src/mimeo/__main__.py" = ["{version}"]
+"src/mimeo/cli/parsers.py" = ["{version}"]
 
 [tool.pylama]
 async = true
 linters = "mccabe,pycodestyle,pydocstyle,pyflakes"
 
 [tool.pylama.linter.pydocstyle]
 convention = "numpy"
```

### Comparing `mimeograph-0.4.1/src/mimeo/resources/cities.csv` & `mimeograph-0.4.2/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/src/mimeo/resources/countries.csv` & `mimeograph-0.4.2/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/src/mimeo/resources/forenames.csv` & `mimeograph-0.4.2/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/src/mimeo/resources/logging.yaml` & `mimeograph-0.4.2/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/src/mimeo/resources/surnames.txt` & `mimeograph-0.4.2/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.1/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.4.2/src/mimeograph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,15 +39,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool generating custom data based on a template.
+**Mimeo** is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -82,20 +82,33 @@
       }
     }
   ]
 }
 ```
 _You can find more configuration examples in the `examples` folder._
 
-### Mimeo CLI
+### Mimeograph
+
+#### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
 ```
 
+#### Python library
+
+```python
+from mimeo import MimeoConfig, Mimeograph
+
+config = {
+    # Your configuration
+}
+mimeo_config = MimeoConfig(config)
+Mimeograph(mimeo_config).process()
+```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
@@ -154,17 +167,17 @@
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
 | Short option | Long option         | Description                                                                          |
 |:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-x`     | `--xml-declaration` | overwrite the `xml_declaration` property                                             |
-|     `-i`     | `--indent`          | overwrite the `indent` property                                                      |
 |     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
+|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
+|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
 |     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
 |     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
 |     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
 |     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
 |     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
 |     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
 |     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
@@ -182,36 +195,36 @@
 |              | `--debug`   | enable DEBUG mode |
 |              | `--fine`    | enable FINE mode  |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                             |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:--------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_format`                 |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details`                |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`      |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/directory_path` |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`      |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`         |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`       |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`           |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`           |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`           |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`       |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `indent`                        |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
+|:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
+| `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
```

### Comparing `mimeograph-0.4.1/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.4.2/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/mimeo/__init__.py
 src/mimeo/__main__.py
-src/mimeo/exc.py
 src/mimeo/mimeo.py
 src/mimeo/tools.py
+src/mimeo/cli/__init__.py
+src/mimeo/cli/exc.py
+src/mimeo/cli/job.py
+src/mimeo/cli/parsers.py
 src/mimeo/config/__init__.py
 src/mimeo/config/exc.py
 src/mimeo/config/mimeo_config.py
 src/mimeo/consumers/__init__.py
 src/mimeo/consumers/consumer.py
 src/mimeo/consumers/consumer_factory.py
 src/mimeo/consumers/file_consumer.py
 src/mimeo/consumers/http_consumer.py
 src/mimeo/consumers/raw_consumer.py
 src/mimeo/context/__init__.py
-src/mimeo/context/annotations.py
+src/mimeo/context/decorators.py
 src/mimeo/context/exc.py
 src/mimeo/context/mimeo_context.py
 src/mimeo/context/mimeo_context_manager.py
 src/mimeo/context/mimeo_iteration.py
 src/mimeo/database/__init__.py
 src/mimeo/database/cities.py
 src/mimeo/database/countries.py
@@ -44,17 +47,16 @@
 src/mimeo/resources/exc.py
 src/mimeo/resources/forenames.csv
 src/mimeo/resources/logging.yaml
 src/mimeo/resources/surnames.txt
 src/mimeo/utils/__init__.py
 src/mimeo/utils/exc.py
 src/mimeo/utils/mimeo_utils.py
-src/mimeo/utils/renderer.py
+src/mimeo/utils/renderers.py
 src/mimeograph.egg-info/PKG-INFO
 src/mimeograph.egg-info/SOURCES.txt
 src/mimeograph.egg-info/dependency_links.txt
 src/mimeograph.egg-info/entry_points.txt
 src/mimeograph.egg-info/requires.txt
 src/mimeograph.egg-info/top_level.txt
-tests/test_mimeo_cli.py
 tests/test_mimeograph.py
 tests/test_tools.py
```

### Comparing `mimeograph-0.4.1/tests/test_mimeograph.py` & `mimeograph-0.4.2/tests/test_mimeograph.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     yield
     # Teardown
     shutil.rmtree("test_mimeograph-dir")
 
 
 def test_produce():
     config = {
-        "output_format": "xml",
-        "indent": 4,
-        "xml_declaration": True,
         "output_details": {
             "direction": "file",
+            "format": "xml",
+            "indent": 4,
+            "xml_declaration": True,
             "directory_path": "test_mimeograph-dir",
             "file_name": "output"
         },
         "_templates_": [
             {
                 "count": 10,
                 "model": {
@@ -40,15 +40,15 @@
         ]
     }
     mimeo_config = MimeoConfig(config)
     with MimeoContextManager(mimeo_config):
         mimeo = Mimeograph(mimeo_config)
 
         assert not path.exists("test_mimeograph-dir")
-        mimeo.produce()
+        mimeo.process()
         assert path.exists("test_mimeograph-dir")
         for i in range(1, 11):
             file_path = f"test_mimeograph-dir/output-{i}.xml"
             assert path.exists(file_path)
 
             with open(file_path, "r") as file_content:
                 assert file_content.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
```

