# Comparing `tmp/common-test-29.9.24.tar.gz` & `tmp/common-test-29.9.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.24.tar", last modified: Thu Apr 27 05:56:13 2023, max compression
+gzip compressed data, was "common-test-29.9.25.tar", last modified: Thu May  4 06:22:01 2023, max compression
```

## Comparing `common-test-29.9.24.tar` & `common-test-29.9.25.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.145079 common-test-29.9.24/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-27 05:56:13.145620 common-test-29.9.24/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.106168 common-test-29.9.24/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.24/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.108386 common-test-29.9.24/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.24/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.24/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.24/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.24/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.111274 common-test-29.9.24/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.24/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.24/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.24/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.24/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.112285 common-test-29.9.24/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.24/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.114844 common-test-29.9.24/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.24/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17498 2023-04-24 05:17:14.000000 common-test-29.9.24/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.24/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.119747 common-test-29.9.24/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.24/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.125156 common-test-29.9.24/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.24/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11776 2023-04-27 05:55:54.000000 common-test-29.9.24/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.24/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.126164 common-test-29.9.24/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.24/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.130190 common-test-29.9.24/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.24/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.24/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.140271 common-test-29.9.24/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.24/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.24/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.24/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3908 2023-04-23 08:05:34.000000 common-test-29.9.24/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    11215 2023-04-24 05:43:36.000000 common-test-29.9.24/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.24/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.24/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.143609 common-test-29.9.24/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-27 05:56:13.147838 common-test-29.9.24/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-27 05:55:54.000000 common-test-29.9.24/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.683143 common-test-29.9.25/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-04 06:22:01.683347 common-test-29.9.25/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.651921 common-test-29.9.25/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.25/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.653728 common-test-29.9.25/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.25/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.25/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.25/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.25/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.655934 common-test-29.9.25/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.25/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.25/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3551 2023-05-04 02:54:16.000000 common-test-29.9.25/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.25/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.656784 common-test-29.9.25/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.25/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.658461 common-test-29.9.25/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.25/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17403 2023-05-04 01:35:15.000000 common-test-29.9.25/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.25/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.661200 common-test-29.9.25/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.25/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.669298 common-test-29.9.25/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.25/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11195 2023-05-04 01:28:37.000000 common-test-29.9.25/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.25/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.670060 common-test-29.9.25/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.25/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.673501 common-test-29.9.25/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.25/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.25/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-05-04 02:54:16.000000 common-test-29.9.25/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.679717 common-test-29.9.25/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.25/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.25/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.25/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7982 2023-05-04 02:29:22.000000 common-test-29.9.25/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6732 2023-05-04 05:54:33.000000 common-test-29.9.25/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.25/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    11215 2023-04-24 05:43:36.000000 common-test-29.9.25/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.25/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.25/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.682658 common-test-29.9.25/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-04 06:22:01.684225 common-test-29.9.25/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-27 05:55:54.000000 common-test-29.9.25/setup.py
```

### Comparing `common-test-29.9.24/PKG-INFO` & `common-test-29.9.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.24
+Version: 29.9.25
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.24/common/autotest/base_requests.py` & `common-test-29.9.25/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/autotest/handle_allure.py` & `common-test-29.9.25/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/autotest/handle_assert.py` & `common-test-29.9.25/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/common/api_driver.py` & `common-test-29.9.25/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/common/constant.py` & `common-test-29.9.25/common/common/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     CASE_TYPE_AUTO = "自动化"
     CASE_TYPE_Man = "手工"
 
     #配置
     ENV = 'env'
     Jenkins_RESULT = 'Result'
     PROJECT_NAME = 'projectname'
+    PROJECT_ALICE = 'ProjectAlice'
     PORJECT_ID = 'projectId'
     ISSUE_KEY = 'issueKey'
     TEST_TYPE = 'type'
     PASS_RATE = 'passrate'
     CURRENT_PATH = 'currentpath'
     TEST_CASE_PATH = 'TestCasePath'
     TEST_CASE_MARK = 'TestCaseMark'
@@ -109,14 +110,15 @@
     MSG_URL = 'msgapi'
     MSG_TOKEN= 'msgtoken'
     MSG_id = 'msgid'
 
     # ATF配置：
     ATF_URL_API='http://10.18.20.175:9999/api'
     ATF_URL = 'http://10.18.20.175:9999'
