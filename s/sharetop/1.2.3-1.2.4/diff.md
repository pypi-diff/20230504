# Comparing `tmp/sharetop-1.2.3.tar.gz` & `tmp/sharetop-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.2.3.tar", last modified: Wed May  3 13:46:06 2023, max compression
+gzip compressed data, was "sharetop-1.2.4.tar", last modified: Thu May  4 04:13:57 2023, max compression
```

## Comparing `sharetop-1.2.3.tar` & `sharetop-1.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.672424 sharetop-1.2.3/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    39532 2023-05-03 13:46:06.672424 sharetop-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    38260 2023-05-02 15:48:40.000000 sharetop-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 13:46:06.672424 sharetop-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.274110 sharetop-1.2.3/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.2.3/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-03 13:45:48.000000 sharetop-1.2.3/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.292267 sharetop-1.2.3/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.2.3/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.311683 sharetop-1.2.3/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.2.3/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.2.3/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.354522 sharetop-1.2.3/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.2.3/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.390549 sharetop-1.2.3/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.2.3/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.2.3/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.2.3/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.2.3/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.2.3/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.428268 sharetop-1.2.3/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.2.3/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     2374 2023-05-02 15:19:23.000000 sharetop-1.2.3/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.2.3/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12300 2023-05-02 15:02:38.000000 sharetop-1.2.3/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.2.3/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.514090 sharetop-1.2.3/sharetop/core/fund/
--rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.2.3/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.2.3/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.2.3/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.2.3/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.2.3/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.2.3/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.538196 sharetop-1.2.3/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.2.3/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.2.3/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.598254 sharetop-1.2.3/sharetop/core/stock/
--rw-rw-rw-   0        0        0      569 2023-05-02 15:39:30.000000 sharetop-1.2.3/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.2.3/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.2.3/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14302 2023-05-02 01:29:25.000000 sharetop-1.2.3/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.2.3/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.2.3/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.2.3/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.2.3/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.614078 sharetop-1.2.3/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.2.3/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.2.3/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2873 2023-05-02 14:46:41.000000 sharetop-1.2.3/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.638480 sharetop-1.2.3/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.2.3/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     3678 2023-05-03 06:46:06.000000 sharetop-1.2.3/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     1948 2023-05-02 15:34:17.000000 sharetop-1.2.3/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.672424 sharetop-1.2.3/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.2.3/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.2.3/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.2.3/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.2.3/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      151 2023-05-03 07:12:44.000000 sharetop-1.2.3/sharetop/test/test4.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:46:06.292267 sharetop-1.2.3/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39532 2023-05-03 13:46:06.000000 sharetop-1.2.3/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1715 2023-05-03 13:46:06.000000 sharetop-1.2.3/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:46:06.000000 sharetop-1.2.3/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-03 13:46:06.000000 sharetop-1.2.3/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 13:46:06.000000 sharetop-1.2.3/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.167508 sharetop-1.2.4/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    39532 2023-05-04 04:13:57.166507 sharetop-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    38260 2023-05-02 15:48:40.000000 sharetop-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 04:13:57.167508 sharetop-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.069973 sharetop-1.2.4/sharetop/
+-rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.2.4/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-05-04 04:13:40.000000 sharetop-1.2.4/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.120562 sharetop-1.2.4/sharetop/api/
+-rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.2.4/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.122562 sharetop-1.2.4/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.2.4/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.127839 sharetop-1.2.4/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.2.4/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.131838 sharetop-1.2.4/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.2.4/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.2.4/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.2.4/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.2.4/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.134838 sharetop-1.2.4/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.2.4/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     2374 2023-05-02 15:19:23.000000 sharetop-1.2.4/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.2.4/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12266 2023-05-04 04:12:59.000000 sharetop-1.2.4/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.2.4/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.147263 sharetop-1.2.4/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.2.4/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.2.4/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.2.4/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.2.4/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.149363 sharetop-1.2.4/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.2.4/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.2.4/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.154843 sharetop-1.2.4/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      569 2023-05-02 15:39:30.000000 sharetop-1.2.4/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.2.4/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.2.4/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14302 2023-05-02 01:29:25.000000 sharetop-1.2.4/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.2.4/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.2.4/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.2.4/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.160153 sharetop-1.2.4/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.2.4/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.2.4/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2873 2023-05-02 14:46:41.000000 sharetop-1.2.4/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.163507 sharetop-1.2.4/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.2.4/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     3678 2023-05-03 06:46:06.000000 sharetop-1.2.4/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     1948 2023-05-02 15:34:17.000000 sharetop-1.2.4/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.166507 sharetop-1.2.4/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.2.4/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.2.4/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.2.4/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.2.4/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.2.4/sharetop/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:13:57.119563 sharetop-1.2.4/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    39532 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1715 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 04:13:57.000000 sharetop-1.2.4/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.2.3/LICENSE` & `sharetop-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/PKG-INFO` & `sharetop-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.2.3
+Version: 1.2.4
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.2.3/README.md` & `sharetop-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/setup.py` & `sharetop-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/application/base.py` & `sharetop-1.2.4/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/bond/__init__.py` & `sharetop-1.2.4/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/bond/config.py` & `sharetop-1.2.4/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/bond/get_bond_info.py` & `sharetop-1.2.4/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.2.4/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/cache.py` & `sharetop-1.2.4/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/common/common_base.py` & `sharetop-1.2.4/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/common/config.py` & `sharetop-1.2.4/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/common/getter.py` & `sharetop-1.2.4/sharetop/core/common/getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
         **kwargs
 ) -> pd.DataFrame:
     """
         获取单只股票、债券 实时的基本数据
     """
     columns = list(EM_REAL_TIME_FIELDS.values())
     quote_id = get_quote_id(code)