+    ATF_API = 'http://10.18.20.175:9996/autotest/api'
 
     #Python服务配置
     ATF_PYTHON_URL = 'http://10.18.20.175:5000'
 
     #浏览器类型
     USER_AGENTS = [
         "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2228.0 Safari/537.36",
```

### Comparing `common-test-29.9.24/common/common/test.py` & `common-test-29.9.25/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/config/config.py` & `common-test-29.9.25/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/data/data_process.py` & `common-test-29.9.25/common/data/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from common.config.config import TEST_FILE_PATH, TEST_DATA_PATH
 from common.data.handle_common import req_expr, convert_json,format_caseName,get_system_key
 from common.common.constant import Constant
 from common.file.ReadFile import get_yaml_config
 from jsonschema import validate
 from jsonschema.exceptions import SchemaError, ValidationError
 from common.db.handle_db import MysqlDB
+from common.plat.service_platform import ServicePlatForm
 
 
 class DataProcess:
     response_dict = {}
     @classmethod
     def save_response(cls, key: str, value: object) -> None:
         """
@@ -340,25 +341,23 @@
             ts = int(time.mktime(time.strptime(_date, "%Y-%m-%d")))
         return ts
 
     @classmethod
     def check_test_data(self, testdatas:list):
         _testDatas=[]
         try:
-            _config = {'key': 'traffic', 'env': 'test'}
-            _mysql = MysqlDB(_config)
             for testdata in testdatas:
                 casename = format_caseName(testdata[Constant.CASE_TITLE])
-                if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(
-                        get_system_key(Constant.TEST_SRTCYCLE_ID)):
-                    jirakey = get_system_key(Constant.ISSUE_KEY)
+                if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
                     cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-                    _sql = f"select * from `traffic_test`.`test_autotest_run` where jirakey='{jirakey}' and `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and casename='{casename}'"
-                    _info = _mysql.execute(_sql).fetchall()
-                    if len(_info) > 0:
+                    caserunid = ServicePlatForm.getCaseByCycle(cycleId, casename, Constant.STATUS_PRE, caseNo)[
+                        'caserunid']
+                    logger.info(
+                        f'获取周期编号：{cycleId} 用例名称:{casename} 状态:{Constant.STATUS_PRE} 用例编号:{caseNo}  运行编号:{caserunid}')
+                    if caserunid != '00000':
                         _testDatas.append(testdata)
                 else:
                     if Constant.CASE_STATUS in testdata:
                         if testdata[Constant.CASE_STATUS].strip() != '否':
                             _testDatas.append(testdata)
                     else:
                         _testDatas.append(testdata)
```

### Comparing `common-test-29.9.24/common/data/handle_common.py` & `common-test-29.9.25/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/db/handle_db.py` & `common-test-29.9.25/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/db/handle_db_batch.py` & `common-test-29.9.25/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/db/handle_mysqldb.py` & `common-test-29.9.25/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/db/handle_oracle.py` & `common-test-29.9.25/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/db/handle_sqlserver.py` & `common-test-29.9.25/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/file/ReadFile.py` & `common-test-29.9.25/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/file/handle_excel.py` & `common-test-29.9.25/common/file/handle_excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import openpyxl
+import xlrd
 from common.plugin.data_bus import DataBus
 from datetime import datetime
 from xlrd import xldate_as_tuple
 from xlutils.copy import copy
-import xlrd
 from common.file.handle_system import adjust_path_data,adjust_path
 from common.data.handle_common import get_system_key, format_caseName,print_info
-from common.db.handle_db import MysqlDB
+from common.plat.service_platform import ServicePlatForm
 from common.common.constant import Constant
 from loguru import logger
 from common.data.data_process import DataProcess
 
 
 def is_josn(inStr):
     try:
@@ -223,55 +223,43 @@
             if ctype == 3:
                 date = datetime(*xldate_as_tuple(cell_data, 0))
                 cell_data = date.strftime('%Y-%m-%d')
             col_title = sh.cell_value(0, col).strip()
             d[col_title] = cell_data
             d['$'+col_title] = cell_data
             d[col_title+'_cell'] = {"row": row, "col": col}
-        if check_excel_data(d, _mysql, _filter, _checkData):
+        if check_excel_data(d, _filter, _checkData):
             if _replace:
                 temp = DataBus.get_data(d)
                 temp['_excelPath'] = data_file
                 temp['_sheetName'] = sheet
             else:
                 temp = d
                 temp['_excelPath'] = data_file
                 temp['_sheetName'] = sheet
             print_info(f'添加单个参数化用例数据: {temp}')
             data_list.append(temp)
         print_info(f'用例参数化数据: {data_list}')
     return data_list
 
-
-
-def check_excel_data(testdata:dict, _mysql, _filter, _checkData):
+def check_excel_data(testdata:dict, _filter, _checkData):
     if _checkData:
         casename = format_caseName(testdata[Constant.CASE_TITLE])
         caseNo = testdata[Constant.CASE_NO]
         if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
             return True
         if DataProcess.isNotNull(casename) == False or DataProcess.isNotNull(caseNo) == False:
             return False
-        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)) and _mysql is not None:
+        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
             cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-            _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and casename='{casename}'"
-            _mysql = MysqlDB({'key': 'traffic', 'env': 'test'})
-            _info = _mysql.execute(_sql).fetchall()
-            if len(_info) < 1:
-                _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and caseid='{caseNo}'"
-                _info = _mysql.execute(_sql).fetchall()
-
-            if len(_info) < 1:
-                _mysql.close()
+            caserunid = ServicePlatForm.getCaseByCycle(cycleId, casename, Constant.STATUS_PRE, caseNo)['caserunid']
+            logger.info(f'获取周期编号：{cycleId} 用例名称:{casename} 状态:{Constant.STATUS_PRE} 用例编号:{caseNo}  运行编号:{caserunid}')
+            if caserunid == '00000':
                 return False
             else:
-                _temp = _info[0]
-                logger.info(f"执行参数化用例编号:{_temp['caseid']} 用例名称：{_temp['casename']}  运行ID:{_temp['caserunid']} ")
-                print_info(f'执行参数化测试数据: {testdata}')
-                _mysql.close()
                 return True
         if testdata[Constant.CASE_STATUS].strip() == '否':
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
             if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
                 return True
             else:
```

### Comparing `common-test-29.9.24/common/file/handle_file.py` & `common-test-29.9.25/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/file/handle_reques.py` & `common-test-29.9.25/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/file/handle_system.py` & `common-test-29.9.25/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/file/handle_yaml.py` & `common-test-29.9.25/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/mq/handle_rabbit.py` & `common-test-29.9.25/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plat/ATF_platform.py` & `common-test-29.9.25/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plat/jenkin_platform.py` & `common-test-29.9.25/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plat/jira_platform.py` & `common-test-29.9.25/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plat/mysql_platform.py` & `common-test-29.9.25/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/allure_plugin.py` & `common-test-29.9.25/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/assert_plugin.py` & `common-test-29.9.25/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/atf_plugin.py` & `common-test-29.9.25/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,33 @@
             _result, _desc = ATFPlugin.getResultData(report_html_path)
             ATFPlugin.syncJiraCase()
             if _result['result'] == 'success':
                 JiraPlatForm.setJiraFlowStatus("2551")
             if DataProcess.isNotNull(get_system_key(Constant.SEND_URSER_LIST)):
                 logger.info('推送结果到MUC')
                 _userList = get_system_key(Constant.SEND_URSER_LIST).split(',')
-                ServicePlatForm.sendMsg(_desc, _userList)
+                self.sendMsg(_desc, _userList)
             dict = {"issuekey": f'{_result["jirakey"]}', "project": f'{_result["projectName"]}',
                     "result": f'{_result["result"]}'}
             ATFPlatForm.runDeploy("AutoTest-Result", dict)
             #JiraPlatForm.setJiraComment(_desc)
 
 
+    @classmethod
+    def sendMsg(self, content, _list):
+        for _index in range(len(_list)):
+            _arr = str(_list[_index]).split('&')
+            os.environ['toUserId'] = str(_arr[0]).lower()
+            os.environ['toMail'] = str(_arr[1])
+            DataBus.set_key('content',content)
+            _data = FilePlugin.load_file("muc.xml",file_path=CONFIG_PATH)
+            ServicePlatForm.sendMsg(_data)
+
+
+
 
     @classmethod
     def getResultData(self, report_html_path):
         _summary = FilePlugin.load_json(f'{report_html_path}/widgets/summary.json')
         _result = dict()
         _result['projectId'] = ""
         _result['projectName'] = ""
```

### Comparing `common-test-29.9.24/common/plugin/data_bus.py` & `common-test-29.9.25/common/plugin/data_bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from common.common.constant import Constant
 from common.data.data_process import DataProcess
 from common.data.handle_common import get_system_key, set_system_key, print_databus_info
 from common.file.ReadFile import get_yaml_config
 from common.file.handle_file import get_item
 from common.plat.ATF_platform import ATFPlatForm
+from common.plat.service_platform import ServicePlatForm
 from loguru import logger
 
 
 class DataBus(object):
 
     @classmethod
     def get_key(cls,_key):
@@ -122,25 +123,41 @@
 
     @classmethod
     def get_env(cls):
         """
         获取当前环境
         :return:
         """
-        return get_system_key('env')
+        return get_system_key(Constant.ENV)
+
+    @classmethod
+    def get_data_atf(cls):
+        """
+        获取当前环境ATF配置数据
+        :return:
+        """
+        env = cls.get_env()
+        projectAlice = get_system_key(Constant.PROJECT_ALICE)
+        _data = ServicePlatForm.getATFData(projectAlice, env)
+        for temp in _data:
+            if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
+                cls.set_key(temp['_key'], temp['_value'])
+            else:
+                cls.set_key(temp['_key'], temp['_value'], False)
 
     @classmethod
     def save_init_data(cls):
         """
         初始化DataBus数据
         :return:
         """
         cls.save_yaml('common.setting',_replace=False)
         cls.save_yaml('common')
         cls.save_yaml(cls.get_env())
+        cls.get_data_atf()
         cls.get_param()
 
     @classmethod
     def run_info(cls):
         """
         打印信息
         :return:
@@ -163,7 +180,14 @@
         print_databus_info(Constant.RUN_TYPE, "运行方式")
         print_databus_info(Constant.ENV, "运行环境")
         print_databus_info(Constant.PASS_RATE,"预期通过率")
         print_databus_info(Constant.SEND_URSER_LIST, "通知人列表")
 
 
 
+if __name__ == '__main__':
+    DataBus.set_key('RuntType',"3343434")
+    DataBus.save_init_data()
+    print(os.environ.values())
+
+
+
```

### Comparing `common-test-29.9.24/common/plugin/data_plugin.py` & `common-test-29.9.25/common/plugin/data_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from typing import Iterable
 from common.plugin.data_bus import DataBus
 import xmltodict
 from common.data.data_process import DataProcess
 from common.data.handle_common import req_expr, convert_json, extractor
 
+
 class DataPlugin(object):
     @classmethod
     def convert_json(self, _temp, _replace: bool = True):
         """
         任意的数据类型转换成Json
         :param _temp:
         :param _replace: 是否清洗数据
@@ -118,17 +119,14 @@
     def get_date(self, now):
        return DataProcess.getDate(now)
 
 
 
 if __name__ == '__main__':
     DataBus.set_key('883434','9999999')
-    _xml=DataPlugin.dict_convert_xml({"abc":{'ticketNo':'883334','registrationNo':'733','subFrom':DataBus.get_key('883434')}})
-    print(DataPlugin.xml_convert_dict(_xml))
-    print(_xml)
```

### Comparing `common-test-29.9.24/common/plugin/file_plugin.py` & `common-test-29.9.25/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/hooks_plugin.py` & `common-test-29.9.25/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/pytest_playwright.py` & `common-test-29.9.25/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common/plugin/pytest_plugin.py` & `common-test-29.9.25/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common_test.egg-info/PKG-INFO` & `common-test-29.9.25/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.24
+Version: 29.9.25
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.24/common_test.egg-info/SOURCES.txt` & `common-test-29.9.25/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/common_test.egg-info/requires.txt` & `common-test-29.9.25/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.24/setup.py` & `common-test-29.9.25/setup.py`

 * *Files identical despite different names*