-    print("quote_id:", quote_id)
     params = {
         "fields": EM_REAL_TIME_FIELDS_PARAMS
     }
     params = quote_id_process(params, quote_id)
     url = ''.join(real_time_url_list)
     json_response = requests_obj.get(
         url, params, user_agent=False
```

### Comparing `sharetop-1.2.3/sharetop/core/config.py` & `sharetop-1.2.4/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/__init__.py` & `sharetop-1.2.4/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/fund_list.py` & `sharetop-1.2.4/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_rank.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_rank.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.2.4/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.2.4/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.2.4/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/futures/get_futures_info.py` & `sharetop-1.2.4/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/__init__.py` & `sharetop-1.2.4/sharetop/core/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/bill_monitor.py` & `sharetop-1.2.4/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/config.py` & `sharetop-1.2.4/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/getter.py` & `sharetop-1.2.4/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/quarterly_report.py` & `sharetop-1.2.4/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/stock/rank_list.py` & `sharetop-1.2.4/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/core/utils.py` & `sharetop-1.2.4/sharetop/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     if len(str(stock_code).strip()) == 0:
         raise Exception('证券代码应为长度不应为 0')
     quote = search_quote(stock_code)
     if isinstance(quote, Quote):
         return quote.quote_id
     if quote is None:
         rich.print(f'证券代码 "{stock_code}" 可能有误')
-        return ''
+        return stock_code
 
 
 def process_dataframe_and_series(
     function_fields: Dict[str, Callable] = dict(),
     remove_columns_and_indexes: List[str] = list(),
 ):
     """
```

### Comparing `sharetop-1.2.3/sharetop/crawl/base.py` & `sharetop-1.2.4/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/crawl/settings.py` & `sharetop-1.2.4/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/parser/base.py` & `sharetop-1.2.4/sharetop/parser/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/parser/config.py` & `sharetop-1.2.4/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/test/test2-akshare.py` & `sharetop-1.2.4/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop/test/test3.py` & `sharetop-1.2.4/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.2.3/sharetop.egg-info/PKG-INFO` & `sharetop-1.2.4/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.2.3
+Version: 1.2.4
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.2.3/sharetop.egg-info/SOURCES.txt` & `sharetop-1.2.4/sharetop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

