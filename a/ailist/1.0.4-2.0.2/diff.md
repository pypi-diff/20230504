# Comparing `tmp/ailist-1.0.4.tar.gz` & `tmp/ailist-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailist-1.0.4.tar", last modified: Tue Jan  4 02:37:33 2022, max compression
+gzip compressed data, was "ailist-2.0.2.tar", max compression
```

## Comparing `ailist-1.0.4.tar` & `ailist-2.0.2.tar`

### file list

```diff
@@ -1,93 +1,64 @@
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-04 02:37:33.705710 ailist-1.0.4/
--rwxr--r--   0 ksmith10 (271238760) 633320910    17895 2019-08-12 18:05:36.000000 ailist-1.0.4/LICENSE.md
--rw-r--r--   0 ksmith10 (271238760) 633320910       44 2022-01-04 02:31:53.000000 ailist-1.0.4/MANIFEST.in
--rw-r--r--   0 ksmith10 (271238760) 633320910     7686 2022-01-04 02:37:33.706054 ailist-1.0.4/PKG-INFO
--rwxr--r--   0 ksmith10 (271238760) 633320910     4923 2021-08-28 14:14:30.000000 ailist-1.0.4/README.md
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-04 02:37:33.674192 ailist-1.0.4/ailist/
--rw-r--r--   0 ksmith10 (271238760) 633320910  1569938 2021-12-09 20:53:57.000000 ailist-1.0.4/ailist/AIList_core.c
--rwxr--r--   0 ksmith10 (271238760) 633320910    11530 2021-06-08 19:16:29.000000 ailist-1.0.4/ailist/AIList_core.pxd
--rwxr--r--   0 ksmith10 (271238760) 633320910    37671 2021-06-08 19:19:03.000000 ailist-1.0.4/ailist/AIList_core.pyx
--rw-r--r--   0 ksmith10 (271238760) 633320910  1691773 2021-12-09 20:53:58.000000 ailist-1.0.4/ailist/IntervalArray_core.c
--rwxr--r--   0 ksmith10 (271238760) 633320910    12248 2021-02-15 15:58:22.000000 ailist-1.0.4/ailist/IntervalArray_core.pxd
--rwxr--r--   0 ksmith10 (271238760) 633320910    45104 2021-02-15 15:59:41.000000 ailist-1.0.4/ailist/IntervalArray_core.pyx
--rw-r--r--   0 ksmith10 (271238760) 633320910   391220 2021-12-09 20:53:58.000000 ailist-1.0.4/ailist/Interval_core.c
--rwxr--r--   0 ksmith10 (271238760) 633320910      815 2021-02-11 02:16:32.000000 ailist-1.0.4/ailist/Interval_core.pxd
--rwxr--r--   0 ksmith10 (271238760) 633320910     2234 2021-02-03 18:39:09.000000 ailist-1.0.4/ailist/Interval_core.pyx
--rw-r--r--   0 ksmith10 (271238760) 633320910  1901371 2021-12-13 20:56:08.000000 ailist-1.0.4/ailist/LabeledIntervalArray_core.c
--rw-r--r--   0 ksmith10 (271238760) 633320910    21353 2021-09-08 15:23:11.000000 ailist-1.0.4/ailist/LabeledIntervalArray_core.pxd
--rw-r--r--   0 ksmith10 (271238760) 633320910    65161 2021-12-13 20:50:22.000000 ailist-1.0.4/ailist/LabeledIntervalArray_core.pyx
--rw-r--r--   0 ksmith10 (271238760) 633320910   410470 2021-12-09 20:54:00.000000 ailist-1.0.4/ailist/LabeledInterval_core.c
--rwxr--r--   0 ksmith10 (271238760) 633320910      999 2021-04-19 17:28:24.000000 ailist-1.0.4/ailist/LabeledInterval_core.pxd
--rwxr--r--   0 ksmith10 (271238760) 633320910     2734 2021-06-01 03:04:41.000000 ailist-1.0.4/ailist/LabeledInterval_core.pyx
--rwxr--r--   0 ksmith10 (271238760) 633320910      569 2022-01-04 02:37:13.000000 ailist-1.0.4/ailist/__init__.py
--rw-r--r--   0 ksmith10 (271238760) 633320910   301798 2021-12-09 20:54:00.000000 ailist-1.0.4/ailist/array_query_core.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1062 2021-02-05 17:59:48.000000 ailist-1.0.4/ailist/array_query_core.pxd
--rwxr--r--   0 ksmith10 (271238760) 633320910     1406 2021-02-04 16:17:10.000000 ailist-1.0.4/ailist/array_query_core.pyx
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-04 02:37:33.702768 ailist-1.0.4/ailist/src/
--rw-r--r--   0 ksmith10 (271238760) 633320910     1795 2021-02-09 19:52:25.000000 ailist-1.0.4/ailist/src/aiarray_add.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3214 2021-02-08 18:41:49.000000 ailist-1.0.4/ailist/src/aiarray_construct.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3743 2021-01-15 18:28:18.000000 ailist-1.0.4/ailist/src/aiarray_coverage.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1012 2021-02-02 18:49:19.000000 ailist-1.0.4/ailist/src/aiarray_extract.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2217 2021-02-15 15:31:35.000000 ailist-1.0.4/ailist/src/aiarray_filter.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     4246 2021-02-09 19:54:31.000000 ailist-1.0.4/ailist/src/aiarray_index.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3552 2021-02-09 19:29:55.000000 ailist-1.0.4/ailist/src/aiarray_merge.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2533 2020-12-21 18:54:09.000000 ailist-1.0.4/ailist/src/aiarray_nhits.c
--rw-r--r--   0 ksmith10 (271238760) 633320910    10421 2021-02-04 23:27:36.000000 ailist-1.0.4/ailist/src/aiarray_ops.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     8491 2021-02-10 00:36:48.000000 ailist-1.0.4/ailist/src/aiarray_query.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3617 2020-12-21 18:55:01.000000 ailist-1.0.4/ailist/src/aiarray_wps.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1878 2021-02-04 20:43:19.000000 ailist-1.0.4/ailist/src/ailist_add.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3203 2021-02-04 23:09:27.000000 ailist-1.0.4/ailist/src/ailist_construct.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3738 2021-01-30 21:10:54.000000 ailist-1.0.4/ailist/src/ailist_coverage.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1004 2021-02-01 19:00:33.000000 ailist-1.0.4/ailist/src/ailist_extract.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1654 2021-02-01 16:36:22.000000 ailist-1.0.4/ailist/src/ailist_filter.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1561 2021-02-04 23:14:59.000000 ailist-1.0.4/ailist/src/ailist_index.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3059 2021-09-27 02:46:23.000000 ailist-1.0.4/ailist/src/ailist_iter.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1368 2021-02-04 23:16:11.000000 ailist-1.0.4/ailist/src/ailist_merge.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2520 2020-10-19 17:22:45.000000 ailist-1.0.4/ailist/src/ailist_nhits.c
--rw-r--r--   0 ksmith10 (271238760) 633320910    10990 2021-02-04 23:05:45.000000 ailist-1.0.4/ailist/src/ailist_ops.c
--rw-r--r--   0 ksmith10 (271238760) 633320910    10760 2021-02-01 18:58:23.000000 ailist-1.0.4/ailist/src/ailist_query.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3612 2020-10-19 17:27:23.000000 ailist-1.0.4/ailist/src/ailist_wps.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1631 2019-11-12 16:41:08.000000 ailist-1.0.4/ailist/src/array_query_utilities.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1174 2021-01-14 20:03:59.000000 ailist-1.0.4/ailist/src/array_query_utilities.h
--rwxr--r--   0 ksmith10 (271238760) 633320910     2501 2021-02-20 21:47:58.000000 ailist-1.0.4/ailist/src/augmented_interval_array.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     8754 2021-02-15 15:33:21.000000 ailist-1.0.4/ailist/src/augmented_interval_array.h
--rwxr--r--   0 ksmith10 (271238760) 633320910     2463 2021-02-04 23:13:03.000000 ailist-1.0.4/ailist/src/augmented_interval_list.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     8268 2021-06-08 19:15:36.000000 ailist-1.0.4/ailist/src/augmented_interval_list.h
--rw-r--r--   0 ksmith10 (271238760) 633320910      804 2021-02-03 17:09:02.000000 ailist-1.0.4/ailist/src/interval.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1088 2021-02-03 17:08:42.000000 ailist-1.0.4/ailist/src/interval.h
--rw-r--r--   0 ksmith10 (271238760) 633320910    21510 2021-04-26 19:06:11.000000 ailist-1.0.4/ailist/src/khash.h
--rw-r--r--   0 ksmith10 (271238760) 633320910     5245 2021-08-28 19:51:43.000000 ailist-1.0.4/ailist/src/labeled_aiarray_add.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     5872 2021-04-23 16:08:33.000000 ailist-1.0.4/ailist/src/labeled_aiarray_construct.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2722 2021-05-10 18:03:26.000000 ailist-1.0.4/ailist/src/labeled_aiarray_coverage.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1083 2021-02-20 03:38:24.000000 ailist-1.0.4/ailist/src/labeled_aiarray_extract.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2761 2021-05-10 18:05:39.000000 ailist-1.0.4/ailist/src/labeled_aiarray_filter.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     8854 2022-01-03 04:28:50.000000 ailist-1.0.4/ailist/src/labeled_aiarray_get.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1126 2021-06-08 02:45:28.000000 ailist-1.0.4/ailist/src/labeled_aiarray_has_hit.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     7312 2021-06-07 18:38:33.000000 ailist-1.0.4/ailist/src/labeled_aiarray_index.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     3813 2021-09-27 02:47:47.000000 ailist-1.0.4/ailist/src/labeled_aiarray_iter.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     1838 2022-01-03 04:00:12.000000 ailist-1.0.4/ailist/src/labeled_aiarray_match.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     2821 2021-09-08 15:22:43.000000 ailist-1.0.4/ailist/src/labeled_aiarray_merge.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     5821 2021-06-02 16:14:15.000000 ailist-1.0.4/ailist/src/labeled_aiarray_nhits.c
--rw-r--r--   0 ksmith10 (271238760) 633320910    19677 2021-12-13 20:58:42.000000 ailist-1.0.4/ailist/src/labeled_aiarray_query.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     5651 2021-04-16 15:55:56.000000 ailist-1.0.4/ailist/src/labeled_aiarray_wps.c
--rw-r--r--   0 ksmith10 (271238760) 633320910     5113 2021-05-15 19:11:29.000000 ailist-1.0.4/ailist/src/labeled_augmented_array.c
--rwxr--r--   0 ksmith10 (271238760) 633320910    16293 2021-09-08 15:23:02.000000 ailist-1.0.4/ailist/src/labeled_augmented_array.h
--rw-r--r--   0 ksmith10 (271238760) 633320910      898 2021-05-08 14:50:27.000000 ailist-1.0.4/ailist/src/labeled_interval.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1190 2021-05-08 14:51:00.000000 ailist-1.0.4/ailist/src/labeled_interval.h
--rwxr--r--   0 ksmith10 (271238760) 633320910     1705 2021-02-10 20:32:11.000000 ailist-1.0.4/ailist/src/overlap_index.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     1834 2021-05-10 17:36:00.000000 ailist-1.0.4/ailist/src/overlap_label_index.c
--rwxr--r--   0 ksmith10 (271238760) 633320910     3103 2021-02-20 22:03:14.000000 ailist-1.0.4/ailist/src/utilities.h
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-04 02:37:33.676220 ailist-1.0.4/ailist.egg-info/
--rw-r--r--   0 ksmith10 (271238760) 633320910     7686 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/PKG-INFO
--rw-r--r--   0 ksmith10 (271238760) 633320910     2475 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/SOURCES.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910        1 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/dependency_links.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910        1 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/not-zip-safe
--rw-r--r--   0 ksmith10 (271238760) 633320910       20 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/requires.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910        7 2022-01-04 02:37:33.000000 ailist-1.0.4/ailist.egg-info/top_level.txt
--rwxr--r--   0 ksmith10 (271238760) 633320910       79 2022-01-04 02:37:33.707596 ailist-1.0.4/setup.cfg
--rwxr--r--   0 ksmith10 (271238760) 633320910     9898 2022-01-04 02:36:59.000000 ailist-1.0.4/setup.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-04 02:37:33.704959 ailist-1.0.4/tests/
--rw-r--r--   0 ksmith10 (271238760) 633320910     1137 2021-02-09 20:06:49.000000 ailist-1.0.4/tests/benchmark.py
--rwxr--r--   0 ksmith10 (271238760) 633320910     4734 2021-02-09 23:27:54.000000 ailist-1.0.4/tests/test_AIList.py
--rwxr--r--   0 ksmith10 (271238760) 633320910     5529 2021-02-10 02:26:22.000000 ailist-1.0.4/tests/test_IntervalArray.py
--rwxr--r--   0 ksmith10 (271238760) 633320910     6136 2021-06-02 16:15:57.000000 ailist-1.0.4/tests/test_LabeledIntervalArray.py
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 ailist-2.0.2/LICENSE.md
+-rwxr-xr-x   0        0        0     4923 2021-08-28 14:14:30.000000 ailist-2.0.2/README.md
+-rw-r--r--   0        0        0   399968 2023-05-04 18:13:17.192103 ailist-2.0.2/ailist/AIList_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0    14968 2023-05-01 20:07:58.458938 ailist-2.0.2/ailist/AIList_core.pxd
+-rwxr-xr-x   0        0        0    38543 2023-05-04 15:37:04.815831 ailist-2.0.2/ailist/AIList_core.pyx
+-rw-r--r--   0        0        0    34745 2023-01-20 20:29:03.224385 ailist-2.0.2/ailist/IntervalArray_core.py
+-rw-r--r--   0        0        0    83496 2023-05-04 18:13:17.191544 ailist-2.0.2/ailist/Interval_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      721 2023-01-19 03:35:55.179175 ailist-2.0.2/ailist/Interval_core.pxd
+-rwxr-xr-x   0        0        0     1452 2023-04-12 15:43:30.386933 ailist-2.0.2/ailist/Interval_core.pyx
+-rw-r--r--   0        0        0   650384 2023-05-04 18:13:17.192531 ailist-2.0.2/ailist/LabeledIntervalArray_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0    28088 2023-04-24 14:57:56.149081 ailist-2.0.2/ailist/LabeledIntervalArray_core.pxd
+-rw-r--r--   0        0        0    78595 2023-05-04 14:58:33.650745 ailist-2.0.2/ailist/LabeledIntervalArray_core.pyx
+-rwxr-xr-x   0        0        0      536 2023-04-11 01:36:52.281521 ailist-2.0.2/ailist/__init__.py
+-rw-r--r--   0        0        0    59928 2023-05-04 18:13:17.192770 ailist-2.0.2/ailist/array_query_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0     1086 2022-05-02 21:15:59.000000 ailist-2.0.2/ailist/array_query_core.pxd
+-rwxr-xr-x   0        0        0     1304 2023-04-12 15:43:58.852105 ailist-2.0.2/ailist/array_query_core.pyx
+-rw-r--r--   0        0        0     2228 2023-04-13 02:36:16.801973 ailist-2.0.2/ailist/src/ailist/ailist_add.c
+-rw-r--r--   0        0        0     7229 2022-09-15 17:32:49.000000 ailist-2.0.2/ailist/src/ailist/ailist_construct.c
+-rw-r--r--   0        0        0     5233 2023-02-10 20:43:05.058096 ailist-2.0.2/ailist/src/ailist/ailist_coverage.c
+-rw-r--r--   0        0        0     1004 2021-02-01 19:00:33.000000 ailist-2.0.2/ailist/src/ailist/ailist_extract.c
+-rw-r--r--   0        0        0     1582 2022-06-06 03:22:03.000000 ailist-2.0.2/ailist/src/ailist/ailist_filter.c
+-rw-r--r--   0        0        0     2011 2022-06-16 14:20:03.000000 ailist-2.0.2/ailist/src/ailist/ailist_get_id.c
+-rw-r--r--   0        0        0     3192 2022-07-28 20:03:17.000000 ailist-2.0.2/ailist/src/ailist/ailist_iter.c
+-rw-r--r--   0        0        0     2009 2023-02-21 20:12:11.742021 ailist-2.0.2/ailist/src/ailist/ailist_merge.c
+-rw-r--r--   0        0        0     2758 2022-09-07 00:38:08.000000 ailist-2.0.2/ailist/src/ailist/ailist_nhits.c
+-rw-r--r--   0        0        0     5077 2023-05-04 15:00:47.219735 ailist-2.0.2/ailist/src/ailist/ailist_ops.c
+-rw-r--r--   0        0        0    16745 2023-05-04 15:30:28.093848 ailist-2.0.2/ailist/src/ailist/ailist_query.c
+-rw-r--r--   0        0        0     1066 2022-07-26 17:40:19.000000 ailist-2.0.2/ailist/src/ailist/ailist_simulate.c
+-rw-r--r--   0        0        0     3612 2020-10-19 17:27:23.000000 ailist-2.0.2/ailist/src/ailist/ailist_wps.c
+-rwxr-xr-x   0        0        0     2748 2022-09-15 14:07:25.000000 ailist-2.0.2/ailist/src/ailist/augmented_interval_list.c
+-rwxr-xr-x   0        0        0    10932 2023-04-02 18:45:52.230047 ailist-2.0.2/ailist/src/ailist/augmented_interval_list.h
+-rw-r--r--   0        0        0      804 2021-02-03 17:09:02.000000 ailist-2.0.2/ailist/src/ailist/interval.c
+-rwxr-xr-x   0        0        0     1088 2021-02-03 17:08:42.000000 ailist-2.0.2/ailist/src/ailist/interval.h
+-rwxr-xr-x   0        0        0     1714 2022-02-12 16:20:01.000000 ailist-2.0.2/ailist/src/ailist/overlap_index.c
+-rwxr-xr-x   0        0        0      981 2023-01-26 15:09:47.831548 ailist-2.0.2/ailist/src/array_query/array_query_utilities.c
+-rwxr-xr-x   0        0        0     2105 2023-01-26 15:08:56.094844 ailist-2.0.2/ailist/src/array_query/array_query_utilities.h
+-rw-r--r--   0        0        0    21510 2021-04-26 19:06:11.000000 ailist-2.0.2/ailist/src/labeled_aiarray/khash.h
+-rw-r--r--   0        0        0     2872 2023-01-25 18:17:24.561022 ailist-2.0.2/ailist/src/labeled_aiarray/kvec.h
+-rw-r--r--   0        0        0     4759 2023-05-04 15:01:55.664279 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c
+-rw-r--r--   0        0        0     1207 2023-05-01 20:57:05.670200 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_construct.c
+-rw-r--r--   0        0        0     3846 2023-02-10 20:40:34.313629 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c
+-rw-r--r--   0        0        0     1293 2022-05-11 19:58:25.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c
+-rw-r--r--   0        0        0     2333 2023-02-01 22:05:01.741865 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c
+-rw-r--r--   0        0        0     6944 2023-05-02 02:19:37.520386 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c
+-rw-r--r--   0        0        0     6160 2023-02-09 21:43:40.683985 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c
+-rw-r--r--   0        0        0     4160 2023-02-26 21:23:15.841726 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_iter.c
+-rw-r--r--   0        0        0     9856 2023-05-02 02:17:46.112410 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_match.c
+-rw-r--r--   0        0        0      937 2022-05-11 16:24:30.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_merge.c
+-rw-r--r--   0        0        0     7199 2023-02-10 20:45:56.368299 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c
+-rw-r--r--   0        0        0     2424 2023-05-04 14:53:06.390402 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_ops.c
+-rw-r--r--   0        0        0     1956 2023-02-26 21:24:15.672922 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c
+-rw-r--r--   0        0        0     5350 2023-01-26 15:10:01.828428 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c
+-rw-r--r--   0        0        0     4338 2023-05-02 02:17:29.334654 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c
+-rw-r--r--   0        0        0     6240 2023-01-25 16:50:52.952858 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c
+-rw-r--r--   0        0        0     1013 2022-07-26 19:33:03.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c
+-rw-r--r--   0        0        0     2210 2023-03-22 14:45:22.854467 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_sort.c
+-rw-r--r--   0        0        0     1299 2022-05-02 16:48:19.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_wps.c
+-rw-r--r--   0        0        0     5281 2022-09-14 17:13:56.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.c
+-rwxr-xr-x   0        0        0    20345 2023-05-02 02:18:45.419047 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.h
+-rwxr-xr-x   0        0        0     2298 2023-05-02 02:18:32.335127 ailist-2.0.2/ailist/src/labeled_aiarray/overlap_label_index.c
+-rwxr-xr-x   0        0        0     3103 2021-02-20 22:03:14.000000 ailist-2.0.2/ailist/src/utilities/utilities.h
+-rw-r--r--   0        0        0     3447 2023-04-12 15:10:52.847444 ailist-2.0.2/build.py
+-rw-r--r--   0        0        0     2109 2023-04-13 02:24:05.892680 ailist-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ailist-2.0.2/PKG-INFO
```

### Comparing `ailist-1.0.4/LICENSE.md` & `ailist-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/README.md` & `ailist-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/ailist/AIList_core.pxd` & `ailist-2.0.2/ailist/AIList_core.pxd`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 import numpy as np
 cimport numpy as np
 cimport cython
-from libc.stdint cimport uint32_t, int32_t, int64_t
-from libc.stdlib cimport malloc, free
-from ailist.Interval_core cimport Interval, interval_init, interval_t
+from libc.stdint cimport uint32_t, int64_t, uint8_t
+from ailist.Interval_core cimport Interval, interval_t
 from ailist.array_query_core cimport *
 
-cdef extern from "src/augmented_interval_list.c":
+cdef extern from "src/ailist/augmented_interval_list.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_add.c":
+cdef extern from "src/ailist/ailist_add.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_construct.c":
+cdef extern from "src/ailist/ailist_construct.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_index.c":
+cdef extern from "src/ailist/ailist_query.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+	
+cdef extern from "src/ailist/ailist_iter.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_query.c":
+cdef extern from "src/ailist/ailist_get_id.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
-	
-cdef extern from "src/ailist_iter.c":
+
+cdef extern from "src/ailist/ailist_coverage.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/ailist/ailist_nhits.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/ailist/ailist_wps.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_coverage.c":
+cdef extern from "src/ailist/ailist_merge.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_nhits.c":
+cdef extern from "src/ailist/ailist_extract.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_wps.c":
+cdef extern from "src/ailist/ailist_ops.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_merge.c":
+cdef extern from "src/ailist/ailist_filter.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_extract.c":
+cdef extern from "src/ailist/ailist_simulate.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_ops.c":
+cdef extern from "src/ailist/overlap_index.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/ailist_filter.c":
+cdef extern from "src/utilities/utilities.h":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/utilities.h":
+cdef extern from "src/array_query/array_query_utilities.h":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/augmented_interval_list.h":
+cdef extern from "src/ailist/augmented_interval_list.h":
 
 	ctypedef struct ailist_t:
 		int64_t nr, mr  					# Number of regions
 		interval_t *interval_list			# Regions data
 		uint32_t first, last				# Record range of intervals
 		int nc
 		int lenC[10]
@@ -77,14 +88,20 @@
 		ailist_t *ail						# Interval list
 		int nc								# Number of components
 		int *comp_bounds					# Label component bounds
 		int *comp_used						# Components used
 		interval_t *intv					# Interval
 		int n								# Current position
 
+	ctypedef struct overlap_index_t:
+		int size;							# Current size
+		int max_size;						# Maximum size
+		ailist_t *ail;						# Store ailist
+		long *indices;						# Store indices
+
 
 	#-------------------------------------------------------------------------------------
 	# augmented_interval_list.c
 	#=====================================================================================
 
 	# Initialize ailist_t
 	ailist_t *ailist_init() nogil
@@ -99,71 +116,123 @@
 	int ailist_max_length(ailist_t *ail) nogil
 
 	# Calculate length distribution
 	void ailist_length_distribution(ailist_t *ail, int distribution[]) nogil
 
 
 	#-------------------------------------------------------------------------------------
+	# overlap_index.c
+	#=====================================================================================
+
+	# Initialize overlap_index_t
+	overlap_index_t *overlap_index_init() nogil
+
+	# Free overlap_index memory
+	void overlap_index_destroy(overlap_index_t *oi) nogil
+
+	# Add interval and index to overlap_index
+	void overlap_index_add(overlap_index_t *aq, interval_t *i) nogil
+
+
+	#-------------------------------------------------------------------------------------
 	# ailist_add.c
 	#=====================================================================================
 
 	# Add interval to ailist_t object 
 	void ailist_add(ailist_t *ail, uint32_t start, uint32_t end, uint32_t id) nogil
 
 	# Build ailist from arrays
 	void ailist_from_array(ailist_t *ail, const long starts[], const long ends[], const long ids[], int length) nogil
 
 	# Append two ailist
 	ailist_t *ailist_append(ailist_t *ail1, ailist_t *ail2) nogil
 
+	# Copy ailist
+	ailist_t *ailist_copy(ailist_t *ail) nogil
+
 
 	#-------------------------------------------------------------------------------------
 	# ailist_construct.c
 	#=====================================================================================
 
 	# Construct ailist: decomposition and augmentation
 	void ailist_construct(ailist_t *ail, int cLen) nogil
 
+	# Construct ailist: decomposition and augmentation v0
+	void ailist_construct_v0(ailist_t *ail, int cLen) nogil
+
+	# Validation that construction ran
+	int ailist_validate_construction(ailist_t *ail) nogil
+
+	# Calculate coverage of midpoints
+	void ailist_midpoint_coverage(ailist_t *ail, double coverage[]) nogil
+
+	# Calculate coverage of midpoints with length
+	void ailist_midpoint_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length) nogil
+
+
+
 	#-------------------------------------------------------------------------------------
-	# ailist_index.c
+	# ailist_get_id.c
 	#=====================================================================================
 
 	# Get intervals with id
 	ailist_t *ailist_get_id(ailist_t *ail, int query_id) nogil
 
 	# Get intervals with ids
 	ailist_t *ailist_get_id_array(ailist_t *ail, const long ids[], int length) nogil
 
+	# Reset id_values
+	void ailist_reset_id(ailist_t *ail) nogil
+
+	# Reset id_values with shift
+	void ailist_reset_id_shift(ailist_t *ail, int shift) nogil
+
 
 	#-------------------------------------------------------------------------------------
 	# ailist_query.c
 	#=====================================================================================
 
 	# Binary search
 	uint32_t binary_search(interval_t* As, uint32_t idxS, uint32_t idxE, uint32_t qe) nogil
 
 	# Query ailist intervals
-	ailist_t *ailist_query(ailist_t *ail, uint32_t qs, uint32_t qe) nogil
+	void ailist_query(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe) nogil
 
 	# Query ailist intervals of a length
-	ailist_t *ailist_query_length(ailist_t *ail, uint32_t qs, uint32_t qe, int min_length, int max_length) nogil
+	void ailist_query_length(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe, int min_length, int max_length) nogil
+
+	# Query number of hits in ailist intervals
+	void ailist_query_nhits(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe) nogil
+
+	# Query number of hits in ailist intervals of a length
+	void ailist_query_nhits_length(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe, int min_length, int max_length) nogil
+
+	# Query if interval has any overlap in ailist intervals
+	void ailist_query_has_hit(ailist_t *ail, uint8_t *has_hit, uint32_t qs, uint32_t qe) nogil
 
 	# Query ailist intervals from arrays
-	ailist_t *ailist_query_from_array(ailist_t *ail, const long starts[], const long ends[], int length) nogil
+	void ailist_query_from_array(ailist_t *ail, ailist_t *overlaps, const long starts[], const long ends[], int length) nogil
 
 	# Query ailist intervals from another ailist
-	ailist_t *ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2) nogil
+	void ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2, ailist_t *overlaps) nogil
+
+	# Query aiarray intervals and record original index
+	void ailist_query_with_index(ailist_t *ail, overlap_index_t *overlaps, uint32_t qs, uint32_t qe) nogil
+
+	# Query aiarray intervals and record original index
+	void ailist_query_only_index(ailist_t *ail, array_query_t *aq, uint32_t qs, uint32_t qe, uint32_t id) nogil
 
 	# Query ailist interval ids from array
-	array_query_t *ailist_query_id_from_array(ailist_t *ail, const long starts[], const long ends[], const long ids[], int length) nogil
+	void ailist_query_id_from_array(ailist_t *ail, array_query_t *aq, const long starts[], const long ends[], const long ids[], int length) nogil
 
 	# Query ailist interval ids from another ailist
-	array_query_t *ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2) nogil
-	
-	
+	void ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2, array_query_t *aq) nogil
+
+
 	#-------------------------------------------------------------------------------------
 	# ailist_iter.c
 	#=====================================================================================
 
 	# Get component index
 	int *get_comp_bounds(ailist_t *ail) nogil
 
@@ -183,14 +252,17 @@
 
 	# Calculate coverage for a single interval
 	void ailist_interval_coverage(ailist_t *ail, int start, int end, int coverage[]) nogil
 
 	# Calculate coverage
 	void ailist_coverage(ailist_t *ail, double coverage[]) nogil
 
+	# Calculate coverage of a length
+	void ailist_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length) nogil
+
 	# Calculate coverage within bins
 	void ailist_bin_coverage(ailist_t *ail, double coverage[], int bin_size) nogil
 
 	# Calculate coverage within bins of a length
 	void ailist_bin_coverage_length(ailist_t *ail, double coverage[], int bin_size, int min_length, int max_length) nogil
 
 
@@ -204,18 +276,18 @@
 
 	# Determine number of hits of a length for each query interval
 	void ailist_nhits_from_array_length(ailist_t *ail, const long starts[], const long ends[],
 										int length, int nhits[], int min_length,
 										int max_length) nogil
 
 	# Calculate n hits within bins
-	void ailist_bin_nhits(ailist_t *ail, double coverage[], int bin_size) nogil
+	void ailist_bin_nhits(ailist_t *ail, long coverage[], int bin_size) nogil
 
 	# Calculate n hits of a length within bins
-	void ailist_bin_nhits_length(ailist_t *ail, double coverage[], int bin_size, int min_length, int max_length) nogil
+	void ailist_bin_nhits_length(ailist_t *ail, long coverage[], int bin_size, int min_length, int max_length) nogil
 
 	#-------------------------------------------------------------------------------------
 	# ailist_wps.c
 	#=====================================================================================
 
 	# Calculate Window Protection Score
 	void ailist_wps(ailist_t *ail, double wps[], uint32_t protection) nogil
@@ -246,37 +318,48 @@
 
 
 	#-------------------------------------------------------------------------------------
 	# ailist_ops.c
 	#=====================================================================================
 
 	# Subtract intervals from region
-	void subtract_intervals(ailist_t *ref_ail, ailist_t *result_ail, interval_t query_i, int j) nogil
+	void ailist_subtract_intervals(interval_t *intv, ailist_t *ail, ailist_t *result_ail) nogil
 
 	# Subtract two ailist_t intervals
 	ailist_t *ailist_subtract(ailist_t *ref_ail, ailist_t *query_ail) nogil
 
 	# Subtract intervals from region
-	void common_intervals(ailist_t *ref_ail, ailist_t *result_ail, interval_t query_i, int j) nogil
+	void ailist_common_intervals(interval_t *intv, ailist_t *ail, ailist_t *result_ail) nogil
 
 	# Subtract two ailist_t intervals
-	ailist_t *ailist_common(ailist_t *ref_ail, ailist_t *query_ail) nogil
+	ailist_t *ailist_common(ailist_t *ail, ailist_t *other_ail) nogil
+
+	# Union of two ailist_t intervals
+	ailist_t *ailist_union(ailist_t *ail, ailist_t *other_ail) nogil
 
 
 	#-------------------------------------------------------------------------------------
 	# ailist_filter.c
 	#=====================================================================================
 
 	# Filter ailist by length
-	ailist_t *ailist_length_filter(ailist_t *ail, int min_length, int max_length) nogil
+	void ailist_length_filter(ailist_t *ail, ailist_t *filtered_ail, int min_length, int max_length) nogil
 
 	# Randomly downsample
 	ailist_t *ailist_downsample(ailist_t *ail, double proportion) nogil
 
 
+	#-------------------------------------------------------------------------------------
+	# ailist_simulate.c
+	#=====================================================================================
+
+	# Simulate intervals
+	void ailist_simulate(ailist_t *ail, ailist_t *simulation, int n) nogil
+
+
 cpdef object rebuild_AIList(bytes data, bytes b_length)
 
 
 cdef class AIList(object):
 	"""
 	Wrapper for C ailist_t
 	"""
@@ -294,21 +377,24 @@
 	# AIList methods
 	cdef void set_list(AIList self, ailist_t *input_list)
 	cdef void _insert(AIList self, int start, int end, int id_value)
 	cdef void _construct(AIList self, int min_length)
 	cdef ailist_t *_array_id(AIList self, const long[::1] ids)
 	cdef ailist_t *_interval_id(AIList self, int id_value)
 	cdef ailist_t *_intersect(AIList self, int start, int end)
+	cdef ailist_t *_intersect_from_array(AIList self, const long[::1] starts, const long[::1] ends)
 	cdef np.ndarray _intersect_ids(AIList self, int start, int end)
 	cpdef _intersect_ids_from_array(AIList self, const long[::1] starts, const long[::1] ends, const long[::1] ids)
-	cpdef _intersect_ids_from_ailist(AIList self, AIList ail)
+	cdef ailist_t *_intersect_from_ailist(AIList self, AIList ail)
 	cdef np.ndarray _coverage(AIList self)
 	cdef np.ndarray _bin_coverage(AIList self, int bin_size)
 	cdef np.ndarray _bin_coverage_length(AIList self, int bin_size, int min_length, int max_length)
 	cdef np.ndarray _bin_nhits(AIList self, int bin_size)
 	cdef np.ndarray _bin_nhits_length(AIList self, int bin_size, int min_length, int max_length)
+	cdef void _nhits(AIList self, long *nhits, int start, int end)
+	cdef void _nhits_length(AIList self, long *nhits, int start, int end, int min_length, int max_length)
 	cdef np.ndarray _wps(AIList self, int protection)
 	cdef np.ndarray _wps_length(AIList self, int protection, int min_length, int max_length)
 	cdef np.ndarray _length_dist(AIList self)
 	cdef np.ndarray _nhits_from_array(AIList self, const long[::1] starts, const long[::1] ends)
 	cdef np.ndarray _nhits_from_array_length(AIList self, const long[::1] starts, const long[::1] ends, int min_length, int max_length)
 	cdef np.ndarray _interval_coverage(AIList self, int start, int end)
```

### Comparing `ailist-1.0.4/ailist/AIList_core.pyx` & `ailist-2.0.2/ailist/AIList_core.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 import numpy as np
 cimport numpy as np
 import math
 cimport cython
 import pandas as pd
 from libc.string cimport memcpy
+from .Interval_core import Interval
 np.import_array()
-from time import time
 
 # Set byteorder for __reduce__
 byteorder = sys.byteorder
 
 
 def get_include():
 	"""
@@ -34,22 +34,22 @@
 
 cpdef AIList rebuild_AIList(bytes data, bytes b_length):
 	"""
 	Rebuild function for __reduce__()
 
 	Parameters
 	----------
-		data : bytes 
+		data : bytes
 			Bytes representation of ailist_t
-		b_length : bytes 
+		b_length : bytes
 			Length of ailist_t
 
 	Returns
 	-------
-		c : ailist_t* 
+		c : ailist_t*
 			Translated ailist_t from data
 	"""
 
 	# Initialize new AIList
 	c = AIList()
 
 	# Build ailist from serialized data
@@ -95,17 +95,14 @@
 		pass
 
 
 	def __dealloc__(self):
 		"""
 		Free AIList.c_ailist
 		"""
-		
-		#if hasattr(self, "interval_list"):
-			#ailist_destroy(self.c_ailist)
 
 		ailist_destroy(self.c_ailist)
 
 
 	cdef bytes _get_data(self):
 		"""
 		Function to convert ailist_t to bytes
@@ -118,59 +115,60 @@
 	cdef ailist_t *_set_data(self, bytes data, bytes b_length):
 		"""
 		Function to build ailist_t object from
 		serialized bytes using __reduce__()
 
 		Parameters
 		----------
-			data : bytes 
+			data : bytes
 				Bytes representation of ailist_t
 			b_length : bytes
 				Length of ailist_t
 
 		Returns
-		---------
+		-------
 			interval_list : ailist_t*
 				Translated ailist_t for bytes
 		"""
-		
+
 		# Convert bytes to ints
 		cdef int length = int.from_bytes(b_length, byteorder)
-		
+
 		# Create new ailist_t
 		cdef ailist_t *ail = ailist_init()
 		cdef interval_t *interval_list = <interval_t*>malloc(length * sizeof(interval_t))
 		memcpy(interval_list, <char*>data, sizeof(interval_t)*length)
 
-		# Iteratively add intervals to interval_list		
+		# Iteratively add intervals to interval_list
 		cdef int i
 		for i in range(length):
-			ailist_add(ail, interval_list[i].start, interval_list[i].end, interval_list[i].id_value)
+			ailist_add(ail, interval_list[i].start, interval_list[i].end,
+						interval_list[i].id_value)
 
 		return ail
 
 
 	def __reduce__(self):
 		"""
 		Used for pickling. Convert ailist to bytes and back.
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
-		
+
 		# Convert ints to bytes
 		b_length = int(self.c_ailist.nr).to_bytes(4, byteorder)
 
 		# Convert ailist_t to bytes
 		data = self._get_data()
 
 		return (rebuild_AIList, (data, b_length))
 
-	
+
 	@property
 	def nc(self):
 		"""
 		Number of components in constructed AIList
 		"""
 
 		# Check if object is still open
@@ -196,15 +194,15 @@
 
 		# Check if object is constructed
 		if self.is_constructed:
 			return self.c_ailist.lenC[self.c_ailist.nc]
 		else:
 			return None
 
-	
+
 	@property
 	def idxC(self):
 		"""
 		Index of components in constructed AIList
 		"""
 
 		# Check if object is still open
@@ -214,36 +212,36 @@
 		# Check if object is constructed
 		if self.is_constructed:
 			return self.c_ailist.idxC[self.c_ailist.nc]
 		else:
 			return None
 
 
-	@property	
+	@property
 	def size(self):
 		"""
 		Number of intervals in AIList
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		return self.c_ailist.nr
-	
+
 	@property
 	def first(self):
 		"""
 		Start of first interval in AIList
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
-		
+
 		# Check if there are any intervals
 		if self.size == 0:
 			return None
 		else:
 			return self.c_ailist.first
 
 	@property
@@ -273,45 +271,43 @@
 			raise NameError("AIList object has been closed.")
 
 		# Check if ther are any intervals
 		if self.size == 0:
 			return 0
 		else:
 			return self.last - self.first
-		
+
 
 	def __len__(self):
 		"""
 		Return size of interval_list
 		"""
-		
+
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		return self.size
 
-	
+
 	def __iter__(self):
 		"""
 		Iterate over AIList object
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Iterate over interval list
-		cdef Interval interval
 		cdef int i
-		
 		for i in range(self.size):
-			interval = Interval()
-			interval.set_i(&self.c_ailist.interval_list[i])
-			
+			interval = Interval(self.c_ailist.interval_list[i].start,
+								self.c_ailist.interval_list[i].end)
+
 			yield interval
 
 
 	def __sub__(self, AIList query_ail):
 		"""
 		Subtract values
 		"""
@@ -342,84 +338,91 @@
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		return self.append(query_ail)
 
-	
+
 	def __hash__(self):
 		"""
 		Get hash value
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		return hash(self)
-		
-		
+
+
 	cdef ailist_t *_array_id(AIList self, const long[::1] ids):
 		cdef int length = len(ids)
 		cdef ailist_t *cindexed_ailist
-		
+
 		# Call C function
 		cindexed_ailist = ailist_get_id_array(self.c_ailist, &ids[0], length)
-		
+
 		return cindexed_ailist
-	
+
 	cdef ailist_t *_interval_id(AIList self, int id_value):
 		cdef ailist_t *cindexed_ailist
-		
+
 		# Call C function
 		cindexed_ailist = ailist_get_id(self.c_ailist, id_value)
-		
+
 		return cindexed_ailist
 
 	def __getitem__(self, key):
 		"""
 		Index Intervals by id_value
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Initialize variables
 		cdef AIList indexed_ailist
 		cdef ailist_t *cindexed_ailist
+		cdef interval_t cinterval
 
 		# Initialize results
 		indexed_ailist = AIList()
 
 		# Check if key is iterable
 		try:
-			iter(key) # Test if iterable
+			# Test if iterable
+			iter(key)
 
 			# Check if keys are booleans
 			if isinstance(key[0], np.bool_):
 				raise IndexError("Cannot use boolean array as key")
 
 			# Must be integers
 			else:
 				cindexed_ailist = self._array_id(key)
-		
+
 		# key is not iterable, treat as int
 		except TypeError:
 			# Check if key is slice
 			if isinstance(key, slice):
 				raise IndexError("Cannot use slice as key")
 
 			# Find id
-			cindexed_ailist = self._interval_id(key)
+			#cindexed_ailist = self._interval_id(key)
+			cinterval = self.c_ailist.interval_list[key]
+			interval = Interval(cinterval.start, cinterval.end)
+			#interval.set_i(cinterval)
+
+			return interval
 
 		# Wrap c object
 		indexed_ailist.set_list(cindexed_ailist)
-		
+
 		return indexed_ailist
 
 
 	def __repr__(self):
 		"""
 		Representation of ailist object
 		"""
@@ -434,23 +437,23 @@
 			repr_string += " range: (None-None)\n"
 		else:
 			repr_string += " range: (%d-%d)\n" % (self.first, self.last)
 
 		# Iterate over interval_list
 		if self.c_ailist.nr > 10:
 			for i in range(5):
-				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].id_value)
+				repr_string += "   (%d-%d)\n" % (self[i].start, self[i].end)
 			repr_string += "   ...\n"
 			for i in range(-5, 0, 1):
-				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].id_value)
+				repr_string += "   (%d-%d)\n" % (self[i].start, self[i].end)
 		else:
 			for i in range(self.c_ailist.nr):
-				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].id_value)
+				repr_string += "   (%d-%d)\n" % (self[i].start, self[i].end)
 
-		return repr_string		
+		return repr_string
 
 
 	cdef void set_list(AIList self, ailist_t *input_list):
 		"""
 		Set wrapper of C ailist
 
 		Parameters
@@ -459,24 +462,72 @@
 				ailist_t to replace existing one
 
 		Returns
 		-------
 			None
 		"""
 
-		# Free old skiplist
-		#if self.c_ailist:
-			#ailist_destroy(self.c_ailist)
 		ailist_destroy(self.c_ailist)
-		
+
 		# Replace new skiplist
 		self.c_ailist = input_list
 		self.is_closed = False
 
 
+	@property
+	def ids(self):
+		"""
+		Return the ID values
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Extract id_values
+		cdef long[::1] ids = np.zeros(self.size, dtype=np.int_)
+		ailist_extract_ids(self.c_ailist, &ids[0])
+
+		return np.asarray(ids, dtype=np.intc)
+
+
+	@property
+	def starts(self):
+		"""
+		Return the start values
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Extract start values
+		cdef long[::1] starts = np.zeros(self.size, dtype=np.int_)
+		ailist_extract_starts(self.c_ailist, &starts[0])
+
+		return np.asarray(starts, dtype=np.intc)
+
+
+	@property
+	def ends(self):
+		"""
+		Return the end values
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Extract end values
+		cdef long[::1] ends = np.zeros(self.size, dtype=np.int_)
+		ailist_extract_ends(self.c_ailist, &ends[0])
+
+		return np.asarray(ends, dtype=np.intc)
+
+
 	def freeze(self):
 		"""
 		Make :class:`~ailist.AIList` immutable
 
 		Parameters
 		----------
 			None
@@ -511,15 +562,15 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure it is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Change to frozen
 		self.is_frozen = True
 
 
 	def unfreeze(self):
@@ -564,22 +615,22 @@
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Change to not frozen
 		self.is_frozen = False
 
-	
+
 	cdef void _insert(AIList self, int start, int end, int id_value):
 		ailist_add(self.c_ailist, start, end, id_value)
 
-	def add(self, int start, int end, id_value=None):
+	def add(self, start, end, id_value=None):
 		"""
 		Add an interval to AIList inplace
-		
+
 		Parameters
 		----------
 			start : int
 				Start position of interval
 			end : int
 				End position of interval
 			id_value : double
@@ -601,42 +652,83 @@
 		>>> ail = AIList()
 		>>> ail.add(1, 2)
 		>>> ail.add(3, 4)
 		>>> ail.add(3, 6)
 		>>> ail
 		AIList
 		  range: (1-6)
-		   (1-2, 0)
-		   (3-4, 1)
-		   (3-6, 2)
+		   (1-2)
+		   (3-4)
+		   (3-6)
+		>>> import numpy as np
+		>>> starts = np.arange(100)
+		>>> ends = starts + 10
+		>>> index = np.arange(len(starts))
+		>>> ail = AIList()
+		>>> ail.add(starts, ends, index)
+		>>> ail
+		AIList
+		 range: (0-109)
+			(0-10)
+			(1-11)
+			(2-12)
+			(3-13)
+			(4-14)
+			...
+			(95-105)
+			(96-106)
+			(97-107)
+			(98-108)
+			(99-109)
+
 
 		"""
-		
+
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Check that object is not frozen
 		if self.is_frozen:
 			raise TypeError("AIList is frozen and currently immutatable. Try '.unfreeze()' to reverse.")
 
-		# Insert interval
-		if id_value is None:
-			self._insert(start, end, self.c_ailist.nr)
+		# Check if start is int
+		cdef int array_length
+		cdef const long[::1] starts
+		cdef const long[::1] ends
+		cdef const long[::1] ids
+		if isinstance(start, int):
+			# Check interval
+			if start > end:
+				raise IndexError("Start is greater than end.")
+
+			# Insert interval
+			if id_value is None:
+				self._insert(start, end, self.c_ailist.nr)
+			else:
+				self._insert(start, end, id_value)
+
+		elif isinstance(start, np.ndarray):
+			array_length = len(start)
+			starts = start
+			ends = end
+			ids = id_value
+			ailist_from_array(self.c_ailist, &starts[0], &ends[0], &ids[0], array_length)
+
 		else:
-			self._insert(start, end, id_value)
-		
+			raise TypeError("Start must be int or np.ndarray.")
+
 		# Object is no longer constructed
 		self.is_constructed = False
 
-
-	def from_array(self, const long[::1] starts, const long[::1] ends, const long[::1] ids):
+	@staticmethod
+	def from_array(const long[::1] starts, const long[::1] ends, const long[::1] ids):
 		"""
 		Add intervals from arrays to AIList inplace
-		
+
 		Parameters
 		----------
 			starts : ~numpy.ndarray{long}
 				Start positions of intervals
 			ends : numpy.ndarray{long}
 				End positions of intervals
 			ids : numpy.ndarray{long}
@@ -655,17 +747,16 @@
 		Examples
 		--------
 		>>> from ailist import AIList
 		>>> import numpy as np
 		>>> starts = np.arange(100)
 		>>> ends = starts + 10
 		>>> index = np.arange(len(starts))
-		>>> ail = AIList()
-		>>> ail.from_array(starts, ends, index)
-		>>> ail.
+		>>> ail = AIList.from_array(starts, ends, index)
+		>>> ail
 		AIList
 		  range: (0-109)
 		   (0-10, 0)
 		   (1-11, 1)
 		   (2-12, 2)
 		   (3-13, 3)
 		   (4-14, 4)
@@ -673,30 +764,25 @@
 		   (95-105, 95)
 		   (96-106, 96)
 		   (97-107, 97)
 		   (98-108, 98)
 
 		"""
 
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("AIList object has been closed.")
-
-		# Check that object is not frozen
-		if self.is_frozen:
-			raise TypeError("AIList is frozen and currently immutatable. Try '.unfreeze()' to reverse.")
-
+		ail = AIList()
 		cdef int array_length = len(starts)
-		ailist_from_array(self.c_ailist, &starts[0], &ends[0], &ids[0], array_length)
-		self.is_constructed = False
+		ailist_from_array(ail.c_ailist, &starts[0], &ends[0], &ids[0], array_length)
+
+		return ail
 
 
 	cdef void _construct(AIList self, int min_length):
 		# Contruct
 		ailist_construct(self.c_ailist, min_length)
+		#ailist_construct_v0(self.c_ailist, min_length)
 
 	def construct(self, int min_length=20):
 		"""
 		Construct ailist_t *Required to call intersect
 
 		Parameters
 		----------
@@ -739,21 +825,21 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Check if already constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self._construct(min_length)
 			self.is_constructed = True
 		else:
 			pass
-			
-			
+
+
 	def iter_sorted(self):
 		"""
 		Iterate over an AIList in sorted way
 
 		Parameters
 		----------
 			None
@@ -761,56 +847,67 @@
 		Returns
 		-------
 			sorted_iter : Generator
 				Generator of Intervals
 		"""
 
 		# Check if is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Iterate over  ail
 		cdef interval_t *cintv
-		cdef Interval output_interval
-		
+		#cdef Interval output_interval
+
 		# Create sorted iterators
 		cdef ailist_sorted_iter_t *ail_iter = ailist_sorted_iter_init(self.c_ailist)
 		while ailist_sorted_iter_next(ail_iter) != 0:
 			cintv = ail_iter.intv
 			# Create Interval wrapper
-			output_interval = Interval()
-			output_interval.set_i(cintv)
+			output_interval = Interval(cintv.start, cintv.end)
+			#output_interval.set_i(cintv)
 			yield output_interval
 
 		ailist_sorted_iter_destroy(ail_iter)
-	
+
 
 	cdef ailist_t *_intersect(AIList self, int start, int end):
-		cdef ailist_t *overlaps = ailist_query(self.c_ailist, start, end)
+		cdef ailist_t *overlaps = ailist_init()
+		ailist_query(self.c_ailist, overlaps, start, end)
 
 		return overlaps
 
-	def intersect(self, int start, int end):
+	cdef ailist_t *_intersect_from_array(AIList self,
+										 const long[::1] starts,
+										 const long[::1] ends):
+		cdef int length = starts.size
+		cdef ailist_t *overlaps = ailist_init()
+		ailist_query_from_array(self.c_ailist, overlaps, &starts[0], &ends[0], length)
+
+		return overlaps
+
+	def intersect(self, start, end):
 		"""
 		Find intervals overlapping given range
-		
+
 		Parameters
 		----------
-			start : int
+			start : int | np.ndarray{int}
 				Start position of query range
-			end : int
+			end : int | np.ndarray{int}
 				End position of query range
 
 		Returns
 		-------
 			overlaps : AIList
 				Overlapping intervals
 
 		.. warning::
-			This requires :func:`~ailist.AIList.construct` and will run it if not already run. This will re-sort intervals inplace.
+			This requires :func:`~ailist.AIList.construct` and will run it if not already run.
+			This will re-sort intervals inplace.
 
 		See Also
 		--------
 		AIList.construct: Construct AIList, required to call AIList.intersect
 		AIList.add: Add interval to AIList
 		AIList.intersect_index: Find interval indices overlapping given range
 		AIList.intersect_from_array: Find interval indices overlapping given ranges
@@ -838,52 +935,82 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Check if is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Intersect
-		cdef ailist_t *i_list = self._intersect(start, end)
+		cdef const long[::1] starts
+		cdef const long[::1] ends
+		cdef ailist_t *i_list
 		cdef AIList overlaps = AIList()
-		overlaps.set_list(i_list)
+		if isinstance(start, int):
+			i_list = self._intersect(start, end)
+			overlaps.set_list(i_list)
+		elif isinstance(start, np.ndarray):
+			starts = start
+			ends = end
+			i_list = self._intersect_from_array(starts, ends)
+			overlaps.set_list(i_list)
+		else:
+			raise TypeError("Start must be int or np.ndarray.")
 
 		return overlaps
 
 
 	cdef np.ndarray _intersect_ids(AIList self, int start, int end):
-		cdef ailist_t *overlaps = ailist_query(self.c_ailist, start, end)
+		cdef ailist_t *overlaps = ailist_init()
+		ailist_query(self.c_ailist, overlaps, start, end)
 		cdef long[::1] ids = np.zeros(overlaps.nr, dtype=np.long)
 
 		# Extract IDs
 		ailist_extract_ids(overlaps, &ids[0])
 
 		return np.asarray(ids)
 
-	def intersect_ids(self, int start, int end):
+	@cython.boundscheck(False)
+	@cython.wraparound(False)
+	@cython.initializedcheck(False)
+	cpdef _intersect_ids_from_array(AIList self, const long[::1] starts, const long[::1] ends,
+									const long[::1] ids):
+		cdef int length = len(starts)
+		cdef array_query_t *total_overlaps = array_query_init()
+		ailist_query_id_from_array(self.c_ailist, total_overlaps, &starts[0],
+									&ends[0], &ids[0], length)
+
+		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index,
+														   total_overlaps.size)
+		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index,
+															 total_overlaps.size)
+
+		return ref_index, query_index
+
+	def intersect_ids(self, start, end):
 		"""
 		Find interval indices overlapping given range
-		
+
 		Parameters
 		----------
-			start : int
+			start : int | np.ndarray{int}
 				Start position of query range
-			end : int
+			end : int | np.ndarray{int}
 				End position of query range
 
 		Returns
 		-------
 			ids : numpy.ndarray{int}
 				Overlapping interval indices
 
 		.. warning::
-			This requires :func:`~ailist.AIList.construct` and will run it if not already run. This will re-sort intervals inplace.
+			This requires :func:`~ailist.AIList.construct` and will run it if not already run.
+			This will re-sort intervals inplace.
 
 		See Also
 		--------
 		AIList.construct: Construct AIList, required to call AIList.intersect
 		AIList.add: Add interval to AIList
 		AIList.intersect: Find intervals overlapping given range
 		AIList.intersect_from_array: Find interval indices overlapping given ranges
@@ -908,133 +1035,61 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Check if object has been constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Intersect
-		cdef np.ndarray ids = self._intersect_ids(start, end)
-
-		return ids
-
-
-	@cython.boundscheck(False)
-	@cython.wraparound(False)
-	@cython.initializedcheck(False)
-	cpdef _intersect_ids_from_array(AIList self, const long[::1] starts, const long[::1] ends, const long[::1] ids):
-		cdef int length = len(starts)
-		cdef array_query_t *total_overlaps
-		total_overlaps = ailist_query_id_from_array(self.c_ailist, &starts[0], &ends[0], &ids[0], length)
-
-		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index, total_overlaps.size)
-		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index, total_overlaps.size)
-
-		return ref_index, query_index
-
-	def intersect_from_array(self, const long[::1] starts, const long[::1] ends, const long[::1] ids):
-		"""
-		Find interval indices overlapping given ranges
-		
-		Parameters
-		----------
-			starts : numpy.ndarray{long}
-				Start positions of intervals
-			ends : numpy.ndarray{long}
-				End positions of intervals
-			ids : numpy.ndarray{long}
-				ID of intervals
-
-		Returns
-		-------
-			ref_index : np.ndarray{int}
-				Overlapping interval indices from AIList
-			query_index : np.ndarray{int}
-				Overlapping interval indices from query AIList
-
-		.. warning::
-			This requires :func:`~ailist.AIList.construct` and will run it if not already run. This will re-sort intervals inplace.
-
-		See Also
-		--------
-		AIList.construct: Construct AIList, required to call AIList.intersect
-		AIList.add: Add interval to AIList
-		AIList.intersect: Find intervals overlapping given range
-		AIList.intersect_index: Find interval indices overlapping given range
-
-		Examples
-		--------
-		>>> from ailist import AIList
-		>>> ail1 = AIList()
-		>>> ail1.add(1, 2)
-		>>> ail1.add(3, 4)
-		>>> ail1.add(2, 6)
-		>>> ail1
-		AIList
-		  range: (1-6)
-		   (1-2, 0)
-		   (3-4, 1)
-		   (2-6, 2)
-		>>> ail2 = AIList()
-		>>> ail2.add(1, 2)
-		>>> ail2.add(3, 6)
-		>>> ail2
-		AIList
-		  range: (1-6)
-		    (1-2, 0)
-		    (3-6, 1)
-		>>> q = ail1.intersect_from_array(ail2)
-		>>> q
-		(array([2, 1]), array([]))
-
-		"""
-
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("AIList object has been closed.")
+		cdef const long[::1] starts
+		cdef const long[::1] ends
+		cdef np.ndarray ref_ids
+		cdef np.ndarray query_ids
+		if isinstance(start, int):
+			ref_ids = self._intersect_ids(start, end)
+			return ref_ids
+
+		elif isinstance(start, np.ndarray):
+			starts = start
+			ends = end
+			ids = np.arange(len(starts), dtype=np.long)
+			ref_ids, query_ids = self._intersect_ids_from_array(starts, ends, ids)
+			return ref_ids, query_ids
 
-		# Check if object is constructed
-		if self.is_constructed == False:
-			self.construct()
-
-		ref_index, query_index = self._intersect_ids_from_array(starts, ends, ids)
-		
-		return ref_index, query_index
+		else:
+			raise TypeError("Start must be int or np.ndarray.")
 
 
-	cpdef _intersect_ids_from_ailist(AIList self, AIList ail):
+	cdef ailist_t *_intersect_from_ailist(AIList self, AIList ail):
 		# Intersect with other AIList
-		cdef array_query_t *total_overlaps = ailist_query_id_from_ailist(self.c_ailist, ail.c_ailist)
+		cdef ailist_t *overlaps = ailist_init()
+		ailist_query_from_ailist(self.c_ailist, ail.c_ailist, overlaps)
 
-		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index, total_overlaps.size)
-		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index, total_overlaps.size)
-
-		return ref_index, query_index
+		return overlaps
 
 	def intersect_from_ailist(self, AIList ail_query):
 		"""
 		Find interval indices overlapping given ranges
-		
+
 		Parameters
 		----------
 			ail_query : AIList
 				Intervals to query
 
 		Returns
 		-------
-			ref_index : np.ndarray{int}
-				Overlapping interval indices from AIList
-			query_index : np.ndarray{int}
-				Overlapping interval indices from query AIList
+			ail : AIList
+				Overlapping intervals
 
 		.. warning::
-			This requires :func:`~ailist.AIList.construct` and will run it if not already run. This will re-sort intervals inplace.
+			This requires :func:`~ailist.AIList.construct` and will run it if not already run.
+			This will re-sort intervals inplace.
 
 		See Also
 		--------
 		AIList.construct: Construct AIList, required to call AIList.intersect
 		AIList.add: Add interval to AIList
 		AIList.intersect: Find intervals overlapping given range
 		AIList.intersect_index: Find interval indices overlapping given range
@@ -1068,22 +1123,24 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Check if object is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Intersect
-		ref_index, query_index = self._intersect_from_ailist(ail_query)
-		
-		return ref_index, query_index
-		
+		cdef ailist_t *c_ailist = self._intersect_from_ailist(ail_query)
+		cdef AIList ail = AIList()
+		ail.set_list(c_ailist)
+
+		return ail
+
 
 	cdef np.ndarray _coverage(AIList self):
 		# Initialize coverage
 		cdef double[::1] coverage = np.zeros(self.range, dtype=np.double)
 
 		# Call C function
 		ailist_coverage(self.c_ailist, &coverage[0])
@@ -1110,43 +1167,44 @@
 			raise NameError("AIList object has been closed.")
 
 		# Initialize coverage
 		cdef np.ndarray coverage
 
 		# Calculate coverage
 		coverage = self._coverage()
-		
+
 		return pd.Series(coverage, index=np.arange(self.first, self.last))
 
 
 	cdef np.ndarray _bin_coverage(AIList self, int bin_size):
 		# Initialize coverage
 		cdef int n_bins = math.ceil(self.last / bin_size) - (self.first // bin_size)
 		cdef double[::1] bins = np.zeros(n_bins, dtype=np.double)
 
 		# Call C function
 		ailist_bin_coverage(self.c_ailist, &bins[0], bin_size)
 
 		return np.asarray(bins)
 
-	cdef np.ndarray _bin_coverage_length(AIList self, int bin_size, int min_length, int max_length):
+	cdef np.ndarray _bin_coverage_length(AIList self, int bin_size, int min_length,
+										 int max_length):
 		# Initialize coverage
 		cdef int n_bins = math.ceil(self.last / bin_size) - (self.first // bin_size)
 		cdef double[::1] bins = np.zeros(n_bins, dtype=np.double)
 
 		# Call C function
 		ailist_bin_coverage_length(self.c_ailist, &bins[0], bin_size, min_length, max_length)
 
 		return np.asarray(bins)
 
 	def bin_coverage(self, int bin_size=100000, min_length=None, max_length=None):
 		"""
 		Find sum of coverage within binned
 		positions
-		
+
 		Parameters
 		----------
 			bin_size : int
 				Size of the bin to use
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
@@ -1167,43 +1225,43 @@
 		cdef np.ndarray bins
 
 		# Calculate coverage
 		if min_length is None or max_length is None:
 			bins = self._bin_coverage(bin_size)
 		else:
 			bins = self._bin_coverage_length(bin_size, min_length, max_length)
-		
+
 		return pd.Series(bins, index=(np.arange(len(bins)) + int(self.first / bin_size)) * bin_size)
 
 
 	cdef np.ndarray _bin_nhits(AIList self, int bin_size):
 		# Initialize coverage
 		cdef int n_bins = math.ceil(self.last / bin_size) - (self.first // bin_size)
-		cdef double[::1] bins = np.zeros(n_bins, dtype=np.double)
-		
+		cdef long[::1] bins = np.zeros(n_bins, dtype=np.double)
+
 		# Call C function
 		ailist_bin_nhits(self.c_ailist, &bins[0], bin_size)
 
 		return np.asarray(bins)
 
 	cdef np.ndarray _bin_nhits_length(AIList self, int bin_size, int min_length, int max_length):
 		# Initialize coverage
 		cdef int n_bins = math.ceil(self.last / bin_size) - (self.first // bin_size)
-		cdef double[::1] bins = np.zeros(n_bins, dtype=np.double)
+		cdef long[::1] bins = np.zeros(n_bins, dtype=np.double)
 
 		# Call C function
 		ailist_bin_nhits_length(self.c_ailist, &bins[0], bin_size, min_length, max_length)
 
 		return np.asarray(bins)
 
 	def bin_nhits(self, int bin_size=100000, min_length=None, max_length=None):
 		"""
 		Find number of intervals overlapping binned
 		positions
-		
+
 		Parameters
 		----------
 			bin_size : int
 				Size of the bin to use
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
@@ -1218,24 +1276,74 @@
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Initialize coverage
 		cdef np.ndarray bins
-		
+
 		# Calculate coverage
 		if min_length is None or max_length is None:
 			bins = self._bin_nhits(bin_size)
 		else:
 			bins = self._bin_nhits_length(bin_size, min_length, max_length)
-		
+
 		return pd.Series(bins, index=(np.arange(len(bins)) + int(self.first / bin_size)) * bin_size)
 
 
+	cdef void _nhits(AIList self, long *nhits, int start, int end):
+
+		# Call C function
+		ailist_query_nhits(self.c_ailist, nhits, start, end)
+
+		return
+
+	cdef void _nhits_length(AIList self, long *nhits, int start, int end, int min_length,
+							int max_length):
+
+		# Call C function
+		ailist_query_nhits_length(self.c_ailist, nhits, start, end, min_length, max_length)
+
+		return
+
+	def nhits(self, start, end, min_length=None, max_length=None):
+		"""
+		Find number of intervals overlapping binned
+		positions
+
+		Parameters
+		----------
+			min_length : int
+				Minimum length of intervals to include [default = None]
+			max_length : int
+				Maximum length of intervals to include [default = None]
+
+		Returns
+		-------
+			nhits : int
+				Number of overlaps
+
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Initialize nhits
+		cdef long nhits = 0
+
+		# Calculate coverage
+		if min_length is None or max_length is None:
+			bins = self._nhits(&nhits, start, end)
+		else:
+			bins = self._nhits_length(&nhits, start, end, min_length, max_length)
+
+		return nhits
+
+
 	def display(self):
 		"""
 		Print all intervals
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
@@ -1243,15 +1351,15 @@
 
 		display_list(self.c_ailist)
 
 
 	def merge(self, int gap=0):
 		"""
 		Merge intervals within a gap
-		
+
 		Parameters
 		----------
 			gap : int
 				Gap between intervals to merge
 
 		Returns
 		-------
@@ -1261,15 +1369,15 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Create merged
 		cdef AIList merged_list = AIList()
 
 		# Call C function
 		cdef ailist_t *merged_clist = ailist_merge(self.c_ailist, gap)
@@ -1277,15 +1385,15 @@
 
 		return merged_list
 
 
 	def subtract(self, AIList query_ail):
 		"""
 		Subtract intervals within another AIList
-		
+
 		Parameters
 		----------
 			query_ail : AIList
 				AIList of intervals to subtract
 
 		Returns
 		-------
@@ -1294,34 +1402,34 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed or query_ail.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
-		if query_ail.is_constructed == False:
+		if query_ail.is_constructed is False:
 			query_ail.construct()
 
 		# Create subracted
 		cdef AIList subtracted_list = AIList()
 
 		# Call Cfunction
-		cdef ailist_t *subtracted_clist = ailist_subtract(query_ail.c_ailist,
-														  self.c_ailist)
+		cdef ailist_t *subtracted_clist = ailist_subtract(self.c_ailist,
+														  query_ail.c_ailist)
 		subtracted_list.set_list(subtracted_clist)
 
 		return subtracted_list
 
 
 	def common(self, AIList query_ail):
 		"""
 		Common intervals within another AIList
-		
+
 		Parameters
 		----------
 			query_ail : AIList
 				AIList of intervals to find commons
 
 		Returns
 		-------
@@ -1331,32 +1439,32 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed or query_ail.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
-		if query_ail.is_constructed == False:
+		if query_ail.is_constructed is False:
 			query_ail.construct()
 
 		# Create common
 		cdef AIList common_list = AIList()
-		cdef ailist_t *common_clist = ailist_common(query_ail.c_ailist,
-													self.c_ailist)
+		cdef ailist_t *common_clist = ailist_common(self.c_ailist,
+													query_ail.c_ailist)
 		common_list.set_list(common_clist)
 
 		return common_list
 
 
 	def append(self, AIList query_ail):
 		"""
 		Union of intervals within two AIList
-		
+
 		Parameters
 		----------
 			query_ail : AIList
 				AIList of intervals to append
 
 		Returns
 		-------
@@ -1394,15 +1502,15 @@
 
 		return np.asarray(wps)
 
 	def wps(self, int protection=60, min_length=None, max_length=None):
 		"""
 		Calculate Window Protection Score
 		for each position in AIList range
-		
+
 		Parameters
 		----------
 			protection : int
 				Protection window to use
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
@@ -1416,35 +1524,35 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
-		
+
 		# Initialize wps
 		cdef np.ndarray wps
 
 		# Calculate wps
 		if self.range == 0:
 			return None
 		if min_length is None or max_length is None:
 			wps = self._wps(protection)
 		else:
 			wps = self._wps_length(protection, min_length, max_length)
-		
+
 		return pd.Series(wps, index=np.arange(self.first, self.last))
 
-	
+
 	def filter(self, int min_length=1, int max_length=400):
 		"""
 		Filter out intervals outside of a length range
-		
+
 		Parameters
 		----------
 			min_length : int
 				Minimum length to keep
 			max_length : int
 				Maximum langth to keep
 
@@ -1459,16 +1567,16 @@
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Initialize filtered list
 		cdef AIList filtered_ail = AIList()
 
 		# Call C function
-		cdef ailist_t *cfiltered_ail = ailist_length_filter(self.c_ailist, min_length, max_length)
-		filtered_ail.set_list(cfiltered_ail)
+		ailist_length_filter(self.c_ailist, filtered_ail.c_ailist, min_length, max_length)
+		#filtered_ail.set_list(cfiltered_ail)
 
 		return filtered_ail
 
 
 	cdef np.ndarray _length_dist(AIList self):
 		# Initialize distribution
 		cdef int max_length = ailist_max_length(self.c_ailist)
@@ -1482,15 +1590,15 @@
 	def length_dist(self):
 		"""
 		Calculate length distribution of intervals
 
 		Parameters
 		----------
 			None
-		
+
 		Returns
 		-------
 			distribution : numpy.ndarray{int}
 				Interval length distribution
 
 		"""
 
@@ -1513,29 +1621,33 @@
 		cdef int[::1] nhits = np.zeros(length, dtype=np.intc)
 
 		# Calculate distribution
 		ailist_nhits_from_array(self.c_ailist, &starts[0], &ends[0], length, &nhits[0])
 
 		return np.asarray(nhits, dtype=np.intc)
 
-	cdef np.ndarray _nhits_from_array_length(AIList self, const long[::1] starts, const long[::1] ends, int min_length, int max_length):
+	cdef np.ndarray _nhits_from_array_length(AIList self, const long[::1] starts,
+											 const long[::1] ends, int min_length,
+											 int max_length):
 		# Initialize hits
 		cdef int length = starts.size
 		cdef int[::1] nhits = np.zeros(length, dtype=np.intc)
 
 		# Calculate distribution
-		ailist_nhits_from_array_length(self.c_ailist, &starts[0], &ends[0], length, &nhits[0], min_length, max_length)
+		ailist_nhits_from_array_length(self.c_ailist, &starts[0], &ends[0], length,
+										&nhits[0], min_length, max_length)
 
 		return np.asarray(nhits, dtype=np.intc)
 
-	def nhits_from_array(self, const long[::1] starts, const long[::1] ends, min_length=None, max_length=None):
+	def nhits_from_array(self, const long[::1] starts, const long[::1] ends,
+						 min_length=None, max_length=None):
 		"""
 		Find number of intervals overlapping given
 		positions
-		
+
 		Parameters
 		----------
 			starts : numpy.ndarray{long}
 				Start positions to intersect
 			ends : numpy.ndarray{long}
 				End positions to intersect
 			min_length : int
@@ -1551,15 +1663,15 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Initialize distribution
 		cdef np.ndarray nhits
 		# Calculate distribution
 		if min_length is None or max_length is None:
 			nhits = self._nhits_from_array(starts, ends)
@@ -1573,20 +1685,20 @@
 		# Initialize hits
 		cdef int[::1] coverage = np.zeros(end - start, dtype=np.intc)
 
 		# Calculate distribution
 		ailist_interval_coverage(self.c_ailist, start, end, &coverage[0])
 
 		return np.asarray(coverage, dtype=np.intc)
-	
+
 	def interval_coverage(self, int start, int end):
 		"""
 		Find number of intervals overlapping each
 		position in given interval
-		
+
 		Parameters
 		----------
 			start : int
 				Start position to intersect
 			end : int
 				End position to intersect
 
@@ -1598,30 +1710,30 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Initialize distribution
 		cdef np.ndarray coverage
 
 		# Calculate distribution
 		coverage = self._interval_coverage(start, end)
 
 		return pd.Series(coverage, index=np.arange(start, end))
 
-	
+
 	def downsample(self, double proportion):
 		"""
 		Randomly downsample AIList
-		
+
 		Parameters
 		----------
 			proportion : double
 				Proportion of intervals to keep
 
 		Returns
 		-------
@@ -1640,94 +1752,32 @@
 		# Call C function
 		cdef ailist_t *cfiltered_ail = ailist_downsample(self.c_ailist, proportion)
 		filtered_ail.set_list(cfiltered_ail)
 
 		return filtered_ail
 
 
-	def extract_id(self):
-		"""
-		Return the ID values
-
-		Parameters
-		----------
-			None
-
-		Returns
-		-------
-			ids : numpy.ndarray
-				ID values
-		"""
-
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("AIList object has been closed.")
-
-		# Extract id_values
-		cdef long[::1] ids = np.zeros(self.size, dtype=np.int_)
-		ailist_extract_ids(self.c_ailist, &ids[0])
-
-		return np.asarray(ids, dtype=np.intc)
-
-
-	def extract_starts(self):
+	def copy(self):
 		"""
-		Return the start values
-
-		Parameters
-		----------
-			None
-
-		Returns
-		-------
-			numpy.ndarray
-				Start values
+		Make a copy of the AIList
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("AIList object has been closed.")
 
-		# Extract start values
-		cdef long[::1] starts = np.zeros(self.size, dtype=np.int_)
-		ailist_extract_starts(self.c_ailist, &starts[0])
-
-		return np.asarray(starts, dtype=np.intc)
-
-	
-	def extract_ends(self):
-		"""
-		Return the end values
-
-		Parameters
-		----------
-			None
-
-		Returns
-		-------
-			numpy.ndarray
-				End values
-		"""
-
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("AIList object has been closed.")
+		cdef AIList new_ail = AIList()
+		cdef ailist_t *c_new_ail = ailist_copy(self.c_ailist)
+		new_ail.set_list(c_new_ail)
 
-		# Extract end values
-		cdef long[::1] ends = np.zeros(self.size, dtype=np.int_)
-		ailist_extract_ends(self.c_ailist, &ends[0])
+		return new_ail
 
-		return np.asarray(ends, dtype=np.intc)
 
-	
 	def close(self):
 		"""
 		Close object and clear memory
 		"""
 
-		# Free interval_list memory
-		#if self.c_ailist:
-			#ailist_destroy(self.c_ailist)
 		ailist_destroy(self.c_ailist)
 		self.c_ailist = NULL
-		
-		self.is_closed = True
+
+		self.is_closed = True
```

### Comparing `ailist-1.0.4/ailist/Interval_core.pyx` & `ailist-2.0.2/ailist/Interval_core.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 #cython: embedsignature=True
 #cython: profile=False
 
 import os
 import sys
 import numpy as np
 cimport numpy as np
-import math
-cimport cython
-import pandas as pd
-from libc.string cimport memcpy
 np.import_array()
-from time import time
 
 # Set byteorder for __reduce__
 byteorder = sys.byteorder
 
 
 def get_include():
 	"""
@@ -37,114 +32,65 @@
 
 
 cdef class Interval(object):
 	"""
 	Wrapper of C interval_t
 
 	:class:`~Interval_core.Interval` stores an interval
-	
+
 	"""
 
-	def __init__(self, start=None, end=None, id_value=None):
+	def __init__(self, start=None, end=None):
 		"""
 		Initialize Interval
 
 		Parameters
 		----------
 			start : int
 				Starting position [default = None]
 			end : int
 				Ending position [default = None]
-			id_value : int
-				ID [defualt = None]
-
-		Returns
-		-------
-			None
-
-		"""
-
-		if start is not None:
-			if id_value is None:
-				id_value = 0
-			# Create interval
-			self.i = interval_init(start, end, id_value)
-
-	cdef void set_i(Interval self, interval_t *i):
-		"""
-		Initialize wrapper of C interval
-
-		Parameters
-		----------
-			i : interval_t
-				C interval_t to be wrapped
 
 		Returns
 		-------
 			None
 
 		"""
 
-		# Set i
-		self.i = i
+		self.start = start
+		self.end = end
 
 
-	@property
-	def start(self):
-		"""
-		Start of interval
-		"""
-
-		return self.i.start
-
-	@property
-	def end(self):
-		"""
-		End of interval
-		"""
-
-		return self.i.end
-	
-	@property
-	def id_value(self):
-		"""
-		ID of interval
-		"""
-
-		return self.i.id_value
-	
-
 	def __hash__(self):
 		"""
 		Get hash value
 		"""
 
 		return hash(repr(self))
 
-	
+
 	def __eq__(self, other):
 		"""
 		Check if there is overlap
 		"""
 
 		# Check that the classes match
 		is_equal = self.__class__ == other.__class__
 
 		# Check for overlap
 		if is_equal:
-			if other.start < self.i.end and other.end > self.i.start:
+			if other.start < self.end and other.end > self.start:
 				is_equal = True
 			else:
 				is_equal = False
-		
+
 		return is_equal
 
 
 	def __str__(self):
-		format_string = "Interval(%d-%d, %s)" % (self.start, self.end, self.id_value)
+		format_string = "Interval(%d-%d)" % (self.start, self.end)
 		return format_string
 
 
 	def __repr__(self):
-		format_string = "Interval(%d-%d, %s)" % (self.start, self.end, self.id_value)
+		format_string = "Interval(%d-%d)" % (self.start, self.end)
 		return format_string
-
```

### Comparing `ailist-1.0.4/ailist/LabeledIntervalArray_core.pxd` & `ailist-2.0.2/ailist/LabeledIntervalArray_core.pxd`

 * *Files 15% similar despite different names*

```diff
@@ -1,473 +1,602 @@
 import numpy as np
 cimport numpy as np
-cimport cython
-from libc.stdint cimport uint32_t, int32_t, int64_t, uint16_t
-from libc.stdlib cimport malloc, free
-from .LabeledInterval_core cimport *
+from libc.stdint cimport uint32_t, int32_t, int64_t, int16_t
+from .AIList_core cimport *
+from .Interval_core cimport interval_init
 from .array_query_core cimport *
 ctypedef np.uint8_t uint8
 
 
-cdef extern from "src/labeled_augmented_array.c":
+cdef extern from "src/labeled_aiarray/labeled_augmented_array.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/overlap_label_index.c":
+cdef extern from "src/labeled_aiarray/overlap_label_index.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_add.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_add.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_get.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_get.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_construct.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_construct.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_index.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_index.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_query.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_query_single.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_has_hit.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_query_index.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_nhits.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_query_array.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_wps.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_nhits.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_coverage.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_wps.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_merge.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_coverage.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_filter.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_merge.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_extract.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_filter.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_iter.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_extract.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_aiarray_match.c":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_iter.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/khash.h":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_match.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/labeled_augmented_array.h":
+cdef extern from "src/labeled_aiarray/labeled_aiarray_sort.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/labeled_aiarray/labeled_aiarray_simulate.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/labeled_aiarray/labeled_aiarray_ops.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/labeled_aiarray/labeled_aiarray_percent.c":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/labeled_aiarray/khash.h":
+	# C is include here so that it doesn't need to be compiled externally
+	pass
+
+cdef extern from "src/labeled_aiarray/labeled_augmented_array.h":
+
+	ctypedef struct label_t:
+		const char *name    				# Name of the label
+		ailist_t *ail						# AIList object
+
+	ctypedef struct labeled_interval_t:
+		const char *name
+		interval_t *i
 
 	ctypedef struct labeled_aiarray_t:
-		int64_t nr							# Number of intervals
-		int64_t mr							# Max number of intervals
-		int64_t nl							# Number of unique labels
-		int64_t ml							# Max number of unique labels
-		labeled_interval_t *interval_list	# List of interval_t objects
-		int *nc								# Number of components
-		int *lenC							# Length of components
-		int *idxC							# Index of components in interval_list
-		uint32_t *maxE						# Augmentation
+		label_t *labels        				# List of Labels (of size _n_ctg_)
+		int32_t n_labels, max_labels 		# Number and max number of labels
+		void *label_lookup           	  	# Dict for converting label names to int
 		uint32_t *first						# Record first position of intervals
 		uint32_t *last						# Record last position of intervals
-		uint32_t *label_count				# Record number of label values
-		void *label_map						# Hash table to convert labels to int
-		void *rev_label_map					# Hash table to convert labels to int
-	
-	# C overlap_label_index struct
+		int64_t total_nr					# Total number of regions
+		uint32_t *id_index					# Record id index values
+		int16_t is_constructed				# Flag for whether constructed or not
+
+	ctypedef struct label_sorted_iter_t:
+		const char *name					# Label
+		ailist_sorted_iter_t *ail_iter		# Sorted AIList iterator
+		interval_t *intv					# Interval
+
+	ctypedef struct labeled_aiarray_iter_t:
+		labeled_aiarray_t *laia				# Labeled aiarray
+		int n								# Current position
+		labeled_interval_t *intv			# Interval
+		const char *name					# Label
+
+	ctypedef struct labeled_aiarray_overlap_iter_t:
+		labeled_aiarray_t *ref_laia		# Labeled aiarray
+		labeled_aiarray_iter_t *query_iter	# Reference iterator
+		labeled_aiarray_t *overlaps			# Overlaps
+
 	ctypedef struct overlap_label_index_t:
 		int size							# Current size
 		int max_size						# Maximum size
-		labeled_aiarray_t *ail				# Store labeled_aiarray
+		labeled_aiarray_t *laia				# Store labeled_aiarray
 		long *indices						# Store indices
 
-	ctypedef struct label_sorted_iter_t:
-		labeled_aiarray_t *ail				# Labeled array
-		uint16_t label						# Label
-		int nc								# Number of components
-		int label_start						# First index for label
-		int label_end						# Last index for label
-		int *label_comp_bounds				# Label component bounds
-		int *label_comp_used				# Components used
-		labeled_interval_t *intv			# Interval
-		int n								# Current position
-
 
 	#-------------------------------------------------------------------------------------
 	# labeled_augmented_array.c
 	#=====================================================================================
 
 	# Initialize aiarray_t
 	labeled_aiarray_t *labeled_aiarray_init() nogil
 
 	# Free aiarray data
-	void labeled_aiarray_destroy(labeled_aiarray_t *ail) nogil
+	void labeled_aiarray_destroy(labeled_aiarray_t *laia) nogil
+
+	# Return index for given label
+	int32_t get_label(const labeled_aiarray_t *laia, const char *label) nogil
 
-	# Print aiarray
-	void labeled_display_list(labeled_aiarray_t *ail) nogil
+	# Extract strings from array
+	void slice_str(const char *str, char *buffer, size_t start, size_t end) nogil
 
-	# Print label map
-	void display_label_map(labeled_aiarray_t *ail) nogil
+	# Print labeled_aiarray
+	void labeled_aiarray_print(labeled_aiarray_t *laia) nogil
 
 	# Calculate maximum length
-	int labeled_aiarray_max_length(labeled_aiarray_t *ail) nogil
+	int labeled_aiarray_max_length(labeled_aiarray_t *laia) nogil
 
 	# Calculate length distribution
-	void labeled_aiarray_length_distribution(labeled_aiarray_t *ail, int distribution[]) nogil
-
+	void labeled_aiarray_length_distribution(labeled_aiarray_t *laia, int distribution[]) nogil
 
 	#-------------------------------------------------------------------------------------
 	# overlap_label_index.c
 	#=====================================================================================
 
-	# Initialize overlap_label_index_t
+	# Initialize overlap_index
 	overlap_label_index_t *overlap_label_index_init() nogil
 
 	# Free overlap_label_index memory
 	void overlap_label_index_destroy(overlap_label_index_t *oi) nogil
 
-	# Add interval and index to overlap_label_index
-	void overlap_label_index_add(overlap_label_index_t *aq, labeled_interval_t i, const char *label_name) nogil
+	# Add interval to overlap_label_index
+	void overlap_label_index_add(overlap_label_index_t *oi, interval_t i, const char *label_name) nogil
+
+	void overlap_label_index_wrap_ail(overlap_label_index_t * oi, ailist_t *ail, const char *label_name) nogil
 
 
 	#-------------------------------------------------------------------------------------
 	# labeled_aiarray_add.c
 	#=====================================================================================
 
-	# Add a interval_t from array
-	void labeled_aiarray_from_array(labeled_aiarray_t *ail, const long starts[], const long ends[], const char label_names[], int length, int label_str_len) nogil
+	# Expand and add label
+	void labeled_aiarray_add_label(labeled_aiarray_t *laia, const char*label) nogil
 
 	# Add a interval_t interval
-	void labeled_aiarray_add(labeled_aiarray_t *ail, uint32_t start, uint32_t end, const char *label_name) nogil
+	void labeled_aiarray_add(labeled_aiarray_t *laia, uint32_t s, uint32_t e, const char *label) nogil
+
+	# Link memory of single label labeled_aiarrays and transfer data owership
+	void labeled_aiarray_multi_merge(labeled_aiarray_t *laia, labeled_aiarray_t **laia_array, int length) nogil
+
+	# Add a interval_t from array
+	void labeled_aiarray_from_array(labeled_aiarray_t *laia, const long starts[], const long ends[], const char label_names[], int length, int label_str_len) nogil
 
 	# Add intervals from another labeled_aiarray
-	void labeled_aiarray_append(labeled_aiarray_t *ail, labeled_aiarray_t *ail2) nogil
+	void labeled_aiarray_append(labeled_aiarray_t *laia, labeled_aiarray_t *laia2) nogil
 
 	# Copy labeled_aiarray
-	labeled_aiarray_t *labeled_aiarray_copy(labeled_aiarray_t *ail) nogil
+	labeled_aiarray_t *labeled_aiarray_copy(labeled_aiarray_t *laia) nogil
+
+	# Append AIList in labeled_aiarry
+	void labeled_aiarray_append_ail(labeled_aiarray_t *laia, ailist_t *ail, const char *label_name) nogil
+
+	# Wrap AIList in labeled_aiarry
+	void labeled_aiarray_wrap_ail(labeled_aiarray_t *laia, ailist_t *ail, const char *label_name) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_get.c
+	# labeled_aiarray_construct.c
 	#=====================================================================================
 
-	# Determine if label_name is in array
-	int label_is_present(labeled_aiarray_t *ail, const char *label_name) nogil
+	# Construct aiarray: decomposition and augmentation
+	void labeled_aiarray_construct(labeled_aiarray_t *laia, int cLen) nogil
 
-	# Query label map for label name
-	uint16_t query_label_map(labeled_aiarray_t *ail, const char *label_name) nogil
+	# Validation construction ran
+	int labeled_aiarray_validate_construction(labeled_aiarray_t *laia) nogil
 
-	# Query rev_label_map for label
-	const char *query_rev_label_map(labeled_aiarray_t *ail, uint16_t label) nogil
+	# Deconstruct
+	void labeled_aiarray_deconstruct(labeled_aiarray_t *laia) nogil
 
-	# Get intervals with label name
-	labeled_aiarray_t *get_label(labeled_aiarray_t *ail, const char *label_name) nogil
 
-	# Get intervals with label name and original index
-	overlap_label_index_t *get_label_with_index(labeled_aiarray_t *ail, const char *label_name) nogil
-
-	# Get intervals with labels names from array
-	labeled_aiarray_t *get_label_array(labeled_aiarray_t *ail, const char *label_names[], int length) nogil
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_query_single.c
+	#=====================================================================================
 
-	# Get intervals with labels from array and original index
-	overlap_label_index_t *get_label_array_with_index(labeled_aiarray_t *ail, const char label_names[], int n_labels, int label_str_len) nogil
+	# Base query logic
+	void labeled_aiarray_query(labeled_aiarray_t *laia, labeled_aiarray_t *overlaps, const char *label, uint32_t qs, uint32_t qe) nogil
 
-	# Get index start of label
-	int get_label_index(labeled_aiarray_t *ail, int label) nogil
+	# Base query logic filtered by length
+	void labeled_aiarray_query_length(labeled_aiarray_t *laia, labeled_aiarray_t *overlaps, const char *label_name, 
+									uint32_t qs, uint32_t qe, int min_length, int max_length) nogil
 
-	# Determine label indices
-	void get_label_index_array(labeled_aiarray_t *ail, int *label_index) nogil
+	# Base query logic for nhits
+	void labeled_aiarray_query_nhits(labeled_aiarray_t *laia, long *nhits, const char *label_name, uint32_t qs, uint32_t qe) nogil
 
-	# Get ids for labels in a label array
-	void get_label_array_ids(labeled_aiarray_t *ail, const char *label_names[], int n_labels, long index[]) nogil
+	# Base query logic for nhits filtered by length
+	void labeled_aiarray_query_nhits_length(labeled_aiarray_t *laia, long *nhits, const char *label_name, uint32_t qs,
+											uint32_t qe, int min_length, int max_length) nogil
 
-	# Determine if an index is of a label array
-	void get_label_array_presence(labeled_aiarray_t *ail, const char label_names[], int n_labels, uint8 index[], int label_str_len) nogil
+	# Base query logic if present
+	void labeled_aiarray_query_has_hit(labeled_aiarray_t *laia, const char *label_name, uint8_t *has_hit, uint32_t qs, uint32_t qe) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_construct.c
+	# labeled_aiarray_query_index.c
 	#=====================================================================================
 
-	# Sort intervals in aiarray
-	void labeled_aiarray_sort(labeled_aiarray_t *ail) nogil
+	# Base query logic with index
+	void labeled_aiarray_query_with_index(labeled_aiarray_t *laia, const char *label_name, overlap_label_index_t *overlaps, uint32_t qs, uint32_t qe) nogil
 
-	# Sort intervals by label
-	void labeled_aiarray_radix_label_sort(labeled_aiarray_t *ail) nogil
+	# Query with index from arrays
+	void labeled_aiarray_query_with_index_from_array(labeled_aiarray_t *laia, overlap_label_index_t *overlaps, const char label_names[], const long starts[], const long ends[], int length, int label_str_len) nogil
 
-	# Construct aiarray: decomposition and augmentation
-	void labeled_aiarray_construct(labeled_aiarray_t *ail, int cLen_init) nogil
+	# Query with index from labeled_aiarray
+	void labeled_aiarray_query_with_index_from_labeled_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia, overlap_label_index_t *overlaps) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_iter.c
+	# labeled_aiarray_query_array.c
 	#=====================================================================================
 
-	# Get component index for label
-	int *get_label_comp_bounds(labeled_aiarray_t *ail, int label) nogil
+	# Base query logic with index
+	void labeled_aiarray_query_only_index(labeled_aiarray_t *laia, const char *label_name, array_query_t *overlaps, uint32_t qs, uint32_t qe, uint32_t id) nogil
 
-	label_sorted_iter_t *iter_init(labeled_aiarray_t *ail, const char *label_name) nogil
+	# Query aiarray intervals from array
+	array_query_t *labeled_aiarray_query_index_from_array(labeled_aiarray_t *laia, const char label_names[], const long starts[], const long ends[], int length, int label_str_len) nogil
 
-	int iter_next(label_sorted_iter_t *iterator) nogil
+	# Query intervals from array
+	void labeled_aiarray_query_from_array(labeled_aiarray_t *laia, labeled_aiarray_t *overlaps, const char label_names[], const long starts[], const long ends[], int length, int label_str_len) nogil	
 
-	void iter_destroy(label_sorted_iter_t *iterator) nogil
+	# Query array if present
+	void labeled_aiarray_query_has_hit_from_array(labeled_aiarray_t *laia, const char label_names[], const long starts[], const long ends[], int length, int label_str_len, uint8_t has_hit[]) nogil
 
+	# Query aiarray intervals from aiarray
+	void labeled_aiarray_query_from_labeled_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *laia2, labeled_aiarray_t *overlaps) nogil
 
-	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_match.c
-	#=====================================================================================
+	# Query aiarray intervals from aiarray
+	void labeled_aiarray_query_index_from_labeled_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *laia2, array_query_t *aq) nogil
 
-	overlap_label_index_t *has_exact_match(labeled_aiarray_t *ail1, labeled_aiarray_t *ail2) nogil
 
 	#-------------------------------------------------------------------------------------
 	# labeled_aiarray_index.c
 	#=====================================================================================
 
-	# Record id positions by id
 	void labeled_aiarray_cache_id(labeled_aiarray_t *ail) nogil
 
-	# Get intervals with ids
-	labeled_aiarray_t *labeled_aiarray_slice_index(labeled_aiarray_t *ail, const long ids[], int length) nogil
+	labeled_interval_t *labeled_aiarray_get_index(labeled_aiarray_t *ail, int32_t i) nogil
 
-	# Get intervals with range
-	labeled_aiarray_t *labeled_aiarray_slice_range(labeled_aiarray_t *ail, int start, int end, int step) nogil
+	labeled_aiarray_t *labeled_aiarray_slice_index(labeled_aiarray_t *laia, const long ids[], int length) nogil
 
-	# Get intervals with boolean array
-	labeled_aiarray_t *labeled_aiarray_slice_bool(labeled_aiarray_t *ail, uint8 bool_index[]) nogil
+	labeled_aiarray_t *labeled_aiarray_slice_range(labeled_aiarray_t *laia, int start, int end, int step) nogil
 
-	# Get interval with id
-	labeled_interval_t *labeled_aiarray_get_id(labeled_aiarray_t *ail, int id_value) nogil
+	labeled_aiarray_t *labeled_aiarray_slice_bool(labeled_aiarray_t *laia, uint8_t bool_index[]) nogil
 
-	# Index aiarray by another aiarray inplace
-	int labeled_aiarray_index_by_aiarray_inplace(labeled_aiarray_t *ail1, labeled_aiarray_t *ail2) nogil
+	int labeled_aiarray_index_with_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_query.c
+	# labeled_aiarray_iter.c
 	#=====================================================================================
 
-	# Binary search
-	uint32_t binary_search_labeled(labeled_interval_t* As, uint32_t idxS, uint32_t idxE, uint32_t qe) nogil
+	label_sorted_iter_t *label_sorted_iter_init(labeled_aiarray_t *laia, const char *label_name) nogil
 
-	# Base query logic
-	void labeled_aiarray_query(labeled_aiarray_t *ail, labeled_aiarray_t *overlaps, uint32_t qs, uint32_t qe, const char *label_name) nogil
+	int label_sorted_iter_next(label_sorted_iter_t *iter) nogil
 
-	# Base query logic filtered by length
-	void labeled_aiarray_query_length(labeled_aiarray_t *ail, labeled_aiarray_t *overlaps, uint32_t qs, uint32_t qe, const char *label_name, int min_length, int max_length) nogil
+	void label_sorted_iter_destroy(label_sorted_iter_t *iter) nogil
 
-	# Base query logic for nhits
-	void labeled_aiarray_query_nhits(labeled_aiarray_t *ail, long *nhits, uint32_t qs, uint32_t qe, const char *label_name) nogil
+	labeled_aiarray_iter_t *labeled_aiarray_iter_init(labeled_aiarray_t *laia) nogil
 
-	# Base query logic for nhits filtered by length
-	void labeled_aiarray_query_nhits_length(labeled_aiarray_t *ail, long *nhits, uint32_t qs, uint32_t qe, const char *label_name, int min_length, int max_length) nogil
+	int labeled_aiarray_iter_next(labeled_aiarray_iter_t *iter) nogil
 
-	# Base query logic with index
-	void labeled_aiarray_query_with_index(labeled_aiarray_t *ail, overlap_label_index_t *overlaps, uint32_t qs, uint32_t qe, const char *label_name) nogil
+	void labeled_aiarray_iter_destroy(labeled_aiarray_iter_t *iter) nogil
 
-	# Base query logic with index
-	void labeled_aiarray_query_only_index(labeled_aiarray_t *ail, array_query_t *overlaps, uint32_t qs, uint32_t qe, uint32_t id_value, const char *label_name) nogil
+	labeled_aiarray_overlap_iter_t *labeled_aiarray_overlap_iter_init(labeled_aiarray_t *ref_laia, labeled_aiarray_t *query_laia) nogil
 
-	# Base query logic if present
-	void labeled_aiarray_query_has_hit(labeled_aiarray_t *ail, uint8 has_hit[], uint32_t qs, uint32_t qe, const char *label_name) nogil
+	int labeled_aiarray_overlap_iter_next(labeled_aiarray_overlap_iter_t *iter) nogil
 
-	# Query interval
-	labeled_aiarray_t *labeled_aiarray_query_single(labeled_aiarray_t *ail, uint32_t qs, uint32_t qe, const char *label_name) nogil
+	void labeled_aiarray_overlap_iter_destroy(labeled_aiarray_overlap_iter_t *iter) nogil
 
-	# Query aiarray intervals of a length
-	labeled_aiarray_t *labeled_aiarray_query_single_length(labeled_aiarray_t *ail, uint32_t qs, uint32_t qe, const char *label_name, int min_length, int max_length) nogil
 
-	# Query aiarray intervals from arrays
-	array_query_t *labeled_aiarray_query_from_array(labeled_aiarray_t *ail, const long starts[], const long ends[], const char label_names[], int length, int label_str_len) nogil
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_nhits.c
+	#=====================================================================================
 
-	# Query aiarray intervals from aiarray
-	array_query_t *labeled_aiarray_query_from_labeled_aiarray(labeled_aiarray_t *ail, labeled_aiarray_t *ail2) nogil
+	void labeled_aiarray_nhits(labeled_aiarray_t *laia, long *nhits, const char *label_name, uint32_t qs, uint32_t qe) nogil
 
-	# Query aiarray intervals and record original index
-	overlap_label_index_t *labeled_aiarray_query_single_with_index(labeled_aiarray_t *ail, uint32_t qs, uint32_t qe, const char *label_name) nogil
+	void labeled_aiarray_nhits_length(labeled_aiarray_t *laia, long *nhits, const char *label_name, uint32_t qs,
+											uint32_t qe, int min_length, int max_length) nogil
 
-	# Query aiarray intervals and record original index from labled_aiarray
-	overlap_label_index_t *labeled_aiarray_query_with_index_from_labeled_aiarray(labeled_aiarray_t *ail, labeled_aiarray_t *ail2) nogil
+	void labeled_aiarray_nhits_from_array(labeled_aiarray_t *laia, const char label_names[], const long starts[], const long ends[],
+											int length, int label_str_len, long *nhits) nogil
 
-	
-	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_has_hits.c
-	#=====================================================================================
+	void labeled_aiarray_nhits_from_array_length(labeled_aiarray_t *laia, const char label_names[], const long starts[], const long ends[],
+											int length, int label_str_len, long *nhits, int min_length, int max_length) nogil
 
-	# Determine if hit is present for each query interval
-	void labeled_aiarray_has_hit_from_array(labeled_aiarray_t *ail, const long starts[], const long ends[],
-                                        const char label_names[], int length, int label_str_len, uint8 has_hit[]) nogil
+	void labeled_aiarray_nhits_from_labeled_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia,
+													long *nhits) nogil
 
-	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_nhits.c
-	#=====================================================================================
+	void labeled_aiarray_nhits_from_labeled_aiarray_length(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia,
+													long *nhits, int min_length, int max_length) nogil
 
-	# Determine number of hits for interval
-	long labeled_aiarray_nhits(labeled_aiarray_t *ail, long start, long end, const char *label_name) nogil
+	void labeled_aiarray_has_hit(labeled_aiarray_t *laia, const char *label_name, uint8_t has_hit[], uint32_t qs, uint32_t qe) nogil
 
-	# Determine number of hits for interval of a length
-	long labeled_aiarray_nhits_length(labeled_aiarray_t *ail, long start, long end, const char *label_name, int min_length, int max_length) nogil
+	void labeled_aiarray_bin_nhits(labeled_aiarray_t *laia, long *nhits, int bin_size) nogil
 
-	# Determine number of hits for each query interval
-	void labeled_aiarray_nhits_from_array(labeled_aiarray_t *ail, const long starts[], const long ends[],
-											const char *label_names[], int length, int nhits[]) nogil
-
-	# Determine number of hits of a length for each query interval
-	void labeled_aiarray_nhits_from_array_length(labeled_aiarray_t *ail, const long starts[], const long ends[],
-												const char *label_names[], int length, int nhits[], int min_length,
-												int max_length) nogil
-
-	# Calculate n hits within bins
-	void labeled_aiarray_bin_nhits(labeled_aiarray_t *ail, labeled_aiarray_t *bins, double nhits[], int bin_size) nogil
-
-	# Calculate n hits of a length within bins
-	void labeled_aiarray_bin_nhits_length(labeled_aiarray_t *ail, labeled_aiarray_t *bins, double nhits[], int bin_size,
-											int min_length, int max_length) nogil
+	void labeled_aiarray_bin_nhits_length(labeled_aiarray_t *laia, long *nhits, int bin_size, int min_length, int max_length) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_wps.c
+	# labeled_aiarray_coverage.c
 	#=====================================================================================
 
-	# Calculate Window Protection Score for a label
-	void labeled_aiarray_label_wps(labeled_interval_t *interval_list, double wps[], uint32_t protection, int nr, int first, int last) nogil
+	# Determine coverage for an interval
+	void labeled_aiarray_interval_coverage(labeled_aiarray_t *laia, int start, int end, const char *label_name, int coverage[]) nogil
 
-	# Calculate Window Protection Score
-	void labeled_aiarray_wps(labeled_aiarray_t *ail, double wps[], uint32_t protection) nogil
+	# Calculate coverage for a label
+	void labeled_aiarray_label_coverage(labeled_aiarray_t *laia, double coverage[], const char *label_name) nogil
 
-	# Calculate Window Protection Score for a label of a length
-	void labeled_aiarray_label_wps_length(labeled_interval_t *interval_list, double wps[], uint32_t protection, int nr, int first, int last,
-											int min_length, int max_length) nogil
+	# Calculate coverage for a label of a length
+	void labeled_aiarray_label_coverage_length(labeled_aiarray_t *laia, double coverage[], const char *label_name,
+												int min_length, int max_length) nogil
+
+	# Calculate coverage within bins
+	void labeled_aiarray_label_bin_coverage(labeled_aiarray_t *laia, double coverage[], int bin_size, const char *label_name) nogil
+
+	# Calculate coverage of intervals of a given length within bins
+	void labeled_aiarray_label_bin_coverage_length(labeled_aiarray_t *laia, double coverage[], int bin_size, const char *label_name,
+													int min_length, int max_length) nogil
+	
+	# Calculate interval midpoint coverage
+	void labeled_aiarray_label_midpoint_coverage(labeled_aiarray_t *laia, double coverage[], const char *label_name) nogil
 
-	# Calculate Window Protection Score of a length
-	void labeled_aiarray_wps_length(labeled_aiarray_t *ail, double wps[], uint32_t protection, int min_length, int max_length) nogil
+	# Calculate interval midpoitn coverage with lengths
+	void labeled_aiarray_label_midpoint_coverage_length(labeled_aiarray_t *laia, double coverage[], const char *label_name,
+														int min_length, int max_length) nogil
 
 
 	#-------------------------------------------------------------------------------------
-	# labeled_aiarray_coverage.c
+	# labeled_aiarray_wps.c
 	#=====================================================================================
 
-	# Determine coverage for an interval
-	void labeled_aiarray_interval_coverage(labeled_aiarray_t *ail, int start, int end, const char *label_name, int coverage[]) nogil
+	# Calculate Window Protection Score for a label
+	void labeled_aiarray_label_wps(labeled_aiarray_t *laia, double wps[], uint32_t protection, const char *label_name) nogil
 
-	# Calculate coverage for a label
-	void labeled_aiarray_label_coverage(labeled_interval_t *interval_list, double coverage[], const char *label_name, int nr) nogil
+	# Calculate Window Protection Score for a label of a length
+	void labeled_aiarray_label_wps_length(labeled_aiarray_t *laia, double wps[], uint32_t protection, int min_length, int max_length, const char *label_name) nogil
 
-	# Calculate coverage
-	void labeled_aiarray_coverage(labeled_aiarray_t *ail, double coverage[]) nogil
 
 	#-------------------------------------------------------------------------------------
 	# labeled_aiarray_merge.c
 	#=====================================================================================
 
 	# Merge nearby intervals
-	labeled_aiarray_t *labeled_aiarray_merge(labeled_aiarray_t *ail, uint32_t gap) nogil
+	labeled_aiarray_t *labeled_aiarray_merge(labeled_aiarray_t *laia, uint32_t gap) nogil
 
 
 	#-------------------------------------------------------------------------------------
 	# labeled_aiarray_filter.c
 	#=====================================================================================
 
-	# Filter labeled_aiarray by length
-	labeled_aiarray_t *labeled_aiarray_length_filter(labeled_aiarray_t *ail, int min_length, int max_length) nogil
-
-	# Randomly downsample
-	labeled_aiarray_t *labeled_aiarray_downsample(labeled_aiarray_t *ail, double proportion) nogil
+	# Filter labeled_aiarray by length 
+	labeled_aiarray_t *labeled_aiarray_length_filter(labeled_aiarray_t *laia, int min_length, int max_length) nogil
 
-	# Randomly downsample with original index
-	overlap_label_index_t *labeled_aiarray_downsample_with_index(labeled_aiarray_t *ail, double proportion) nogil
+	# Randomly downsample 
+	labeled_aiarray_t *labeled_aiarray_downsample(labeled_aiarray_t *laia, double proportion) nogil
 
+	overlap_label_index_t *labeled_aiarray_downsample_with_index(labeled_aiarray_t *laia, double proportion) nogil
 
 	#-------------------------------------------------------------------------------------
 	# labeled_aiarray_extract.c
 	#=====================================================================================
 
 	# Extract start for labeled_aiarray
-	void labeled_aiarray_extract_starts(labeled_aiarray_t *ail, long starts[]) nogil
+	void labeled_aiarray_extract_starts(labeled_aiarray_t *laia, long starts[]) nogil
 
 	# Extract end for labeled_aiarray
-	void labeled_aiarray_extract_ends(labeled_aiarray_t *ail, long ends[]) nogil
+	void labeled_aiarray_extract_ends(labeled_aiarray_t *laia, long ends[]) nogil
 
 	# Extract id for labeled_aiarray
-	void labeled_aiarray_extract_ids(labeled_aiarray_t *ail, long ids[]) nogil
+	void labeled_aiarray_extract_ids(labeled_aiarray_t *laia, long ids[]) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_match.c
+	#=====================================================================================
+
+	# Return all exact matches between labeled_aiarrays
+	overlap_label_index_t *labeled_aiarray_exact_match(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2) nogil
+
+	void labeled_aiarray_has_exact_match(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2, uint8_t has_match[]) nogil
+
+	# Return exact matches between labeled_aiarrays
+	void labeled_aiarray_is_exact_match(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2, uint8_t has_match_laia1[], uint8_t has_match_laia2[]) nogil
+
+	# Return exact matches between labeled_aiarrays
+	void labeled_aiarray_which_exact_match(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2, array_query_t *matches) nogil
+
+	# Return exact match between labeled_aiarray and an interval
+	int labeled_aiarray_where_interval(labeled_aiarray_t *laia, const char *label, uint32_t qs, uint32_t qe) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_get.c
+	#=====================================================================================
+
+	# Get intervals with label name
+	labeled_aiarray_t *labeled_aiarray_get_label(labeled_aiarray_t *laia, const char *label_name) nogil
+
+	# Get intervals with label name
+	labeled_aiarray_t *labeled_aiarray_view_label(labeled_aiarray_t *laia, const char *label_name) nogil
 
+	# Get intervals with label name and original index
+	overlap_label_index_t *labeled_aiarray_get_label_with_index(labeled_aiarray_t *laia, const char *label_name) nogil
+
+	# Get intervals with labels names from array
+	labeled_aiarray_t *labeled_aiarray_get_label_array(labeled_aiarray_t *laia, const char label_names[], int n_labels, int label_str_len) nogil
+
+	# Get intervals with labels from array and original index
+	overlap_label_index_t *labeled_aiarray_get_label_array_with_index(labeled_aiarray_t *laia, const char label_names[], int n_labels, int label_str_len) nogil
+
+	# Determine if an index is of a label array
+	void labeled_aiarray_get_label_array_presence(labeled_aiarray_t *ail, const char label_names[], int n_labels, uint8_t index[], int label_str_len) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_sort.c
+	#=====================================================================================
+
+	# Sort intervals by actual order
+	void labeled_aiarray_order_sort(labeled_aiarray_t *laia) nogil
+
+	# Sort intervals by starts
+	void labeled_aiarray_sort_index(labeled_aiarray_t *laia, long *index) nogil
+
+	# Sort intervals by starts
+	void labeled_aiarray_sort(labeled_aiarray_t *laia) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_simulate.c
+	#=====================================================================================
+
+	# Simulate intervals
+	void labeled_aiarray_simulate(labeled_aiarray_t *laia, labeled_aiarray_t *sim_laia) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_ops.c
+	#=====================================================================================
+
+	# Find common intervals between two labeled_aiarrays
+	labeled_aiarray_t *labeled_aiarray_common(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2) nogil
+
+	# Subtract intervals from laia1 that are in laia2
+	labeled_aiarray_t *labeled_aiarray_subtract(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2) nogil
+
+	# Find union of intervals between two labeled_aiarrays
+	labeled_aiarray_t *labeled_aiarray_union(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2) nogil
+
+
+	#-------------------------------------------------------------------------------------
+	# labeled_aiarray_percent.c
+	#=====================================================================================
+
+	# Find percent coverage of intervals in laia1 that are in laia2
+	void labeled_aiarray_percent_coverage(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2, double coverage[]) nogil
+
+
+#cpdef object rebuild_LabeledIntervalArray(bytes data, bytes b_length, bytes b_label_list)
+
+cdef class LabeledInterval(object):
+	"""
+	Wrapper for C labeled interval
+	"""
+
+	# Define attributes
+	cdef str _label
+
+	# C instance of struct
+	cdef interval_t *i
+
+	# Methods for serialization
+	cdef void set_i(self, interval_t *i, str label)
 
-cpdef object rebuild_LabeledIntervalArray(bytes data, bytes b_length, bytes b_label_list)
 
 cdef class LabeledIntervalArray(object):
 	"""
 	Wrapper for C aiarray_t
 	"""
 
 	# Define class properties
-	cdef labeled_aiarray_t *ail
-	cdef public bint is_constructed
+	cdef labeled_aiarray_t *laia
 	cdef public bint is_closed
 	cdef public bint is_frozen
 
 	# Functions for serialization
-	cdef bytes _get_data(self)
-	cdef labeled_aiarray_t *_set_data(self, bytes data, bytes b_length, bytes b_label_list)
+	#cdef bytes _get_data(self)
+	#cdef labeled_aiarray_t *_set_data(self, bytes data, bytes b_length, bytes b_label_list)
 
 	# Class methods
 	cdef void set_list(LabeledIntervalArray self, labeled_aiarray_t *input_list)
+	cdef ailist_t *_get_ail(LabeledIntervalArray self, char *label_name)
 
 	cdef labeled_aiarray_t *_array_index(LabeledIntervalArray self, const long[::1] ids)
 	cdef np.ndarray _get_index(LabeledIntervalArray self, str label)
 	cdef np.ndarray _get_index_multi(LabeledIntervalArray self, np.ndarray labels)
 
 	cdef void _insert(LabeledIntervalArray self, int start, int end, const char *label)
 	cdef void _construct(LabeledIntervalArray self, int min_length)
 	cdef void _from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *label_names, int array_length, int label_str_len)
-	cdef void _append(LabeledIntervalArray self, LabeledIntervalArray other_ail)
+	cdef void _append(LabeledIntervalArray self, LabeledIntervalArray other_laia)
 
-	cdef int _get_label_index(LabeledIntervalArray self, int label)
-	cdef np.ndarray _get_label_comp_bounds(LabeledIntervalArray self, int label)
-	cdef np.ndarray _get_label_comp_length(LabeledIntervalArray self, int label)
-	cdef labeled_aiarray_t *get_labels(LabeledIntervalArray self, const char[:,::1] labels, int length)
+	#cdef int _get_label_index(LabeledIntervalArray self, int label)
+	#cdef np.ndarray _get_label_comp_bounds(LabeledIntervalArray self, int label)
+	#cdef np.ndarray _get_label_comp_length(LabeledIntervalArray self, int label)
+	cdef labeled_aiarray_t *get_labels(LabeledIntervalArray self, const char *label_names, int str_label_len, int length)
 	cdef overlap_label_index_t *get_labels_with_index(LabeledIntervalArray self, const char *label_names, int str_label_len, int length)
 
 	cdef labeled_aiarray_t *_intersect(LabeledIntervalArray self, int start, int end, const char *label_name)
-	cpdef _intersect_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *labels, int label_str_len)
-	cpdef _has_hit_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, uint8[::1] has_hit, const char *labels, int label_str_len)
-	cpdef _intersect_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray ail)
+	cdef labeled_aiarray_t *_intersect_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *labels, int label_str_len)
+	cpdef _intersect_from_array_only_index(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *labels, int label_str_len)
+	
+	cdef void _has_hit_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, uint8[::1] has_hit, const char *labels, int label_str_len)
+	cdef labeled_aiarray_t *_intersect_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray laia)
+	cpdef _intersect_index_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray laia)
 	cpdef _intersect_with_index(LabeledIntervalArray self, int start, int end, const char *label_name)
-	cpdef _intersect_with_index_from_LabeledIntervalArray(LabeledIntervalArray self, LabeledIntervalArray ail2)
+	cpdef _intersect_with_index_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray ail2)
+	cpdef _intersect_from_array_with_index(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *labels, int label_str_len)
 
-	cdef np.ndarray _nhits_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char[:,::1] labels)
-	cdef np.ndarray _nhits_from_array_length(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char[:,::1] labels, int min_length, int max_length)
+	cdef void _nhits_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, long[::1] nhits,
+								const char *labels, int label_str_len)
+	cdef void _nhits_from_array_length(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, long[::1] nhits,
+										const char *labels, int label_str_len, int min_length, int max_length)
 
 	cdef labeled_aiarray_t *_determine_bins(LabeledIntervalArray self, int bin_size)
-	cdef np.ndarray _bin_nhits(LabeledIntervalArray self, labeled_aiarray_t *bins, int bin_size)
-	cdef np.ndarray _bin_nhits_length(LabeledIntervalArray self, labeled_aiarray_t *bins, int bin_size, int min_length, int max_length)
+	cdef void _bin_nhits(LabeledIntervalArray self, long[::1] nhits, int bin_size)
+	cdef void _bin_nhits_length(LabeledIntervalArray self, long[::1] nhits, int bin_size, int min_length, int max_length)
 
-	cdef np.ndarray _wps(LabeledIntervalArray self, int protection)
-	cdef np.ndarray _wps_length(LabeledIntervalArray self, int protection, int min_length, int max_length)
+	cdef np.ndarray _wps(LabeledIntervalArray self, const char *label_name, int protection)
+	cdef np.ndarray _wps_length(LabeledIntervalArray self, const char *label_name, int protection, int min_length, int max_length)
 
-	cdef np.ndarray _coverage(LabeledIntervalArray self)
+	cdef np.ndarray _coverage(LabeledIntervalArray self, const char *label_name)
+	cdef np.ndarray _coverage_length(LabeledIntervalArray self, const char *label_name, int min_length, int max_length)
 
 	cpdef _downsample_with_index(LabeledIntervalArray self, double proportion)
 	cdef np.ndarray _length_dist(LabeledIntervalArray self)
 	cpdef _filter_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray)
-	cdef np.ndarray _has_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray)
+	cdef void _has_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray, uint8_t[::1] has_match)
+	cdef void _is_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray, uint8_t[::1] has_match1, uint8_t[::1] has_match2)
+	cpdef _which_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray)
+	cdef int _where_interval(LabeledIntervalArray self, int start, int end, const char *label_name)
 	cdef int _index_with_aiarray(LabeledIntervalArray self, LabeledIntervalArray other_aiarray)
-	cdef void _get_locs(LabeledIntervalArray self, uint8[::1] locs_view, char *label_names, int label_str_len, int n_labels)
+	cdef void _get_locs(LabeledIntervalArray self, uint8[::1] locs_view, char *label_names, int label_str_len, int n_labels)
+
+	cdef void _create_bin(LabeledIntervalArray self, int bin_size, int bin_range, const char* label_name)
+	cdef np.ndarray _midpoint_coverage(LabeledIntervalArray self, const char *label_name)
+
+	cdef np.ndarray _percent_coverage(LabeledIntervalArray self, LabeledIntervalArray other_laia)
+
```

### Comparing `ailist-1.0.4/ailist/LabeledIntervalArray_core.pyx` & `ailist-2.0.2/ailist/LabeledIntervalArray_core.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 #cython: embedsignature=True
 #cython: profile=False
 
+import pandas as pd
 import os
 import sys
 import numpy as np
 cimport numpy as np
 import math
-cimport cython
-import pandas as pd
-from libc.string cimport memcpy
 np.import_array()
-from time import time
-from libc.stdio cimport printf
 
 # Set byteorder for __reduce__
 byteorder = sys.byteorder
 
 
 def get_include():
 	"""
@@ -29,58 +25,171 @@
 	-------
 		str (Directory to header files)
 	"""
 
 	return os.path.split(os.path.realpath(__file__))[0]
 
 
-cpdef LabeledIntervalArray rebuild_LabeledIntervalArray(bytes data, bytes b_length, bytes b_label_list):
+cdef class LabeledInterval(object):
 	"""
-	Rebuild function for __reduce__()
+	Wrapper of C interval_t and label
 
-	Parameters
-	----------
-		data : bytes 
-			Bytes representation of labeled_aiarray_t
-		b_length : bytes 
-			Length of labeled_aiarray_t
+	:class:`~ailist.LabeledInterval` stores an interval
 
-	Returns
-	-------
-		c : labeled_aiarray_t* 
-			Translated labeled_aiarray_t from data
 	"""
 
-	# Initialize new LabeledIntervalArray
-	c = LabeledIntervalArray()
+	def __init__(self,
+				 start = None,
+				 end = None,
+				 id_value = None,
+				 label = None):
+		"""
+		Initialize LabeledInterval
+
+		Parameters
+		----------
+			start : int
+				Starting position [default = None]
+			end : int
+				Ending position [default = None]
+			id_value : int
+				ID [defualt = None]
+			label : str
+				Label
+
+		Returns
+		-------
+			None
+
+		"""
+
+		if start is not None:
+			if id_value is None:
+				id_value = 0
+
+			# Create interval
+			self.i = interval_init(start, end, id_value)
+			self._label = label
+
+	# Set the interval
+	cdef void set_i(LabeledInterval self,
+					interval_t *i,
+					str label):
+		"""
+		Initialize wrapper of C interval
+
+		Parameters
+		----------
+			i : interval_t
+				C interval_t to be wrapped
+
+		Returns
+		-------
+			None
+		"""
+
+		# Set i
+		self.i = i
+		self._label = label
+
+
+	@property
+	def start(self):
+		"""
+		Start of interval
+		"""
+		return self.i.start
+
+	@property
+	def end(self):
+		"""
+		End of interval
+		"""
+		return self.i.end
+
+	@property
+	def id_value(self):
+		"""
+		ID of interval
+		"""
+		return self.i.id_value
+
+	@property
+	def label(self):
+		"""
+		Label of interval
+		"""
+		return self._label
+
+
+	def __hash__(self):
+		"""
+		Get hash value
+		"""
+
+		return hash(repr(self))
+
 
-	# Build aiarray from serialized data
-	cdef labeled_aiarray_t *interval_list = c._set_data(data, b_length, b_label_list)
-	c.set_list(interval_list)
+	def __eq__(self, other):
+		"""
+		Check if there is overlap
+		"""
 
-	return c
+		# Check that the classes match
+		is_equal = self.__class__ == other.__class__
 
+		# Check for overlap
+		if is_equal:
+			if self.label == other.label:
+				if other.start < self.i.end and other.end > self.i.start:
+					is_equal = True
+				else:
+					is_equal = False
+			else:
+				is_equal = False
 
-@cython.auto_pickle(True)
+		return is_equal
+
+
+	def __str__(self):
+		format_string = "Interval(%d-%d, %s)" % (self.start, self.end, self.label)
+		return format_string
+
+
+	def __repr__(self):
+		format_string = "Interval(%d-%d, %s)" % (self.start, self.end, self.label)
+		return format_string
+
+
+	def to_array(self):
+		"""
+		"""
+
+		laia = LabeledIntervalArray()
+		laia.add(self.start, self.end, self.label)
+
+		return laia
+
+
+#@cython.auto_pickle(True)
 cdef class LabeledIntervalArray(object):
 	"""
 	Wrapper for C labeled_aiarray_t
 
-	:class:`~aiarray.LabeledIntervalArray` stores a list of intervals
+	:class:`~ailist.LabeledIntervalArray` stores a list of intervals
 	"""
 
 	def __cinit__(self):
 		"""
 		C Initialize LabeledIntervalArray object
 		(Runs after __init__)
 		"""
 
 		# Initialize C level attributes
-		self.ail = labeled_aiarray_init()
-		self.is_constructed = False
+		self.laia = labeled_aiarray_init()
 		self.is_closed = False
 		self.is_frozen = False
 
 
 	def __init__(self):
 		"""
 		Initialize LabeledIntervalArray object
@@ -97,263 +206,258 @@
 
 		# Initialize Python level attributes
 		pass
 
 
 	def __dealloc__(self):
 		"""
-		Free LabeledIntervalArray.ail
+		Free LabeledIntervalArray.laia
 		"""
-		
-		# Free C labeled_aiarray_t
-		#if self.ail:
-			#labeled_aiarray_destroy(self.ail)
-		labeled_aiarray_destroy(self.ail)
-
 
-	cdef bytes _get_data(self):
-		"""
-		Function to convert labeled_aiarray_t to bytes
-		for serialization by __reduce__()
-		"""
+		labeled_aiarray_destroy(self.laia)
 
-		return <bytes>(<char*>self.ail.interval_list)[:(sizeof(labeled_interval_t) * self.ail.nr)]
-
-	cdef labeled_aiarray_t *_set_data(self, bytes data, bytes b_length, bytes b_label_list):
-		"""
-		Function to build labeled_aiarray_t object from
-		serialized bytes using __reduce__()
-
-		Parameters
-		----------
-			data : bytes 
-				Bytes representation of labeled_aiarray_t
-			b_length : bytes
-				Length of labeled_aiarray_t
-
-		Returns
-		---------
-			interval_list : labeled_aiarray_t*
-				Translated labeled_aiarray_t for bytes
-		"""
-		
-		# Convert bytes to ints
-		cdef int length = int.from_bytes(b_length, byteorder)
-		
-		# Create new labeled_aiarray_t
-		cdef labeled_aiarray_t *aia = labeled_aiarray_init()
-		cdef labeled_interval_t *interval_list = <labeled_interval_t*>malloc(length * sizeof(labeled_interval_t))
-		memcpy(interval_list, <char*>data, sizeof(labeled_interval_t)*length)
-
-		# Iteratively add intervals to labeled_interval_list
-		cdef list label_list = b_label_list.split(b";;")
-		#cdef bytes label_name	
-		cdef int i
-		for i in range(length):
-			labeled_aiarray_add(aia, interval_list[i].start, interval_list[i].end, label_list[interval_list[i].label])
-			#pass
 
-		return aia
-
-
-	def __reduce__(self):
+	@property
+	def size(self):
 		"""
-		Used for pickling. Convert labeled_aiarray to bytes and back.
+		Number of intervals in LabeledIntervalArray
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
-		
-		# Convert ints to bytes
-		b_length = int(self.ail.nr).to_bytes(4, byteorder)
-
-		# Convert labeled_aiarray_t to bytes
-		data = self._get_data()
 
-		# Record label_map
-		label_list = ";;".join(list(self.label_map.keys()))
-		b_label_list = label_list.encode()
+		return self.laia.total_nr
 
-		return (rebuild_LabeledIntervalArray, (data, b_length, b_label_list))
-
-	
 	@property
-	def label_map(self):
+	def unique_labels(self):
 		"""
-		Dictionary of label names toe integer representation
+		Array of unique labels
 		"""
 
-		# Initialize label map
-		lmap = {}
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Iterate over keys
 		cdef const char *label_name
+
+		labels = []
 		cdef int i
-		for i in range(self.ail.nl):
-			label_name = query_rev_label_map(self.ail, i)
-			lmap[label_name.decode()] = i
+		for i in range(self.laia.n_labels):
+			label_name = self.laia.labels[i].name
+			labels.append(label_name.decode())
 
-		return lmap
+		# Convert to numpy array
+		labels = np.array(labels)
+
+		return labels
 
 	@property
-	def rev_label_map(self):
+	def label_counts(self):
 		"""
-		Dictionary of label names to integer representation
+		Count number of intervals per label
 		"""
 
-		# Initialize label map
-		lmap = {}
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Iterate over keys
+		# Iterate over labels
+		counts = {}
 		cdef const char *label_name
 		cdef int i
-		for i in range(self.ail.nl):
-			label_name = query_rev_label_map(self.ail, i)
-			lmap[i] = label_name.decode()
+		for i in range(self.laia.n_labels):
+			label_name = self.laia.labels[i].name
+			counts[label_name.decode()] = self.laia.labels[i].ail.nr
 
-		return lmap
-	
-	@property	
-	def size(self):
+		return counts
+
+
+	@property
+	def label_ranges(self):
 		"""
-		Number of intervals in LabeledIntervalArray
+		Ranges(start,  end) for each label
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		return self.ail.nr
+		# Iterate over first and last
+		cdef dict ranges = {}
+		cdef const char *label_name
+		cdef int i
+		for i in range(self.laia.n_labels):
+			label_name = self.laia.labels[i].name
+			ranges[label_name.decode()] = (self.laia.labels[i].ail.first, self.laia.labels[i].ail.last)
+
+		return ranges
+
 
 	@property
-	def unique_labels(self):
+	def is_constructed(self):
 		"""
-		Array of unique labels
+		Whether LabeledIntervalArray is constructed or not
 		"""
 
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("LabeledIntervalArray object has been closed.")
+		if self.laia.is_constructed == 0:
+			return False
+		else:
+			return True
 
-		# Find labels
-		labels = np.array(list(self.label_map.keys()))
-		
-		return labels
 
 	@property
-	def label_counts(self):
+	def starts(self):
 		"""
-		Count number of intervals per label
+		Start values
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Iterate over labels
-		counts = {}
-		for label in self.label_map:
-			start = self._get_label_index(self.label_map[label])
-			end = self._get_label_index(self.label_map[label]+1)
-			counts[label] = end - start
+		# Extract start values
+		cdef long[::1] starts = np.zeros(self.size, dtype=np.int_)
+		labeled_aiarray_extract_starts(self.laia, &starts[0])
+
+		return np.asarray(starts, dtype=np.int_)
 
-		return counts
 
 	@property
-	def label_index(self):
+	def ends(self):
 		"""
-		Index of labels in sorted LabeledIntervalArray
+		End values
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Iterate over label_index
-		cdef int i
-		cdef np.ndarray index = np.zeros(self.ail.nl, dtype=int)
-		for i in range(self.ail.nl):
-			index[i] = self._get_label_index(i)
-		
-		return index
+		# Extract end values
+		cdef long[::1] ends = np.zeros(self.size, dtype=np.int_)
+		labeled_aiarray_extract_ends(self.laia, &ends[0])
+
+		return np.asarray(ends, dtype=np.int_)
+
 
 	@property
-	def label_ranges(self):
+	def labels(self):
 		"""
-		Ranges(start,  end) for each label
+		Label values
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Iterate over first and last
+		# Extract end values
+		cdef np.ndarray labels = np.zeros(self.size, dtype=object)
 		cdef int i
-		cdef dict ranges = {}
-		for i in range(self.ail.nl):
-			ranges[self.rev_label_map[i]] = (self.ail.first[i], self.ail.last[i])
-		
-		return ranges
-		
+		cdef LabeledInterval interval
+		for i, interval in enumerate(self):
+			labels[i] = interval.label
+
+		return labels
+
+
+	cdef ailist_t *_get_ail(LabeledIntervalArray self, char *label_name):
+		# Get label
+		cdef int32_t t = get_label(self.laia, label_name)
+
+		# Check if label present
+		cdef ailist_t *ail
+		if (t != -1):
+			ail = ailist_copy(self.laia.labels[t].ail)
+		else:
+			ail = ailist_init()
+
+		return ail
+
+	def get_ail(self, label):
+		cdef bytes b_label = label.encode()
+		cdef AIList ail = AIList()
+		c_ail = self._get_ail(b_label)
+		ail.set_list(c_ail)
+
+		return ail
+
+
+	def set_ail(self, AIList ail, str label):
+		cdef bytes b_label = label.encode()
+		#cdef ailist_t *copied_ail = ailist_copy(ail.c_ailist)
+		labeled_aiarray_append_ail(self.laia, ail.c_ailist, b_label)
+
+		return
+
 
 	def __len__(self):
 		"""
 		Return size of labeled_interval_list
 		"""
-		
+
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		return self.size
 
-	
+
 	def __iter__(self):
 		"""
 		Iterate over LabeledIntervalArray object
 		"""
 
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("LabeledIntervalArray object has been closed.")
+		# Check if is constructed
+		if self.is_constructed is False:
+			self.construct()
+
+		# Iterate over labels in ail
+		cdef const char *label_name
+		cdef labeled_aiarray_iter_t *laia_iter
+		cdef labeled_interval_t *cintv
+		cdef LabeledInterval output_interval
+		cdef bytes label_bytes
+
+		# Create iterator
+		laia_iter = labeled_aiarray_iter_init(self.laia)
+		while labeled_aiarray_iter_next(laia_iter) != 0:
+			cintv = laia_iter.intv
+			# Create LabeledInterval wrapper
+			label_name = cintv.name
+			label_bytes = label_name
+			output_interval = LabeledInterval()
+			output_interval.set_i(cintv.i, label_bytes.decode())
+			yield output_interval
+
+		labeled_aiarray_iter_destroy(laia_iter)
 
-		# Iterate over interval list
-		cdef LabeledInterval interval
-		cdef labeled_interval_t *cinterval
-		cdef int i
-		for i in range(self.size):
-			interval = LabeledInterval()
-			cinterval = labeled_aiarray_get_id(self.ail, i)
-			interval.set_i(cinterval, self.rev_label_map[cinterval.label])
-			
-			yield interval
 
-	
 	def __hash__(self):
 		"""
 		Get hash value
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		return hash(self)
-		
-		
-	cdef labeled_aiarray_t *_array_index(LabeledIntervalArray self, const long[::1] ids):
+
+
+	cdef labeled_aiarray_t *_array_index(LabeledIntervalArray self,
+										 const long[::1] ids):
 		cdef int length = len(ids)
 		cdef labeled_aiarray_t *cindexed_aiarray
 
-		cindexed_aiarray = labeled_aiarray_slice_index(self.ail, &ids[0], length)
+		cindexed_aiarray = labeled_aiarray_slice_index(self.laia, &ids[0], length)
 
 		if cindexed_aiarray == NULL:
 			cindexed_aiarray = labeled_aiarray_init()
-		
+
 		return cindexed_aiarray
 
 	def __getitem__(self, key):
 		"""
 		Index LabeledIntervals by value
 		"""
 
@@ -366,76 +470,73 @@
 			raise IndexError("Incorrect number of dimensions given.")
 
 		# Check if key is iterable
 		cdef LabeledIntervalArray indexed_aiarray
 		cdef labeled_aiarray_t *cindexed_aiarray
 		cdef LabeledInterval output_interval
 		cdef labeled_interval_t *coutput_interval
-		cdef int k
-		cdef labeled_interval_t i
-		cdef labeled_interval_t *id_i
-		cdef labeled_aiarray_t *label_i
 		cdef int slice_start
 		cdef int slice_end
 		cdef int slice_step
-		cdef int label_code
-		cdef int j
-		cdef const char *label_name
+		cdef bytes label_name
 		cdef uint8[::1] bool_index
-		
+
 		try:
-			iter(key) # Test is present
+			# Test is present
+			iter(key)
 			# Iterate over key
 			indexed_aiarray = LabeledIntervalArray()
 
 			# Check if keys are booleans
 			if isinstance(key[0], np.bool_):
 				# Check array is the same size
 				if len(key) != self.size:
 					raise IndexError("Index and LabeledIntervalArray of different sizes.")
 
 				bool_index = key
-				cindexed_aiarray = labeled_aiarray_slice_bool(self.ail, &bool_index[0])
+				cindexed_aiarray = labeled_aiarray_slice_bool(self.laia, &bool_index[0])
 
 			# Must be integers
 			else:
 				cindexed_aiarray = self._array_index(key)
 
 			# Wrap
 			indexed_aiarray.set_list(cindexed_aiarray)
-			
+
 			return indexed_aiarray
-		
+
 		# key is not iterable, treat as int
 		except TypeError:
 			# Check if key is slice
 			if isinstance(key, slice):
 				# Determine indices
 				slice_start, slice_end, slice_step = key.indices(self.size)
 				# Iterate over key
 				indexed_aiarray = LabeledIntervalArray()
-				cindexed_aiarray = labeled_aiarray_slice_range(self.ail, slice_start, slice_end, slice_step)
+				cindexed_aiarray = labeled_aiarray_slice_range(self.laia, slice_start,
+																slice_end, slice_step)
 				# Wrap
 				indexed_aiarray.set_list(cindexed_aiarray)
-					
+
 				return indexed_aiarray
 
 			# Check if key is greater than length
-			if key >= self.ail.nr:
+			if key >= self.laia.total_nr:
 				raise IndexError("Value larger than LabeledIntervalArray length")
 
 			# Check if negative
 			if key < 0:
-				key = self.ail.nr + key
+				key = self.laia.total_nr - key
 
 			# Create LabeledInterval wrapper
 			output_interval = LabeledInterval()
-			coutput_interval = labeled_aiarray_get_id(self.ail, key)
-			output_interval.set_i(coutput_interval, self.rev_label_map[coutput_interval.label])
-		
+			coutput_interval = labeled_aiarray_get_index(self.laia, key)
+			label_name = coutput_interval.name
+			output_interval.set_i(coutput_interval.i, label_name.decode())
+
 		return output_interval
 
 
 	def __repr__(self):
 		"""
 		Representation of LabeledIntervalArray object
 		"""
@@ -444,226 +545,328 @@
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Initialize string
 		repr_string = "LabeledIntervalArray\n"
 
 		# Iterate over labeled_interval_list
-		if self.ail.nr > 10:
+		if self.laia.total_nr > 10:
 			for i in range(5):
 				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].label)
 			repr_string += "   ...\n"
 			for i in range(-5, 0, 1):
 				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].label)
 		else:
-			for i in range(self.ail.nr):
+			for i in range(self.laia.total_nr):
 				repr_string += "   (%d-%d, %s)\n" % (self[i].start, self[i].end, self[i].label)
 
 		return repr_string
 
-
-	cdef void set_list(LabeledIntervalArray self, labeled_aiarray_t *input_list):
+	
+	def __getstate__(self):
+		"""
+		Get state of LabeledIntervalArray object
 		"""
-		Set wrapper of C aiarray
 
-		Parameters
-		----------
-			input_list : labeled_aiarray_t*
-				labeled_aiarray_t to replace existing one
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		Returns
-		-------
-			None
+		# Get state
+		state = self.to_dict()
+
+		return state
+
+
+	def __setstate__(self, state):
+		"""
 		"""
 
-		# Free old labeled_aiarray
-		#if self.ail:
-			#labeled_aiarray_destroy(self.ail)
-		labeled_aiarray_destroy(self.ail)
-		
-		# Replace new lebeled_aiarray
-		self.ail = input_list
-		self.is_closed = False
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
+		# Set state
+		self.from_dict(state)
 
-	cdef labeled_aiarray_t *get_labels(LabeledIntervalArray self, const char[:,::1] labels, int length):
-		#cdef const char[::1] *label_names = label_array
-		cdef const char *first_char = &labels[0,0]
-		cdef labeled_aiarray_t *cintervals = get_label_array(self.ail, &first_char, length)
+		return None
 
-		return cintervals
 
-	def get(self, label):
+	def __sub__(self, LabeledIntervalArray query_laia):
 		"""
-		Get LabeledIntervalArray for given label
-		
-		Parameters
-		----------
-			label : str
-				Label to get
-				
-		Returns
-		-------
-			intervals : LabeledIntervalArray
-				Intervals with given label
+		Subtract values
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
-		
-		# Find intervals with label
-		cdef LabeledIntervalArray intervals = LabeledIntervalArray()
-		cdef labeled_aiarray_t *cintervals
-		cdef np.ndarray label_array
-		if isinstance(label, str) or isinstance(label, int):
-			cintervals = get_label(self.ail, label.encode())
-		else:
-			try:
-				iter(label)
-				label_array = np.array([l for l in label]).astype(str)
-				cintervals = self.get_labels(label_array, label_array.size)
-			except TypeError:
-				raise TypeError(" Could not determine label type.")
-		
-		# Wrap intervals
-		intervals.set_list(cintervals)
 
-		return intervals
+		return self.subtract(query_laia)
 
+	
+	def __add__(self, LabeledIntervalArray query_laia):
+		"""
+		Common values
+		"""
 
-	cdef overlap_label_index_t *get_labels_with_index(LabeledIntervalArray self, const char *label_names, int str_label_len, int length):
-		#cdef const char[::1] *label_names = label_array
-		cdef overlap_label_index_t *cintervals = get_label_array_with_index(self.ail, &label_names[0], length, str_label_len)
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		return cintervals
+		return self.common(query_laia)
 
-	def get_with_index(self, label):
+
+	def __or__(self, LabeledIntervalArray query_laia):
 		"""
+		Common values
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
-		
-		# Find intervals with label
-		cdef LabeledIntervalArray intervals = LabeledIntervalArray()
-		#cdef labeled_aiarray_t *cintervals
-		cdef overlap_label_index_t *cintervals_index
-		cdef int n_labels
-		cdef np.ndarray labels
-		cdef np.ndarray byte_labels
-		if isinstance(label, str) or isinstance(label, int):
-			cintervals_index = get_label_with_index(self.ail, label.encode())
-		else:
-			try:
-				iter(label)
-				# Add array intervals
-				labels = np.array(label)
-				n_labels = len(labels)
-				byte_labels = labels.astype(bytes)
-				
-				cintervals_index = self.get_labels_with_index(np.PyArray_BYTES(byte_labels), byte_labels.itemsize, n_labels)
-			except TypeError:
-				raise TypeError(" Could not determine label type.")
-		
-		# Wrap intervals
-		intervals.set_list(cintervals_index.ail)
 
-		# Create numpy array from C pointer
-		cdef np.ndarray indices = pointer_to_numpy_array(cintervals_index.indices, cintervals_index.size)
+		return self.append(query_laia)
 
-		return intervals, indices
 
-	
+	cdef void set_list(LabeledIntervalArray self, labeled_aiarray_t *input_list):
+		"""
+		Set wrapper of C aiarray
+
+		Parameters
+		----------
+			input_list : labeled_aiarray_t*
+				labeled_aiarray_t to replace existing one
+
+		Returns
+		-------
+			None
+		"""
+
+		labeled_aiarray_destroy(self.laia)
+
+		# Replace new lebeled_aiarray
+		self.laia = input_list
+		self.is_closed = False
+
+	#===========================================
+	#             FUNCTION: get
+	#===========================================
+
+	#-------------------------------------------
+	#              get: CYTHON
+	#-------------------------------------------
+
+	cdef labeled_aiarray_t *get_labels(LabeledIntervalArray self, const char *label_names,
+										int str_label_len, int length):
+		cdef labeled_aiarray_t *cintervals = labeled_aiarray_get_label_array(self.laia,
+																			&label_names[0],
+																			length, str_label_len)
+
+		return cintervals
+
+	cdef overlap_label_index_t *get_labels_with_index(LabeledIntervalArray self,
+														const char *label_names,
+														int str_label_len, int length):
+		cdef overlap_label_index_t *cintervals = labeled_aiarray_get_label_array_with_index(self.laia,
+																							&label_names[0],
+																							length,
+																							str_label_len)
+
+		return cintervals
+
 	cdef np.ndarray _get_index(LabeledIntervalArray self, str label):
 		"""
 		"""
 
 		# Check if any with label
 		try:
 			if self.label_counts[label] == 0:
 				return np.array([], dtype=np.double)
 		except KeyError:
 			return np.array([], dtype=np.double)
-		
+
 		# Find intervals with label
 		cdef long[::] index = np.zeros(self.label_counts[label], dtype=np.int_)
-		cdef int start_i
-		cdef int end_i
-		
+
 		# Determine where labels are
-		start_i = self.label_index[self.label_map[label]]
-		if self.label_map[label] + 1 == self.ail.nl:
-			end_i = self.ail.nr
-		else:
-			end_i = self.label_index[self.label_map[label] + 1] 
-		
-		# Iterate over intervals
-		cdef labeled_interval_t found_interval
+		cdef bytes label_name = label.encode()
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef label_t *p = &self.laia.labels[t]
 		cdef int i
-		cdef int index_i = 0
-		for i in range(start_i, end_i):
-			found_interval = self.ail.interval_list[i]
-			index[index_i] = found_interval.id_value
-			index_i += 1
+		for i in range(p.ail.nr):
+			index[i] = p.ail.interval_list[i].id_value
 
 		return np.asarray(index)
 
-	
+
 	cdef np.ndarray _get_index_multi(LabeledIntervalArray self, np.ndarray labels):
 		"""
 		"""
-		
+
 		# Find intervals with label
-		cdef n = 0
-		cdef int label
-		for label in range(len(labels)):
-			n += self.label_counts[labels[label]]
+		cdef int n = 0
+		#cdef str label
+		for label in labels:
+			n += self.label_counts[label]
+
 		cdef long[::] index = np.zeros(n, dtype=np.int_)
-		cdef int start_i
-		cdef int end_i
 		cdef int i
-		cdef int index_i = 0
-		cdef labeled_interval_t found_interval
-		
-		for label in range(len(labels)):
+		cdef int j = 0
+		cdef bytes label_name
+		cdef uint32_t t
+		cdef label_t *p
+
+		# Iterate over labels
+		for label in labels:
 			# Determine where labels are
-			start_i = self.label_index[self.label_map[labels[label]]]
-			if self.label_map[labels[label]] + 1 == self.ail.nl:
-				end_i = self.ail.nr
-			else:
-				end_i = self.label_index[self.label_map[labels[label]] + 1] 
-			
+			label_name = label.encode()
+			t = get_label(self.laia, label_name)
+			p = &self.laia.labels[t]
+
 			# Iterate over intervals
-			for i in range(start_i, end_i):
-				found_interval = self.ail.interval_list[i]
-				index[index_i] = found_interval.id_value
-				index_i += 1
+			for i in range(p.ail.nr):
+				index[j] = p.ail.interval_list[i].id_value
+				j += 1
 
 		return np.asarray(index)
 
-	def get_index(self, label):
+	#-------------------------------------------
+	#              get: PYTHON
+	#-------------------------------------------
+
+	def get(self,
+			label,
+			return_intervals = True,
+			return_index = False):
 		"""
+		Get :class:`~aiarray.LabeledIntervalArray` for given label
+
+		Parameters
+		----------
+			label : str
+				Label to get
+			return_intervals : bool
+				Flag to return intervals
+			return_index : bool
+				Flag to return index array
+
+		Returns
+		-------
+			intervals : LabeledIntervalArray
+				Intervals with given label
+			indices : numpy.ndarray
+				Array of indices
+
+		See Also
+		--------
+		LabeledIntervalArray.from_array: Add intervals from arrays
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
+		LabeledIntervalArray.intersect: Find intervals overlapping given range
+
+		Examples
+		--------
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(1, 2, 'a')
+		>>> ail.add(3, 4, 'a')
+		>>> ail.add(3, 6, 'a')
+		>>> ail.add(3, 6, 'b')
+		>>> ail.get("b")
+		LabeledIntervalArray
+   			(3-6, b)
+		>>> ail.get(["b","a"])
+		LabeledIntervalArray
+			(3-6, b)
+			(1-2, a)
+			(3-4, a)
+			(3-6, a)
+		>>> ail.get(["b","a"], return_index=True)
+		(LabeledIntervalArray
+			(3-6, b)
+			(1-2, a)
+			(3-4, a)
+			(3-6, a),
+		array([3, 0, 1, 2]))
+		>>> ail.get(["b","a"], return_index=True, return_intervals=False)
+		array([3, 0, 1, 2])
+
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Make sure it is constructed
-		if self.is_constructed == False:
-			self.construct()
-
+		# Find intervals with label
+		cdef LabeledIntervalArray intervals = LabeledIntervalArray()
+		cdef labeled_aiarray_t *cintervals
+		cdef overlap_label_index_t *cintervals_index
+		cdef int n_labels
+		cdef np.ndarray labels
+		cdef np.ndarray byte_labels
+		cdef np.ndarray indices
+		cdef bytes label_name
 		if isinstance(label, str):
-			index = self._get_index(str(label))
+			label_name = label.encode()
+			if return_intervals:
+				if return_index:
+					cintervals_index = labeled_aiarray_get_label_with_index(self.laia, label_name)
+					# Wrap intervals
+					intervals.set_list(cintervals_index.laia)
+
+					# Create numpy array from C pointer
+					indices = pointer_to_numpy_array(cintervals_index.indices, cintervals_index.size)
+
+					return intervals, indices
+
+				cintervals = labeled_aiarray_get_label(self.laia, label_name)
+				# Wrap intervals
+				intervals.set_list(cintervals)
+
+				return intervals
+
+			elif return_index:
+				indices = self._get_index(str(label))
+
+				return indices
+
 		else:
-			index = self._get_index_multi(label)
+			try:
+				iter(label)
+				#label_array = np.array([l for l in label]).astype(str)
+				# Add array intervals
+				labels = np.array(label)
+				n_labels = len(labels)
+				byte_labels = labels.astype(bytes)
 
-		return index
+				if return_intervals:
+					if return_index:
+						cintervals_index = self.get_labels_with_index(np.PyArray_BYTES(byte_labels),
+																		byte_labels.itemsize, n_labels)
+						# Wrap intervals
+						intervals.set_list(cintervals_index.laia)
+
+						# Create numpy array from C pointer
+						indices = pointer_to_numpy_array(cintervals_index.indices, cintervals_index.size)
+
+						return intervals, indices
+
+					cintervals = self.get_labels(np.PyArray_BYTES(byte_labels), byte_labels.itemsize,
+												 n_labels)
+					# Wrap intervals
+					intervals.set_list(cintervals)
+
+					return intervals
+
+				elif return_index:
+					indices = self._get_index_multi(labels)
+
+					return indices
+
+			except TypeError:
+				raise TypeError(" Could not determine label type.")
 
 
 	def freeze(self):
 		"""
 		Make :class:`~aiarray.LabeledIntervalArray` immutable
 
 		Parameters
@@ -674,15 +877,15 @@
 		-------
 			None
 
 		See Also
 		--------
 		LabeledIntervalArray.unfreeze: Make mutable
 		LabeledIntervalArray.sort: Sort intervals inplace
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 
 		Examples
 		--------
 		>>> from aiarray import LabeledIntervalArray
 		>>> ail = LabeledIntervalArray()
 		>>> ail.add(1, 2, 'a')
 		>>> ail.add(3, 4, 'a')
@@ -700,15 +903,15 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Make sure it is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Change to frozen
 		self.is_frozen = True
 
 
 	def unfreeze(self):
@@ -723,15 +926,15 @@
 		-------
 			None
 
 		See Also
 		--------
 		LabeledIntervalArray.freeze: Make immutable
 		LabeledIntervalArray.sort: Sort intervals inplace
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 
 		Examples
 		--------
 		>>> from aiarray import LabeledIntervalArray
 		>>> ail = LabeledIntervalArray()
 		>>> ail.add(1, 2, 'a')
 		>>> ail.add(3, 4, 'a')
@@ -755,20 +958,29 @@
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Change to not frozen
 		self.is_frozen = False
 
 
 	cdef void _insert(LabeledIntervalArray self, int start, int end, const char *label_name):
-		labeled_aiarray_add(self.ail, start, end, label_name)
+		labeled_aiarray_add(self.laia, start, end, label_name)
+
+	cdef void _from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends,
+							const char *label_names, int array_length, int label_str_len):
+
+		# Run C function
+		labeled_aiarray_from_array(self.laia, &starts[0], &ends[0], &label_names[0],
+									array_length, label_str_len)
 
-	def add(self, int start, int end, str label):
+		return
+
+	def add(self, start, end, label):
 		"""
 		Add an interval to LabeledIntervalArray inplace
-		
+
 		Parameters
 		----------
 			start : int
 				Start position of interval
 			end : int
 				End position of interval
 			label : str
@@ -777,145 +989,101 @@
 		Returns
 		-------
 			None
 
 		See Also
 		--------
 		LabeledIntervalArray.from_array: Add intervals from arrays
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 		LabeledIntervalArray.intersect: Find intervals overlapping given range
 
 		Examples
 		--------
-		>>> from aiarray import LabeledIntervalArray
+		>>> from ailist import LabeledIntervalArray
 		>>> ail = LabeledIntervalArray()
 		>>> ail.add(1, 2, 'a')
 		>>> ail.add(3, 4, 'a')
 		>>> ail.add(3, 6, 'a')
 		>>> ail
-		aiarray
-		  range: (1-6)
+		LabeledIntervalArray
 		   (1-2, 'a')
 		   (3-4, 'a')
 		   (3-6, 'a')
 
 		"""
-		
+
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Check that object is not frozen
 		if self.is_frozen:
-			raise TypeError("LabeledIntervalArray is frozen and currently immutatable. Try '.unfreeze()' to reverse.")
-
-		# Insert interval
-		self._insert(start, end, label.encode())
-		self.is_constructed = False
-
+			raise TypeError("LabeledIntervalArray is frozen and currently immutatable. "
+							"Try '.unfreeze()' to reverse.")
 
-	cdef void _from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *label_names, int array_length, int label_str_len):
-		#cdef const char *label_name
-		labeled_aiarray_from_array(self.ail, &starts[0], &ends[0], &label_names[0], array_length, label_str_len)
-		#cdef int i
-		#for i in range(array_length):
-			#label_name = &label_names[i,:][0]
-			#labeled_aiarray_add(self.ail, starts[i], ends[i], label_name)
-		return
-	
-	def from_array(self, const long[::1] starts, const long[::1] ends, np.ndarray labels):
-		"""
-		Add intervals from arrays to LabeledIntervalArray inplace
-		
-		Parameters
-		----------
-			starts : numpy.ndarray {long}
-				Start positions of intervals
-			ends : numpy.ndarray {long}
-				End positions of intervals
-			labels : numpy.ndarray {object/str}
-				ID of intervals
+		# Static type variables
+		cdef int array_length
+		cdef np.ndarray byte_labels
 
-		Returns
-		-------
-			None
+		if isinstance(start, int):
+			# Check interval
+			if start > end:
+				raise IndexError("Start is larger than end.")
+
+			# Insert interval
+			self._insert(start, end, label.encode())
+
+		elif isinstance(start, np.ndarray):
+			# Add array intervals
+			array_length = len(start)
+			if array_length == 0:
+				return
+			byte_labels = label.astype(bytes)
+
+			self._from_array(start, end, np.PyArray_BYTES(byte_labels), array_length,
+								byte_labels.itemsize)
+
+		elif isinstance(start, np.integer):
+			# Check interval
+			if start > end:
+				raise IndexError("Start is larger than end.")
 
-		See Also
-		--------
-		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
-		LabeledIntervalArray.intersect: Find intervals overlapping given range
+			# Insert interval
+			self._insert(int(start), int(end), label.encode())
 
-		Examples
-		--------
-		>>> from aiarray import LabeledIntervalArray
-		>>> import numpy as np
-		>>> starts = np.arange(100)
-		>>> ends = starts + 10
-		>>> labeld = np.repeat('a', len(starts))
-		>>> ail = LabeledIntervalArray()
-		>>> ail.from_array(starts, ends, labels)
-		>>> ail
-		LabeledIntervalArray
-		  range: (0-109)
-		   (0-10, 'a')
-		   (1-11, 'a')
-		   (2-12, 'a')
-		   (3-13, 'a')
-		   (4-14, 'a')
-		   ...
-		   (95-105, 'a')
-		   (96-106, 'a')
-		   (97-107, 'a')
-		   (98-108, 'a')
+		else:
+			raise TypeError("Start must be int or np.ndarray.")
 
-		"""
+		return
 
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check that object is not frozen
-		if self.is_frozen:
-			raise TypeError("LabeledIntervalArray is frozen and currently immutatable. Try '.unfreeze()' to reverse.")
+	cdef void _append(LabeledIntervalArray self, LabeledIntervalArray other_laia):
 
-		# Add array intervals
-		cdef int array_length = len(starts)
-		cdef np.ndarray byte_labels = labels.astype(bytes)
-		
-		self._from_array(starts, ends, np.PyArray_BYTES(byte_labels), array_length, byte_labels.itemsize)
-		self.is_constructed = False
+		# Run C function
+		labeled_aiarray_append(self.laia, other_laia.laia)
 
-	
-	cdef void _append(LabeledIntervalArray self, LabeledIntervalArray other_ail):
-		#cdef const char *label_name
-		labeled_aiarray_append(self.ail, other_ail.ail)
-		#cdef int i
-		#for i in range(array_length):
-			#label_name = &label_names[i,:][0]
-			#labeled_aiarray_add(self.ail, starts[i], ends[i], label_name)
 		return
-	
+
 	def append(self, LabeledIntervalArray other_ail):
 		"""
 		Add intervals from arrays to LabeledIntervalArray inplace
-		
+
 		Parameters
 		----------
 			other_ail : LabeledIntervalArray
 				Intervals to add to current LabeledIntervalArray
 
 		Returns
 		-------
 			None
 
 		See Also
 		--------
 		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 		LabeledIntervalArray.intersect: Find intervals overlapping given range
 
 		Examples
 		--------
 		>>> from ailist import LabeledIntervalArray
 		>>> import numpy as np
 		>>> starts = np.arange(100)
@@ -932,15 +1100,15 @@
 			(4-14, a)
 			...
 			(95-105, a)
 			(96-106, a)
 			(97-107, a)
 			(98-108, a)
 			(99-109, a)
-		
+
 		>>> len(ail)
 		100
 
 		>>> ail2 = LabeledIntervalArray()
 		>>> ail2.from_array(starts, ends, labels)
 		>>> ail.append(ail2)
 		>>> ail
@@ -952,54 +1120,50 @@
 			(4-14, a)
 			...
 			(95-105, a)
 			(96-106, a)
 			(97-107, a)
 			(98-108, a)
 			(99-109, a)
-		
+
 		>>> len(ail)
 		200
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Check that object is not frozen
 		if self.is_frozen:
-			raise TypeError("LabeledIntervalArray is frozen and currently immutatable. Try '.unfreeze()' to reverse.")
-		
+			raise TypeError("LabeledIntervalArray is frozen and currently immutatable. "
+							"Try '.unfreeze()' to reverse.")
+
 		self._append(other_ail)
-		self.is_constructed = False
 
 
 	cdef void _construct(LabeledIntervalArray self, int min_length):
 		# Contruct
-		labeled_aiarray_radix_label_sort(self.ail)
-		labeled_aiarray_sort(self.ail)
-		labeled_aiarray_construct(self.ail, min_length)
-		labeled_aiarray_cache_id(self.ail)
+		labeled_aiarray_construct(self.laia, min_length)
+		labeled_aiarray_cache_id(self.laia)
 
 	def construct(self, int min_length=20):
 		"""
 		Construct labeled_aiarray_t *Required to call intersect
 
 		Parameters
 		----------
 			min_length : int
 				Minimum length
 
 		Returns
 		-------
 			None
 
-		.. warning::
-			This will re-sort intervals inplace if ail.track_index = False
 
 		See Also
 		--------
 		LabeledIntervalArray.sort: Sort intervals inplace
 		LabeledIntervalArray.intersect: Find intervals overlapping given range
 
 		Examples
@@ -1026,386 +1190,431 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("Labledaiarray object has been closed.")
 
 		# Check if already constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self._construct(min_length)
-			self.is_constructed = True
 		else:
 			pass
 
 
-	cdef int _get_label_index(LabeledIntervalArray self, int label):
-		"""
-		"""
-
-		cdef int count = 0
-		cdef int i
-		for i in range(label):
-			count += self.ail.label_count[i]
-
-		return count
-
-	cdef np.ndarray _get_label_comp_bounds(LabeledIntervalArray self, int label):
-		"""
-		Get component index for label
-		"""
-
-		# Initialize label specific variables
-		cdef int label_start = self._get_label_index(label)
-		cdef int *idxC = &self.ail.idxC[label * 10]
-		cdef int n_comps = self.ail.nc[label]
-		cdef np.ndarray comps_bounds = np.zeros(n_comps + 1, dtype=int)
-
-		# Iterate over components
-		cdef int i
-		for i in range(n_comps):
-			comps_bounds[i] = label_start + idxC[i]
-		comps_bounds[n_comps] = self._get_label_index(label + 1)
-
-		return comps_bounds
-
-	cdef np.ndarray _get_label_comp_length(LabeledIntervalArray self, int label):
-		"""
-		Get component lengths for label
-		"""
-
-		# Initialize label specifc variables
-		cdef int *lenC = &self.ail.idxC[label * 10]
-		cdef int n_comps = self.ail.nc[label]
-		cdef np.ndarray comps_length = np.zeros(n_comps, dtype=int)
-
-		# Iterate over components
-		cdef int i
-		for i in range(n_comps):
-			comps_length[i] = lenC[i]
-
-		return comps_length
-
 	def iter_sorted(self):
 		"""
 		Iterate over an LabeledIntervalArray in sorted way
-		
+
 		Parameters
 		----------
 			None
-		
+
 		Returns
 		-------
 			sorted_iter : Generator
 				Generator of LabeledIntervals
+
+		See Also
+		--------
+		LabeledIntervalArray.sort: Sort intervals inplace
+		LabeledIntervalArray.intersect: Find intervals overlapping given range
+
+		Examples
+		--------
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(1, 2, 'a')
+		>>> ail.add(3, 4, 'a')
+		>>> ail.add(2, 6, 'a')
+		>>> ail
+		LabledIntervalArray
+		   (1-2, 'a')
+		   (3-4, 'a')
+		   (2-6, 'a')
+		>>> s_iter = ail.iter_sorted()
+		>>> for i in s_iter:
+		>>>		print(i)
+		Interval(1-2, a)
+		Interval(2-6, a)
+		Interval(3-4, a)
+
 		"""
 
 		# Check if is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Iterate over labels in ail
 		cdef const char *label_name
-		cdef label_sorted_iter_t *ail_iter
-		cdef labeled_interval_t *cintv
+		cdef label_sorted_iter_t *laia_iter
+		cdef interval_t *cintv
 		cdef LabeledInterval output_interval
 		cdef bytes label_bytes
-		cdef int label
-		for label in range(self.ail.nl):
-			label_name = query_rev_label_map(self.ail, label)
+
+		for i in range(self.laia.n_labels):
 			# Create sorted iterators
-			ail_iter = iter_init(self.ail, label_name)
-			while iter_next(ail_iter) != 0:
-				cintv = ail_iter.intv
+			label_name = self.laia.labels[i].name
+			laia_iter = label_sorted_iter_init(self.laia, label_name)
+			while label_sorted_iter_next(laia_iter) != 0:
+				cintv = laia_iter.intv
 				# Create LabeledInterval wrapper
 				label_bytes = label_name
 				output_interval = LabeledInterval()
 				output_interval.set_i(cintv, label_bytes.decode())
 				yield output_interval
 
-			iter_destroy(ail_iter)
-
-
-	cdef labeled_aiarray_t *_intersect(LabeledIntervalArray self, int start, int end, const char *label_name):
-		cdef labeled_aiarray_t *overlaps = labeled_aiarray_query_single(self.ail, start, end, label_name)
+			label_sorted_iter_destroy(laia_iter)
 
-		return overlaps
 
-	def intersect(self, int start, int end, str label):
+	def from_dict(self, 
+				  dict interval_dict):
 		"""
-		Find intervals overlapping given range
-		
+		Construct LabeledIntervalArray from dictionary
+
 		Parameters
 		----------
-			start : int
-				Start position of query range
-			end : int
-				End position of query range
-			label : str
-				Label of quert range
+			interval_dict : dict
+				Dictionary of intervals
 
 		Returns
 		-------
-			overlaps : LabeledIntervalArray
-				Overlapping intervals
-
-		.. warning::
-			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run. This will re-sort intervals inplace is ail.track_index = False.
+			None
 
 		See Also
 		--------
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
-		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
-		LabeledIntervalArray.intersect_index: Find interval indices overlapping given range
-		LabeledIntervalArray.intersect_from_array: Find interval indices overlapping given ranges
+		LabeledIntervalArray.sort: Sort intervals inplace
+		LabeledIntervalArray.intersect: Find intervals overlapping given range
 
 		Examples
 		--------
-		>>> from aiarray import LabeledIntervalArray
+		>>> from ailist import LabeledIntervalArray
 		>>> ail = LabeledIntervalArray()
-		>>> ail.add(1, 2, 'a')
-		>>> ail.add(3, 4, 'a')
-		>>> ail.add(2, 6, 'a')
+		>>> ail.from_dict({'a': [(1, 2), (3, 4), (2, 6)]})
 		>>> ail
-		aiarray
-		  range: (1-6)
-		   (1-2, 'a')
-		   (3-4, 'a')
-		   (2-6, 'a')
-		>>> q = ail.intersect(2, 10, 'a')
-		>>> q
-		aiarray
-		  range: (2-6)
-		   (2-6, 'a')
-		   (3-4, 'a')
+		LabeledIntervalArray
+		   (1-2, a)
+		   (3-4, a)
+		   (2-6, a)
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check if is constructed
-		if self.is_constructed == False:
+		# Check if already constructed
+		if self.is_constructed is False:
 			self.construct()
+		else:
+			pass
 
-		# Check if label is present
-		try:
-			self.label_map[label]
-		except KeyError:
-			raise KeyError("Label given is not in LabeledIntervalArray.")
+		# Iterate over labels in dict
+		for label_name in interval_dict:
+			self.set_ail(interval_dict[label_name], str(label_name))
 
-		# Intersect
-		cdef labeled_aiarray_t *i_list = self._intersect(start, end, label.encode())
-		cdef LabeledIntervalArray overlaps = LabeledIntervalArray()
-		overlaps.set_list(i_list)
+		return None
 
-		return overlaps
 
-	
-	def has_hit(self, int start, int end, str label):
+	def to_dict(self):
 		"""
-		Find interval indices overlapping given ranges
-		
+		Convert LabeledIntervalArray to dictionary
+
 		Parameters
 		----------
-			starts : numpy.ndarray {long}
-				Start positions of intervals
-			ends : numpy.ndarray {long}
-				End positions of intervals
-			labels : numpy.ndarray {str}
-				Labels of intervals
+			None
 
 		Returns
 		-------
-			ref_index : np.ndarray {int}
-				Overlapping interval indices from LabeledIntervalArray
-			query_index : np.ndarray {int}
-				Overlapping interval indices from query LabeledIntervalArray
-
-		.. warning::
-			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run. This will re-sort intervals inplace if ail.track_index = False.
+			interval_dict : dict
+				Dictionary of intervals
 
 		See Also
 		--------
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
-		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
+		LabeledIntervalArray.sort: Sort intervals inplace
 		LabeledIntervalArray.intersect: Find intervals overlapping given range
-		LabeledIntervalArray.intersect_index: Find interval indices overlapping given range
 
 		Examples
 		--------
-		>>> from aiarray import LabeledIntervalArray
-		>>> ail1 = LabeledIntervalArray()
-		>>> ail1.add(1, 2, 'a')
-		>>> ail1.add(3, 4, 'a')
-		>>> ail1.add(2, 6, 'a')
-		>>> ail1
-		LabeledIntervalArray
-		  range: (1-6)
-		   (1-2, 'a')
-		   (3-4, 'a')
-		   (2-6, 'a')
-		>>> ail2 = LabeledIntervalArray()
-		>>> ail2.add(1, 2, 'a')
-		>>> ail2.add(3, 6, 'a')
-		>>> ail2
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(1, 2, 'a')
+		>>> ail.add(3, 4, 'a')
+		>>> ail.add(2, 6, 'a')
+		>>> ail
 		LabeledIntervalArray
-		  range: (1-6)
-		    (1-2, 'a')
-		    (3-6, 'a')
-		>>> q = ail1.intersect_from_array(ail2)
-		>>> q
-		(array([2, 1]), array([]))
+		   (1-2, a)
+		   (3-4, a)
+		   (2-6, a)
+		>>> ail.to_dict()
+		{'a': [(1, 2), (2, 6), (3, 4)]}
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check if object is constructed
-		if self.is_constructed == False:
-			self.construct()
+		# Get ail
+		interval_dict = {}
+		for label in self.unique_labels:
+			interval_dict[label] = self.get_ail(label)
 
-		# Check that labels are bytes
-		cdef bytes byte_label = str(label).encode()
+		return interval_dict
 
-		cdef np.ndarray has_hit = np.zeros(self.size, dtype=bool)
-		cdef uint8[::1] has_hit_mem = has_hit
 
-		# Intersect
-		labeled_aiarray_query_has_hit(self.ail, &has_hit_mem[0], start, end, byte_label)
-		
-		return has_hit
+	def iter_intersect(self,
+					   LabeledIntervalArray query_laia,
+					   return_intervals = True,
+					   return_index = False):
+		"""
+		"""
+
+		# Check if is constructed
+		if self.is_constructed is False:
+			self.construct()
 
+		cdef LabeledIntervalArray overlaps
+		cdef LabeledInterval i
+		for i in query_laia:
+			if return_intervals:
+				if return_index:
+					overlaps, index = self.intersect(i.start, i.end, i.label,
+													return_intervals=True, return_index=True)
+					yield overlaps, index
+				else:
+					overlaps = self.intersect(i.start, i.end, i.label,
+											return_intervals=True, return_index=False)
+					yield overlaps
+
+			elif return_index:
+				index = self.intersect(i.start, i.end, i.label,
+										return_intervals=False, return_index=True)
+				yield index
+
+
+	cdef labeled_aiarray_t *_intersect(LabeledIntervalArray self, int start, int end,
+										const char *label_name):
+		# Call C function
+		cdef labeled_aiarray_t *overlaps = labeled_aiarray_init()
+		labeled_aiarray_query(self.laia, overlaps, label_name, start, end)
 
-	@cython.boundscheck(False)
-	@cython.wraparound(False)
-	@cython.initializedcheck(False)
-	cpdef _intersect_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char *labels, int label_str_len):
+		return overlaps
+
+	cdef labeled_aiarray_t *_intersect_from_array(LabeledIntervalArray self, const long[::1] starts,
+													const long[::1] ends, const char *labels, int label_str_len):
 		cdef int length = len(starts)
-		cdef array_query_t *total_overlaps
-		#cdef const char *first_char = &labels[0,0]
-		#cdef const char *first_char = np.PyArray_BYTES(labels)
-		total_overlaps = labeled_aiarray_query_from_array(self.ail, &starts[0], &ends[0], &labels[0], length, label_str_len)
+		cdef labeled_aiarray_t *overlaps = labeled_aiarray_init()
+		labeled_aiarray_query_from_array(self.laia, overlaps, &labels[0], &starts[0], &ends[0],
+										length, label_str_len)
+
+		return overlaps
 
-		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index, total_overlaps.size)
-		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index, total_overlaps.size)
+	cpdef _intersect_from_array_only_index(LabeledIntervalArray self, const long[::1] starts,
+											const long[::1] ends, const char *labels, int label_str_len):
+
+		cdef int length = len(starts)
+		cdef array_query_t *total_overlaps = labeled_aiarray_query_index_from_array(self.laia, &labels[0],
+																					&starts[0], &ends[0],
+																					length, label_str_len)
+
+		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index,
+															total_overlaps.size)
+		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index,
+															total_overlaps.size)
 
 		return ref_index, query_index
 
-	def intersect_from_array(self, const long[::1] starts, const long[::1] ends, np.ndarray labels):
+	cpdef _intersect_from_array_with_index(LabeledIntervalArray self, const long[::1] starts,
+											const long[::1] ends, const char *labels, int label_str_len):
+
+		cdef int length = len(starts)
+		cdef overlap_label_index_t *total_overlaps = overlap_label_index_init()
+		labeled_aiarray_query_with_index_from_array(self.laia, total_overlaps, &labels[0],
+													&starts[0], &ends[0], length, label_str_len)
+
+		# Create numpy array from C pointer
+		cdef np.ndarray indices = pointer_to_numpy_array(total_overlaps.indices, total_overlaps.size)
+		cdef LabeledIntervalArray overlaps = LabeledIntervalArray()
+		overlaps.set_list(total_overlaps.laia)
+
+		return overlaps, indices
+
+	cpdef _intersect_with_index(LabeledIntervalArray self, int start, int end, const char *label_name):
+		# Intersect with interval
+		cdef overlap_label_index_t *total_overlaps = overlap_label_index_init()
+		labeled_aiarray_query_with_index(self.laia, label_name, total_overlaps, start, end)
+
+		# Create numpy array from C pointer
+		cdef np.ndarray indices = pointer_to_numpy_array(total_overlaps.indices, total_overlaps.size)
+		cdef LabeledIntervalArray overlaps = LabeledIntervalArray()
+		overlaps.set_list(total_overlaps.laia)
+
+		return overlaps, indices
+
+	def intersect(self,
+				  start,
+				  end,
+				  label,
+				  return_intervals = True,
+				  return_index = False):
 		"""
-		Find interval indices overlapping given ranges
-		
+		Find intervals overlapping given range
+
 		Parameters
 		----------
-			starts : numpy.ndarray {long}
-				Start positions of intervals
-			ends : numpy.ndarray {long}
-				End positions of intervals
-			labels : numpy.ndarray {str}
-				Labels of intervals
+			start : int | np.ndarray
+				Start position of query range
+			end : int | np.ndarray
+				End position of query range
+			label : str | np.ndarray
+				Label of quert range
 
 		Returns
 		-------
-			ref_index : np.ndarray {int}
-				Overlapping interval indices from LabeledIntervalArray
-			query_index : np.ndarray {int}
-				Overlapping interval indices from query LabeledIntervalArray
+			overlaps : LabeledIntervalArray
+				Overlapping intervals
 
 		.. warning::
-			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run. This will re-sort intervals inplace if ail.track_index = False.
+			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run.
+			This will re-sort intervals inplace is ail.track_index = False.
 
 		See Also
 		--------
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
-		LabeledIntervalArray.intersect: Find intervals overlapping given range
 		LabeledIntervalArray.intersect_index: Find interval indices overlapping given range
+		LabeledIntervalArray.intersect_from_array: Find interval indices overlapping given ranges
 
 		Examples
 		--------
-		>>> from aiarray import LabeledIntervalArray
-		>>> ail1 = LabeledIntervalArray()
-		>>> ail1.add(1, 2, 'a')
-		>>> ail1.add(3, 4, 'a')
-		>>> ail1.add(2, 6, 'a')
-		>>> ail1
-		LabeledIntervalArray
-		  range: (1-6)
-		   (1-2, 'a')
-		   (3-4, 'a')
-		   (2-6, 'a')
-		>>> ail2 = LabeledIntervalArray()
-		>>> ail2.add(1, 2, 'a')
-		>>> ail2.add(3, 6, 'a')
-		>>> ail2
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(1, 2, 'a')
+		>>> ail.add(3, 4, 'a')
+		>>> ail.add(3, 6, 'a')
+		>>> ail.add(3, 6, 'b')
+		>>> ail
 		LabeledIntervalArray
-		  range: (1-6)
-		    (1-2, 'a')
-		    (3-6, 'a')
-		>>> q = ail1.intersect_from_array(ail2)
+		   (1-2, a)
+		   (3-4, a)
+		   (3-6, a)
+		   (3-6, b)
+		>>> q = ail.intersect(2, 10, 'a')
 		>>> q
-		(array([2, 1]), array([]))
+		LabeledIntervalArray
+		   (3-4, a)
+		   (3-6, a)
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check if object is constructed
-		if self.is_constructed == False:
+		# Check if is constructed
+		if self.is_constructed is False:
 			self.construct()
 
-		# Check that labels are bytes
-		byte_labels = labels.astype(bytes)
+		# Intersect
+		cdef np.ndarray indices
+		cdef labeled_aiarray_t *i_list
+		cdef LabeledIntervalArray overlaps
 
-		# Intersect from array
-		ref_index, query_index = self._intersect_from_array(starts, ends, np.PyArray_BYTES(byte_labels), byte_labels.itemsize)
-		
-		return ref_index, query_index
+		if isinstance(start, np.ndarray):
 
+			# Check that labels are bytes
+			if isinstance(label, str):
+				byte_labels = np.repeat(label, len(start), dtype=bytes)
+			else:
+				byte_labels = label.astype(bytes)
+
+			if return_intervals:
+				if return_index:
+					# Intersect from array
+					overlaps, indices = self._intersect_from_array_with_index(start, end,
+																			  np.PyArray_BYTES(byte_labels),
+																			  byte_labels.itemsize)
+					return overlaps, indices
+
+				else:
+					i_list = self._intersect_from_array(start, end,
+														np.PyArray_BYTES(byte_labels),
+														byte_labels.itemsize)
+					overlaps = LabeledIntervalArray()
+					overlaps.set_list(i_list)
+					return overlaps
+
+			elif return_index:
+				# Intersect from array
+				ref_index, query_index = self._intersect_from_array_only_index(start, end,
+																			   np.PyArray_BYTES(byte_labels),
+																			   byte_labels.itemsize)
+				return ref_index, query_index
+
+		if isinstance(start, int):
+
+			if return_intervals:
+				if return_index:
+					overlaps, indices = self._intersect_with_index(start, end, label.encode())
+					return overlaps, indices
+
+				else:
+					i_list = self._intersect(start, end, label.encode())
+					overlaps = LabeledIntervalArray()
+					overlaps.set_list(i_list)
+					return overlaps
+
+			elif return_index:
+				overlaps, indices = self._intersect_with_index(start, end, label.encode())
+				return indices
+
+
+	cdef void _has_hit_from_array(LabeledIntervalArray self,
+								  const long[::1] starts,
+								  const long[::1] ends,
+								  uint8[::1] has_hit,
+								  const char *labels,
+								  int label_str_len):
 
-	@cython.boundscheck(False)
-	@cython.wraparound(False)
-	@cython.initializedcheck(False)
-	cpdef _has_hit_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, uint8[::1] has_hit, const char *labels, int label_str_len):
+		# Call C function
 		cdef int length = len(starts)
-		labeled_aiarray_has_hit_from_array(self.ail, &starts[0], &ends[0], &labels[0], length, label_str_len, &has_hit[0])
+		labeled_aiarray_query_has_hit_from_array(self.laia,
+												 &labels[0],
+												 &starts[0],
+												 &ends[0],
+												 length,
+												 label_str_len,
+												 &has_hit[0])
 
 		return
-	
-	def has_hit_from_array(self, const long[::1] starts, const long[::1] ends, np.ndarray labels):
+
+	def has_hit(self, start, end, label):
 		"""
 		Find interval indices overlapping given ranges
-		
+
 		Parameters
 		----------
-			starts : numpy.ndarray {long}
+			starts : int | numpy.ndarray {long}
 				Start positions of intervals
-			ends : numpy.ndarray {long}
+			ends : int | numpy.ndarray {long}
 				End positions of intervals
-			labels : numpy.ndarray {str}
+			labels : int | numpy.ndarray {str}
 				Labels of intervals
 
 		Returns
 		-------
-			ref_index : np.ndarray {int}
-				Overlapping interval indices from LabeledIntervalArray
-			query_index : np.ndarray {int}
-				Overlapping interval indices from query LabeledIntervalArray
+			has_hit : np.ndarray {bool}
+				Bool array indicated overlap detected
 
 		.. warning::
-			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run. This will re-sort intervals inplace if ail.track_index = False.
+			This requires :func:`~aiarray.LabeledIntervalArray.construct` and will run it if not already run.
 
 		See Also
 		--------
-		LabeledIntervalArray.construct: Construct LabeledIntervalArray, required to call LabeledIntervalArray.intersect
+		LabeledIntervalArray.construct: Construct LabeledIntervalArray
 		LabeledIntervalArray.add: Add interval to LabeledIntervalArray
 		LabeledIntervalArray.intersect: Find intervals overlapping given range
 		LabeledIntervalArray.intersect_index: Find interval indices overlapping given range
 
 		Examples
 		--------
 		>>> from aiarray import LabeledIntervalArray
@@ -1434,293 +1643,197 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Check if object is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
-		# Check that labels are bytes
-		byte_labels = labels.astype(bytes)
+		# Initialize variables
+		cdef uint8_t has_hit_single_c = 0
+		cdef np.ndarray has_hit
+		cdef uint8[::1] has_hit_mem
+		cdef bytes byte_label
 
-		cdef np.ndarray has_hit = np.zeros(self.size, dtype=bool)
-		cdef uint8[::1] has_hit_mem = has_hit
+		# Intersect
+		if isinstance(start, np.ndarray):
+			# Check that labels are bytes
+			has_hit = np.zeros(len(start), dtype=bool)
+			has_hit_mem = has_hit
+			byte_labels = label.astype(bytes)
+			self._has_hit_from_array(start, end, has_hit_mem, np.PyArray_BYTES(byte_labels),
+									byte_labels.itemsize)
+
+			return has_hit
+
+		elif isinstance(start, int):
+			# Check that labels are bytes
+			byte_label = str(label).encode()
+			labeled_aiarray_query_has_hit(self.laia, byte_label, &has_hit_single_c, start, end)
+			if has_hit_single_c == 1:
+				return True
+			else:
+				return False
 
-		# Intersect from array
-		self._has_hit_from_array(starts, ends, has_hit_mem, np.PyArray_BYTES(byte_labels), byte_labels.itemsize)
-		
-		return has_hit
 
-	
-	cpdef _intersect_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray ail):
+	cdef labeled_aiarray_t *_intersect_from_labeled_aiarray(LabeledIntervalArray self,
+															LabeledIntervalArray laia):
 		# Intersect with other LabeledIntervalArray
-		cdef array_query_t *total_overlaps = labeled_aiarray_query_from_labeled_aiarray(self.ail, ail.ail)
-
-		# Create numpy array from C pointer
-		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index, total_overlaps.size)
-		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index, total_overlaps.size)
-
-		return ref_index, query_index
-
-	def intersect_from_LabeledIntervalArray(self, LabeledIntervalArray ail_query):
-		"""
-		Find interval indices overlapping given ranges
-		
-		Parameters
-		----------
-			ail_query : IntervalArray
-				Intervals to query
-
-		Returns
-		-------
-			ref_index : np.ndarray{int}
-				Overlapping interval indices from IntervalArray
-			query_index : np.ndarray{int}
-				Overlapping interval indices from query IntervalArray
-
-		See Also
-		--------
-		IntervalArray.construct: Construct IntervalArray, required to call IntervalArray.intersect
-		IntervalArray.add: Add interval to IntervalArray
-		IntervalArray.intersect: Find intervals overlapping given range
-		IntervalArray.intersect_from_array: Find interval indices overlapping given range
-
-		Examples
-		--------
-		>>> from IntervalArray import IntervalArray
-		>>> ail1 = IntervalArray()
-		>>> ail1.add(1, 2)
-		>>> ail1.add(3, 4)
-		>>> ail1.add(2, 6)
-		>>> ail1
-		IntervalArray
-		  range: (1-6)
-		   (1-2, 0)
-		   (3-4, 1)
-		   (2-6, 2)
-		>>> ail2 = IntervalArray()
-		>>> ail2.add(1, 2)
-		>>> ail2.add(3, 6)
-		>>> ail2
-		IntervalArray
-		  range: (1-6)
-		    (1-2, 0)
-		    (3-6, 1)
-		>>> q = ail1.intersect_from_IntervalArray(ail2)
-		>>> q
-		(array([0, 1, 1]), array([0, 2, 1]))
-
-		"""
-
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("LabeledIntervalArray object has been closed.")
-
-		# Check if object is constructed
-		if self.is_constructed == False:
-			self.construct()
-
-		# Intersect
-		query_index, ref_index = self._intersect_from_labeled_aiarray(ail_query)
-		
-		return query_index, ref_index
+		cdef labeled_aiarray_t *overlaps = labeled_aiarray_init()
+		labeled_aiarray_query_from_labeled_aiarray(self.laia, laia.laia, overlaps)
 
+		return overlaps
 
-	cpdef _intersect_with_index(LabeledIntervalArray self, int start, int end, const char *label_name):
-		# Intersect with interval
-		cdef overlap_label_index_t *total_overlaps = labeled_aiarray_query_single_with_index(self.ail, start, end, label_name)
+	cpdef _intersect_index_from_labeled_aiarray(LabeledIntervalArray self, LabeledIntervalArray laia):
+		# Intersect with other LabeledIntervalArray
+		cdef array_query_t *total_overlaps = array_query_init()
+		labeled_aiarray_query_index_from_labeled_aiarray(self.laia, laia.laia, total_overlaps)
 
 		# Create numpy array from C pointer
-		cdef np.ndarray indices = pointer_to_numpy_array(total_overlaps.indices, total_overlaps.size)
-		cdef LabeledIntervalArray overlaps = LabeledIntervalArray()
-		overlaps.set_list(total_overlaps.ail)
-
-		return overlaps, indices
-	
-	def intersect_with_index(self, int start, int end, str label):
-		"""
-		Find interval indices overlapping given ranges
-		
-		Parameters
-		----------
-			ail_query : IntervalArray
-				Intervals to query
-
-		Returns
-		-------
-			ref_index : np.ndarray{int}
-				Overlapping interval indices from IntervalArray
-			query_index : np.ndarray{int}
-				Overlapping interval indices from query IntervalArray
-
-		See Also
-		--------
-		IntervalArray.construct: Construct IntervalArray, required to call IntervalArray.intersect
-		IntervalArray.add: Add interval to IntervalArray
-		IntervalArray.intersect: Find intervals overlapping given range
-		IntervalArray.intersect_from_array: Find interval indices overlapping given range
-
-		Examples
-		--------
-		>>> from IntervalArray import IntervalArray
-		>>> ail1 = IntervalArray()
-		>>> ail1.add(1, 2)
-		>>> ail1.add(3, 4)
-		>>> ail1.add(2, 6)
-		>>> ail1
-		IntervalArray
-		  range: (1-6)
-		   (1-2)
-		   (3-4)
-		   (2-6)
-		>>> ail2 = IntervalArray()
-		>>> ail2.add(1, 2)
-		>>> ail2.add(3, 6)
-		>>> ail2
-		IntervalArray
-		  range: (1-6)
-		    (1-2)
-		    (3-6)
-		>>> q = ail1.intersect_from_IntervalArray(ail2)
-		>>> q
-		(array([0, 1, 1]), array([0, 2, 1]))
-
-		"""
-
-		# Check if object is still open
-		if self.is_closed:
-			raise NameError("IntervalArray object has been closed.")
-
-		# Check if object is constructed
-		if self.is_constructed == False:
-			self.construct()
-
-		# Check if label is present
-		try:
-			self.label_map[label]
-		except KeyError:
-			raise KeyError("Label given is not in LabeledIntervalArray.")
-
-		# Intersect
-		cdef LabeledIntervalArray overlaps
-		cdef np.ndarray indices
-		overlaps, indices = self._intersect_with_index(start, end, label.encode())
-		
-		return overlaps, indices
+		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index,
+															total_overlaps.size)
+		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index,
+																total_overlaps.size)
 
+		return ref_index, query_index
 
-	cpdef _intersect_with_index_from_LabeledIntervalArray(LabeledIntervalArray self, LabeledIntervalArray ail2):
+	cpdef _intersect_with_index_from_labeled_aiarray(LabeledIntervalArray self,
+														LabeledIntervalArray laia2):
 		# Intersect with interval
-		cdef overlap_label_index_t *total_overlaps = labeled_aiarray_query_with_index_from_labeled_aiarray(self.ail, ail2.ail)
+		cdef overlap_label_index_t *total_overlaps = overlap_label_index_init()
+		labeled_aiarray_query_with_index_from_labeled_aiarray(self.laia, laia2.laia, total_overlaps)
 
 		# Create numpy array from C pointer
+		print("total_overlaps.size", total_overlaps.size, flush=True)
 		cdef np.ndarray indices = pointer_to_numpy_array(total_overlaps.indices, total_overlaps.size)
 		cdef LabeledIntervalArray overlaps = LabeledIntervalArray()
-		overlaps.set_list(total_overlaps.ail)
+		overlaps.set_list(total_overlaps.laia)
 
 		return overlaps, indices
-	
-	def intersect_with_index_from_LabeledIntervalArray(self, LabeledIntervalArray ail):
+
+	def intersect_from_LabeledIntervalArray(self,
+											LabeledIntervalArray ail_query,
+											return_intervals = True,
+											return_index = False):
 		"""
 		Find interval indices overlapping given ranges
-		
+
 		Parameters
 		----------
-			ail_query : IntervalArray
+			ail_query : LabeledIntervalArray
 				Intervals to query
 
 		Returns
 		-------
 			ref_index : np.ndarray{int}
 				Overlapping interval indices from IntervalArray
 			query_index : np.ndarray{int}
 				Overlapping interval indices from query IntervalArray
 
 		See Also
 		--------
-		IntervalArray.construct: Construct IntervalArray, required to call IntervalArray.intersect
-		IntervalArray.add: Add interval to IntervalArray
-		IntervalArray.intersect: Find intervals overlapping given range
-		IntervalArray.intersect_from_array: Find interval indices overlapping given range
+		LabeledIntervalArray.construct: Construct IntervalArray
+		LabeledIntervalArray.add: Add interval to IntervalArray
+		LabeledIntervalArray.intersect: Find intervals overlapping given range
+		LabeledIntervalArray.intersect_from_array: Find interval indices overlapping given range
 
 		Examples
 		--------
-		>>> from IntervalArray import IntervalArray
+		>>> from ailist import LabeledIntervalArray
 		>>> ail1 = IntervalArray()
 		>>> ail1.add(1, 2)
 		>>> ail1.add(3, 4)
 		>>> ail1.add(2, 6)
 		>>> ail1
 		IntervalArray
 		  range: (1-6)
-		   (1-2)
-		   (3-4)
-		   (2-6)
-		>>> ail2 = IntervalArray()
-		>>> ail2.add(1, 2)
-		>>> ail2.add(3, 6)
+		   (1-2, 0)
+		   (3-4, 1)
+		   (2-6, 2)
+		>>> ail2 = LabeledIntervalArray()
+		>>> ail2.add(1, 2, "a")
+		>>> ail2.add(3, 6, "b")
+		>>> ail2.add(3, 6, "a")
 		>>> ail2
 		IntervalArray
 		  range: (1-6)
-		    (1-2)
-		    (3-6)
-		>>> q = ail1.intersect_from_IntervalArray(ail2)
+		    (1-2, 0)
+		    (3-6, 1)
+		>>> q = ail1.intersect_from_LabeledIntervalArray(ail2)
 		>>> q
 		(array([0, 1, 1]), array([0, 2, 1]))
 
 		"""
-		print("here\n", flush=True)
 
 		# Check if object is still open
 		if self.is_closed:
-			raise NameError("IntervalArray object has been closed.")
+			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Check if object is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
-		# Intersect
+		# Type variables
+		cdef labeled_aiarray_t *i_list
 		cdef LabeledIntervalArray overlaps
 		cdef np.ndarray indices
-		overlaps, indices = self._intersect_with_index_from_LabeledIntervalArray(ail)
-		## Set label_map
-		#overlaps.copy_maps(self)
-		
-		return overlaps, indices
+		cdef np.ndarray query_index
+		cdef np.ndarray ref_index
 
-	
-	cdef np.ndarray _nhits_from_array(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char[:,::1] labels):
-		# Initialize hits
-		cdef int length = starts.size
-		cdef int[::1] nhits = np.zeros(length, dtype=np.intc)
-		cdef const char *first_char = &labels[0,0]
+		# Intersect
+		if return_intervals:
+			if return_index:
+				overlaps, indices = self._intersect_with_index_from_labeled_aiarray(ail_query)
+				return overlaps, indices
+			else:
+				i_list = self._intersect_from_labeled_aiarray(ail_query)
+				overlaps = LabeledIntervalArray()
+				overlaps.set_list(i_list)
+				return overlaps
+
+		elif return_index:
+			query_index, ref_index = self._intersect_index_from_labeled_aiarray(ail_query)
+			return query_index, ref_index
+
+
+	cdef void _nhits_from_array(LabeledIntervalArray self,
+								const long[::1] starts,
+								const long[::1] ends,
+								long[::1] nhits,
+								const char *labels,
+								int label_str_len):
 
-		# Calculate distribution
-		labeled_aiarray_nhits_from_array(self.ail, &starts[0], &ends[0], &first_char, length, &nhits[0])
+		# Call C function
+		cdef int length = len(starts)
+		labeled_aiarray_nhits_from_array(self.laia, &labels[0], &starts[0], &ends[0], length,
+										label_str_len, &nhits[0])
 
-		return np.asarray(nhits, dtype=np.intc)
+		return
 
-	cdef np.ndarray _nhits_from_array_length(LabeledIntervalArray self, const long[::1] starts, const long[::1] ends, const char[:,::1] labels, int min_length, int max_length):
+	cdef void _nhits_from_array_length(LabeledIntervalArray self, const long[::1] starts,
+										const long[::1] ends, long[::1] nhits,
+										const char *labels, int label_str_len,
+										int min_length, int max_length):
 		# Initialize hits
 		cdef int length = starts.size
-		cdef int[::1] nhits = np.zeros(length, dtype=np.intc)
-		cdef const char *first_char = &labels[0,0]
 
 		# Calculate distribution
-		labeled_aiarray_nhits_from_array_length(self.ail, &starts[0], &ends[0], &first_char, length, &nhits[0], min_length, max_length)
+		labeled_aiarray_nhits_from_array_length(self.laia, &labels[0], &starts[0], &ends[0],
+												length, label_str_len, &nhits[0],
+												min_length, max_length)
 
-		return np.asarray(nhits, dtype=np.intc)
+		return
 
-	def nhits_from_array(self, const long[::1] starts, const long[::1] ends, np.ndarray labels, min_length=None, max_length=None):
+	def nhits(self, start, end, label, min_length=None, max_length=None):
 		"""
 		Find number of intervals overlapping given
 		positions
-		
+
 		Parameters
 		----------
 			starts : numpy.ndarray {long}
 				Start positions to intersect
 			ends : numpy.ndarray {long}
 				End positions to intersect
 			labels : numpy.ndarray {long}
@@ -1738,83 +1851,103 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("aiarray object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
-		# Initialize distribution
+		# Static type variables
 		cdef np.ndarray nhits
+		cdef long[::1] nhits_mem
+		cdef long single_nhits = 0
+		cdef bytes label_name
+
+		# Calculate nhits
+		if isinstance(start, int):
+			label_name = label.encode()
+			if min_length is None or max_length is None:
+				labeled_aiarray_nhits(self.laia, &single_nhits, label_name, start, end)
+			else:
+				labeled_aiarray_nhits_length(self.laia, &single_nhits, label_name,
+											 start, end, min_length, max_length)
+
+			return single_nhits
+
+		# Calculate nhits
+		elif isinstance(start, np.ndarray):
+			nhits = np.zeros(len(start), dtype=np.int_)
+			nhits_mem = nhits
+			byte_labels = label.astype(bytes)
+			if min_length is None or max_length is None:
+				self._nhits_from_array(start, end, nhits_mem, np.PyArray_BYTES(byte_labels),
+										byte_labels.itemsize)
+			else:
+				self._nhits_from_array_length(start, end, nhits_mem, np.PyArray_BYTES(byte_labels),
+												byte_labels.itemsize, min_length, max_length)
+
+			return nhits
 
-		# Calculate distribution
-		if min_length is None or max_length is None:
-			nhits = self._nhits_from_array(starts, ends, labels)
 		else:
-			nhits = self._nhits_from_array_length(starts, ends, labels, min_length, max_length)
+			raise TypeError("Could not determine given type for start.")
 
-		return nhits
 
 	cdef labeled_aiarray_t *_determine_bins(LabeledIntervalArray self, int bin_size):
 		"""
 		Create LabeledIntervalArray for bins
 		"""
 
 		# Initialize variables
 		cdef labeled_aiarray_t *bins = labeled_aiarray_init()
-		cdef int nbins
 		cdef int first
 		cdef int first_bin_start
 		cdef int last
 		cdef int start
 		#cdef uint16_t label
 		cdef int i
 		cdef int j
 		cdef const char *label_name
 
 		# Iterate over labels
-		for i in range(self.ail.nl):
-			if self.ail.label_count[i] > 0:
-				#label = self.ail.interval_list[self._get_label_index(i)].label
-				first = self.ail.first[i]
-				first_bin_start = (first // bin_size) * bin_size
-				last = self.ail.last[i]
-				n_bins = math.ceil(last / bin_size) - (first // bin_size)
-
-				# Iterate over label bins
-				for j in range(n_bins):
-					start = first_bin_start + (j * bin_size)
-					label_name = query_rev_label_map(self.ail, i)
-					labeled_aiarray_add(bins, start, start + bin_size, label_name)
+		for i in range(self.laia.n_labels):
+			#label = self.laia.interval_list[self._get_label_index(i)].label
+			first = self.laia.labels[i].ail.first
+			first_bin_start = (first // bin_size) * bin_size
+			last = self.laia.labels[i].ail.last
+			n_bins = math.ceil(last / bin_size) - (first // bin_size)
+			label_name = self.laia.labels[i].name
+
+			# Iterate over label bins
+			for j in range(n_bins):
+				start = first_bin_start + (j * bin_size)
+				labeled_aiarray_add(bins, start, start + bin_size, label_name)
 
 		return bins
 
-	cdef np.ndarray _bin_nhits(LabeledIntervalArray self, labeled_aiarray_t *bins, int bin_size):
-		# Initialize nhits
-		cdef double[::1] nhits = np.zeros(bins.nr, dtype=np.double)
+
+	cdef void _bin_nhits(LabeledIntervalArray self, long[::1] nhits, int bin_size):
 		# Determine bin hits
-		labeled_aiarray_bin_nhits(self.ail, bins, &nhits[0], bin_size)
+		labeled_aiarray_bin_nhits(self.laia, &nhits[0], bin_size)
 
-		return np.asarray(nhits)
+		return
 
-	cdef np.ndarray _bin_nhits_length(LabeledIntervalArray self, labeled_aiarray_t *bins, int bin_size, int min_length, int max_length):
-		# Initialize coverage
-		cdef double[::1] nhits = np.zeros(bins.nr, dtype=np.double)
+	cdef void _bin_nhits_length(LabeledIntervalArray self, long[::1] nhits, int bin_size,
+								int min_length, int max_length):
 		# Determine bin hits
-		labeled_aiarray_bin_nhits_length(self.ail, bins, &nhits[0], bin_size, min_length, max_length)
+		labeled_aiarray_bin_nhits_length(self.laia,  &nhits[0], bin_size, min_length, max_length)
 
-		return np.asarray(nhits)
+		return
 
 	def bin_nhits(self, int bin_size=100000, min_length=None, max_length=None):
 		"""
 		Find number of intervals overlapping binned
 		positions
-		
+
 		Parameters
 		----------
 			bin_size : int
 				Size of the bin to use
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
@@ -1833,41 +1966,37 @@
 
 		# Determine bins
 		cdef labeled_aiarray_t *cbins = self._determine_bins(bin_size)
 		cdef LabeledIntervalArray bins = LabeledIntervalArray()
 		bins.set_list(cbins)
 		bins.construct()
 
-		# Set bins label_map
-		cdef int label
-		cdef int i
-		for i in range(self.ail.nl):
-			bins.label_map[self.rev_label_map[i]] = i
-			bins.rev_label_map[i] = self.rev_label_map[i]
-
 		# Initialize nhits
-		cdef np.ndarray nhits
+		cdef np.ndarray nhits = np.zeros(bins.size, dtype=np.int_)
+		cdef long[::1] nhits_mem = nhits
+
 		# Calculate nhits
 		if min_length is None or max_length is None:
-			nhits = self._bin_nhits(bins.ail, bin_size)
+			self._bin_nhits(nhits_mem, bin_size)
 		else:
-			nhits = self._bin_nhits_length(bins.ail, bin_size, min_length, max_length)
-		
+			self._bin_nhits_length(nhits_mem, bin_size, min_length, max_length)
+
+
 		return bins, nhits
 
 
-	def nhits(self, int start, int end, str label, min_length=None, max_length=None):
+	def nhits_from_LabeledIntervalArray(self, LabeledIntervalArray query_laia, min_length=None,
+										max_length=None):
 		"""
-		Find number of intervals overlapping binned
-		positions
-		
+		Find number of intervals overlapping
+
 		Parameters
 		----------
-			bin_size : int
-				Size of the bin to use
+			query_laia : LabeledIntervalArray
+				Intervals to query
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
 				Maximum length of intervals to include [default = None]
 
 		Returns
 		-------
@@ -1875,57 +2004,61 @@
 				Position on index and coverage as values
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
+		if query_laia.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Initialize nhits
+		cdef np.ndarray nhits = np.zeros(query_laia.size, dtype=np.int_)
+		cdef long[::1] nhits_mem = nhits
 
 		# Calculate nhits
-		cdef int nhits
-		cdef bytes label_name = label.encode()
 		if min_length is None or max_length is None:
-			nhits = labeled_aiarray_nhits(self.ail, start, end, label_name)
+			labeled_aiarray_nhits_from_labeled_aiarray(self.laia, query_laia.laia, &nhits_mem[0])
 		else:
-			nhits = labeled_aiarray_nhits_length(self.ail, start, end, label_name, min_length, max_length)
-		
+			labeled_aiarray_nhits_from_labeled_aiarray_length(self.laia, query_laia.laia,
+																&nhits_mem[0], min_length,
+																max_length)
+
 		return nhits
 
-	
-	cdef np.ndarray _wps(LabeledIntervalArray self, int protection):
+
+	cdef np.ndarray _wps(LabeledIntervalArray self, const char *label_name, int protection):
 		# Initialize wps
-		cdef long n = 0
-		cdef int i
-		for i in range(self.ail.nl):
-			n += self.ail.last[i] - self.ail.first[i]
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef long n = self.laia.labels[t].ail.last - self.laia.labels[t].ail.first
 		cdef double[::1] wps = np.zeros(n, dtype=np.double)
 
 		# Calculate wps
-		labeled_aiarray_wps(self.ail, &wps[0], protection)
+		labeled_aiarray_label_wps(self.laia, &wps[0], protection, label_name)
 
 		return np.asarray(wps)
 
-	cdef np.ndarray _wps_length(LabeledIntervalArray self, int protection, int min_length, int max_length):
+	cdef np.ndarray _wps_length(LabeledIntervalArray self, const char *label_name, int protection,
+								int min_length, int max_length):
 		# Initialize wps
-		cdef long n = 0
-		cdef int i
-		for i in range(self.ail.nl):
-			n += self.ail.last[i] - self.ail.first[i]
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef long n = self.laia.labels[t].ail.last - self.laia.labels[t].ail.first
 		cdef double[::1] wps = np.zeros(n, dtype=np.double)
 
 		# Calculate wps
-		labeled_aiarray_wps_length(self.ail, &wps[0], protection, min_length, max_length)
+		labeled_aiarray_label_wps_length(self.laia, &wps[0], protection, min_length, max_length,
+											label_name)
 
 		return np.asarray(wps)
 
-	def wps(self, int protection=60, min_length=None, max_length=None):
+	def wps(self, int protection=60, labels=None, min_length=None, max_length=None):
 		"""
 		Calculate Window Protection Score
 		for each position in LabeledIntervalArray range
-		
+
 		Parameters
 		----------
 			protection : int
 				Protection window to use
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
@@ -1937,81 +2070,153 @@
 				Position on index and WPS as values
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("aiarray object has been closed.")
-		
-		# Initialize wps
-		cdef np.ndarray wps
-		# Calculate wps
-		if self.ail.nr == 0:
+
+		# Check if empty
+		if self.laia.total_nr == 0:
 			return None
-		if min_length is None or max_length is None:
-			wps = self._wps(protection)
+
+		# Determine which labels to calculate
+		if labels is None:
+			labels = self.unique_labels
+		elif isinstance(labels, str):
+			labels = np.array([labels])
 		else:
-			wps = self._wps_length(protection, min_length, max_length)
-		
-		return wps
+			labels = np.array(labels)
 
-	
-	cdef np.ndarray _coverage(LabeledIntervalArray self):
-		# Initialize wps
-		cdef long n = 0
-		cdef int i
-		for i in range(self.ail.nl):
-			n += self.ail.last[i] - self.ail.first[i]
+		# Check all labels present
+		missing_labels = set(labels) - set(self.unique_labels)
+		if len(missing_labels) > 0:
+			raise KeyError("Provided label not in LabeledIntervalArray. " + str(missing_labels))
+
+		# Get label ranges
+		label_ranges = self.label_ranges
+
+		# Convert to bytes
+		labels = labels.astype(bytes)
 
-		cdef double[::1] coverage = np.zeros(n, dtype=np.double)
+		# Iterate over labels
+		wps_results = {}
+		cdef const char *label_name
+		cdef np.ndarray wps
+		#cdef np.bytes_ label
+		for label in labels:
+			label_name = label
+
+			# Calculate wps
+			if min_length is None or max_length is None:
+				wps = self._wps(label_name, protection)
+			else:
+				wps = self._wps_length(label_name, protection, min_length, max_length)
+
+			wps_results[label.decode()] = pd.Series(wps,
+													index = range(label_ranges[label.decode()][0],
+																  label_ranges[label.decode()][1]))
+
+		return wps_results
 
-		# Calculate coverage
-		labeled_aiarray_coverage(self.ail, &coverage[0])
 
-		return np.asarray(coverage)
+	cdef np.ndarray _coverage(LabeledIntervalArray self, const char *label_name):
+		# Initialize cov
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef long n = self.laia.labels[t].ail.last - self.laia.labels[t].ail.first
+		cdef double[::1] cov = np.zeros(n, dtype=np.double)
 
+		# Calculate cov
+		labeled_aiarray_label_coverage(self.laia, &cov[0], label_name)
 
-	def coverage(self):
+		return np.asarray(cov)
+
+	cdef np.ndarray _coverage_length(LabeledIntervalArray self, const char *label_name,
+									int min_length, int max_length):
+		# Initialize cov
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef long n = self.laia.labels[t].ail.last - self.laia.labels[t].ail.first
+		cdef double[::1] cov = np.zeros(n, dtype=np.double)
+
+		# Calculate cov
+		labeled_aiarray_label_coverage_length(self.laia, &cov[0], label_name,
+												min_length, max_length)
+
+		return np.asarray(cov)
+
+	def coverage(self, labels=None, min_length=None, max_length=None):
 		"""
 		Calculate coverage
 		for each position in LabeledIntervalArray range
-		
+
 		Parameters
 		----------
 			min_length : int
 				Minimum length of intervals to include [default = None]
 			max_length : int
 				Maximum length of intervals to include [default = None]
 
 		Returns
 		-------
-			coverage : numpy.ndarray
+			cov_results : dict {str:numpy.ndarray}
 				Coverage as values
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
-			raise NameError("labeled_aiarray object has been closed.")
-		
-		# Initialize coverage
-		cdef np.ndarray coverage
-		# Calculate coverage
-		if self.ail.nr == 0:
+			raise NameError("aiarray object has been closed.")
+
+		# Check if empty
+		if self.laia.total_nr == 0:
 			return None
-		
-		coverage = self._coverage()
-		
-		return coverage
 
-	
+		# Determine which labels to calculate
+		if labels is None:
+			labels = self.unique_labels
+		elif isinstance(labels, str):
+			labels = np.array([labels])
+		else:
+			labels = np.array(labels)
+
+		# Check all labels present
+		missing_labels = set(labels) - set(self.unique_labels)
+		if len(missing_labels) > 0:
+			raise KeyError("Provided label not in LabeledIntervalArray. " + str(missing_labels))
+
+		# Get label ranges
+		label_ranges = self.label_ranges
+
+		# Convert to bytes
+		labels = labels.astype(bytes)
+
+		# Iterate over labels
+		cov_results = {}
+		cdef const char *label_name
+		cdef np.ndarray cov
+		for label in labels:
+			label_name = label
+
+			# Calculate wps
+			if min_length is None or max_length is None:
+				cov = self._coverage(label_name)
+			else:
+				cov = self._coverage_length(label_name, min_length, max_length)
+
+			cov_results[label.decode()] = pd.Series(cov,
+													index = range(label_ranges[label.decode()][0],
+																  label_ranges[label.decode()][1]))
+
+		return cov_results
+
+
 	def merge(self, int gap=0):
 		"""
 		Merge intervals within a gap
-		
+
 		Parameters
 		----------
 			gap : int
 				Gap between intervals to merge
 
 		Returns
 		-------
@@ -2021,37 +2226,29 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("aiarray object has been closed.")
 
 		# Make sure list is constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
 
 		# Create merged
 		cdef LabeledIntervalArray merged_list = LabeledIntervalArray()
-		cdef labeled_aiarray_t *merged_clist = labeled_aiarray_merge(self.ail, gap)
+		cdef labeled_aiarray_t *merged_clist = labeled_aiarray_merge(self.laia, gap)
 		merged_list.set_list(merged_clist)
-		# Set bins label_map
-		cdef int label
-		cdef int i
-		for i in range(self.ail.nl):
-			if self.ail.label_count[i] > 0:
-				label = self.ail.interval_list[self._get_label_index(i)].label
-				merged_list.label_map[self.rev_label_map[label]] = label
-				merged_list.rev_label_map[label] = self.rev_label_map[label]
 
 		return merged_list
 
-	
+
 	def filter(self, int min_length=1, int max_length=400):
 		"""
 		Filter out intervals outside of a length range
-		
+
 		Parameters
 		----------
 			min_length : int
 				Minimum length to keep
 			max_length : int
 				Maximum langth to keep
 
@@ -2065,32 +2262,40 @@
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Initialize filtered list
 		cdef LabeledIntervalArray filtered_ail = LabeledIntervalArray()
 
-		cdef labeled_aiarray_t *cfiltered_ail = labeled_aiarray_length_filter(self.ail, min_length, max_length)
+		cdef labeled_aiarray_t *cfiltered_ail = labeled_aiarray_length_filter(self.laia, min_length,
+																				max_length)
 		filtered_ail.set_list(cfiltered_ail)
-		# Set bins label_map
-		cdef int label
-		cdef int i
-		for i in range(self.ail.nl):
-			if self.ail.label_count[i] > 0:
-				label = self.ail.interval_list[self._get_label_index(i)].label
-				filtered_ail.label_map[self.rev_label_map[label]] = label
-				filtered_ail.rev_label_map[label] = self.rev_label_map[label]
 
 		return filtered_ail
-	
 
-	def downsample(self, double proportion):
+
+	cpdef _downsample_with_index(LabeledIntervalArray self, double proportion):
+		# Randomly downsample LabeledIntervalArray
+		cdef overlap_label_index_t *new_intervals = labeled_aiarray_downsample_with_index(self.laia,
+																							proportion)
+
+		# Create numpy array from C pointer
+		cdef np.ndarray indices = pointer_to_numpy_array(new_intervals.indices, new_intervals.size)
+		cdef LabeledIntervalArray intervals = LabeledIntervalArray()
+		intervals.set_list(new_intervals.laia)
+
+		return intervals, indices
+
+	def downsample(self,
+				   double proportion,
+				   return_intervals = True,
+				   return_index = True):
 		"""
 		Randomly downsample LabeledIntervalArray
-		
+
 		Parameters
 		----------
 			proportion : double
 				Proportion of intervals to keep
 
 		Returns
 		-------
@@ -2100,424 +2305,891 @@
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Initialize filtered list
-		cdef LabeledIntervalArray filtered_ail = LabeledIntervalArray()
+		cdef LabeledIntervalArray filtered_ail
+		cdef labeled_aiarray_t *cfiltered_ail
+		cdef np.ndarray indices
+		if return_intervals:
+			if return_index:
+				filtered_ail, indices = self._downsample_with_index(proportion)
 
-		cdef labeled_aiarray_t *cfiltered_ail = labeled_aiarray_downsample(self.ail, proportion)
-		filtered_ail.set_list(cfiltered_ail)
-		# Set bins label_map
-		cdef int label
-		cdef int i
-		for i in range(self.ail.nl):
-			if self.ail.label_count[i] > 0:
-				label = self.ail.interval_list[self._get_label_index(i)].label
-				filtered_ail.label_map[self.rev_label_map[label]] = label
-				filtered_ail.rev_label_map[label] = self.rev_label_map[label]
+				return filtered_ail, indices
+			else:
+				filtered_ail = LabeledIntervalArray()
+				cfiltered_ail = labeled_aiarray_downsample(self.laia, proportion)
+				filtered_ail.set_list(cfiltered_ail)
 
-		return filtered_ail
+				return filtered_ail
 
-	
-	cpdef _downsample_with_index(LabeledIntervalArray self, double proportion):
-		# Randomly downsample LabeledIntervalArray
-		cdef overlap_label_index_t *new_intervals = labeled_aiarray_downsample_with_index(self.ail, proportion)
+		elif return_index:
+			# Intersect
+			filtered_ail, indices = self._downsample_with_index(proportion)
 
-		# Create numpy array from C pointer
-		cdef np.ndarray indices = pointer_to_numpy_array(new_intervals.indices, new_intervals.size)
-		cdef LabeledIntervalArray intervals = LabeledIntervalArray()
-		intervals.set_list(new_intervals.ail)
+			return indices
 
-		return intervals, indices
-	
-	def downsample_with_index(self, double proportion):
+
+	cdef np.ndarray _length_dist(LabeledIntervalArray self):
+		# Initialize distribution
+		cdef int max_length = labeled_aiarray_max_length(self.laia)
+		cdef int[::1] distribution = np.zeros(max_length + 1, dtype=np.intc)
+
+		# Calculate distribution
+		labeled_aiarray_length_distribution(self.laia, &distribution[0])
+
+		return np.asarray(distribution, dtype=np.intc)
+
+	def length_dist(self):
 		"""
-		Find interval indices overlapping given ranges
-		
+		Calculate length distribution of intervals
+
 		Parameters
 		----------
-			ail_query : IntervalArray
-				Intervals to query
+			None
 
 		Returns
 		-------
-			ref_index : np.ndarray{int}
-				Overlapping interval indices from IntervalArray
-			query_index : np.ndarray{int}
-				Overlapping interval indices from query IntervalArray
+			distribution : numpy.ndarray{int}
+				Interval length distribution
 
-		See Also
-		--------
-		IntervalArray.construct: Construct IntervalArray, required to call IntervalArray.intersect
-		IntervalArray.add: Add interval to IntervalArray
-		IntervalArray.intersect: Find intervals overlapping given range
-		IntervalArray.intersect_from_array: Find interval indices overlapping given range
+		"""
 
-		Examples
-		--------
-		>>> from IntervalArray import IntervalArray
-		>>> ail1 = IntervalArray()
-		>>> ail1.add(1, 2)
-		>>> ail1.add(3, 4)
-		>>> ail1.add(2, 6)
-		>>> ail1
-		IntervalArray
-		  range: (1-6)
-		   (1-2)
-		   (3-4)
-		   (2-6)
-		>>> ail2 = IntervalArray()
-		>>> ail2.add(1, 2)
-		>>> ail2.add(3, 6)
-		>>> ail2
-		IntervalArray
-		  range: (1-6)
-		    (1-2)
-		    (3-6)
-		>>> q = ail1.intersect_from_IntervalArray(ail2)
-		>>> q
-		(array([0, 1, 1]), array([0, 2, 1]))
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Initialize distribution
+		cdef np.ndarray distribution
+
+		# Calculate distribution
+		distribution = self._length_dist()
+
+		return distribution
+
+
+	cpdef _filter_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
+		"""
+		"""
+
+		cdef overlap_label_index_t *matched_ail = labeled_aiarray_exact_match(self.laia,
+																				other_aiarray.laia)
+
+		# Create numpy array from C pointer
+		cdef np.ndarray indices = pointer_to_numpy_array(matched_ail.indices, matched_ail.size)
+		cdef LabeledIntervalArray matched = LabeledIntervalArray()
+		matched.set_list(matched_ail.laia)
+
+		return matched, indices
+
+	def filter_exact_match(self, LabeledIntervalArray other_aiarray):
+		"""
+		Determine which intervals are present
+
+		Parameters
+		----------
 
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
+			raise NameError("AIList object has been closed.")
+
+		# Check construction
+		if self.is_constructed is False:
+			self.construct()
+		if other_aiarray.is_constructed is False:
+			other_aiarray.construct()
+
+		matched_ail, indices = self._filter_exact_match(other_aiarray)
+
+		return matched_ail, indices
+
+
+	cdef void _has_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray,
+								uint8_t[::1] has_match):
+		"""
+		"""
+
+		# Call C function
+		labeled_aiarray_has_exact_match(self.laia, other_aiarray.laia, &has_match[0])
+
+		return
+
+	def has_exact_match(self, LabeledIntervalArray other_aiarray):
+		"""
+		Determine which intervals are present
+		"""
+
+		# Check if object is still open
+		if self.is_closed or other_aiarray.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check if object is constructed
-		if self.is_constructed == False:
+		# Check if objects are constructed
+		if self.is_constructed is False:
 			self.construct()
+		if other_aiarray.is_constructed is False:
+			other_aiarray.construct()
 
-		# Intersect
-		cdef LabeledIntervalArray filtered_ail
-		cdef np.ndarray indices
-		filtered_ail, indices = self._downsample_with_index(proportion)
-		# Set bins label_map
-		cdef int label
-		cdef int i
-		for i in range(self.ail.nl):
-			if self.ail.label_count[i] > 0:
-				label = self.ail.interval_list[self._get_label_index(i)].label
-				filtered_ail.label_map[self.rev_label_map[label]] = label
-				filtered_ail.rev_label_map[label] = self.rev_label_map[label]
-		
-		return filtered_ail, indices
-	
+		# Find matches
+		cdef np.ndarray has_match = np.zeros(self.laia.total_nr, dtype=bool)
+		cdef uint8_t[::1] has_match_mem = has_match
+		self._has_exact_match(other_aiarray, has_match_mem)
+
+		return has_match
+
+
+	cdef void _is_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray,
+								uint8_t[::1] has_match1, uint8_t[::1] has_match2):
+		"""
+		"""
+
+		# Call C function
+		labeled_aiarray_is_exact_match(self.laia, other_aiarray.laia, &has_match1[0], &has_match2[0])
+
+		return
 
-	def extract_starts(self):
+	def is_exact_match(self, LabeledIntervalArray other_aiarray):
 		"""
-		Return the start values
+		Determine which intervals are present
 
 		Parameters
 		----------
-			None
+			other_aiarray: LabeledIntervalArray
+				Other LabeledIntervalArray object to compare to
 
 		Returns
 		-------
-			numpy.ndarray
-				Start values
+			ref_index : numpy.ndarray{int}
+				Indices of intervals in self that are present in other_aiarray
+			query_index : numpy.ndarray{int}
+				Indices of intervals in other_aiarray that are present in self
+
+		See Also
+		--------
+			:func:`has_exact_match`
+
+		Examples
+		--------
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(0, 10, "a")
+		>>> ail.add(20, 30, "a")
+		>>> ail.add(40, 50, "b")
+		>>> ail.add(60, 70, "b")
+		>>> ail2 = LabeledIntervalArray()
+		>>> ail2.add(0, 10, "a")
+		>>> ail2.add(20, 30, "b")
+		>>> ail2.add(40, 50, "c")
+		>>> ref_index, query_index = ail.is_exact_match(ail2)
 		"""
 
 		# Check if object is still open
-		if self.is_closed:
+		if self.is_closed or other_aiarray.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Extract start values
-		cdef long[::1] starts = np.zeros(self.size, dtype=np.int_)
-		labeled_aiarray_extract_starts(self.ail, &starts[0])
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
+		if other_aiarray.is_constructed is False:
+			other_aiarray.construct()
 
-		return np.asarray(starts, dtype=np.int_)
+		# Find matches
+		cdef np.ndarray has_match1 = np.zeros(self.laia.total_nr, dtype=bool)
+		cdef uint8_t[::1] has_match_mem1 = has_match1
+		cdef np.ndarray has_match2 = np.zeros(other_aiarray.laia.total_nr, dtype=bool)
+		cdef uint8_t[::1] has_match_mem2 = has_match2
+		# Call C function
+		self._is_exact_match(other_aiarray, has_match_mem1, has_match_mem2)
 
-	
-	def extract_ends(self):
+		return has_match1, has_match2
+
+
+	cpdef _which_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
+
+		cdef array_query_t *total_overlaps = array_query_init()
+		labeled_aiarray_which_exact_match(self.laia, other_aiarray.laia, total_overlaps)
+
+		cdef np.ndarray ref_index = pointer_to_numpy_array(total_overlaps.ref_index,
+															total_overlaps.size)
+		cdef np.ndarray query_index = pointer_to_numpy_array(total_overlaps.query_index,
+																total_overlaps.size)
+
+		return ref_index, query_index
+
+
+	def which_exact_match(self, LabeledIntervalArray other_aiarray):
 		"""
-		Return the end values
+		Determine which intervals are present
 
 		Parameters
 		----------
-			None
+			other_aiarray: LabeledIntervalArray
+				Other LabeledIntervalArray object to compare to
 
 		Returns
 		-------
-			numpy.ndarray
-				End values
+			ref_index : numpy.ndarray{int}
+				Indices of intervals in self that are present in other_aiarray
+			query_index : numpy.ndarray{int}
+				Indices of intervals in other_aiarray that are present in self
+
+		See Also
+		--------
+			:func:`has_exact_match`
+
+		Examples
+		--------
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(0, 10, "a")
+		>>> ail.add(20, 30, "a")
+		>>> ail.add(40, 50, "b")
+		>>> ail.add(60, 70, "b")
+		>>> ail2 = LabeledIntervalArray()
+		>>> ail2.add(0, 10, "a")
+		>>> ail2.add(20, 30, "b")
+		>>> ail2.add(40, 50, "c")
+		>>> ref_index, query_index = ail.is_exact_match(ail2)
 		"""
 
 		# Check if object is still open
-		if self.is_closed:
+		if self.is_closed or other_aiarray.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Extract end values
-		cdef long[::1] ends = np.zeros(self.size, dtype=np.int_)
-		labeled_aiarray_extract_ends(self.ail, &ends[0])
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
+		if other_aiarray.is_constructed is False:
+			other_aiarray.construct()
 
-		return np.asarray(ends, dtype=np.int_)
+		# Call C function
+		ref_index, query_index = self._which_exact_match(other_aiarray)
 
-	
-	def extract_labels(self):
+		return ref_index, query_index
+
+
+	cdef int _where_interval(LabeledIntervalArray self, int start, int end, const char *label_name):
+
+		cdef index = labeled_aiarray_where_interval(self.laia, label_name, start, end)
+
+		return index
+
+
+	def where_interval(self, start, end, label):
 		"""
-		Return the label values
+		Determine which intervals are present
 
 		Parameters
 		----------
-			None
+			other_aiarray: LabeledIntervalArray
+				Other LabeledIntervalArray object to compare to
 
 		Returns
 		-------
-			labels : numpy.ndarray
-				label values
+			ref_index : numpy.ndarray{int}
+				Indices of intervals in self that are present in other_aiarray
+			query_index : numpy.ndarray{int}
+				Indices of intervals in other_aiarray that are present in self
+
+		See Also
+		--------
+			:func:`has_exact_match`
+
+		Examples
+		--------
+		>>> from ailist import LabeledIntervalArray
+		>>> ail = LabeledIntervalArray()
+		>>> ail.add(0, 10, "a")
+		>>> ail.add(20, 30, "a")
+		>>> ail.add(40, 50, "b")
+		>>> ail.add(60, 70, "b")
+		>>> ail2 = LabeledIntervalArray()
+		>>> ail2.add(0, 10, "a")
+		>>> ail2.add(20, 30, "b")
+		>>> ail2.add(40, 50, "c")
+		>>> ref_index, query_index = ail.is_exact_match(ail2)
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Extract end values
-		cdef np.ndarray labels = np.zeros(self.size, dtype=np.object)
-		cdef int i
-		cdef LabeledInterval interval
-		for i, interval in enumerate(self):
-			labels[i] = interval.label
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
 
-		return labels
+		# Call C function
+		cdef bytes label_name = label.encode()
+		cdef int index = self._where_interval(start, end, label_name)
 
-	
-	cdef np.ndarray _length_dist(LabeledIntervalArray self):
-		# Initialize distribution
-		cdef int max_length = labeled_aiarray_max_length(self.ail)
-		cdef int[::1] distribution = np.zeros(max_length + 1, dtype=np.intc)
+		return index
 
-		# Calculate distribution
-		labeled_aiarray_length_distribution(self.ail, &distribution[0])
 
-		return np.asarray(distribution, dtype=np.intc)
+	cdef int _index_with_aiarray(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
 
-	def length_dist(self):
+		# Call C function
+		cdef int result = labeled_aiarray_index_with_aiarray(self.laia, other_aiarray.laia)
+
+		return result
+
+
+	def index_with_aiarray(self, LabeledIntervalArray other_aiarray):
+		"""
 		"""
-		Calculate length distribution of intervals
 
-		Parameters
-		----------
-			None
-		
-		Returns
-		-------
-			distribution : numpy.ndarray{int}
-				Interval length distribution
+		# Check if object is still open
+		if self.is_closed or other_aiarray.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		return_code = self._index_with_aiarray(other_aiarray)
+
+		if return_code == 1:
+			raise NameError("Failed to run properly. Values are likely currupted now.")
 
+
+	cdef void _get_locs(LabeledIntervalArray self, uint8[::1] locs_view, char *label_names,
+						int label_str_len, int n_labels):
+		"""
+		"""
+
+		labeled_aiarray_get_label_array_presence(self.laia, &label_names[0], n_labels, &locs_view[0],
+												label_str_len)
+
+		return
+
+	def get_locs(self, labels):
+		"""
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
-			raise NameError("AIList object has been closed.")
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Initialize distribution
-		cdef np.ndarray distribution
+		cdef np.ndarray locs = np.zeros(self.size, dtype=bool)
+		cdef uint8[::1] locs_view = np.frombuffer(locs, dtype=np.uint8)
 
-		# Calculate distribution
-		distribution = self._length_dist()
+		# Check that labels are bytes
+		if isinstance(labels, np.ndarray) is False:
+			labels = np.array(labels)
+		byte_labels = labels.astype(bytes)
 
-		return distribution
+		# Intersect from array
+		self._get_locs(locs_view, np.PyArray_BYTES(byte_labels), byte_labels.itemsize, len(labels))
 
+		return locs
 
-	cpdef _filter_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
+
+	cdef void _create_bin(LabeledIntervalArray self, int bin_size, int bin_range,
+							const char* label_name):
 		"""
+		Create LabeledIntervalArray for bins
 		"""
 
-		cdef overlap_label_index_t *matched_ail = has_exact_match(self.ail, other_aiarray.ail)
+		# Initialize variables
+		cdef int first
+		cdef int first_bin_start
+		cdef int last
+		cdef int start
+		cdef int j
 
-		# Create numpy array from C pointer
-		cdef np.ndarray indices = pointer_to_numpy_array(matched_ail.indices, matched_ail.size)
-		cdef LabeledIntervalArray matched = LabeledIntervalArray()
-		matched.set_list(matched_ail.ail)
+		# Find bounds
+		first = 0
+		first_bin_start = (first // bin_size) * bin_size
+		last = bin_range
+		n_bins = math.ceil(last / bin_size) - (first // bin_size)
+
+		# Iterate over label bins
+		for j in range(n_bins):
+			start = first_bin_start + (j * bin_size)
+			labeled_aiarray_add(self.laia, start, start + bin_size, label_name)
 
-		return matched, indices
+		return
 
-	def filter_exact_match(self, LabeledIntervalArray other_aiarray):
+	@staticmethod
+	def create_bin(dict_range, bin_size=100000):
+		"""
+		"""
+
+		cdef LabeledIntervalArray laia = LabeledIntervalArray()
+		cdef int bin_range
+		cdef bytes label_bytes
+		cdef const char* label_name
+
+		for label in dict_range:
+			label_bytes = label.encode()
+			label_name = label_bytes
+			bin_range = dict_range[label]
+			laia._create_bin(bin_size, bin_range, label_name)
+
+		return laia
+
+
+	def simulate(self):
 		"""
-		Determine which intervals are present
 		"""
 
 		# Check if object is still open
 		if self.is_closed:
-			raise NameError("AIList object has been closed.")
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check construction
-		if self.is_constructed == False:
+		cdef LabeledIntervalArray simulation = LabeledIntervalArray()
+		labeled_aiarray_simulate(self.laia, simulation.laia)
+
+		return simulation
+
+
+	def sorted_index(self):
+		"""
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Check if objects are constructed
+		if self.is_constructed is False:
 			self.construct()
-		if other_aiarray.is_constructed == False:
-			other_aiarray.construct()
 
-		matched_ail, indices = self._filter_exact_match(other_aiarray)
+		cdef np.ndarray sorted_index = np.zeros(self.size, dtype=np.int_)
+		cdef long[::1] sorted_index_mem = sorted_index
+		labeled_aiarray_sort_index(self.laia, &sorted_index_mem[0])
 
-		return matched_ail, indices
+		return sorted_index
 
-	
-	cdef np.ndarray _has_exact_match(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
+
+	def sort(self):
 		"""
 		"""
 
-		cdef LabeledIntervalArray matched_ail = LabeledIntervalArray()
-		cdef LabeledInterval query_interval
-		cdef LabeledInterval interval
-		cdef bint present = False
-		cdef int i
-		cdef int start_i
-		cdef int end_i
-		cdef np.ndarray has_match = np.zeros(len(self), dtype=bool)
-		cdef dict label_counts = self.label_counts
-		cdef np.ndarray label_index = self.label_index
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		for query_interval in other_aiarray:
-			try:
-				if label_counts[query_interval.label] > 0:
-					start_i = label_index[self.label_map[query_interval.label]]
-					if self.label_map[query_interval.label] + 1 == self.ail.nl:
-						end_i = self.ail.nr
-					else:
-						end_i = label_index[self.label_map[query_interval.label] + 1]
-
-					for i in range(start_i, end_i):
-						interval = self[i]
-						if interval.label == query_interval.label and interval.start == query_interval.start and interval.end == query_interval.end:
-							has_match[i] = True
-							break
-			except KeyError:
-				continue
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
 
-		return has_match
+		labeled_aiarray_sort(self.laia)
 
-	def has_exact_match(self, LabeledIntervalArray other_aiarray):
+		return
+
+
+	cdef np.ndarray _midpoint_coverage(LabeledIntervalArray self, const char *label_name):
+		# Initialize cov
+		cdef uint32_t t = get_label(self.laia, label_name)
+		cdef long n = self.laia.labels[t].ail.last - self.laia.labels[t].ail.first
+		cdef double[::1] cov = np.zeros(n, dtype=np.double)
+
+		# Calculate cov
+		labeled_aiarray_label_midpoint_coverage(self.laia, &cov[0], label_name)
+
+		return np.asarray(cov)
+
+	def midpoint_coverage(self, labels=None, min_length=None, max_length=None):
 		"""
-		Determine which intervals are present
+		Calculate coverage
+		for each position in LabeledIntervalArray range
+
+		Parameters
+		----------
+			min_length : int
+				Minimum length of intervals to include [default = None]
+			max_length : int
+				Maximum length of intervals to include [default = None]
+
+		Returns
+		-------
+			cov_results : dict {str:numpy.ndarray}
+				Coverage as values
 		"""
 
 		# Check if object is still open
-		if self.is_closed or other_aiarray.is_closed:
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Check if empty
+		if self.laia.total_nr == 0:
+			return None
+
+		# Determine which labels to calculate
+		if labels is None:
+			labels = self.unique_labels
+		elif isinstance(labels, str):
+			labels = np.array([labels])
+		else:
+			labels = np.array(labels)
+
+		# Check all labels present
+		missing_labels = set(labels) - set(self.unique_labels)
+		if len(missing_labels) > 0:
+			raise KeyError("Provided label not in LabeledIntervalArray. " + str(missing_labels))
+
+		# Get label ranges
+		label_ranges = self.label_ranges
+
+		# Convert to bytes
+		labels = labels.astype(bytes)
+
+		# Iterate over labels
+		cov_results = {}
+		cdef const char *label_name
+		cdef np.ndarray cov
+		for label in labels:
+			label_name = label
+
+			# Calculate wps
+			if min_length is None or max_length is None:
+				cov = self._midpoint_coverage(label_name)
+			else:
+				cov = self._midpoint_coverage_length(label_name, min_length, max_length)
+
+			cov_results[label.decode()] = pd.Series(cov,
+													index = range(label_ranges[label.decode()][0],
+																  label_ranges[label.decode()][1]))
+
+		return cov_results
+
+
+	def common(LabeledIntervalArray self, LabeledIntervalArray other_laia):
+		"""
+		Finds the common intervals between two LabeledIntervalArrays
+
+		Parameters
+		----------
+			other_laia : LabeledIntervalArray
+				LabeledIntervalArray to find common intervals with
+
+		Returns
+		-------
+			common_laia : LabeledIntervalArray
+				LabeledIntervalArray with common intervals
+
+		See Also
+		--------
+			LabeledIntervalArray.union
+			LabeledIntervalArray.subtract
+			LabeledIntervalArray.intersect
+
+		Notes
+		-----
+			- The common intervals are returned as a new LabeledIntervalArray
+			- The common intervals are not sorted
+
+		Examples
+		>>> laia1 = LabeledIntervalArray()
+		>>> laia1.add_interval(0, 10, 'A')
+		>>> laia1.add_interval(10, 20, 'B')
+		>>> laia1.add_interval(20, 30, 'C')
+		>>> laia1.add_interval(30, 40, 'D')
+		>>> laia1.add_interval(40, 50, 'E')
+
+		>>> laia2 = LabeledIntervalArray()
+		>>> laia2.add_interval(0, 10, 'A')
+		>>> laia2.add_interval(10, 20, 'B')
+
+		>>> laia1.common(laia2)
+		>>> LabeledIntervalArray
+		>>> 0-10: A
+		>>> 10-20: B
+
+		"""
+
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Check if other object is still open
+		if other_laia.is_closed:
 			raise NameError("LabeledIntervalArray object has been closed.")
 
 		# Check if objects are constructed
-		if self.is_constructed == False:
+		if self.is_constructed is False:
 			self.construct()
-		#if other_aiarray.is_constructed == False:
-			#other_aiarray.construct()
 
-		# Find matches
-		cdef np.ndarray has_match = self._has_exact_match(other_aiarray)
+		# Check if other objects are constructed
+		if other_laia.is_constructed is False:
+			other_laia.construct()
 
-		return has_match
+		cdef LabeledIntervalArray common_laia = LabeledIntervalArray()
+		cdef labeled_aiarray_t *claia = labeled_aiarray_common(self.laia, other_laia.laia)
+		common_laia.set_list(claia)
 
+		return common_laia
 
-	cdef int _index_with_aiarray(LabeledIntervalArray self, LabeledIntervalArray other_aiarray):
+
+	def union(LabeledIntervalArray self, LabeledIntervalArray other_laia):
 		"""
+		Finds the union of two LabeledIntervalArrays
+
+		Parameters
+		----------
+			other_laia : LabeledIntervalArray
+				LabeledIntervalArray to find union with
+
+		Returns
+		-------
+			union_laia : LabeledIntervalArray
+				LabeledIntervalArray with union
+
+		See Also
+		--------
+			LabeledIntervalArray.common
+			LabeledIntervalArray.subtract
+			LabeledIntervalArray.intersect
+
+		Notes
+		-----
+			- The union is returned as a new LabeledIntervalArray
+			- The union is not sorted
+
+		Examples
+		>>> laia1 = LabeledIntervalArray()
+		>>> laia1.add_interval(0, 10, 'A')
+		>>> laia1.add_interval(10, 20, 'B')
+		>>> laia1.add_interval(20, 30, 'C')
+		>>> laia1.add_interval(30, 40, 'D')
+		>>> laia1.add_interval(40, 50, 'E')
+
+		>>> laia2 = LabeledIntervalArray()
+		>>> laia2.add_interval(0, 10, 'A')
+		>>> laia2.add_interval(10, 20, 'B')
+
+		>>> laia1.union(laia2)
+		>>> LabeledIntervalArray
+		>>> 0-10: A
+		>>> 10-20: B
+		>>> 20-30: C
+		>>> 30-40: D
+		>>> 40-50: E
+
 		"""
 
-		# Iterate over ail
-		cdef int label_start
-		cdef int position_start
-		cdef int position_end
-
-		# Determine label indices
-		cdef int *label_index = <int *>malloc(other_aiarray.ail.nl * sizeof(int))
-		get_label_index_array(other_aiarray.ail, label_index)
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		cdef uint16_t label_code
-		cdef uint16_t other_label_code
+		# Check if other object is still open
+		if other_laia.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		cdef int i
-		for i in range(self.ail.nr):
-			# Set label codes
-			label_code = self.ail.interval_list[i].label
-			other_label_code = other_aiarray.label_map[self.rev_label_map[label_code]]
-
-			# Set ail1 start to start position in ail2
-			position_start = self.ail.interval_list[i].start
-			# Check position
-			if position_start < 0 or position_start >= other_aiarray.ail.nr:
-				return 1
-
-			label_start = label_index[other_label_code]
-			self.ail.interval_list[i].start = other_aiarray.ail.interval_list[label_start + position_start].start
-
-			# Set ail1 end to start position in ail2
-			position_end = self.ail.interval_list[i].end - 1
-			# Check position
-			if position_end < 0 or position_end >= other_aiarray.ail.nr:
-				return 1
-
-			self.ail.interval_list[i].end = other_aiarray.ail.interval_list[label_start + position_end].end
-
-
-			#print("i: %d, start: %d, end: %d, label: %d, label2: %d, label_start: %d\n", i, position_start, position_end, label_code, other_label_code, label_start)
-
-		# Change range
-		for i in range(self.ail.nl):
-			position_start = self.ail.first[i]
-			position_end = self.ail.last[i] - 1
-			label_start = label_index[i]
-			self.ail.first[i] = other_aiarray.ail.interval_list[label_start + position_start].start
-			self.ail.last[i] = other_aiarray.ail.interval_list[label_start + position_end].end - 1
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
 
-		free(label_index)
+		# Check if other objects are constructed
+		if other_laia.is_constructed is False:
+			other_laia.construct()
 
-		return 0
+		cdef LabeledIntervalArray union_laia = LabeledIntervalArray()
+		cdef labeled_aiarray_t *claia = labeled_aiarray_union(self.laia, other_laia.laia)
+		union_laia.set_list(claia)
 
+		return union_laia
 
-	def index_with_aiarray(self, LabeledIntervalArray other_aiarray):
+
+	def subtract(LabeledIntervalArray self, LabeledIntervalArray other_laia):
 		"""
+		Finds the subtraction of two LabeledIntervalArrays
+
+		Parameters
+		----------
+			other_laia : LabeledIntervalArray
+				LabeledIntervalArray to find subtraction with
+
+		Returns
+		-------
+			subtract_laia : LabeledIntervalArray
+				LabeledIntervalArray with subtraction
+
+		See Also
+		--------
+			LabeledIntervalArray.common
+			LabeledIntervalArray.union
+			LabeledIntervalArray.intersect
+
+		Notes
+		-----
+			- The subtraction is returned as a new LabeledIntervalArray
+			- The subtraction is not sorted
+
+		Examples
+		>>> laia1 = LabeledIntervalArray()
+		>>> laia1.add_interval(0, 10, 'A')
+		>>> laia1.add_interval(10, 20, 'B')
+		>>> laia1.add_interval(20, 30, 'C')
+
+		>>> laia2 = LabeledIntervalArray()
+		>>> laia2.add_interval(0, 10, 'A')
+		>>> laia2.add_interval(10, 20, 'B')
+
+		>>> laia1.subtract(laia2)
+		>>> LabeledIntervalArray
+		>>> 20-30: C
+
 		"""
 
-		return_code = self._index_with_aiarray(other_aiarray)
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		if return_code == 1:
-			raise NameError("Failed to run properly. Values are likely currupted now.")
+		# Check if other object is still open
+		if other_laia.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
 
-	cdef void _get_locs(LabeledIntervalArray self, uint8[::1] locs_view, char *label_names, int label_str_len, int n_labels):
+		# Check if other objects are constructed
+		if other_laia.is_constructed is False:
+			other_laia.construct()
+
+		cdef LabeledIntervalArray subtract_laia = LabeledIntervalArray()
+		cdef labeled_aiarray_t *claia = labeled_aiarray_subtract(self.laia, other_laia.laia)
+		subtract_laia.set_list(claia)
+
+		return subtract_laia
+
+
+	cdef np.ndarray _percent_coverage(LabeledIntervalArray self, LabeledIntervalArray other_laia):
+		# Initialize coverage
+		cdef double[::1] cov = np.zeros(self.size, dtype=np.double)
+
+		# Calculate percent coverage
+		labeled_aiarray_percent_coverage(self.laia, other_laia.laia, &cov[0])
+
+		return np.asarray(cov)
+
+	def percent_coverage(LabeledIntervalArray self, LabeledIntervalArray other_laia):
 		"""
+		Finds the percent coverage of two LabeledIntervalArrays
+
+		Parameters
+		----------
+			other_laia : LabeledIntervalArray
+				LabeledIntervalArray to find percent coverage with
+
+		Returns
+		-------
+			percent_coverage : float
+				Percent coverage of two LabeledIntervalArrays
+
+		See Also
+		--------
+			LabeledIntervalArray.common
+			LabeledIntervalArray.union
+			LabeledIntervalArray.intersect
+
+		Notes
+		-----
+			- The percent coverage is returned as a float
+			- The percent coverage is not sorted
+
+		Examples
+		>>> laia1 = LabeledIntervalArray()
+		>>> laia1.add_interval(0, 10, 'A')
+		>>> laia1.add_interval(10, 20, 'B')
+		>>> laia1.add_interval(20, 30, 'C')
+
+		>>> laia2 = LabeledIntervalArray()
+		>>> laia2.add_interval(0, 10, 'A')
+		>>> laia2.add_interval(10, 20, 'B')
+
+		>>> laia1.percent_coverage(laia2)
+		>>> [0.6666666666666666, 0.3333333333333333]
+
 		"""
 
-		get_label_array_presence(self.ail, &label_names[0], n_labels, &locs_view[0], label_str_len)
-	
-	def get_locs(self, labels):
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Check if other object is still open
+		if other_laia.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		# Check if objects are constructed
+		if self.is_constructed is False:
+			self.construct()
+
+		# Check if other objects are constructed
+		if other_laia.is_constructed is False:
+			other_laia.construct()
+
+		cdef np.ndarray percent_coverage = self._percent_coverage(other_laia)
+
+		return percent_coverage
+
+
+	def validate_construction(self):
 		"""
+		Validates the construction of the LabeledIntervalArray
+
+		Returns
+		-------
+			is_valid : bool
+				True if the LabeledIntervalArray is valid, False otherwise
 		"""
 
-		cdef np.ndarray locs = np.zeros(self.size, dtype=bool)
-		cdef uint8[::1] locs_view = np.frombuffer(locs, dtype=np.uint8)
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
 
-		# Check that labels are bytes
-		if isinstance(labels, np.ndarray) == False:
-			labels = np.array(labels)
-		byte_labels = labels.astype(bytes)
+		cdef int res = labeled_aiarray_validate_construction(self.laia)
 
-		# Intersect from array
-		self._get_locs(locs_view, np.PyArray_BYTES(byte_labels), byte_labels.itemsize, len(labels))
+		if res == 0:
+			return False
+		else:
+			return True
 
-		return locs
 
-	
 	def copy(self):
 		"""
 		Copy LabeledIntervalArray
+
+		Returns
+		-------
+			laia_copied : LabeledIntervalArray
+				Copied LabeledIntervalArray
+
+		Notes
+		-----
+			- The copy is not sorted
+
+		Examples
+		>>> laia1 = LabeledIntervalArray()
+		>>> laia1.add_interval(0, 10, 'A')
+		>>> laia1.add_interval(10, 20, 'B')
+
+		>>> laia2 = laia1.copy()
+		>>> laia2
+		>>> LabeledIntervalArray
+		>>> 0-10: A
+		>>> 10-20: B
+
 		"""
 
-		cdef LabeledIntervalArray ail_copied = LabeledIntervalArray()
-		cdef labeled_aiarray_t * c_ail_copied = labeled_aiarray_copy(self.ail)
-		ail_copied.set_list(c_ail_copied)
+		# Check if object is still open
+		if self.is_closed:
+			raise NameError("LabeledIntervalArray object has been closed.")
+
+		cdef LabeledIntervalArray laia_copied = LabeledIntervalArray()
+		cdef labeled_aiarray_t * c_laia_copied = labeled_aiarray_copy(self.laia)
+		laia_copied.set_list(c_laia_copied)
+
+		return laia_copied
 
-		return ail_copied
 
-	
 	def close(self):
 		"""
 		Close object and clear memory
 		"""
 
 		# Free labeled_interval_list memory
-		if self.ail:
-			labeled_aiarray_destroy(self.ail)
-		self.ail = NULL
-		
-		self.is_closed = True
+		if self.laia:
+			labeled_aiarray_destroy(self.laia)
+		self.laia = NULL
+
+		self.is_closed = True
```

### Comparing `ailist-1.0.4/ailist/__init__.py` & `ailist-2.0.2/ailist/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import absolute_import
-from .Interval_core import Interval, get_include
-from .LabeledInterval_core import LabeledInterval
 from .AIList_core import AIList
 from .IntervalArray_core import IntervalArray
-from .LabeledIntervalArray_core import LabeledIntervalArray
+from .Interval_core import Interval
+from .LabeledIntervalArray_core import LabeledIntervalArray, LabeledInterval, get_include
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '1.0.4'
+__version__ = '2.0.1'
 __author__ = "Kyle S. Smith"
 
 
 __doc__ = """\
 API
 ======
```

### Comparing `ailist-1.0.4/ailist/array_query_core.pxd` & `ailist-2.0.2/ailist/array_query_core.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 cimport numpy as np
 cimport cython
 from libc.stdint cimport uint32_t, int32_t, int64_t
 from libc.stdlib cimport malloc, free
 
 
-cdef extern from "src/array_query_utilities.c":
+cdef extern from "src/array_query/array_query_utilities.c":
 	# C is include here so that it doesn't need to be compiled externally
 	pass
 
-cdef extern from "src/array_query_utilities.h":
+cdef extern from "src/array_query/array_query_utilities.h":
 	# C is include here so that it doesn't need to be compiled externally
 	ctypedef struct array_query_t:
 		long *ref_index
 		long *query_index
 		int size
 		int max_size
```

### Comparing `ailist-1.0.4/ailist/array_query_core.pyx` & `ailist-2.0.2/ailist/array_query_core.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 #cython: embedsignature=True
 #cython: profile=False
 
 import os
 import sys
 import numpy as np
 cimport numpy as np
-import math
-cimport cython
-import pandas as pd
-from libc.string cimport memcpy
 np.import_array()
-from time import time
 
 # Set byteorder for __reduce__
 byteorder = sys.byteorder
 
 
 def get_include():
 	"""
@@ -61,13 +56,13 @@
 
 	# Create shape of ndarray
 	cdef np.npy_intp dims[1]
 	dims[0] = size
 
 	# Create ndarray from C pointer
 	cdef np.ndarray arr = np.PyArray_SimpleNewFromData(1, &dims[0], np.NPY_LONG, ptr)
-	
+
 	# Hand control of data freeing to numpy
 	PyArray_ENABLEFLAGS(arr, np.NPY_ARRAY_OWNDATA)
 	#np.PyArray_UpdateFlags(arr, arr.flags.num | np.NPY_OWNDATA)
 
 	return arr
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_add.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-void aiarray_add(aiarray_t *ail, uint32_t start, uint32_t end)
-{   /* Add interval to aiarray_t object */
+labeled_aiarray_t *labeled_aiarray_length_filter(labeled_aiarray_t *laia, int min_length, int max_length)
+{   /* Filter labeled_aiarray by length */
+    
+    // Initialize label_aiarray
+    labeled_aiarray_t *filtered_laia = labeled_aiarray_init();
 
-	// If start is greater than end, invalid interval
-    if (start > end) {return;}
+    // Iterate over labels
+    int32_t i;
+    for (i = 0; i < laia->n_labels; i++)
+    {
+        label_t *p1 = &laia->labels[i];
 
-    // Update first and last
-    ail->first = MIN(ail->first, start);
-    ail->last = MAX(ail->last, end);
-
-    // If max region reached, expand array
-	if (ail->nr == ail->mr)
-		EXPAND(ail->interval_list, ail->mr);
-
-    // Set new interval values
-	interval_t *i = &ail->interval_list[ail->nr++];
-	i->start = start;
-	i->end = end;
-    i->id_value = ail->nr - 1;
+        int32_t j;
+        for (j = 0; j < p1->ail->nr; j++)
+        {   
+            int length = p1->ail->interval_list[j].end - p1->ail->interval_list[j].start;
+            if (length > min_length && length < max_length)
+            {
+                labeled_aiarray_add(filtered_laia, p1->ail->interval_list[j].start, p1->ail->interval_list[j].end, p1->name);
+            }
+        }
+    }
 
-	return;
+    return filtered_laia;
 }
 
 
-void aiarray_from_array(aiarray_t *ail, const long starts[], const long ends[], int length)
-{   /* Build aiarray from arrays */
-    
-    // Iterate over itervals and add
-    int i;
-    for (i = 0; i < length; i++)
+labeled_aiarray_t *labeled_aiarray_downsample(labeled_aiarray_t *laia, double proportion)
+{   /* Randomly downsample */
+
+    // Initialize label_aiarray
+    labeled_aiarray_t *filtered_laia = labeled_aiarray_init();
+
+    // Iterate over labels
+    int32_t i;
+    for (i = 0; i < laia->n_labels; i++)
     {
-        aiarray_add(ail, starts[i], ends[i]);
+        label_t *p = &laia->labels[i];
+        ailist_t *filtered_ail = ailist_downsample(p->ail, proportion);
+        labeled_aiarray_wrap_ail(filtered_laia, filtered_ail, p->name);
     }
 
-    return;
+    return filtered_laia;
 }
 
 
-aiarray_t *aiarray_append(aiarray_t *ail1, aiarray_t *ail2)
-{   /* Append two aiarray */
-    
-    // Initialize appended aiarray
-    aiarray_t *appended_aiarray = aiarray_init();
-    
-    // Append ail1
-    int i;
-    for (i = 0; i < ail1->nr; i++)
-    {
-        aiarray_add(appended_aiarray, ail1->interval_list[i].start, ail1->interval_list[i].end);
-    }
+overlap_label_index_t *labeled_aiarray_downsample_with_index(labeled_aiarray_t *laia, double proportion)
+{   /* Randomly downsample */
+
+    // Initialize label_aiarray
+    overlap_label_index_t *filtered_oi = overlap_label_index_init();
 
-    // Append ail2
-    int j;
-    for (j = 0; j < ail2->nr; j++)
+    // Iterate over labels
+    int32_t i;
+    for (i = 0; i < laia->n_labels; i++)
     {
-        aiarray_add(appended_aiarray, ail2->interval_list[j].start, ail2->interval_list[j].end);
+        label_t *p = &laia->labels[i];
+        ailist_t *filtered_ail = ailist_downsample(p->ail, proportion);
+        overlap_label_index_wrap_ail(filtered_oi, filtered_ail, p->name);
     }
 
-    return appended_aiarray;
+    return filtered_oi;
 }
+
+
+//-----------------------------------------------------------------------------
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_construct.c` & `ailist-2.0.2/ailist/src/ailist/augmented_interval_list.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,130 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
+#include "augmented_interval_list.h"
 
-#include "augmented_interval_array.h"
+//-----------------------------------------------------------------------------
+
+ailist_t *ailist_init(void)
+{   /* Initialize ailist_t object */
+
+    // Initialize variables
+    ailist_t *ail = (ailist_t *)malloc(sizeof(ailist_t));
+    ail->nr = 0;
+    ail->mr = 64;
+    ail->first = INT32_MAX;
+    ail->last = 0;
+	ail->maxE = NULL;
+
+    // Initialize arrays
+    ail->interval_list = malloc(ail->mr * sizeof(interval_t));
+
+    // Check if memory was allocated
+    if (ail == NULL && ail->interval_list == NULL)
+    {
+        fprintf (stderr, "Out of memory!!! (init)\n");
+        exit(1);
+    }
+
+    // Assign values to NULL
+    int i;
+    for (i = 0; i < MAXC; i++)
+    {
+        ail->idxC[i] = 0;
+        ail->lenC[i] = 0;
+    }
 
-#define interval_t_key(r) ((r).start)
-KRADIX_SORT_INIT(intv, interval_t, interval_t_key, 4)
+	return ail;
+}
 
 //-----------------------------------------------------------------------------
 
+void ailist_destroy(ailist_t *ail)
+{   /* Free ailist_t object */
+
+    // Check that ail exists
+	if (ail == 0)
+    {
+        return;
+    }
+	
+    // Free intervals
+	free(ail->interval_list);
+	
+    // Free maxE
+	if (ail->maxE)
+	{
+		free(ail->maxE);
+	}
+
+    // Free ailist
+	free(ail);
+}
+
+//-------------------------------------------------------------------------------
 
-void aiarray_construct(aiarray_t *ail, int cLen)
-{   /* Construct aiarray_t object */  
+int ailist_max_length(ailist_t *ail)
+{   /* Calculate maximum length */
+	
+    // Iterate over intervals and record length
+    int length;
+    int maximum = 0;
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        // Record length (excluding last position)
+        length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
+	    maximum = MAX(maximum, length);
+    }
+
+    return maximum;
+}
 
-    int cLen1 = cLen / 2;
-    int j1, nr;
-    int minL = MAX(64, cLen);     
-    cLen += cLen1;      
-    int lenT, len, iter, j, k, k0, t;  
-
-    //1. Decomposition
-    interval_t *L1 = ail->interval_list;					//L1: to be rebuilt
-    nr = ail->nr;
-    //aiarray_sort(L1, nr);
-    radix_sort_intv(L1, L1+nr);
-
-    if (nr <= minL)
-    {        
-        ail->nc = 1;
-        ail->lenC[0] = nr;
-        ail->idxC[0] = 0;                
-    } else {         
-        interval_t *L0 = malloc(nr * sizeof(interval_t)); 	//L0: serve as input list
-        interval_t *L2 = malloc(nr * sizeof(interval_t));   //L2: extracted list 
-        memcpy(L0, L1, nr * sizeof(interval_t));			
-        iter = 0;
-        k = 0;
-        k0 = 0;
-        lenT = nr;
-
-        while (iter < MAXC && lenT > minL)
-        {   
-            len = 0;            
-            for (t = 0; t < lenT - cLen; t++)
-            {
-                uint32_t tt = L0[t].end;
-                j=1;
-                j1=1;
-
-                while (j < cLen && j1 < cLen1)
-                {
-                    if (L0[j + t].end >= tt) {j1++;}
-                    j++;
-                }
-                
-                if (j1 < cLen1)
-                {
-                    memcpy(&L2[len++], &L0[t], sizeof(interval_t));
-                } else {
-                    memcpy(&L1[k++], &L0[t], sizeof(interval_t));
-                }               
-            } 
-
-            memcpy(&L1[k], &L0[lenT - cLen], cLen * sizeof(interval_t));   
-            k += cLen;
-            lenT = len;               
-            ail->idxC[iter] = k0;
-            ail->lenC[iter] = k - k0;
-            k0 = k;
-            iter++;
-
-            if (lenT <= minL || iter == MAXC - 2)
-            {	//exit: add L2 to the end
-                if (lenT > 0)
-                {
-                    memcpy(&L1[k], L2, lenT * sizeof(interval_t));
-                    ail->idxC[iter] = k;
-                    ail->lenC[iter] = lenT;
-                    iter++;
-                }
-                ail->nc = iter;                   
-            } else {
-                memcpy(L0, L2, lenT * sizeof(interval_t));
-            }
-        }
-        free(L2);
-        free(L0);     
-    }
-
-    //2. Augmentation
-    ail->maxE = malloc(nr * sizeof(uint32_t)); 
-    for (j = 0; j < ail->nc; j++)
-    { 
-        k0 = ail->idxC[j];
-        k = k0 + ail->lenC[j];
-        uint32_t tt = L1[k0].end;
-        ail->maxE[k0] = tt;
-
-        for (t = k0 + 1; t < k; t++)
-        {
-            if (L1[t].end > tt)
-            {
-                tt = L1[t].end;
-            }
 
-            ail->maxE[t] = tt;  
-        }             
+void ailist_length_distribution(ailist_t *ail, int distribution[])
+{   /* Calculate length distribution */
+    
+    // Iterate over intervals and record length
+    int length;
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        // Record length (excluding last position)
+        length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
+        distribution[length] += 1;
     }
 
     return;
 }
 
 
+void display_list(ailist_t *ail)
+{
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        printf("(%d-%d) ", ail->interval_list[i].start, ail->interval_list[i].end);
+    }
+    printf("\n");
+    return;
+}
+
+
+/* Driver program to test above functions*/
+//int main(void)
+//{ 
+    
+//    int x = 0;
+//    int *y;
+//    y = &x;
+
+//    x = 3;
+//    *y = 4;
+
+//    printf("x: %d\n", x);
+//    printf("y: %d\n", *y);
+    
+//    return 0;
+//}
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_coverage.c` & `ailist-2.0.2/ailist/src/ailist/ailist_wps.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,102 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
-void aiarray_interval_coverage(aiarray_t *ail, int start, int end, int coverage[])
-{   /* Determine coverage for an interval */
-    
-    // Query overlaps
-    aiarray_t *overlaps = aiarray_query(ail, start, end);
-
-    // Iterate over overlaps
-    int j;
-    for (j = 0; j < overlaps->nr; j++)
-    {
-        int overlap_start = MAX(start, (int)overlaps->interval_list[j].start);
-        int overlap_end = MIN(end, (int)overlaps->interval_list[j].end);
-
-        // Iterate over overlapping postions
-        int k;
-        for (k = overlap_start; k < overlap_end; k++)
-        {
-            coverage[k - start] += 1;
-        }
-    }
-
-    return;
-}
+void ailist_wps(ailist_t *ail, double wps[], uint32_t protection)
+{   /* Calculate Window Protection Score */
+    int half_window = protection / 2;
+    int first = (int)ail->first;
 
-
-void aiarray_coverage(aiarray_t *ail, double coverage[])
-{   /* Calculate coverage */
-    int length;
-    int n;
+    // Iterate over regions
     int i;
-    int position;
-    int start = (int)ail->first;
-
     for (i = 0; i < ail->nr; i++)
     {
-        length = ail->interval_list[i].end - ail->interval_list[i].start;
-        for (n = 0; n < length; n++)
+        // Find regions around end points
+        int head_start = MAX(first, (int)(ail->interval_list[i].start - half_window));
+        int head_end = MIN((int)ail->interval_list[i].start + half_window, (int)ail->interval_list[i].end);
+        int tail_start = MAX(head_end, (int)(ail->interval_list[i].end - half_window)); // if overlap, set not to overlap
+        int tail_end = MIN((int)ail->interval_list[i].end + half_window, (int)ail->last);
+
+        // Decrement region around head
+        int head_length = head_end - head_start;
+        int j;
+        for (j = (head_start - first); j < (head_length + (head_start - first)); j++)
         {
-            position = (ail->interval_list[i].start - start) + n;
-            coverage[position] = coverage[position] + 1;
+            wps[j] = wps[j] - 1;
         }
-    }
-
-    return;
-}
 
+        // Decrement region around tail
+        int tail_length = tail_end - tail_start;
+        for (j = (tail_start - first); j < (tail_length + (tail_start - first)); j++)
+        {
+            wps[j] = wps[j] - 1;
+        }
 
-void aiarray_bin_coverage(aiarray_t *ail, double coverage[], int bin_size)
-{   /* Calculate coverage within bins */
-    int start = (int)(ail->first / bin_size);
-    
-    int i;
-    for (i = 0; i < ail->nr; i++)
-    {
-        int start_bin = ail->interval_list[i].start / bin_size;
-        
-        double length = (double)(ail->interval_list[i].end - ail->interval_list[i].start);
-        int n_bins = ceil(((double)(ail->interval_list[i].start % bin_size) / bin_size) + (length / bin_size));
-        int n;
-        for (n = 0; n < n_bins; n++)
+        // If head and tail region don't overlap
+        if (head_end != tail_start)
         {
-            int bin = (start_bin - start) + n;
-            int bin_start_position = ((start_bin + n) * bin_size);
-            int i_start_position = MAX(bin_start_position, (int)ail->interval_list[i].start);
-            int i_end_position = MIN((bin_start_position + bin_size), (int)ail->interval_list[i].end);
-            int coverage_value = i_end_position - i_start_position;
-            coverage[bin] = coverage[bin] + coverage_value;
+            for (j = (head_end - first); j < (tail_start - first); j++)
+            {
+                wps[j] = wps[j] + 1;
+            }
         }
     }
 
     return;
 }
 
 
-void aiarray_bin_coverage_length(aiarray_t *ail, double coverage[], int bin_size, int min_length, int max_length)
-{   /* Calculate coverage within bins of a length */
-    int start = (int)(ail->first / bin_size);
-    
+void ailist_wps_length(ailist_t *ail, double wps[], uint32_t protection, int min_length, int max_length)
+{   /* Calculate Window Protection Score */
+    int half_window = protection / 2;
+    int first = (int)ail->first;
+
+    // Iterate over regions
     int i;
     for (i = 0; i < ail->nr; i++)
-    {
-        int start_bin = ail->interval_list[i].start / bin_size;
-        
-        double length = (double)(ail->interval_list[i].end - ail->interval_list[i].start);
+    {   
+        // Check if length is in range
+        int length = ail->interval_list[i].end - ail->interval_list[i].start;
         if (length >= min_length && length < max_length)
         {
-            int n_bins = ceil(((double)(ail->interval_list[i].start % bin_size) / bin_size) + (length / bin_size));
-            int n;
-            for (n = 0; n < n_bins; n++)
+            // Find regions around end points
+            int head_start = MAX(first, (int)(ail->interval_list[i].start - half_window));
+            int head_end = MIN((int)ail->interval_list[i].start + half_window, (int)ail->interval_list[i].end);
+            int tail_start = MAX(head_end, (int)(ail->interval_list[i].end - half_window)); // if overlap, set not to overlap
+            int tail_end = MIN((int)ail->interval_list[i].end + half_window, (int)ail->last);
+
+            // Decrement region around head
+            int head_length = head_end - head_start;
+            int j;
+            for (j = (head_start - first); j < (head_length + (head_start - first)); j++)
+            {
+                wps[j] = wps[j] - 1;
+            }
+
+            // Decrement region around tail
+            int tail_length = tail_end - tail_start;
+            for (j = (tail_start - first); j < (tail_length + (tail_start - first)); j++)
+            {
+                wps[j] = wps[j] - 1;
+            }
+
+            // If head and tail region don't overlap
+            if (head_end != tail_start)
             {
-                int bin = (start_bin - start) + n;
-                int bin_start_position = ((start_bin + n) * bin_size);
-                int i_start_position = MAX(bin_start_position, (int)ail->interval_list[i].start);
-                int i_end_position = MIN((bin_start_position + bin_size), (int)ail->interval_list[i].end);
-                int coverage_value = i_end_position - i_start_position;
-                coverage[bin] = coverage[bin] + coverage_value;
+                for (j = (head_end - first); j < (tail_start - first); j++)
+                {
+                    wps[j] = wps[j] + 1;
+                }
             }
         }
     }
 
     return;
 }
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_filter.c` & `ailist-2.0.2/ailist/src/ailist/ailist_nhits.c`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
-aiarray_t *aiarray_length_filter(aiarray_t *ail, int min_length, int max_length)
-{   /* Filter aiarray by length */
-    
-    // Initiatize filtered aiarray
-    aiarray_t *filtered_ail = aiarray_init();
-
-    // Iterate over intervals and filter
-    int length;
+void ailist_nhits_from_array(ailist_t *ail, const long starts[], const long ends[], int length, int nhits[])
+{
     int i;
-    for (i = 0; i < ail->nr; i++)
+    for (i = 0; i < length; i++)
     {
-        // Record length (excluding last position)
-        length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
-        if (length >= min_length && length <= max_length)
-        {
-            aiarray_add(filtered_ail, ail->interval_list[i].start, ail->interval_list[i].end);
-        }
+        ailist_t *overlaps = ailist_init();
+        ailist_query(ail, overlaps, starts[i], ends[i]);
+        nhits[i] = overlaps->nr;
     }
 
-    return filtered_ail;
+    return;
 }
 
 
-aiarray_t *aiarray_downsample(aiarray_t *ail, double proportion)
-{   /* Randomly downsample */
+void ailist_nhits_from_array_length(ailist_t *ail, const long starts[], const long ends[], int length, int nhits[], int min_length, int max_length)
+{
+    int i;
+    for (i = 0; i < length; i++)
+    {
+        ailist_t *overlaps = ailist_init();
+        ailist_query_length(ail, overlaps, starts[i], ends[i], min_length, max_length);
+        nhits[i] = overlaps->nr;
+    }
 
-    // Initialize downsampled aiarray_t
-    aiarray_t *filtered_ail = aiarray_init();
+    return;
+}
 
-    // Set random seed
-	srand(time(NULL));
 
-    // Iterate over ail
+void ailist_bin_nhits(ailist_t *ail, long coverage[], int bin_size)
+{   /* Calculate n hits within bins */
+    int start = (int)(ail->first / bin_size);
+    //printf("   start: %d\n", start);
+    
     int i;
     for (i = 0; i < ail->nr; i++)
     {
-        // Randomly determine if interval is added
-        double r = (double)rand() / (double)RAND_MAX;
-        if (r < proportion)
+        int start_bin = ail->interval_list[i].start / bin_size;
+        
+        double length = (double)(ail->interval_list[i].end - ail->interval_list[i].start);
+        int n_bins = ceil(((double)(ail->interval_list[i].start % bin_size) / bin_size) + (length / bin_size));
+        //printf("    interval length: %f covers %d bins\n", length, n_bins);
+        int n;
+        for (n = 0; n < n_bins; n++)
         {
-            aiarray_add(filtered_ail, ail->interval_list[i].start, ail->interval_list[i].end);
+            int bin = (start_bin - start) + n;
+            //printf("      putiting in bin : %d\n", bin);
+            coverage[bin] = coverage[bin] + 1;
         }
     }
 
-    return filtered_ail;
+    return;
 }
 
 
-overlap_index_t *aiarray_downsample_with_index(aiarray_t *ail, double proportion)
-{   /* Randomly downsample with original index */
-
-    // Initialize downsampled aiarray_t
-    overlap_index_t *filtered_ail = overlap_index_init();
-
-    // Set random seed
-	srand(time(NULL));
-
-    // Iterate over ail
+void ailist_bin_nhits_length(ailist_t *ail, long coverage[], int bin_size, int min_length, int max_length)
+{   /* Calculate n hits of a length within bins */
+    int start = (int)(ail->first / bin_size);
+    
     int i;
     for (i = 0; i < ail->nr; i++)
     {
-        // Randomly determine if interval is added
-        double r = (double)rand() / (double)RAND_MAX;
-        if (r < proportion)
+        int start_bin = ail->interval_list[i].start / bin_size;
+        
+        double length = (double)(ail->interval_list[i].end - ail->interval_list[i].start);
+        if (length >= min_length && length < max_length)
         {
-            overlap_index_add(filtered_ail, &ail->interval_list[i]);
+            int n_bins = ceil(((double)(ail->interval_list[i].start % bin_size) / bin_size) + (length / bin_size));
+            int n;
+            for (n = 0; n < n_bins; n++)
+            {
+                int bin = (start_bin - start) + n;
+                coverage[bin] = coverage[bin] + 1;
+            }
         }
     }
 
-    return filtered_ail;
+    return;
 }
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_merge.c` & `ailist-2.0.2/ailist/src/ailist/ailist_iter.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,138 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
 
-int *get_comp_bounds(aiarray_t *ail)
+int *get_comp_bounds(ailist_t *ail)
 {   /* Get component index */
 
-    //int label_start = ail->label_index[label];
-    int *idxC = ail->idxC;
-    int n_comps = ail->nc;
-    int *comps_bounds = malloc((n_comps + 1) * sizeof(int));
+    int *idxC = &ail->idxC[0];
+    int *comps_bounds = (int *)malloc((ail->nc + 1) * sizeof(int));
     int i;
-    for (i = 0; i < n_comps; i++)
+    for (i = 0; i < ail->nc; i++)
     {
         comps_bounds[i] = idxC[i];
     }
 
-    comps_bounds[n_comps] = ail->nr;
+    comps_bounds[ail->nc] = ail->nr;
 
     return comps_bounds;
 }
 
 
-aiarray_t *aiarray_merge(aiarray_t *ail, uint32_t gap)
-{   /* Merge nearby intervals */
+ailist_sorted_iter_t *ailist_sorted_iter_init(ailist_t *ail)
+{
 
-    // Initialize merged atrributes
-    int previous_end = ail->interval_list[0].end;
-    int previous_start = ail->interval_list[0].start;
-    int previous_id = ail->interval_list[0].id_value;
-    aiarray_t *merged_list = aiarray_init();
-    
-    // Determine label component bounds
-    int *comp_bounds = get_comp_bounds(ail);
-    int nc = ail->nc;
-
-    // Record number used per component
-    int *comp_used = malloc(nc+1 * sizeof(int));
-    memcpy(&comp_used, &comp_bounds, sizeof(int));
-
-    // Determine label bounds
-    //int label_start = ail->label_index[label];
-    //int label_end = ail->label_index[label + 1];
-    
-    // Iterate over component intervals
-    interval_t *intv = &ail->interval_list[0];
+    // Initialize variables
+    ailist_sorted_iter_t *iter = (ailist_sorted_iter_t *)malloc(sizeof(ailist_sorted_iter_t));
+    iter->ail = ail;
+    iter->comp_bounds = get_comp_bounds(ail);
+    iter->nc = ail->nc;
+    iter->comp_used = (int *)malloc((iter->nc + 1) * sizeof(int));
+    int i;
+    for (i = 0; i < iter->nc + 1; i++)
+    {
+        iter->comp_used[i] = iter->comp_bounds[i];
+    }
+    //memcpy(&iter->comp_used, &iter->comp_bounds, sizeof(int));
+    iter->intv = &ail->interval_list[0];
+    iter->n = -1;
+
+    return iter;
+}
+
+
+int ailist_sorted_iter_next(ailist_sorted_iter_t *iter)
+{
+    // Increment position
+    iter->n++;
+    if (iter->n >= iter->ail->nr)
+    {
+        return 0;
+    }
+
+    int selected_comp = 0;
+    // Iterate over other components
     int position;
-    int n;
-    for (n = 0; n < ail->nr; n++)
+    // Iterate over components
+    int j;
+    for (j = 0; j < iter->nc; j++)
     {
-        int selected_comp = 0;
-        // Iterate over other components
-        int j;
-        for (j = 0; j < nc; j++)
+        // If position is available, assign next interval
+        if (iter->comp_used[j] != iter->comp_bounds[j + 1])
         {
-            // Check component has intervals left to investigate
-            if (comp_used[j] == comp_bounds[j + 1])
-            {
-                continue;
-            }
-
-            // Determine position
-            position = comp_used[j];
-            // Check for lower start
-            if (ail->interval_list[position].start < intv->start)
-            {
-                intv = &ail->interval_list[position];
-                selected_comp = j;
-            }
+            position = iter->comp_used[j];
+            iter->intv = &iter->ail->interval_list[position];
+            break;
         }
+    }
 
-        // Sorted interval found
-        //printf("(%d-%d, %d); (%d-%d, %d)\n", intv->start, intv->end, intv->label, previous_start, previous_end, previous_label);
-        //printf("[%d, %d, %d]\n", label_comp_used[0], label_comp_used[1], label_comp_used[2]);
-        // If previous
-        if (previous_end > (int)(intv->start - gap))
-        {
-            previous_end = MAX(previous_end, (int)intv->end);
-        }
-        else
+    for (j = 0; j < iter->nc; j++)
+    {
+        // Check component has intervals left to investigate
+        if (iter->comp_used[j] == iter->comp_bounds[j + 1])
         {
-            aiarray_add(merged_list, previous_start, previous_end);
-            previous_start = intv->start;
-            previous_end = intv->end;
-            previous_id = intv->id_value;
+            continue;
         }
 
-        // Increment comp_counter for selected comp
-        comp_used[selected_comp] = comp_used[selected_comp] + 1;
-        // Iterate over components
-        for (j = 0; j < nc; j++)
+        // Determine position
+        position = iter->comp_used[j];
+        // Check for lower start
+        if (iter->ail->interval_list[position].start < iter->intv->start)
         {
-            // If position is available, assign next interval
-            if (comp_used[j] != comp_bounds[j + 1])
-            {
-                position = comp_used[j];
-                intv = &ail->interval_list[position];
-                break;
-            }
+            iter->intv = &iter->ail->interval_list[position];
+            selected_comp = j;
         }
 
-        // Free
-        //free(comp_bounds);
-        //free(label_comp_used);
+        // Increment label_comp_counter for selected comp
+        iter->comp_used[selected_comp] = iter->comp_used[selected_comp] + 1;
+    }
+
+    return 1;
+}
+
+
+void ailist_sorted_iter_destroy(ailist_sorted_iter_t *iter)
+{
+    // Check that ail exists
+	if (iter == 0)
+    {
+        return;
     }
 
-    // Add last interval
-    aiarray_add(merged_list, previous_start, previous_end);
+    // Free ail
+	//if (iter->ail)
+	//{
+        //free(iter->ail);
+    //}
+
+    // Free intv
+	//if (iter->intv)
+	//{
+        //free(iter->intv);
+    //}
+    
+    // Free label_comp_bounds
+	//if (iter->label_comp_bounds)
+	//{
+        //free(iter->label_comp_bounds);
+    //}
+
+    // Free label_comp_used
+	//if (iter->label_comp_used)
+	//{
+        //free(iter->label_comp_used);
+    //}
+
+    free(iter);
 
-    return merged_list;
+    return;
 }
 
+//-----------------------------------------------------------------------------
```

### Comparing `ailist-1.0.4/ailist/src/aiarray_query.c` & `ailist-2.0.2/ailist/src/ailist/ailist_construct.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,264 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
-uint32_t binary_search(interval_t* As, uint32_t idxS, uint32_t idxE, uint32_t qe)
-{   /* Find tE: index of the first item satisfying .s<qe from right */
-    
-    int tL = idxS;
-    int tR = idxE - 1;
-    int tM;
-    int tE = -1;
-    
-    if(As[tR].start < qe)
-    {
-        return tR;
-    } else if (As[tL].start >= qe) {
-        return -1;
-    }
-
-    while (tL < tR - 1)
-    {
-        tM = (tL + tR) / 2; 
-
-        if (As[tM].start >= qe)
-        {
-            tR = tM - 1;
-        } else {
-            tL = tM;
-        }
-    }
-
-    if (As[tR].start < qe)
-    {
-        tE = tR;
-    } else if (As[tL].start < qe) {
-        tE = tL;
-    }
-
-    return tE; 
-}
+#define interval_t_key(r) ((r).start)
+KRADIX_SORT_INIT(intv, interval_t, interval_t_key, 4)
 
 //-----------------------------------------------------------------------------
 
-aiarray_t *aiarray_query(aiarray_t *ail, uint32_t qs, uint32_t qe)
-{   
-    // Initialize overlaps
-    int k;
-    aiarray_t *overlaps = aiarray_init();
+void ailist_construct(ailist_t *ail, int cLen)
+{   /* Construct ailist_t object */  
 
-    for (k = 0; k < ail->nc; k++)
-    {   // Search each component
-        int32_t cs = ail->idxC[k];
-        int32_t ce = cs + ail->lenC[k];			
-        int32_t t;
-
-        if (ail->lenC[k] > 15)
-        {
-            t = binary_search(ail->interval_list, cs, ce, qe);
-
-            while (t >= cs && ail->maxE[t] > qs)
+    int cLen1 = cLen / 2;
+    int j1, nr;
+    int minL = MAX(64, cLen);     
+    cLen += cLen1;      
+    int lenT, len, iter, j, k, k0, t;  
+
+    //1. Decomposition
+    interval_t *L1 = ail->interval_list;					//L1: to be rebuilt
+    nr = ail->nr;
+    //ailist_sort(L1);
+    radix_sort_intv(L1, L1+nr);
+
+    if (nr <= minL)
+    {        
+        ail->nc = 1;
+        ail->lenC[0] = nr;
+        ail->idxC[0] = 0;                
+    } else {         
+        interval_t *L0 = malloc(nr * sizeof(interval_t)); 	//L0: serve as input list
+        interval_t *L2 = malloc(nr * sizeof(interval_t));   //L2: extracted list 
+        memcpy(L0, L1, nr * sizeof(interval_t));			
+        iter = 0;
+        k = 0;
+        k0 = 0;
+        lenT = nr;
+
+        while (iter < MAXC && lenT > minL)
+        {   
+            len = 0;            
+            for (t = 0; t < lenT - cLen; t++)
             {
-                if (ail->interval_list[t].end > qs)
-                {               	
-                    aiarray_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end);
+                uint32_t tt = L0[t].end;
+                j=1;
+                j1=1;
+
+                while (j < cLen && j1 < cLen1)
+                {
+                    if (L0[j + t].end >= tt) {j1++;}
+                    j++;
                 }
+                
+                if (j1 < cLen1)
+                {
+                    memcpy(&L2[len++], &L0[t], sizeof(interval_t));
+                } else {
+                    memcpy(&L1[k++], &L0[t], sizeof(interval_t));
+                }               
+            } 
 
-                t--;
-            }
-        } 
-        else {
-            for (t = cs; t < ce; t++)
-            {
-                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+            memcpy(&L1[k], &L0[lenT - cLen], cLen * sizeof(interval_t));   
+            k += cLen;
+            lenT = len;               
+            ail->idxC[iter] = k0;
+            ail->lenC[iter] = k - k0;
+            k0 = k;
+            iter++;
+
+            if (lenT <= minL || iter == MAXC - 2)
+            {	//exit: add L2 to the end
+                if (lenT > 0)
                 {
-                    aiarray_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end);
+                    memcpy(&L1[k], L2, lenT * sizeof(interval_t));
+                    ail->idxC[iter] = k;
+                    ail->lenC[iter] = lenT;
+                    iter++;
                 }
-            }                      
+                ail->nc = iter;                   
+            } else {
+                memcpy(L0, L2, lenT * sizeof(interval_t));
+            }
         }
+        free(L2);
+        free(L0);     
     }
 
-    return overlaps;                            
-}
+    //2. Augmentation
+    ail->maxE = malloc(nr * sizeof(uint32_t)); 
+    for (j = 0; j < ail->nc; j++)
+    { 
+        k0 = ail->idxC[j];
+        k = k0 + ail->lenC[j];
+        uint32_t tt = L1[k0].end;
+        ail->maxE[k0] = tt;
 
-
-aiarray_t *aiarray_query_length(aiarray_t *ail, uint32_t qs, uint32_t qe, int min_length, int max_length)
-{   
-    // Initialize overlaps
-    int k;
-    aiarray_t *overlaps = aiarray_init();
-
-    for (k = 0; k < ail->nc; k++)
-    {   // Search each component
-        int32_t cs = ail->idxC[k];
-        int32_t ce = cs + ail->lenC[k];			
-        int32_t t;
-
-        if (ail->lenC[k] > 15)
+        for (t = k0 + 1; t < k; t++)
         {
-            t = binary_search(ail->interval_list, cs, ce, qe);
-
-            while (t >= cs && ail->maxE[t] > qs)
+            if (L1[t].end > tt)
             {
-                if (ail->interval_list[t].end > qs)
-                {               	
-                    int length = ail->interval_list[t].end - ail->interval_list[t].start;
-                    if (length >= min_length && length < max_length)
-                    {
-                        aiarray_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end);
-                    }
-                }
-
-                t--;
+                tt = L1[t].end;
             }
-        } 
-        else {
-            for (t = cs; t < ce; t++)
-            {
-                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
-                {
-                    int length = ail->interval_list[t].end - ail->interval_list[t].start;
-                    if (length >= min_length && length < max_length)
-                    {
-                        aiarray_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end);
-                    }
-                }
-            }                      
-        }
+
+            ail->maxE[t] = tt;  
+        }             
     }
 
-    return overlaps;                            
+    return;
 }
 
 
-array_query_t *aiarray_query_from_array(aiarray_t *ail, const long starts[], const long ends[], int length)
-{   /* Find overlaps from array */
-    
-    // Initialize overlaps
-    int k;
-    array_query_t *aq = array_query_init();
 
-    // Iterate over queries
-    int i;
-    for (i = 0; i < length; i++)
-    {
-        uint32_t qs = starts[i];
-        uint32_t qe = ends[i];
 
-        for (k = 0; k < ail->nc; k++)
-        {   // Search each component
-            int32_t cs = ail->idxC[k];
-            int32_t ce = cs + ail->lenC[k];			
-            int32_t t;
+void ailist_construct_v0(ailist_t *ail, int cLen)
+{   /* Construct ailist: decomposition and augmentation */
 
-            if (ail->lenC[k] > 15)
-            {
-                t = binary_search(ail->interval_list, cs, ce, qe);
+    int cLen1 = cLen / 2;
+    int nr;
+    int minL = MAX(64, cLen);     
+    cLen += cLen1;      
+    int lenT;
+    int len;
+    int iter;
+    int j;
+    int k;
+    int k0;
+    int t;
 
-                while (t >= cs && ail->maxE[t] > qs)
+    //1. Decomposition
+    interval_t *L1 = ail->interval_list;			//L1: to be rebuilt
+    nr = ail->nr;
+    radix_sort_intv(L1, L1+nr);
+
+    if (nr <= minL)
+    {        
+        ail->nc = 1;
+        ail->lenC[0] = nr;
+        ail->idxC[0] = 0;                
+    } else {         
+        interval_t *L0 = malloc(nr * sizeof(interval_t)); 	//L0: serve as input list
+        interval_t *L2 = malloc(nr * sizeof(interval_t));   //L2: extracted list 
+        //----------------------------------------
+        interval_t *D0 = malloc(nr * sizeof(interval_t)); 	//D0:            
+        int32_t *di = malloc(nr * sizeof(int32_t));	//int64_t?			  
+        //----------------------------------------
+        memcpy(L0, L1, nr*sizeof(interval_t));			
+        iter = 0;
+        k = 0;
+        k0 = 0;
+        lenT = nr;
+        while (iter < MAXC && lenT > minL)
+        {  
+            //setup di---------------------------			
+            for (j = 0; j < lenT; j++)          //L0:{.start= end, .end=idx, .value=idx1}
+            {
+                D0[j].start = L0[j].end;
+                D0[j].end = j;
+            }
+            radix_sort_intv(D0, D0+lenT);
+            
+            for (j = 0; j < lenT; j++)          //assign i=29 to L0[i].end=2
+            {
+                t = D0[j].end;
+                di[t] = j-t;					//>0 indicate containment
+            }  
+            //----------------------------------- 
+            len = 0;
+            for (t = 0; t < lenT - cLen; t++) 
+            {
+                if (di[t] > cLen)
                 {
-                    if (ail->interval_list[t].end > qs)
-                    {               	
-                        array_query_add(aq, i, ail->interval_list[t].id_value);
-                    }
-
-                    t--;
+                    memcpy(&L2[len++], &L0[t], sizeof(interval_t));    			
+                } else {
+                    memcpy(&L1[k++], &L0[t], sizeof(interval_t));
                 }
-            } 
-            else {
-                for (t = cs; t < ce; t++)
+            }             
+            memcpy(&L1[k], &L0[lenT-cLen], cLen*sizeof(interval_t));   
+            k += cLen;
+            lenT = len;                
+            ail->idxC[iter] = k0;
+            ail->lenC[iter] = k - k0;
+            k0 = k;
+            iter++;
+            
+            if (lenT <= minL || iter == MAXC-2)     //exit: add L2 to the end
+            {
+                if (lenT > 0)
                 {
-                    if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
-                    {
-                        array_query_add(aq, i, ail->interval_list[t].id_value);
-                    }
-                }                      
+                    memcpy(&L1[k], L2, lenT*sizeof(interval_t));
+                    ail->idxC[iter] = k;
+                    ail->lenC[iter] = lenT;
+                    iter++;
+                    lenT = 0;						//exit!
+                }
+                ail->nc = iter;                   
+            } else {
+                memcpy(L0, L2, lenT*sizeof(interval_t));
             }
         }
-    }
-
-    // reallocate to remove extra memory
-    aq->ref_index = (long *)realloc(aq->ref_index, sizeof(long) * aq->size);
-    aq->query_index = (long *)realloc(aq->query_index, sizeof(long) * aq->size);
-    aq->max_size = aq->size;
-
-    return aq;                            
-}
 
+        free(L2);
+        free(L0);
+        free(D0);
+        free(di);   
+    }
 
-array_query_t *aiarray_query_from_aiarray(aiarray_t *ail, aiarray_t *ail2)
-{   /* Find overlaps from aiarray */
-    int k;
+    //2. Augmentation
+    ail->maxE = malloc(nr * sizeof(uint32_t)); 
 
-    array_query_t *aq = array_query_init();
+    for (j = 0; j < ail->nc; j++)
+    { 
+        k0 = ail->idxC[j];
+        k = k0 + ail->lenC[j];
+        uint32_t tt = L1[k0].end;
+        ail->maxE[k0]=tt;
 
-    // Iterate over queries
-    int i;
-    for (i = 0; i < ail2->nr; i++)
-    {
-        uint32_t qs = ail2->interval_list[i].start;
-        uint32_t qe = ail2->interval_list[i].end;
-        uint32_t id = ail2->interval_list[i].id_value;
-
-        for (k = 0; k < ail->nc; k++)
-        {   // Search each component
-            int32_t cs = ail->idxC[k];
-            int32_t ce = cs + ail->lenC[k];			
-            int32_t t;
-
-            if (ail->lenC[k] > 15)
+        for (t = k0+1; t < k; t++)
+        {
+            if (L1[t].end > tt)
             {
-                t = binary_search(ail->interval_list, cs, ce, qe);
-
-                while (t >= cs && ail->maxE[t] > qs)
-                {
-                    if (ail->interval_list[t].end > qs)
-                    {               	
-                        array_query_add(aq, id, ail->interval_list[t].id_value);
-                    }
-
-                    t--;
-                }
-            } 
-            else {
-                for (t = cs; t < ce; t++)
-                {
-                    if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
-                    {
-                        array_query_add(aq, id, ail->interval_list[t].id_value);
-                    }
-                }                      
+                tt = L1[t].end;
             }
-        }
-    }
 
-    // reallocate to remove extra memory
-    aq->ref_index = (long *)realloc(aq->ref_index, sizeof(long) * aq->size);
-    aq->query_index = (long *)realloc(aq->query_index, sizeof(long) * aq->size);
-    aq->max_size = aq->size;
+            ail->maxE[t] = tt;  
+        }             
+    } 
 
-    return aq;                           
+    return;
 }
 
 
-overlap_index_t *aiarray_query_with_index(aiarray_t *ail, uint32_t qs, uint32_t qe)
-{   /* Query aiarray intervals and record original index */
-
-    // Initialize overlaps
-    int k;
-    overlap_index_t *overlaps = overlap_index_init();
-
-    for (k = 0; k < ail->nc; k++)
-    {   // Search each component
-        int32_t cs = ail->idxC[k];
-        int32_t ce = cs + ail->lenC[k];			
-        int32_t t;
-
-        if (ail->lenC[k] > 15)
+int ailist_validate_construction(ailist_t *ail)
+{   /* Validation that construction ran */
+    
+    if (ail->maxE != NULL)
+    {
+        int lenC_sum = 0;
+        int idxC_sum = 0;
+        int i;
+        for (i = 0; i < MAXC; i++)
         {
-            t = binary_search(ail->interval_list, cs, ce, qe);
-
-            while (t >= cs && ail->maxE[t] > qs)
+            lenC_sum = lenC_sum + ail->lenC[i];
+            idxC_sum = idxC_sum + ail->idxC[i];
+        }
+        
+        if (ail->nc > 1)
+        {
+            if (lenC_sum > 0 && idxC_sum > 0)
             {
-                if (ail->interval_list[t].end > qs)
-                {               	
-                    overlap_index_add(overlaps, &ail->interval_list[t]);
-                }
-
-                t--;
+                return 1;
             }
-        } 
-        else {
-            for (t = cs; t < ce; t++)
-            {
-                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
-                {
-                    overlap_index_add(overlaps, &ail->interval_list[t]);
-                }
-            }                      
+        } else {
+            return 1;
         }
     }
 
-    // reallocate to remove extra memory
-    overlaps->indices = (long *)realloc(overlaps->indices, sizeof(long) * overlaps->size);
-    overlaps->max_size = overlaps->size;
-
-    return overlaps;                            
+    return 0;
 }
```

### Comparing `ailist-1.0.4/ailist/src/ailist_add.c` & `ailist-2.0.2/ailist/src/ailist/ailist_add.c`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 //-----------------------------------------------------------------------------
 
 void ailist_add(ailist_t *ail, uint32_t start, uint32_t end, uint32_t id)
 {   /* Add interval to ailist_t object */
 
 	// If start is greater than end, invalid interval
     if (start > end)
-        {return;}
+    {
+        return;
+    }
 
     // Update first and last
     ail->first = MIN(ail->first, start);
     ail->last = MAX(ail->last, end);
 
     // If max region reached, expand array
 	if (ail->nr == ail->mr)
+    {
 		EXPAND(ail->interval_list, ail->mr);
+    }
 
     // Set new interval values
 	interval_t *i = &ail->interval_list[ail->nr++];
 	i->start = start;
 	i->end = end;
     i->id_value = id;
 
@@ -65,7 +69,26 @@
     for (j = 0; j < ail2->nr; j++)
     {
         ailist_add(appended_ailist, ail2->interval_list[j].start, ail2->interval_list[j].end,  ail2->interval_list[j].id_value);
     }
 
     return appended_ailist;
 }
+
+
+ailist_t *ailist_copy(ailist_t *ail)
+{   /* Copy ailist */
+
+	// Initalize copy
+    ailist_t *ail_copy = ailist_init();
+
+
+    // Iterate over intervals in p
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        ailist_add(ail_copy, ail->interval_list[i].start, ail->interval_list[i].end, i);
+    }
+
+    return ail_copy;
+
+}
```

### Comparing `ailist-1.0.4/ailist/src/ailist_coverage.c` & `ailist-2.0.2/ailist/src/ailist/ailist_coverage.c`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 //-----------------------------------------------------------------------------
 
 void ailist_interval_coverage(ailist_t *ail, int start, int end, int coverage[])
 {   /* Calculate coverage for a single interval */
     
     // Query overlaps
-    ailist_t *overlaps = ailist_query(ail, start, end);
+    ailist_t *overlaps = ailist_init();
+    ailist_query(ail, overlaps, start, end);
 
     // Iterate over overlaps
     int j;
     for (j = 0; j < overlaps->nr; j++)
     {
         int overlap_start = MAX(start, (int)overlaps->interval_list[j].start);
         int overlap_end = MIN(end, (int)overlaps->interval_list[j].end);
@@ -51,14 +52,39 @@
         }
     }
 
     return;
 }
 
 
+void ailist_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length)
+{   /* Calculate coverage of a length */
+    int length;
+    int n;
+    int i;
+    int position;
+    int start = (int)ail->first;
+
+    for (i = 0; i < ail->nr; i++)
+    {
+        length = ail->interval_list[i].end - ail->interval_list[i].start;
+        if (length > min_length && length < max_length)
+        {
+            for (n = 0; n < length; n++)
+            {
+                position = (ail->interval_list[i].start - start) + n;
+                coverage[position] = coverage[position] + 1;
+            }
+        }
+    }
+
+    return;
+}
+
+
 void ailist_bin_coverage(ailist_t *ail, double coverage[], int bin_size)
 {   /* Calculate coverage within bins */
     int start = (int)(ail->first / bin_size);
     
     int i;
     for (i = 0; i < ail->nr; i++)
     {
@@ -107,7 +133,39 @@
             }
         }
     }
 
     return;
 }
 
+
+void ailist_midpoint_coverage(ailist_t *ail, double coverage[])
+{   /* Calculate coverage of midpoints */
+
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        int length = ail->interval_list[i].end - ail->interval_list[i].start;
+        int midpoint = length / 2;
+        coverage[midpoint] = coverage[midpoint] + 1;
+    }
+
+    return;
+}
+
+
+void ailist_midpoint_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length)
+{   /* Calculate coverage of midpoints with lengths */
+
+    int i;
+    for (i = 0; i < ail->nr; i++)
+    {
+        int length = ail->interval_list[i].end - ail->interval_list[i].start;
+        if (length > min_length && length < max_length)
+        {
+            int midpoint = length / 2;
+            coverage[midpoint] = coverage[midpoint] + 1;
+        }
+    }
+
+    return;
+}
```

### Comparing `ailist-1.0.4/ailist/src/ailist_extract.c` & `ailist-2.0.2/ailist/src/ailist/ailist_extract.c`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/ailist/src/ailist_filter.c` & `ailist-2.0.2/ailist/src/ailist/ailist_filter.c`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,31 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
-ailist_t *ailist_length_filter(ailist_t *ail, int min_length, int max_length)
+void ailist_length_filter(ailist_t *ail, ailist_t *filtered_ail, int min_length, int max_length)
 {   /* Filter ailist by length */
-    // Initiatize filtered ailist
-    ailist_t *filtered_ail = ailist_init();
 
     // Iterate over intervals and filter
     int length;
     int i;
     for (i = 0; i < ail->nr; i++)
     {
         // Record length (excluding last position)
         length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
         if (length >= min_length && length <= max_length)
         {
             ailist_add(filtered_ail, ail->interval_list[i].start, ail->interval_list[i].end, ail->interval_list[i].id_value);
         }
     }
 
-    return filtered_ail;
+    return;
 }
 
 
 ailist_t *ailist_downsample(ailist_t *ail, double proportion)
 {   /* Randomly downsample */
 
     // Initialize downsampled ailist_t
```

### Comparing `ailist-1.0.4/ailist/src/ailist_index.c` & `ailist-2.0.2/ailist/src/ailist/ailist_get_id.c`

 * *Files 6% similar despite different names*

```diff
@@ -35,20 +35,48 @@
     // Initialize ailist_t to return
     ailist_t *id_intervals = ailist_init();
 
     // Iterate over intervals and pull all those with id
     int i;
     for (i = 0; i < length; i++)
     {
-        uint32_t query_id = ids[i];
+        int32_t query_id = ids[i];
         int j;
         for (j = 0; j < ail->nr; j++)
         {
             if (ail->interval_list[j].id_value == query_id)
             {
                 ailist_add(id_intervals, ail->interval_list[j].start, ail->interval_list[j].end, ail->interval_list[j].id_value);
             }
         }
     }
     
     return id_intervals;
 }
+
+
+void ailist_reset_id(ailist_t *ail)
+{   /* Reset id_values */
+
+    // Iterate over ailist
+    int i;
+    for (i = 0; i < ail->nr; ++i)
+    {
+        ail->interval_list[i].id_value = i;
+    }
+
+    return;
+}
+
+
+void ailist_reset_id_shift(ailist_t *ail, int shift)
+{   /* Reset id_values with shift */
+
+    // Iterate over ailist
+    int i;
+    for (i = 0; i < ail->nr; ++i)
+    {
+        ail->interval_list[i].id_value = i + shift;
+    }
+
+    return;
+}
```

### Comparing `ailist-1.0.4/ailist/src/ailist_iter.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,61 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_list.h"
+#include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
 
-int *get_comp_bounds(ailist_t *ail)
-{   /* Get component index */
+void labeled_aiarray_percent_coverage(labeled_aiarray_t *laia1, labeled_aiarray_t *laia2, double coverage[])
+{   /* Find percent coverage of intervals in laia1 that are in laia2 */
 
-    int *idxC = &ail->idxC[0];
-    int *comps_bounds = malloc((ail->nc + 1) * sizeof(int));
-    int i;
-    for (i = 0; i < ail->nc; i++)
-    {
-        comps_bounds[i] = idxC[i];
-    }
-
-    comps_bounds[ail->nc] = ail->nr;
-
-    return comps_bounds;
-}
-
-
-ailist_sorted_iter_t *ailist_sorted_iter_init(ailist_t *ail)
-{
-
-    // Initialize variables
-    ailist_sorted_iter_t *iter = (ailist_sorted_iter_t *)malloc(sizeof(ailist_sorted_iter_t));
-    iter->ail = ail;
-    iter->comp_bounds = get_comp_bounds(ail);
-    iter->nc = ail->nc;
-    iter->comp_used = malloc(iter->nc+1 * sizeof(int));
-    memcpy(&iter->comp_used, &iter->comp_bounds, sizeof(int));
-    iter->intv = &ail->interval_list[0];
-    iter->n = -1;
-
-    return iter;
-}
-
-
-int ailist_sorted_iter_next(ailist_sorted_iter_t *iter)
-{
-    // Increment position
-    iter->n++;
-    if (iter->n >= iter->ail->nr)
+    
+    
+    // Iterate over labels
+    labeled_aiarray_iter_t *iter = labeled_aiarray_iter_init(laia1);
+    
+    while (labeled_aiarray_iter_next(iter) != 0)
     {
-        return 0;
-    }
+        // Get label
+        int32_t t = get_label(laia2, iter->name);
 
-    int selected_comp = 0;
-    // Iterate over other components
-    int position;
-    // Iterate over components
-    int j;
-    for (j = 0; j < iter->nc; j++)
-    {
-        // If position is available, assign next interval
-        if (iter->comp_used[j] != iter->comp_bounds[j + 1])
+        // Check if label present
+        if (t != -1)
         {
-            position = iter->comp_used[j];
-            iter->intv = &iter->ail->interval_list[position];
-            break;
-        }
-    }
+            label_t *p2 = &laia2->labels[t];
 
-    for (j = 0; j < iter->nc; j++)
-    {
-        // Check component has intervals left to investigate
-        if (iter->comp_used[j] == iter->comp_bounds[j + 1])
-        {
-            continue;
+            ailist_t *result_ail = ailist_init();
+            ailist_t *overlaps = ailist_init();
+            ailist_query(p2->ail, overlaps, iter->intv->i->start, iter->intv->i->end);
+            ailist_construct(overlaps, 20);
+            ailist_common_intervals(iter->intv->i, overlaps, result_ail);
+
+            // Iterate over common intervals
+            int32_t k;
+            for (k = 0; k < result_ail->nr; k++)
+            {
+                // Calculate percent coverage
+                coverage[iter->n] += (double)(result_ail->interval_list[k].end - result_ail->interval_list[k].start);
+            }
+
+            // Calculate percent coverage
+            coverage[iter->n] /= (double)(iter->intv->i->end - iter->intv->i->start);
+
+            // Free memory
+            ailist_destroy(overlaps);
+            ailist_destroy(result_ail);
         }
-
-        // Determine position
-        position = iter->comp_used[j];
-        // Check for lower start
-        if (iter->ail->interval_list[position].start < iter->intv->start)
-        {
-            iter->intv = &iter->ail->interval_list[position];
-            selected_comp = j;
+        // If label not present, set coverage to 0
+        else {
+            coverage[iter->n] = 0;
         }
-
-        // Increment label_comp_counter for selected comp
-        iter->comp_used[selected_comp] = iter->comp_used[selected_comp] + 1;
-    }
-
-    return 1;
-}
-
-
-void ailist_sorted_iter_destroy(ailist_sorted_iter_t *iter)
-{
-    // Check that ail exists
-	if (iter == 0)
-    {
-        return;
     }
 
-    // Free ail
-	//if (iter->ail)
-	//{
-        //free(iter->ail);
-    //}
-
-    // Free intv
-	//if (iter->intv)
-	//{
-        //free(iter->intv);
-    //}
-    
-    // Free label_comp_bounds
-	//if (iter->label_comp_bounds)
-	//{
-        //free(iter->label_comp_bounds);
-    //}
-
-    // Free label_comp_used
-	//if (iter->label_comp_used)
-	//{
-        //free(iter->label_comp_used);
-    //}
-
-    free(iter);
+    // Free memory
+    labeled_aiarray_iter_destroy(iter);
 
     return;
-}
-
-//-----------------------------------------------------------------------------
+}
```

### Comparing `ailist-1.0.4/ailist/src/ailist_query.c` & `ailist-2.0.2/ailist/src/ailist/ailist_query.c`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         return tR;
     } else if (As[tL].start >= qe) {
         return -1;
     }
 
     while (tL < tR - 1)
     {
-        tM = (tL + tR) / 2; 
+        //tM = (tL + tR) / 2;
+        tM = tL + (tR - tL)/2;
 
         if (As[tM].start >= qe)
         {
             tR = tM - 1;
         } else {
             tL = tM;
         }
@@ -45,21 +46,18 @@
     return tE; 
 }
 
 //-----------------------------------------------------------------------------
 // Queries returning ailist_t objects
 //-----------------------------------------------------------------------------
 
-ailist_t *ailist_query(ailist_t *ail, uint32_t qs, uint32_t qe)
+void ailist_query(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe)
 {   /* Query ailist intervals */
 
-    // Initialize overlaps
     int k;
-    ailist_t *overlaps = ailist_init();
-
     for (k = 0; k < ail->nc; k++)
     {   // Search each component
         int32_t cs = ail->idxC[k];
         int32_t ce = cs + ail->lenC[k];			
         int32_t t;
 
         if (ail->lenC[k] > 15)
@@ -83,24 +81,22 @@
                 {
                     ailist_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end, ail->interval_list[t].id_value);
                 }
             }                      
         }
     }
 
-    return overlaps;                            
+    return;                            
 }
 
 
-ailist_t *ailist_query_length(ailist_t *ail, uint32_t qs, uint32_t qe, int min_length, int max_length)
+void ailist_query_length(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe, int min_length, int max_length)
 {   
-    // Initialize overlaps
-    int k;
-    ailist_t *overlaps = ailist_init();
 
+    int k;
     for (k = 0; k < ail->nc; k++)
     {   // Search each component
         int32_t cs = ail->idxC[k];
         int32_t ce = cs + ail->lenC[k];			
         int32_t t;
 
         if (ail->lenC[k] > 15)
@@ -132,25 +128,22 @@
                         ailist_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end, ail->interval_list[t].id_value);
                     }
                 }
             }                      
         }
     }
 
-    return overlaps;                            
+    return;                            
 }
 
 
-ailist_t *ailist_query_from_array(ailist_t *ail, const long starts[], const long ends[], int length)
+void ailist_query_from_array(ailist_t *ail, ailist_t *overlaps, const long starts[], const long ends[], int length)
 {   /* Query ailist intervals from arrays */
 
-    // Initialize overlaps
     int k;
-    ailist_t *overlaps = ailist_init();
-
     // Iterate over queries
     int i;
     for (i = 0; i < length; i++)
     {
         uint32_t qs = starts[i];
         uint32_t qe = ends[i];
 
@@ -182,25 +175,22 @@
                         ailist_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end, ail->interval_list[t].id_value);
                     }
                 }                      
             }
         }
     }
 
-    return overlaps;                            
+    return;                            
 }
 
 
-ailist_t *ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2)
+void ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2, ailist_t *overlaps)
 {   /* Query ailist intervals from another ailist */
 
-    // Initialize overlaps
     int k;
-    ailist_t *overlaps = ailist_init();
-
     // Iterate over queries
     int i;
     for (i = 0; i < ail2->nr; i++)
     {
         uint32_t qs = ail2->interval_list[i].start;
         uint32_t qe = ail2->interval_list[i].end;
 
@@ -232,29 +222,243 @@
                         ailist_add(overlaps, ail->interval_list[t].start, ail->interval_list[t].end, ail->interval_list[t].id_value);
                     }
                 }                      
             }
         }
     }
 
-    return overlaps;                            
+    return;                            
+}
+
+
+//-----------------------------------------------------------------------------
+// Queries for nhits
+//-----------------------------------------------------------------------------
+
+void ailist_query_nhits(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe)
+{   /* Query number of hits in ailist intervals */
+
+    int k;
+    for (k = 0; k < ail->nc; k++)
+    {   // Search each component
+        int32_t cs = ail->idxC[k];
+        int32_t ce = cs + ail->lenC[k];			
+        int32_t t;
+
+        if (ail->lenC[k] > 15)
+        {
+            t = binary_search(ail->interval_list, cs, ce, qe);
+
+            while (t >= cs && ail->maxE[t] > qs)
+            {
+                if (ail->interval_list[t].end > qs)
+                {               	
+                    (*nhits)++;
+                }
+
+                t--;
+            }
+        } 
+        else {
+            for (t = cs; t < ce; t++)
+            {
+                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+                {
+                    (*nhits)++;
+                }
+            }                      
+        }
+    }
+
+    return;                            
+}
+
+
+void ailist_query_nhits_length(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe, int min_length, int max_length)
+{   /* Query number of hits in ailist intervals within a length */
+
+    int k;
+    for (k = 0; k < ail->nc; k++)
+    {   // Search each component
+        int32_t cs = ail->idxC[k];
+        int32_t ce = cs + ail->lenC[k];			
+        int32_t t;
+
+        if (ail->lenC[k] > 15)
+        {
+            t = binary_search(ail->interval_list, cs, ce, qe);
+
+            while (t >= cs && ail->maxE[t] > qs)
+            {
+                if (ail->interval_list[t].end > qs)
+                {               	
+                    int length = ail->interval_list[t].end - ail->interval_list[t].start;
+                    if (length >= min_length && length < max_length)
+                    {
+                        (*nhits)++;
+                    }
+                }
+
+                t--;
+            }
+        } 
+        else {
+            for (t = cs; t < ce; t++)
+            {
+                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+                {
+                    int length = ail->interval_list[t].end - ail->interval_list[t].start;
+                    if (length >= min_length && length < max_length)
+                    {
+                        (*nhits)++;
+                    }
+                }
+            }                      
+        }
+    }
+
+    return;                            
+}
+
+
+void ailist_query_has_hit(ailist_t *ail, uint8_t *has_hit, uint32_t qs, uint32_t qe)
+{   /* Query if interval has any overlap in ailist intervals */
+
+    int k;
+    for (k = 0; k < ail->nc; k++)
+    {   // Search each component
+        int32_t cs = ail->idxC[k];
+        int32_t ce = cs + ail->lenC[k];			
+        int32_t t;
+
+        if (ail->lenC[k] > 15)
+        {
+            t = binary_search(ail->interval_list, cs, ce, qe);
+
+            while (t >= cs && ail->maxE[t] > qs)
+            {
+                if (ail->interval_list[t].end > qs)
+                {               	
+                    *has_hit = (uint32_t)1;
+                    return;
+                }
+
+                t--;
+            }
+        } 
+        else {
+            for (t = cs; t < ce; t++)
+            {
+                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+                {
+                    *has_hit = (uint32_t)1;
+                    return;
+                }
+            }                      
+        }
+    }
+
+    return;                            
 }
 
+//-----------------------------------------------------------------------------
+// Queries returning overlap_index_t objects
+//-----------------------------------------------------------------------------
+
+void ailist_query_with_index(ailist_t *ail, overlap_index_t *overlaps, uint32_t qs, uint32_t qe)
+{   /* Query aiarray intervals and record original index */
+
+    // Initialize overlaps
+    int k;
+    for (k = 0; k < ail->nc; k++)
+    {   // Search each component
+        int32_t cs = ail->idxC[k];
+        int32_t ce = cs + ail->lenC[k];			
+        int32_t t;
+
+        if (ail->lenC[k] > 15)
+        {
+            t = binary_search(ail->interval_list, cs, ce, qe);
+
+            while (t >= cs && ail->maxE[t] > qs)
+            {
+                if (ail->interval_list[t].end > qs)
+                {               	
+                    overlap_index_add(overlaps, &ail->interval_list[t]);
+                }
+
+                t--;
+            }
+        } 
+        else {
+            for (t = cs; t < ce; t++)
+            {
+                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+                {
+                    overlap_index_add(overlaps, &ail->interval_list[t]);
+                }
+            }                      
+        }
+    }
+
+    // reallocate to remove extra memory
+    overlaps->indices = (long *)realloc(overlaps->indices, sizeof(long) * overlaps->size);
+    overlaps->max_size = overlaps->size;
+
+    return;                            
+}
 
 //-----------------------------------------------------------------------------
 // Queries returning array_query_t objects
 //-----------------------------------------------------------------------------
 
-array_query_t *ailist_query_id_from_array(ailist_t *ail, const long starts[], const long ends[], const long ids[], int length)
-{   /* Query ailist interval ids from array */
-    
+void ailist_query_only_index(ailist_t *ail, array_query_t *aq, uint32_t qs, uint32_t qe, uint32_t id)
+{   /* Query aiarray intervals and record original index */
+
     // Initialize overlaps
     int k;
-    array_query_t *aq = array_query_init();
+    for (k = 0; k < ail->nc; k++)
+    {   // Search each component
+        int32_t cs = ail->idxC[k];
+        int32_t ce = cs + ail->lenC[k];			
+        int32_t t;
+
+        if (ail->lenC[k] > 15)
+        {
+            t = binary_search(ail->interval_list, cs, ce, qe);
+
+            while (t >= cs && ail->maxE[t] > qs)
+            {
+                if (ail->interval_list[t].end > qs)
+                {               	
+                    array_query_add(aq, id, ail->interval_list[t].id_value);
+                }
 
+                t--;
+            }
+        } 
+        else {
+            for (t = cs; t < ce; t++)
+            {
+                if (ail->interval_list[t].start < qe && ail->interval_list[t].end > qs)
+                {
+                    array_query_add(aq, id, ail->interval_list[t].id_value);
+                }
+            }                      
+        }
+    }
+
+    return;                            
+}
+
+
+void ailist_query_id_from_array(ailist_t *ail, array_query_t *aq, const long starts[], const long ends[], const long ids[], int length)
+{   /* Query ailist interval ids from array */
+    
+    int k;
     // Iterate over queries
     int i;
     for (i = 0; i < length; i++)
     {
         uint32_t qs = starts[i];
         uint32_t qe = ends[i];
         uint32_t id = ids[i];
@@ -292,24 +496,22 @@
     }
 
     // reallocate to remove extra memory
     aq->ref_index = (long *)realloc(aq->ref_index, sizeof(long) * aq->size);
     aq->query_index = (long *)realloc(aq->query_index, sizeof(long) * aq->size);
     aq->max_size = aq->size;
 
-    return aq;                            
+    return;                            
 }
 
 
-array_query_t *ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2)
+void ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2, array_query_t *aq)
 {   /* Query ailist interval ids from another ailist */
+    
     int k;
-
-    array_query_t *aq = array_query_init();
-
     // Iterate over queries
     int i;
     for (i = 0; i < ail2->nr; i++)
     {
         uint32_t qs = ail2->interval_list[i].start;
         uint32_t qe = ail2->interval_list[i].end;
         uint32_t id = ail2->interval_list[i].id_value;
@@ -347,10 +549,10 @@
     }
 
     // reallocate to remove extra memory
     aq->ref_index = (long *)realloc(aq->ref_index, sizeof(long) * aq->size);
     aq->query_index = (long *)realloc(aq->query_index, sizeof(long) * aq->size);
     aq->max_size = aq->size;
 
-    return aq;                           
+    return;                           
 }
```

### Comparing `ailist-1.0.4/ailist/src/array_query_utilities.c` & `ailist-2.0.2/ailist/src/array_query/array_query_utilities.c`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     array_query_t *aq = (array_query_t *)malloc(sizeof(array_query_t));
     if (aq == NULL)
     {
         printf("Memory allocation failed");
         exit(1); // exit the program
     }
     aq->size = 0;
-    aq->max_size = 64;
-    aq->ref_index = (long *)malloc(sizeof(long) * 64);
+    aq->max_size = 32;
+    aq->ref_index = (long *)malloc(sizeof(long) * 32);
     if (aq->ref_index == NULL)
     {
         printf("Memory allocation failed");
         exit(1); // exit the program
     }
-    aq->query_index = (long *)malloc(sizeof(long) * 64);
+    aq->query_index = (long *)malloc(sizeof(long) * 32);
     if (aq->query_index == NULL)
     {
         printf("Memory allocation failed");
         exit(1); // exit the program
     }
 
     return aq;
@@ -36,32 +36,13 @@
     free(aq);
 }
 
 
 void array_query_add(array_query_t *aq, long ref, long query)
 {
 
-    // Check if size needs to be increased
-    if (aq->size == aq->max_size)
-    {
-        aq->max_size = aq->max_size + 64;
-        aq->ref_index = (long *)realloc(aq->ref_index, sizeof(long) * aq->max_size);
-        if (aq->ref_index == NULL)
-        {
-            printf("Memory allocation failed");
-            exit(1); // exit the program
-        }
-        aq->query_index = (long *)realloc(aq->query_index, sizeof(long) * aq->max_size);
-        if (aq->query_index == NULL)
-        {
-            printf("Memory allocation failed");
-            exit(1); // exit the program
-        }
-    }
+    // Push values to array query
+    push_array_query(aq, ref, query);
 
-    // Increment size
-    aq->size++;
+    return;
 
-    // Add new indices
-    aq->ref_index[aq->size-1] = ref;
-    aq->query_index[aq->size-1] = query;
 }
```

### Comparing `ailist-1.0.4/ailist/src/augmented_interval_list.h` & `ailist-2.0.2/ailist/src/ailist/augmented_interval_list.h`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <time.h>
 #include <ctype.h>
 #include <math.h>
 #include <assert.h>
-#include "utilities.h"
-#include "array_query_utilities.h"
+#include "../utilities/utilities.h"
+#include "../array_query/array_query_utilities.h"
 #include "interval.h"
 
 //-------------------------------------------------------------------------------------
 
 typedef struct {
 	int64_t nr, mr;						// Number of intervals
 	interval_t *interval_list;			// List of interval_t objects
@@ -32,14 +32,21 @@
 	int nc;								// Number of components
 	int *comp_bounds;					// Label component bounds
 	int *comp_used;						// Components used
 	interval_t *intv;					// Interval
 	int n;								// Current position
 } ailist_sorted_iter_t;
 
+typedef struct {
+	int size;							// Current size
+    int max_size;						// Maximum size
+	ailist_t *ail;						// Store ailist
+	long *indices;						// Store indices
+} overlap_index_t;
+
 //-------------------------------------------------------------------------------------
 // augmented_interval_list.c
 //=====================================================================================
 
 // Initialize ailist_t
 ailist_t *ailist_init(void);
 
@@ -53,70 +60,114 @@
 int ailist_max_length(ailist_t *ail);
 
 // Calculate length distribution
 void ailist_length_distribution(ailist_t *ail, int distribution[]);
 
 
 //-------------------------------------------------------------------------------------
+// overlap_index.c
+//=====================================================================================
+
+// Initialize overlap_index_t
+overlap_index_t *overlap_index_init(void);
+
+// Free overlap_index memory
+void overlap_index_destroy(overlap_index_t *oi);
+
+// Add interval and index to overlap_index
+void overlap_index_add(overlap_index_t *aq, interval_t *i);
+
+
+//-------------------------------------------------------------------------------------
 // ailist_add.c
 //=====================================================================================
 
 // Add interval to ailist_t object 
 void ailist_add(ailist_t *ail, uint32_t start, uint32_t end, uint32_t id);
 
 // Build ailist from arrays
 void ailist_from_array(ailist_t *ail, const long starts[], const long ends[], const long ids[], int length);
 
 // Append two ailist
 ailist_t *ailist_append(ailist_t *ail1, ailist_t *ail2);
 
+// Copy ailist
+ailist_t *ailist_copy(ailist_t *ail);
+
 
 //-------------------------------------------------------------------------------------
 // ailist_construct.c
 //=====================================================================================
 
 // Construct ailist: decomposition and augmentation
 void ailist_construct(ailist_t *ail, int cLen);
 
+// Construct ailist: decomposition and augmentation v0
+void ailist_construct_v0(ailist_t *ail, int cLen);
+
+// Validation that construction ran
+int ailist_validate_construction(ailist_t *ail);
+
 
 //-------------------------------------------------------------------------------------
-// ailist_index.c
+// ailist_get_id.c
 //=====================================================================================
 
 // Get intervals with id
 ailist_t *ailist_get_id(ailist_t *ail, int query_id);
 
 // Get intervals with ids
 ailist_t *ailist_get_id_array(ailist_t *ail, const long ids[], int length);
 
+// Reset id_values
+void ailist_reset_id(ailist_t *ail);
+
+// Reset id_values with shift
+void ailist_reset_id_shift(ailist_t *ail, int shift);
+
 
 //-------------------------------------------------------------------------------------
 // ailist_query.c
 //=====================================================================================
 
 // Binary search
 uint32_t binary_search(interval_t* As, uint32_t idxS, uint32_t idxE, uint32_t qe);
 
 // Query ailist intervals
-ailist_t *ailist_query(ailist_t *ail, uint32_t qs, uint32_t qe);
+void ailist_query(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe);
 
 // Query ailist intervals of a length
-ailist_t *ailist_query_length(ailist_t *ail, uint32_t qs, uint32_t qe, int min_length, int max_length);
+void ailist_query_length(ailist_t *ail, ailist_t *overlaps, uint32_t qs, uint32_t qe, int min_length, int max_length);
+
+// Query number of hits in ailist intervals
+void ailist_query_nhits(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe);
+
+// Query number of hits in ailist intervals of a length
+void ailist_query_nhits_length(ailist_t *ail, long *nhits, uint32_t qs, uint32_t qe, int min_length, int max_length);
+
+// Query if interval has any overlap in ailist intervals
+void ailist_query_has_hit(ailist_t *ail, uint8_t *has_hit, uint32_t qs, uint32_t qe);
 
 // Query ailist intervals from arrays
-ailist_t *ailist_query_from_array(ailist_t *ail, const long starts[], const long ends[], int length);
+void ailist_query_from_array(ailist_t *ail, ailist_t *overlaps, const long starts[], const long ends[], int length);
 
 // Query ailist intervals from another ailist
-ailist_t *ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2);
+void ailist_query_from_ailist(ailist_t *ail, ailist_t *ail2, ailist_t *overlaps);
+
+// Query aiarray intervals and record original index
+void ailist_query_with_index(ailist_t *ail, overlap_index_t *overlaps, uint32_t qs, uint32_t qe);
+
+// Query aiarray intervals and record original index
+void ailist_query_only_index(ailist_t *ail, array_query_t *aq, uint32_t qs, uint32_t qe, uint32_t id);
 
 // Query ailist interval ids from array
-array_query_t *ailist_query_id_from_array(ailist_t *ail, const long starts[], const long ends[], const long ids[], int length);
+void ailist_query_id_from_array(ailist_t *ail, array_query_t *aq, const long starts[], const long ends[], const long ids[], int length);
 
 // Query ailist interval ids from another ailist
-array_query_t *ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2);
+void ailist_query_id_from_ailist(ailist_t *ail, ailist_t *ail2, array_query_t *aq);
 
 
 //-------------------------------------------------------------------------------------
 // ailist_iter.c
 //=====================================================================================
 
 // Get component index
@@ -138,20 +189,29 @@
 
 // Calculate coverage for a single interval
 void ailist_interval_coverage(ailist_t *ail, int start, int end, int coverage[]);
 
 // Calculate coverage
 void ailist_coverage(ailist_t *ail, double coverage[]);
 
+// Calculate coverage of a length
+void ailist_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length);
+
 // Calculate coverage within bins
 void ailist_bin_coverage(ailist_t *ail, double coverage[], int bin_size);
 
 // Calculate coverage within bins of a length
 void ailist_bin_coverage_length(ailist_t *ail, double coverage[], int bin_size, int min_length, int max_length);
 
+// Calculate coverage of midpoints
+void ailist_midpoint_coverage(ailist_t *ail, double coverage[]);
+
+// Calculate coverage of midpoints with length
+void ailist_midpoint_coverage_length(ailist_t *ail, double coverage[], int min_length, int max_length);
+
 
 //-------------------------------------------------------------------------------------
 // ailist_nhits.c
 //=====================================================================================
 
 // Determine number of hits for each query interval
 void ailist_nhits_from_array(ailist_t *ail, const long starts[], const long ends[],
@@ -159,18 +219,18 @@
 
 // Determine number of hits of a length for each query interval
 void ailist_nhits_from_array_length(ailist_t *ail, const long starts[], const long ends[],
 									int length, int nhits[], int min_length,
 									int max_length);
 
 // Calculate n hits within bins
-void ailist_bin_nhits(ailist_t *ail, double coverage[], int bin_size);
+void ailist_bin_nhits(ailist_t *ail, long coverage[], int bin_size);
 
 // Calculate n hits of a length within bins
-void ailist_bin_nhits_length(ailist_t *ail, double coverage[], int bin_size, int min_length, int max_length);
+void ailist_bin_nhits_length(ailist_t *ail, long coverage[], int bin_size, int min_length, int max_length);
 
 //-------------------------------------------------------------------------------------
 // ailist_wps.c
 //=====================================================================================
 
 // Calculate Window Protection Score
 void ailist_wps(ailist_t *ail, double wps[], uint32_t protection);
@@ -201,30 +261,42 @@
 
 
 //-------------------------------------------------------------------------------------
 // ailist_ops.c
 //=====================================================================================
 
 // Subtract intervals from region
-void subtract_intervals(ailist_t *ref_ail, ailist_t *result_ail, interval_t query_i, int j);
+void ailist_subtract_intervals(interval_t *intv, ailist_t *ail, ailist_t *result_ail);
 
 // Subtract two ailist_t intervals
 ailist_t *ailist_subtract(ailist_t *ref_ail, ailist_t *query_ail);
 
 // Subtract intervals from region
-void common_intervals(ailist_t *ref_ail, ailist_t *result_ail, interval_t query_i, int j);
+void ailist_common_intervals(interval_t *intv, ailist_t *ail, ailist_t *result_ail);
 
-// Subtract two ailist_t intervals
-ailist_t *ailist_common(ailist_t *ref_ail, ailist_t *query_ail);
+// Common intervals of two ailist_t intervals
+ailist_t *ailist_common(ailist_t *ail, ailist_t *other_ail);
+
+// Union of two ailist_t intervals
+ailist_t *ailist_union(ailist_t *ail, ailist_t *other_ail);
 
 
 //-------------------------------------------------------------------------------------
 // ailist_filter.c
 //=====================================================================================
 
 // Filter ailist by length
-ailist_t *ailist_length_filter(ailist_t *ail, int min_length, int max_length);
+void ailist_length_filter(ailist_t *ail, ailist_t *filtered_ail, int min_length, int max_length);
 
 // Randomly downsample
 ailist_t *ailist_downsample(ailist_t *ail, double proportion);
 
+
+//-------------------------------------------------------------------------------------
+// ailist_simulate.c
+//=====================================================================================
+
+// Simulate intervals
+void ailist_simulate(ailist_t *ail, ailist_t *simulation, int n);
+
+
 #endif
```

### Comparing `ailist-1.0.4/ailist/src/interval.c` & `ailist-2.0.2/ailist/src/ailist/interval.c`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/ailist/src/interval.h` & `ailist-2.0.2/ailist/src/ailist/interval.h`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/ailist/src/khash.h` & `ailist-2.0.2/ailist/src/labeled_aiarray/khash.h`

 * *Files identical despite different names*

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_add.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c`

 * *Files 23% similar despite different names*

```diff
@@ -4,166 +4,208 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-//const int khStrInt = 33;
-//KHASH_MAP_INIT_STR(khStrInt, int32_t)
-//typedef khash_t(khStrInt) strhash_t;
-//const int khIntStr = 32;
-//KHASH_MAP_INIT_INT(khIntStr, char*)
-//typedef khash_t(khIntStr) inthash_t;
 
-//-----------------------------------------------------------------------------
+void labeled_aiarray_add_label(labeled_aiarray_t *laia, const char*label_name)
+{	/* Expand and add label */
 
-void labeled_aiarray_add(labeled_aiarray_t *ail, uint32_t start, uint32_t end, const char *label_name)
-{   /* Add interval to aiarray_t object */
+	//int ret_name;
+    //int ret_label;
 
-	// If start is greater than end, invalid interval
-    if (start > end)
-    {
-        return;
-    }
+	khiter_t k;
+	strhash_t *h = (strhash_t*)laia->label_lookup;
+
+	k = kh_get(khStrInt, h, label_name);
+	if (k == kh_end(h))
+    {
+		if (laia->n_labels == laia->max_labels)
+        {
+			EXPAND(laia->labels, laia->max_labels);
+        }
 
-    // Determine if
-    int ret_name;
-    int ret_label;
-    //khint_t ks;
-	khiter_t ks;
-    khiter_t ki;
-	strhash_t *hs = (strhash_t*)ail->label_map;
-    inthash_t *hi = (inthash_t*)ail->rev_label_map;
-	//ks = kh_put(khStrInt, hs, label_name, &ret_name);
-    ks = kh_get(khStrInt, hs, label_name);
-	if (ks == kh_end(hs))
-    {
 		// Add label_name to label_map
-        ret_name = kh_name_set(khStrInt, hs, label_name, ail->nl);
-        //ks = kh_put(khStrInt, hs, label_name, &ret_name);
-        //kh_value(hs, ks) = ail->nl;		
-		//kh_key(hs, ks) = label_name;
+        kh_name_set(khStrInt, h, label_name, laia->n_labels);
+		laia->n_labels++;
 
-        // Add label to label_map
-        //uint16_t n_labels = (uint16_t)ail->nl;
-        ret_label = kh_label_set(khIntStr, hi, ail->nl, label_name);
-        //ki = kh_put(khIntStr, hi, ail->nl, &ret_label);
-        //kh_value(hi, ki) = label_name;
-        //kh_key(hi, ki) = ail->nl;
+		// Determine label code
+		uint32_t t = kh_value(h, k);
+
+		label_t *p = &laia->labels[t];
+		p->name = strdup(label_name);
+		p->ail = ailist_init();
 
-        //printf("   adding key:%s, val:%lld\n", label_name, ail->nl);
 	}
 
-    //printf("   label_name:%s, present:%d\n", label_name, name_absent);
+	return;
 
-    // Determine label code
-    uint16_t label = kh_value(hs, ks);
+}
 
-    // If max region reached, expand array
-	if (ail->nr + 1 == ail->mr)
-    {
-		EXPAND(ail->interval_list, ail->mr);
-    }
-    // If max label reached, expand array
-	while (label >= ail->ml)
+
+void labeled_aiarray_add(labeled_aiarray_t *laia, uint32_t s, uint32_t e, const char *label_name)
+{
+	// Check if start is greater than end
+	if (s > e)
     {
-        uint32_t max_labels = ail->ml;
-        // Record max labels
-		EXPAND(ail->label_count, ail->ml);
-        memset(&ail->label_count[ail->nl], 0, (ail->ml - ail->nl) * sizeof(uint32_t));
-
-        // Reset max labels because EXPAND increments
-        ail->ml = max_labels;
-        EXPAND(ail->first, ail->ml);
-        // Set new values to INT32_MAX
-        memset(&ail->first[ail->nl], INT32_MAX, (ail->ml - ail->nl) * sizeof(uint32_t));
-
-        // Reset max labels because EXPAND increments
-        ail->ml = max_labels;
-        EXPAND(ail->last, ail->ml);
-        // Set new values to 0
-        memset(&ail->last[ail->nl], 0, (ail->ml - ail->nl) * sizeof(uint32_t));
+        return;
     }
 
-    // Update first
-    ail->first[label] = MIN(ail->first[label], start);
-    // Update last
-    ail->last[label] = MAX(ail->last[label], end);
+	// Add label to laia
+	labeled_aiarray_add_label(laia, label_name);
 
-    // Determine if label is new
-    if (label >= ail->nl)
-    {
-        ail->nl = label + 1;
-    }
+	// Lookup label
+	uint32_t t = get_label(laia, label_name);
+	label_t *p = &laia->labels[t];
+
+	// Add interval to laia
+	ailist_add(p->ail, s, e, laia->total_nr);
+	laia->total_nr++;
+
+	// No longer constructed
+	labeled_aiarray_deconstruct(laia);
+
+	return;
+}
+
+
+void labeled_aiarray_multi_merge(labeled_aiarray_t *laia, labeled_aiarray_t **laia_array, int length)
+{
+	// Iterate over ail_array
+	int i;
+	for (i = 0; i < length; i++)
+	{
+		// Find label
+		label_t p = laia_array[i]->labels[0];
+		const char *label = p.name;
+		
+		// Add label
+		int absent;
+		khint_t k;
+		strhash_t *h = (strhash_t*)laia->label_lookup;
+		k = kh_put(khStrInt, h, label, &absent);
+		if (laia->n_labels == laia->max_labels)
+        {
+			EXPAND(laia->labels, laia->max_labels);
+        }
+		kh_val(h, k) = laia->n_labels;
+		laia->n_labels++;
+
+		// Add interval_list
+		int32_t kk = kh_val(h, k);
+		laia->labels[kk] = laia_array[i]->labels[0];
+		laia->total_nr = laia->total_nr + p.ail->nr;
+
+	}
 
-    // Increment label_index as running count
-    // Once constructed, becomes index
-    ail->label_count[label]++;
-
-    // Set new interval values
-	labeled_interval_t *i = &ail->interval_list[ail->nr++];
-	i->start = start;
-	i->end = end;
-    i->id_value = ail->nr - 1;
-    i->label = label;
+	// No longer constructed
+	laia->is_constructed = 0;
 
 	return;
 }
 
 
-void labeled_aiarray_from_array(labeled_aiarray_t *ail, const long starts[], const long ends[], const char label_names[], int length, int label_str_len)
+void labeled_aiarray_from_array(labeled_aiarray_t *laia, const long starts[], const long ends[], const char label_names[], int length, int label_str_len)
 {
-    
-    //const size_t len = strlen(label_names);
-    //const size_t len = sizeof(label_names) / sizeof(label_names[0]);
-    //printf("   strlen:%zu\n", len);
 
     // Iterate over itervals and add
     int j = 0;
     int i;
     int total_length = length * label_str_len;
     for (i = 0; i < total_length; i+=label_str_len)
     {
-        //char label_name[len + 1];
         char label_name[label_str_len+1];
-        slice_str2(label_names, label_name, i, i+label_str_len);
-        //const char *final_name = label_name;
-        labeled_aiarray_add(ail, starts[j], ends[j], label_name);
+        slice_str(label_names, label_name, i, i+label_str_len);
+        labeled_aiarray_add(laia, starts[j], ends[j], label_name);
         j++;
-        //printf("start:%d, end:%d, label:%d, label_name:%s\n", ail->interval_list[i].start, ail->interval_list[i].end, ail->interval_list[i].label, label_name);
-        //display_label_map(ail);
-        //printf("\n\n");
     }
 
+	// No longer constructed
+	laia->is_constructed = 0;
+
     return;
 }
 
 
-void labeled_aiarray_append(labeled_aiarray_t *ail, labeled_aiarray_t *ail2)
+void labeled_aiarray_append(labeled_aiarray_t *laia, labeled_aiarray_t *laia2)
 {   /* Add intervals from another labeled_aiarray */
-    
-    int i;
-    for (i = 0; i < ail2->nr; i++)
-    {
-        const char *label_name = query_rev_label_map(ail2, ail2->interval_list[i].label);
-        labeled_aiarray_add(ail, ail2->interval_list[i].start, ail2->interval_list[i].end, label_name);
-    }
+
+	// Iterate over labels
+	labeled_aiarray_iter_t *laia2_iter = labeled_aiarray_iter_init(laia2);
+
+	while (labeled_aiarray_iter_next(laia2_iter))
+	{
+
+		labeled_aiarray_add(laia, laia2_iter->intv->i->start, laia2_iter->intv->i->end, laia2_iter->intv->name);
+	}
+
+	labeled_aiarray_iter_destroy(laia2_iter);
+
+	// No longer constructed
+	laia->is_constructed = 0;
 
     return;
 }
 
 
-labeled_aiarray_t *labeled_aiarray_copy(labeled_aiarray_t *ail)
+labeled_aiarray_t *labeled_aiarray_copy(labeled_aiarray_t *laia)
 {   /* Copy labeled_aiarray */
 
-    labeled_aiarray_t *ail_copy = labeled_aiarray_init();
-    int i;
-    for (i = 0; i < ail->nr; i++)
-    {
-        const char *label_name = query_rev_label_map(ail, ail->interval_list[i].label);
-        labeled_aiarray_add(ail_copy, ail->interval_list[i].start, ail->interval_list[i].end, label_name);
-    }
+	// Initalize copy
+    labeled_aiarray_t *laia_copy = labeled_aiarray_init();
+
+	// Iterate over labels
+	labeled_aiarray_iter_t *laia_iter = labeled_aiarray_iter_init(laia);
 
-    return ail_copy;
+	while (labeled_aiarray_iter_next(laia_iter))
+	{
+
+		labeled_aiarray_add(laia_copy, laia_iter->intv->i->start, laia_iter->intv->i->end, laia_iter->intv->name);
+	}
 
+	labeled_aiarray_iter_destroy(laia_iter);
+
+    return laia_copy;
+
+}
+
+
+void labeled_aiarray_append_ail(labeled_aiarray_t *laia, ailist_t *ail, const char *label_name)
+{	/* Append AIList in labeled_aiarry */
+
+	// Add intervals
+	int i;
+	for (i = 0; i < ail->nr; i++)
+	{
+		labeled_aiarray_add(laia, ail->interval_list[i].start, ail->interval_list[i].end, label_name);
+	}
+
+	return;
+}
+
+
+void labeled_aiarray_wrap_ail(labeled_aiarray_t *laia, ailist_t *ail, const char *label_name)
+{	/* Wrap AIList in labeled_aiarry */
+
+	// Add label
+	labeled_aiarray_add_label(laia, label_name);
+	
+	// Wrap ailist_t
+	int32_t t = get_label(laia, label_name);
+	label_t *p = &laia->labels[t];
+	ailist_destroy(p->ail);
+	p->ail = ail;
+
+	// Adjust ail id_value
+	int i;
+	for (i = 0; i < ail->nr; i++)
+	{
+		p->ail->interval_list[i].id_value = laia->total_nr + i;
+	}
+
+	// Adjust total_nr
+	laia->total_nr = laia->total_nr + ail->nr;
+
+	return;
 }
```

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_coverage.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/overlap_label_index.c`

 * *Files 26% similar despite different names*

```diff
@@ -4,88 +4,86 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-void labeled_aiarray_interval_coverage(labeled_aiarray_t *ail, int start, int end, const char *label_name, int coverage[])
-{   /* Determine coverage for an interval */
-    
-    // Query overlaps
-    labeled_aiarray_t *overlaps = labeled_aiarray_query_single(ail, start, end, label_name);
 
-    // Iterate over overlaps
-    int j;
-    for (j = 0; j < overlaps->nr; j++)
+overlap_label_index_t *overlap_label_index_init(void)
+{   /* Initialize overlap_index */
+    
+    // Initialize variables
+    overlap_label_index_t *oi = (overlap_label_index_t *)malloc(sizeof(overlap_label_index_t));
+    if (oi == NULL)
     {
-        int overlap_start = MAX(start, (int)overlaps->interval_list[j].start);
-        int overlap_end = MIN(end, (int)overlaps->interval_list[j].end);
-
-        // Iterate over overlapping postions
-        int k;
-        for (k = overlap_start; k < overlap_end; k++)
-        {
-            coverage[k - start] += 1;
-        }
+        printf("Memory allocation failed");
+        exit(1); // exit the program
+    }
+    oi->size = 0;
+    oi->max_size = 64;
+    oi->indices = (long *)malloc(sizeof(long) * 64);
+    if (oi->indices == NULL)
+    {
+        printf("Memory allocation failed");
+        exit(1); // exit the program
     }
+    oi->laia = labeled_aiarray_init();
 
-    return;
+    return oi;
 }
 
 
-//-------------------------------------------------------------------------------
+void overlap_label_index_destroy(overlap_label_index_t *oi)
+{   /* Free overlap_label_index memory */
 
-
-void labeled_aiarray_label_coverage(labeled_interval_t *interval_list, double coverage[], const char *label_names, int nr)
-{   /* Calculate coverage for a label */
-    int length;
-    int n;
-
-    // Iterate over regions
-    int i;
-    for (i = 0; i < nr; i++)
-    {
-        length = interval_list[i].end - interval_list[i].start;
-        for (n = 0; n < length; n++)
-        {
-            coverage[i+n] = coverage[i+n] + 1;
-        }
-    }
+    labeled_aiarray_destroy(oi->laia);
+    free(oi->indices);
+    free(oi);
 
     return;
 }
 
 
-void labeled_aiarray_coverage(labeled_aiarray_t *ail, double coverage[])
-{   /* Calculate coverage */
+void overlap_label_index_add(overlap_label_index_t *oi, interval_t i, const char *label_name)
+{   /* Add interval to overlap_label_index */
 
-    uint32_t cov_shift = 0;
-    uint16_t label;
-    for (label = 0; label < ail->nl; label++)
-    {
-        const char *label_name = query_rev_label_map(ail, label);
-        if (ail->label_count[label] != 0)
-        {
-            // Find bounds for labels
-            uint32_t ail_label_start = get_label_index(ail, label);
-            uint32_t ail_label_end = get_label_index(ail, label + 1);
-            int first = (int)ail->first[label];
-            int last = (int)ail->last[label];
-            int length = last - first;
-            int nr = ail_label_end - ail_label_start;
-            labeled_aiarray_label_coverage(&ail->interval_list[ail_label_start], &coverage[cov_shift], label_name, nr);
+    // Check if size needs to be increased
+    push_indices(oi, i.id_value);
 
-            // Increment cov_shift
-            cov_shift = cov_shift + length;
-        }
-    }
+    // Add new indices
+    labeled_aiarray_add(oi->laia, i.start, i.end, label_name);
 
     return;
 }
 
-//-------------------------------------------------------------------------------
 
+void overlap_label_index_wrap_ail(overlap_label_index_t * oi, ailist_t *ail, const char *label_name)
+{
+    labeled_aiarray_wrap_ail(oi->laia, ail, label_name);
 
+    int j;
+    for (j = 0; j < ail->nr; j++)
+    {
+        interval_t i = ail->interval_list[j];
 
-//-------------------------------------------------------------------------------
+        // Check if size needs to be increased
+        if (oi->size == oi->max_size)
+        {
+            oi->max_size = oi->max_size + 64;
+            oi->indices = (long *)realloc(oi->indices, sizeof(long) * oi->max_size);
+            if (oi->indices == NULL)
+            {
+                printf("Memory allocation failed");
+                exit(1); // exit the program
+            }
+        }
+
+        // Increment size
+        oi->size++;
 
+        // Add new indices
+        oi->indices[oi->size-1] = i.id_value;
+    }
+
+    return;
+}
```

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_extract.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c`

 * *Files 22% similar despite different names*

```diff
@@ -4,45 +4,48 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-void labeled_aiarray_extract_starts(labeled_aiarray_t *ail, long starts[])
+void labeled_aiarray_extract_starts(labeled_aiarray_t *laia, long starts[])
 {   /* Extract start for labeled_aiarray */
 
     int i;
-    for (i = 0; i < ail->nr; i++)
+    for (i = 0; i < laia->total_nr; i++)
     {
-        starts[i] = ail->interval_list[i].start;
+        labeled_interval_t *laia_i = labeled_aiarray_get_index(laia, i);
+        starts[i] = laia_i->i->start;
     }
 
     return;
 }
 
 
-void labeled_aiarray_extract_ends(labeled_aiarray_t *ail, long ends[])
+void labeled_aiarray_extract_ends(labeled_aiarray_t *laia, long ends[])
 {   /* Extract end for labeled_aiarray */
 
     int i;
-    for (i = 0; i < ail->nr; i++)
+    for (i = 0; i < laia->total_nr; i++)
     {
-        ends[i] = ail->interval_list[i].end;
+        labeled_interval_t *laia_i = labeled_aiarray_get_index(laia, i);
+        ends[i] = laia_i->i->end;
     }
 
     return;
 }
 
 
 
-void labeled_aiarray_extract_ids(labeled_aiarray_t *ail, long ids[])
+void labeled_aiarray_extract_ids(labeled_aiarray_t *laia, long ids[])
 {   /* Extract id for labeled_aiarray */
 
     int i;
-    for (i = 0; i < ail->nr; i++)
+    for (i = 0; i < laia->total_nr; i++)
     {
-        ids[i] = ail->interval_list[i].id_value;
+        labeled_interval_t *laia_i = labeled_aiarray_get_index(laia, i);
+        ids[i] = laia_i->i->id_value;
     }
 
     return;
 }
```

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_get.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c`

 * *Files 21% similar despite different names*

```diff
@@ -4,348 +4,244 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-//const int khStrInt = 33;
-//KHASH_MAP_INIT_STR(khStrInt, int32_t)
-//typedef khash_t(khStrInt) strhash_t;
-//const int khIntStr = 32;
-//KHASH_MAP_INIT_INT(khIntStr, char*)
-//typedef khash_t(khIntStr) inthash_t;
-
-//-----------------------------------------------------------------------------
-
-int label_is_present(labeled_aiarray_t *ail, const char *label_name)
-{   /* Determine if label_name is in array */
+labeled_aiarray_t *labeled_aiarray_get_label(labeled_aiarray_t *laia, const char *label_name)
+{   /* Get intervals with label name */
 
-    //int name_absent;
-    strhash_t *h = (strhash_t*)ail->label_map;
-	
-	khiter_t k = kh_get(khStrInt, h, label_name);
-    
-    //if (kh_exist(h, k))
-	if (k != kh_end(h))
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-		return 1;
-	}
-	else {
-		return 0;
-	}
-    //k = kh_get(khStrInt, h, label_name);
-	//int k = kh_put(khStrInt, h, label_name, &name_absent);
-    //if (name_absent)
-    //{
-    //    return 0;
-    //}
-
-    return 1;
-}
-
+        labeled_aiarray_construct(laia, 20);
+    }
 
-uint16_t query_label_map(labeled_aiarray_t *ail, const char *label_name)
-{   /* Query label map for label name */
-    
-    int name_absent;
-    strhash_t *h = (strhash_t*)ail->label_map;
-    int k = kh_put(khStrInt, h, label_name, &name_absent);
-    if (name_absent)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        printf("KeyError\n");
+        labeled_aiarray_cache_id(laia);
     }
 
-    uint16_t label = kh_val(h, k);
-
-    return label;
-}
+    // Initialize interval
+    labeled_aiarray_t *label_laia = labeled_aiarray_init();
 
+    // Get label
+    int32_t t = get_label(laia, label_name);
 
-const char *query_rev_label_map(labeled_aiarray_t *ail, uint16_t label)
-{   /* Query rev_label_map for label */
-    
-    int label_absent;
-    inthash_t *h = (inthash_t*)ail->rev_label_map;
-    int k = kh_put(khIntStr, h, label, &label_absent);
-    if (label_absent)
+    // Check if label present
+    if (t != -1)
     {
-        printf("KeyError\n");
+        // Find intervals
+        //labeled_aiarray_add_label(label_laia, laia->labels[t].name);
+        int i;
+        for (i = 0; i < laia->labels[t].ail->nr; i++)
+        {
+            labeled_aiarray_add(label_laia, laia->labels[t].ail->interval_list[i].start,
+                                            laia->labels[t].ail->interval_list[i].end,
+                                            laia->labels[t].name);
+        }
     }
-    const char *label_name = kh_val(h, k);
-
-    return label_name;
+    
+    return label_laia;
 }
 
 
-labeled_aiarray_t *get_label(labeled_aiarray_t *ail, const char *label_name)
+labeled_aiarray_t *labeled_aiarray_view_label(labeled_aiarray_t *laia, const char *label_name)
 {   /* Get intervals with label name */
 
-    // Initialize interval
-    labeled_aiarray_t *label_intervals = labeled_aiarray_init();
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
+    {
+        labeled_aiarray_construct(laia, 20);
+    }
 
-    // Check that label is present
-    if (label_is_present(ail, label_name) == 0)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        return label_intervals;
+        labeled_aiarray_cache_id(laia);
     }
 
-    // Determine label
-    uint16_t label = query_label_map(ail, label_name);
+    // Initialize interval
+    labeled_aiarray_t *label_laia = labeled_aiarray_init();
 
-    // Find intervals
-    int i;
-    if (ail->label_count[label] != 0)
+    // Get label
+    int32_t t = get_label(laia, label_name);
+
+    // Check if label present
+    if (t != -1)
     {
-        for (i = get_label_index(ail, label); i < get_label_index(ail, label + 1); i++)
-        {
-            labeled_aiarray_add(label_intervals, ail->interval_list[i].start, ail->interval_list[i].end, label_name);
-        }
+        // Find intervals
+        labeled_aiarray_add_label(label_laia, laia->labels[t].name);
+        labeled_aiarray_wrap_ail(label_laia, laia->labels[t].ail, laia->labels[t].name);
     }
     
-    return label_intervals;
+    return label_laia;
 }
 
 
-overlap_label_index_t *get_label_with_index(labeled_aiarray_t *ail, const char *label_name)
+overlap_label_index_t *labeled_aiarray_get_label_with_index(labeled_aiarray_t *laia, const char *label_name)
 {   /* Get intervals with label name and original index */
 
-    // Initialize interval
-    overlap_label_index_t *label_intervals = overlap_label_index_init();
-
-    // Check that label is present
-    if (label_is_present(ail, label_name) == 0)
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-        return label_intervals;
+        labeled_aiarray_construct(laia, 20);
     }
 
-    // Determine label
-    uint16_t label = query_label_map(ail, label_name);
-
-    // Find intervals
-    int i;
-    if (ail->label_count[label] != 0)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        for (i = get_label_index(ail, label); i < get_label_index(ail, label + 1); i++)
-        {
-            overlap_label_index_add(label_intervals, ail->interval_list[i], label_name);
-        }
+        labeled_aiarray_cache_id(laia);
     }
-    
-    return label_intervals;
-}
-
-
-labeled_aiarray_t *get_label_array(labeled_aiarray_t *ail, const char *label_names[], int length)
-{   /* Get intervals with labels names from array */
 
     // Initialize interval
-    labeled_aiarray_t *label_intervals = labeled_aiarray_init();
+    overlap_label_index_t *label_laia = overlap_label_index_init();
 
-    // Find intervals
-    int j;
-    for (j = 0; j < length; j++)
-    {
-        // Find label name
-        const char *label_name = label_names[j];
-        
-        // Check that label is present
-        if (label_is_present(ail, label_name) == 0)
-        {
-            return label_intervals;
-        }
-
-        // Determine label
-        uint16_t label = query_label_map(ail, label_name);
+    // Get label
+    int32_t t = get_label(laia, label_name);
 
+    // Check if label present
+    if (t != -1)
+    {
         // Find intervals
+        //labeled_aiarray_add_label(label_laia, laia->labels[t].name);
         int i;
-        if (ail->label_count[label] != 0)
+        for (i = 0; i < laia->labels[t].ail->nr; i++)
         {
-            for (i = get_label_index(ail, label); i < get_label_index(ail, label + 1); i++)
-            {
-                labeled_aiarray_add(label_intervals, ail->interval_list[i].start, ail->interval_list[i].end, label_name);
-            }
+            overlap_label_index_add(label_laia, laia->labels[t].ail->interval_list[i],
+                                            laia->labels[t].name);
         }
     }
     
-    
-    return label_intervals;
+    return label_laia;
 }
 
 
-overlap_label_index_t *get_label_array_with_index(labeled_aiarray_t *ail, const char label_names[], int n_labels, int label_str_len)
-{   /* Get intervals with labels from array and original index */
+labeled_aiarray_t *labeled_aiarray_get_label_array(labeled_aiarray_t *laia, const char label_names[], int n_labels, int label_str_len)
+{   /* Get intervals with labels names from array */
+
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
+    {
+        labeled_aiarray_construct(laia, 20);
+    }
+
+    // Check index is initialized
+    if (laia->id_index == NULL)
+    {
+        labeled_aiarray_cache_id(laia);
+    }
 
     // Initialize interval
-    overlap_label_index_t *label_intervals = overlap_label_index_init();
+    labeled_aiarray_t *label_laia = labeled_aiarray_init();
 
     // Find intervals
     int j;
     for (j = 0; j < n_labels; j++)
     {
         // Find label name
         char label_name[label_str_len + 1];
-        slice_str2(label_names, label_name, (j*label_str_len), (j*label_str_len)+label_str_len);
-
-        // Check that label is present
-        if (label_is_present(ail, label_name) == 0)
-        {
-            return label_intervals;
-        }
-
-        // Determine label
-        uint16_t label = query_label_map(ail, label_name);
-
-        // Find intervals
-        int label_start;
-        int label_end;
-        int i;
+        slice_str(label_names, label_name, (j*label_str_len), (j*label_str_len)+label_str_len);
+        
+        // Get label
+        int32_t t = get_label(laia, label_name);
 
-        if (ail->label_count[label] != 0)
+        // Check if label present
+        if (t != -1)
         {
-            label_start = get_label_index(ail, label);
-            if (label + 1 > ail->nl)
-            {
-                label_end = ail->nr;
-            } else {
-                label_end = label_start + ail->label_count[label];
-            }
 
-            for (i = label_start; i < label_end; i++)
+            // Find intervals
+            //labeled_aiarray_add_label(label_laia, laia->labels[t].name);
+            int i;
+            for (i = 0; i < laia->labels[t].ail->nr; i++)
             {
-                overlap_label_index_add(label_intervals, ail->interval_list[i], label_name);
+                labeled_aiarray_add(label_laia, laia->labels[t].ail->interval_list[i].start,
+                                                laia->labels[t].ail->interval_list[i].end,
+                                                laia->labels[t].name);
             }
         }
     }
     
     
-    return label_intervals;
+    return label_laia;
 }
 
 
-int get_label_index(labeled_aiarray_t *ail, int label)
-{   /* Get index start of label */
-
-    // Initialize position
-    int count = 0;
+overlap_label_index_t *labeled_aiarray_get_label_array_with_index(labeled_aiarray_t *laia, const char label_names[], int n_labels, int label_str_len)
+{   /* Get intervals with labels from array and original index */
 
-    // Iterate over labels
-    int i;
-    for (i = 0; i < label; i++)
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-        count = count + ail->label_count[i];
+        labeled_aiarray_construct(laia, 20);
     }
 
-    return count;
-}
-
-
-void get_label_index_array(labeled_aiarray_t *ail, int *label_index)
-{   /* Determine label indices */
-
-    // Initialize position
-    int count = 0;
-
-    // Iterate over labels
-    int i;
-    for (i = 0; i < ail->nl; i++)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        label_index[i] = count;
-        count = count + ail->label_count[i];
+        labeled_aiarray_cache_id(laia);
     }
 
-    return;
-}
-
-
-void get_label_array_ids(labeled_aiarray_t *ail, const char *label_names[], int n_labels, long index[])
-{   /* Get ids for labels in a label array */
+    // Initialize interval
+    overlap_label_index_t *label_intervals = overlap_label_index_init();
 
     // Find intervals
-    int index_i = 0;
-    int i;
-    for (i = 0; i < n_labels; i++)
+    int j;
+    for (j = 0; j < n_labels; j++)
     {
         // Find label name
-        const char *label_name = label_names[i];
-
-        // Check that label is present
-        if (label_is_present(ail, label_name) == 0)
-        {
-            return;
-        }
-
-        // Determine label
-        uint16_t label = query_label_map(ail, label_name);
+        char label_name[label_str_len + 1];
+        slice_str(label_names, label_name, (j*label_str_len), (j*label_str_len)+label_str_len);
 
-        // Find intervals
-        int label_start;
-        int label_end;
-        int j;
+        // Get label
+        int32_t t = get_label(laia, label_name);
 
-        if (ail->label_count[label] != 0)
+        // Check if label present
+        if (t != -1)
         {
-            label_start = get_label_index(ail, label);
-            if (label + 1 > ail->nl)
-            {
-                label_end = ail->nr;
-            } else {
-                label_end = label_start + ail->label_count[label];
-            }
 
-            for (j = label_start; j < label_end; j++)
+            // Find intervals
+            //labeled_aiarray_add_label(label_laia, laia->labels[t].name);
+            int i;
+            for (i = 0; i < laia->labels[t].ail->nr; i++)
             {
-                index[index_i] = ail->interval_list[j].id_value;
-                index_i++;
+                overlap_label_index_add(label_intervals, laia->labels[t].ail->interval_list[i],
+                                                laia->labels[t].name);
             }
         }
     }
-
-    return;
+    
+    return label_intervals;
 }
 
 
-void get_label_array_presence(labeled_aiarray_t *ail, const char label_names[], int n_labels, uint8_t index[], int label_str_len)
+void labeled_aiarray_get_label_array_presence(labeled_aiarray_t *laia, const char label_names[], int n_labels, uint8_t index[], int label_str_len)
 {   /* Determine if an index is of a label array */
 
     // Find intervals
     int i;
     for (i = 0; i < n_labels; i++)
     {
         // Find label name
         char label_name[label_str_len + 1];
-        slice_str2(label_names, label_name, (i*label_str_len), (i*label_str_len)+label_str_len);
-
-        // Check that label is present
-        if (label_is_present(ail, label_name) == 0)
-        {
-            return;
-        }
+        slice_str(label_names, label_name, (i*label_str_len), (i*label_str_len)+label_str_len);
 
-        // Determine label
-        uint16_t label = query_label_map(ail, label_name);
-
-        // Find intervals
-        int label_start;
-        int label_end;
-        int j;
+        // Get label
+        int32_t t = get_label(laia, label_name);
 
-        if (ail->label_count[label] != 0)
+        // Check if label present
+        if (t != -1)
         {
-            label_start = get_label_index(ail, label);
-            if (label + 1 > ail->nl)
-            {
-                label_end = ail->nr;
-            } else {
-                label_end = label_start + ail->label_count[label];
-            }
-
-            for (j = label_start; j < label_end; j++)
+            // Find intervals
+            //labeled_aiarray_add_label(label_laia, laia->labels[t].name);
+            int i;
+            for (i = 0; i < laia->labels[t].ail->nr; i++)
             {
-                index[ail->interval_list[j].id_value] = 1;
+                index[laia->labels[t].ail->interval_list[i].id_value] = 1;
             }
         }
     }
 
     return;
 }
```

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_index.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c`

 * *Files 25% similar despite different names*

```diff
@@ -4,233 +4,226 @@
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
 
-void labeled_aiarray_cache_id(labeled_aiarray_t *ail)
+void labeled_aiarray_cache_id(labeled_aiarray_t *laia)
 {   /* Record id positions by id */
 
     // Initialize id index
-    if (ail->id_index == NULL)
+    if (laia->id_index == NULL)
     {
-        ail->id_index = malloc(ail->nr * sizeof(uint32_t));
+        laia->id_index = malloc(laia->total_nr * sizeof(uint32_t));
     }
     else {
-        free(ail->id_index);
-        ail->id_index = malloc(ail->nr * sizeof(uint32_t));
+        free(laia->id_index);
+        laia->id_index = malloc(laia->total_nr * sizeof(uint32_t));
     }
 
     // Iterate over intervals
-    int i;
-    for (i = 0; i < ail->nr; i++)
+    int count = 0;
+    int t;
+    for (t = 0; t < laia->n_labels; t++)
     {
-        ail->id_index[ail->interval_list[i].id_value] = i;
+        label_t *p = &laia->labels[t];
+        int i;
+        for (i = 0; i < p->ail->nr; i++)
+        {
+            laia->id_index[p->ail->interval_list[i].id_value] = count;
+            count++;
+        }
     }
 
     return;
 }
 
 
-labeled_aiarray_t *labeled_aiarray_slice_index(labeled_aiarray_t *ail, const long ids[], int length)
-{   /* Get intervals with ids */
-    
+labeled_interval_t *labeled_aiarray_get_index(labeled_aiarray_t *laia, int32_t i)
+{   /* Retrieve labeled_interval given index */
+
     // Initialize interval
-    labeled_aiarray_t *sliced_intervals = labeled_aiarray_init();
+    labeled_interval_t *id_interval = NULL;
+    
+    // Check i is in id_index
+    if (i > laia->total_nr)
+    {
+        printf("IndexError: index outside of bounds.");
+        return id_interval;
+    }
+    
+    // Check index is initialized
+    if (laia->id_index == NULL)
+    {
+        labeled_aiarray_cache_id(laia);
+    }
 
-    // Determine if ail has cached ids
-    if (ail->id_index != NULL)
+    int index = laia->id_index[i];
+    int count = 0;
+    int t;
+    
+    for (t = 0; t < laia->n_labels; t++)
     {
-        // Iterate over ids
-        int i;
-        for (i = 0; i < length; i++)
-        {   
-            uint32_t id = ail->id_index[ids[i]];
+        label_t *p = &laia->labels[t];
+        if (index > (p->ail->nr + count - 1))
+        {
+            count = count + p->ail->nr;
+            continue;
+        }
+        else {
+            int id_value = index - count;
+            id_interval = labeled_interval_init(&p->ail->interval_list[id_value], p->name);
+            break;
+        }
+    }
 
-            // Check values are present
-            if (id < 0 || id > ail->nr)
-            {
-                labeled_aiarray_destroy(sliced_intervals);
-                return NULL;
-            }
+    return id_interval;
 
-            uint16_t label = ail->interval_list[id].label;
-            const char *label_name = query_rev_label_map(ail, label);
-            labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                label_name);
-        }
-    } else {
-        // Iterate over index
-        int i;
-        for (i = 0; i < length; i++)
+}
+
+
+labeled_aiarray_t *labeled_aiarray_slice_index(labeled_aiarray_t *laia, const long ids[], int length)
+{   /* Get intervals with ids */
+    
+    // Initialize interval
+    labeled_aiarray_t *sliced_laia = labeled_aiarray_init();
+
+    // Iterate over ids
+    int i;
+    for (i = 0; i < length; i++)
+    {   
+        // Check values are present
+        if (ids[i] < 0 || ids[i] > laia->total_nr)
         {
-            int id = ids[i];
+            labeled_aiarray_destroy(sliced_laia);
+            return NULL;
+        }
 
-            // Check values are present
-            if (id < 0 || id > ail->nr)
-            {
-                labeled_aiarray_destroy(sliced_intervals);
-                return NULL;
-            }
+        // Fetch true id
+        labeled_interval_t *i_laia = labeled_aiarray_get_index(laia, ids[i]);
 
-            uint16_t label = ail->interval_list[id].label;
-            const char *label_name = query_rev_label_map(ail, label);
-            labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                label_name);
+        // Add interval
+        if (i_laia != NULL)
+        {
+            labeled_aiarray_add(sliced_laia, i_laia->i->start,
+                                            i_laia->i->end,
+                                            i_laia->name);
         }
     }
     
-    return sliced_intervals;
+    return sliced_laia;
 }
 
 
-labeled_aiarray_t *labeled_aiarray_slice_range(labeled_aiarray_t *ail, int start, int end, int step)
+labeled_aiarray_t *labeled_aiarray_slice_range(labeled_aiarray_t *laia, int start, int end, int step)
 {   /* Get intervals with range */
     
     // Initialize intervals
-    labeled_aiarray_t *sliced_intervals = labeled_aiarray_init();
+    labeled_aiarray_t *sliced_laia = labeled_aiarray_init();
 
     // Check values are present
-    if (start < 0 || end > ail->nr)
+    if (start < 0 || end > laia->total_nr)
     {
         return NULL;
     }
 
-    // Determine if ail has cached ids
-    if (ail->id_index != NULL)
+    // Iterate over ids
+    int i;
+    for (i = start; i < end; i+=step)
     {
-        // Iterate over ids
-        int i;
-        for (i = start; i < end; i+=step)
-        {
-            uint32_t id = ail->id_index[i];
-            uint16_t label = ail->interval_list[id].label;
-            const char *label_name = query_rev_label_map(ail, label);
-            labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                label_name);
-        }
-    } else {
-        // Iterate over index
-        int i;
-        for (i = start; i < end; i+=step)
-        {
-            int id = i;
-            uint16_t label = ail->interval_list[id].label;
-            const char *label_name = query_rev_label_map(ail, label);
-            labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                label_name);
+        // Fetch true id
+        labeled_interval_t *i_laia = labeled_aiarray_get_index(laia, i);
+        
+        // Add interval
+        if (i_laia != NULL)
+        {
+            labeled_aiarray_add(sliced_laia, i_laia->i->start,
+                                            i_laia->i->end,
+                                            i_laia->name);
         }
     }
     
-    return sliced_intervals;
+    
+    return sliced_laia;
 }
 
 
-labeled_aiarray_t *labeled_aiarray_slice_bool(labeled_aiarray_t *ail, uint8_t bool_index[])
+labeled_aiarray_t *labeled_aiarray_slice_bool(labeled_aiarray_t *laia, uint8_t bool_index[])
 {   /* Get intervals with boolean array */
 
     // Initialize intervals
-    labeled_aiarray_t *sliced_intervals = labeled_aiarray_init();
+    labeled_aiarray_t *sliced_laia = labeled_aiarray_init();
 
-    // Determine if ail has cached ids
-    if (ail->id_index != NULL)
+    // Iterate over bool_index
+    int i;
+    for (i = 0; i < laia->total_nr; i++)
     {
-        // Iterate over bool_index
-        int i;
-        for (i = 0; i < ail->nr; i++)
+        if (bool_index[i] == 1)
         {
-            if (bool_index[i] == 1)
+            // Fetch true id
+            labeled_interval_t *i_laia = labeled_aiarray_get_index(laia, i);
+            
+            // Add interval
+            if (i_laia != NULL)
             {
-                uint32_t id = ail->id_index[i];
-                uint16_t label = ail->interval_list[id].label;
-                const char *label_name = query_rev_label_map(ail, label);
-                labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                    label_name);
-            }
-        }
-    } else {
-        // Iterate over bool_index
-        int i;
-        for (i = 0; i < ail->nr; i++)
-        {
-            if (bool_index[i] == 1)
-            {
-                uint32_t id = ail->id_index[i];
-                uint16_t label = ail->interval_list[id].label;
-                const char *label_name = query_rev_label_map(ail, label);
-                labeled_aiarray_add(sliced_intervals, ail->interval_list[id].start, ail->interval_list[id].end,
-                                    label_name);
+                labeled_aiarray_add(sliced_laia, i_laia->i->start,
+                                                i_laia->i->end,
+                                                i_laia->name);
             }
         }
     }
 
-    return sliced_intervals;
+    return sliced_laia;
 }
 
 
-labeled_interval_t *labeled_aiarray_get_id(labeled_aiarray_t *ail, int id_value)
-{   /* Get interval with id */
-
-    // Initialize interval
-    labeled_interval_t *id_interval;
+int labeled_aiarray_index_with_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia)
+{   /* Re-assign interval bounds based on other given intervals */
 
-    // Find interval
-    if (ail->id_index != NULL)
+    // Iterate over labels
+    int l;
+    for (l = 0; l < other_laia->n_labels; l++)
     {
-        id_interval = &ail->interval_list[ail->id_index[id_value]];
-    } else {
-        id_interval = &ail->interval_list[id_value];
-    }
-    
-    return id_interval;
-}
+        const char *label_name = other_laia->labels[l].name;
+        uint32_t t = get_label(laia, label_name);
 
+        if (t >= 0)
+        {
+            label_t *p1 = &laia->labels[t];
+            label_t *p2 = &other_laia->labels[l];
 
-int labeled_aiarray_index_by_aiarray_inplace(labeled_aiarray_t *ail1, labeled_aiarray_t *ail2)
-{   /* Index aiarray by another aiarray inplace */
+            int first = 0;
+            int last = 0;
+            int i;
+            for (i = 0; i < p1->ail->nr; i++)
+            {
+                uint32_t position_start = p1->ail->interval_list[i].start;
+                // Check position
+                if (position_start < 0 || position_start >= p2->ail->nr)
+                {
+                    return 1;
+                }
+                p1->ail->interval_list[i].start = p2->ail->interval_list[position_start].start;
+                first = MIN(INT32_MAX, p1->ail->interval_list[i].start);
+
+                uint32_t position_end = p1->ail->interval_list[i].end - 1;
+                // Check position
+                if (position_end < 0 || position_end >= p2->ail->nr)
+                {
+                    return 1;
+                }
+                p1->ail->interval_list[i].end = p2->ail->interval_list[position_end].end;
+                last = MAX(0, p1->ail->interval_list[i].end);
+            }
 
-    // Iterate over ail
-    int label_start;
-    int position_start;
-    int position_end;
-
-    // Determine label indices
-    int *label_index = malloc(ail2->nl * sizeof(int));
-    get_label_index_array(ail2, label_index);
+            p1->ail->first = first;
+            p1->ail->last = last;
+        
+        } else {
 
-    int i;
-    for (i = 0; i < ail1->nr; i++)
-    {   
-        // Set ail1 start to start position in ail2
-        position_start = ail1->interval_list[i].start;
-        // Check position
-        if (ail1->interval_list[i].label > ail2->nl || position_start < 0 || position_start >= ail2->nr)
-        {
-            return 1;
-        }
-        label_start = label_index[ail1->interval_list[i].label];
-        ail1->interval_list[i].start = ail2->interval_list[label_start + position_start].start;
-
-        // Set ail1 end to start position in ail2
-        position_end = ail1->interval_list[i].end - 1;
-        // Check position
-        if (position_end < 0 || position_end >= ail2->nr)
-        {
             return 1;
         }
-        ail1->interval_list[i].end = ail2->interval_list[label_start + position_end].end;
-        //printf("i: %d, start: %d, end: %d, label: %d, label_start: %d\n", i, position_start, position_end, ail1->interval_list[i].label, label_start);
-    }
-
-    // Change range
-    for (i = 0; i < ail1->nl; i++)
-    {
-        position_start = ail1->first[i];
-        position_end = ail1->last[i] - 1;
-        label_start = label_index[i];
-        ail1->first[i] = ail2->interval_list[label_start + position_start].start;
-        ail1->last[i] = ail2->interval_list[label_start + position_end].end - 1;
     }
 
     return 0;
 }
```

### Comparing `ailist-1.0.4/ailist/src/labeled_aiarray_merge.c` & `ailist-2.0.2/ailist/src/ailist/ailist_merge.c`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,62 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "labeled_augmented_array.h"
-
-//-------------------------------------------------------------------------------
+#include "augmented_interval_list.h"
 
+//-----------------------------------------------------------------------------
 
-labeled_aiarray_t *labeled_aiarray_merge(labeled_aiarray_t *ail, uint32_t gap)
-{   /* Merge nearby intervals */
+ailist_t *ailist_merge(ailist_t *ail, uint32_t gap)
+{   /* Merge intervals in constructed ailist_t object */
 
     // Initialize merged atrributes
     int previous_end = ail->interval_list[0].end;
     int previous_start = ail->interval_list[0].start;
     int previous_id = ail->interval_list[0].id_value;
-    int previous_label = ail->interval_list[0].label;
-    const char *previous_label_name = query_rev_label_map(ail, previous_label);
-    labeled_aiarray_t *merged_list = labeled_aiarray_init();
-
-    // Iterate over labels in ail
-    const char *label_name;
-    label_sorted_iter_t *ail_iter;
-    labeled_interval_t *intv;
-    int label;
-    for (label = 0; label < ail->nl; label++)
-    {
-        label_name = query_rev_label_map(ail, label);
-        // Create sorted iterators
-        ail_iter = iter_init(ail, label_name);
-        while (iter_next(ail_iter) != 0)
-        {
-            intv = ail_iter->intv;
-
-            // Check if intervals merge
-            if (previous_end > (int)(intv->start - gap) && previous_label == intv->label)
-                {
-                    previous_end = MAX(previous_end, (int)intv->end);
-                }
-                else
-                {
-                    labeled_aiarray_add(merged_list, previous_start, previous_end, previous_label_name);
-                    previous_start = intv->start;
-                    previous_end = intv->end;
-                    previous_id = intv->id_value;
-                    previous_label = intv->label;
-                    previous_label_name = query_rev_label_map(ail, previous_label);
-                }
-        }
+    ailist_t *merged_list = ailist_init();
+    interval_t *intv;
 
+    // Create sorted iterators
+    ailist_sorted_iter_t* ail_iter = ailist_sorted_iter_init(ail);
+    intv = ail_iter->intv;
+    while (ailist_sorted_iter_next(ail_iter) != 0)
+    {
+        intv = ail_iter->intv;
+        
         // Check if intervals merge
-        if (previous_end > (int)(intv->start - gap) && previous_label == intv->label)
+        if (previous_end > (int)(intv->start - gap))
             {
                 previous_end = MAX(previous_end, (int)intv->end);
             }
             else
             {
-                labeled_aiarray_add(merged_list, previous_start, previous_end, previous_label_name);
+                ailist_add(merged_list, previous_start, previous_end, previous_id);
                 previous_start = intv->start;
                 previous_end = intv->end;
                 previous_id = intv->id_value;
-                previous_label = intv->label;
-                previous_label_name = query_rev_label_map(ail, previous_label);
             }
-
-        // Destroy iterator
-        iter_destroy(ail_iter);
     }
 
-    // Add last interval
-    labeled_aiarray_add(merged_list, previous_start, previous_end, previous_label_name);
-
-    return merged_list;
-}
+    // Check if intervals merge
+    if (previous_end > (int)(intv->start - gap))
+        {
+            previous_end = MAX(previous_end, (int)intv->end);
+        }
+        else
+        {
+            ailist_add(merged_list, previous_start, previous_end, previous_id);
+            previous_start = intv->start;
+            previous_end = intv->end;
+            previous_id = intv->id_value;
+        }
 
+    // Destroy iterator
+    ailist_sorted_iter_destroy(ail_iter);
 
+    // Add last interval
+    ailist_add(merged_list, previous_start, previous_end, previous_id);
 
+    return merged_list;
+}
```

### Comparing `ailist-1.0.4/ailist/src/labeled_augmented_array.c` & `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c`

 * *Files 23% similar despite different names*

```diff
@@ -3,222 +3,148 @@
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
 #include "labeled_augmented_array.h"
 
 //-----------------------------------------------------------------------------
+// Queries that record intervals and index
+//=============================================================================
 
-//const int khStrInt = 33;
-//KHASH_MAP_INIT_STR(khStrInt, int32_t)
-//typedef khash_t(khStrInt) strhash_t;
-//const int khIntStr = 32;
-//KHASH_MAP_INIT_INT(khIntStr, char*)
-//typedef khash_t(khIntStr) inthash_t;
 
-//-----------------------------------------------------------------------------
-
-labeled_aiarray_t *labeled_aiarray_init(void)
-{   /* Initialize labeled_aiarray_t object */
-
-    // Initialize variables
-    labeled_aiarray_t *ail = (labeled_aiarray_t *)malloc(sizeof(labeled_aiarray_t));
-    ail->nr = 0;
-    ail->mr = 64;
-    ail->nl = 0;
-    ail->ml = 64;
-	ail->maxE = NULL;
-    ail->nc = NULL;
-    ail->lenC = NULL;
-    ail->idxC = NULL;
-    ail->id_index = NULL;
-    ail->label_map = kh_init(khStrInt);
-    ail->rev_label_map = kh_init(khIntStr);
-
-    // Initialize arrays
-    ail->interval_list = malloc(ail->mr * sizeof(labeled_interval_t));
-    ail->label_count = calloc(ail->ml, sizeof(uint32_t)); 
-    //ail->label_count[0] = 0;
-    // Initialize label ranges
-    ail->first = malloc(ail->ml * sizeof(uint32_t));
-    memset(ail->first, INT32_MAX, ail->ml * sizeof(uint32_t));
-    ail->last = malloc(ail->ml * sizeof(uint32_t));
-    memset(ail->last, 0, ail->ml * sizeof(uint32_t));
+void labeled_aiarray_query_with_index(labeled_aiarray_t *laia, const char *label_name, overlap_label_index_t *overlaps, uint32_t qs, uint32_t qe)
+{   /* Base query logic with index */
 
-    // Check if memory was allocated
-    if (ail == NULL && ail->interval_list == NULL)
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-        fprintf (stderr, "Out of memory!!! (init)\n");
-        exit(1);
+        labeled_aiarray_construct(laia, 20);
     }
 
-	return ail;
-}
-
-//-----------------------------------------------------------------------------
-
-void labeled_aiarray_destroy(labeled_aiarray_t *ail)
-{   /* Free labeled_aiarray_t object */
-
-    // Check that ail exists
-	if (ail == 0)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        return;
+        labeled_aiarray_cache_id(laia);
     }
-	
-    // Free intervals
-    if (ail->interval_list)
+    
+    // Get label
+    int32_t l = get_label(laia, label_name);
+
+    // Check if label present
+    if (l != -1)
     {
-        free(ail->interval_list);
-    }
-	
-    // Free maxE
-	if (ail->maxE)
-	{
-		free(ail->maxE);
-	}
+        label_t *p = &laia->labels[l];
 
-    // Free label_count
-    if (ail->label_count)
-	{
-		free(ail->label_count);
-	}
+        // Initialize overlaps
+        int k;
+        for (k = 0; k < p->ail->nc; k++)
+        {   // Search each component
+            int32_t cs = p->ail->idxC[k];
+            int32_t ce = cs + p->ail->lenC[k];			
+            int32_t t;
+
+            if (p->ail->lenC[k] > 15)
+            {
+                t = binary_search(p->ail->interval_list, cs, ce, qe);
+
+                while (t >= cs && p->ail->maxE[t] > qs)
+                {
+                    if (p->ail->interval_list[t].end > qs)
+                    {               	
+                        overlap_label_index_add(overlaps, p->ail->interval_list[t], label_name);
+                    }
+
+                    t--;
+                }
+            } 
+            else {
+                for (t = cs; t < ce; t++)
+                {
+                    if (p->ail->interval_list[t].start < qe && p->ail->interval_list[t].end > qs)
+                    {
+                        overlap_label_index_add(overlaps, p->ail->interval_list[t], label_name);
+                    }
+                }                      
+            }
+        }
+
+        // reallocate to remove extra memory
+        //overlaps->indices = (long *)realloc(overlaps->indices, sizeof(long) * overlaps->size);
+        //overlaps->max_size = overlaps->size;
+    }
 
-    // Free nc
-	if (ail->nc)
-	{
-		free(ail->nc);
-	}
+    return;
+}
 
-    // Free lenC
-	if (ail->lenC)
-	{
-		free(ail->lenC);
-	}
 
-    // Free idxC
-	if (ail->idxC)
-	{
-		free(ail->idxC);
-	}
+void labeled_aiarray_query_with_index_from_array(labeled_aiarray_t *laia, overlap_label_index_t *overlaps, const char label_names[], const long starts[], const long ends[], int length, int label_str_len)
+{   /* Base query logic with index */
 
-    // Free id_index
-    if (ail->id_index)
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-        free(ail->id_index);
+        labeled_aiarray_construct(laia, 20);
     }
 
-    // Free first
-    if (ail->first)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        free(ail->first);
+        labeled_aiarray_cache_id(laia);
     }
-
-    // Free last
-    if (ail->last)
+    
+    // Iterate over queries
+    int i;
+    for (i = 0; i < length; i++)
     {
-        free(ail->last);
-    }
-
-    // Free label hash table
-    kh_destroy(khStrInt, (strhash_t*)ail->label_map);
+        // Determine interval to query
+        uint32_t qs = starts[i];
+        uint32_t qe = ends[i];
+        char label_name[label_str_len + 1];
+        slice_str(label_names, label_name, (i * label_str_len), (i * label_str_len) + label_str_len);
 
-    // Free reverse label hash table
-    kh_destroy(khIntStr, (inthash_t*)ail->rev_label_map);
+        // Query interval
+        labeled_aiarray_query_with_index(laia, label_name, overlaps, qs, qe);
+    
+    }
 
-    // Free ailist
-	free(ail);
+    return;
 }
 
 
-//-----------------------------------------------------------------------------
-
+void labeled_aiarray_query_with_index_from_labeled_aiarray(labeled_aiarray_t *laia, labeled_aiarray_t *other_laia, overlap_label_index_t *overlaps)
+{   /* Query with index from labeled_aiarray */
 
-void labeled_display_list(labeled_aiarray_t *ail)
-{
-    int i;
-    for (i = 0; i < ail->nr; i++)
+    // Determine if constructed yet
+    if (laia->is_constructed == 0)
     {
-        printf("(%d-%d, %d) ", ail->interval_list[i].start, ail->interval_list[i].end, ail->interval_list[i].label);
+        labeled_aiarray_construct(laia, 20);
     }
-    printf("\n");
-    return;
-}
-
 
-void display_label_map(labeled_aiarray_t *ail)
-{
-    khiter_t k;
-    uint64_t tval;
-    khash_t(khStrInt) *h = ail->label_map;
-    for (k = kh_begin(h); k != kh_end(h); ++k)
-    {
-      if (kh_exist(h, k))
-      {
-         const char *key = kh_key(h,k);
-         tval = kh_value(h, k);
-         printf("key=%s  val=%llu\n", key, tval);
-      }
-   }
-}
-
-
-int labeled_aiarray_max_length(labeled_aiarray_t *ail)
-{   /* Calculate maximum length */
-	
-    // Iterate over intervals and record length
-    int length;
-    int maximum = 0;
-    int i;
-    for (i = 0; i < ail->nr; i++)
+    // Check index is initialized
+    if (laia->id_index == NULL)
     {
-        // Record length (excluding last position)
-        length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
-	    maximum = MAX(maximum, length);
+        labeled_aiarray_cache_id(laia);
     }
 
-    return maximum;
-}
+    // Iterate over queries
+    int t2;
+    for (t2 = 0; t2 < other_laia->n_labels; t2++)
+    {
+        label_t *p2 = &other_laia->labels[t2];
+        ailist_t *l2 = p2->ail;
+        
+        int i;
+        for (i = 0; i < l2->nr; i++)
+        {
+            // Determine interval to query
+            uint32_t qs = l2->interval_list[i].start;
+            uint32_t qe = l2->interval_list[i].end;
 
+            // Query interval
+            labeled_aiarray_query_with_index(laia, p2->name, overlaps, qs, qe);
 
-void labeled_aiarray_length_distribution(labeled_aiarray_t *ail, int distribution[])
-{   /* Calculate length distribution */
-    
-    // Iterate over intervals and record length
-    int length;
-    int i;
-    for (i = 0; i < ail->nr; i++)
-    {
-        // Record length (excluding last position)
-        length = ail->interval_list[i].end - ail->interval_list[i].start - 1;
-        distribution[length] += 1;
+        }
     }
 
     return;
 }
 
-
-int main()
-{
-    labeled_aiarray_t *ail = labeled_aiarray_init();
-    labeled_aiarray_add(ail, 1, 12, "0");
-    labeled_aiarray_add(ail, 10, 12, "0");
-    labeled_aiarray_add(ail, 1, 13, "1");
-    labeled_aiarray_add(ail, 1, 13, "2");
-    labeled_aiarray_add(ail, 1, 13, "3");
-    labeled_aiarray_add(ail, 10, 22, "0");
-    labeled_aiarray_add(ail, 1, 13, "13");
-    labeled_display_list(ail);
-
-    labeled_aiarray_construct(ail, 20);
-    labeled_display_list(ail);
-
-    printf("nl:%lld, ml:%lld\n", ail->nl, ail->ml);
-    int i;
-    for (i = 0; i < ail->ml; i++)
-    {
-        printf("index_label:%d\n", ail->label_count[i]);
-    }
-    labeled_aiarray_destroy(ail);
-
-    return 0;
-}
```

### Comparing `ailist-1.0.4/ailist/src/overlap_index.c` & `ailist-2.0.2/ailist/src/ailist/overlap_index.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //=============================================================================
 // Quick and efficient storing/querying of intervals 
 // by Kyle S. Smith and Jianglin Feng
 //
 //-----------------------------------------------------------------------------
 
-#include "augmented_interval_array.h"
+#include "augmented_interval_list.h"
 
 //-----------------------------------------------------------------------------
 
 
 overlap_index_t *overlap_index_init(void)
 {   /* Initialize overlap_index */
     
@@ -23,24 +23,24 @@
     oi->max_size = 64;
     oi->indices = (long *)malloc(sizeof(long) * 64);
     if (oi->indices == NULL)
     {
         printf("Memory allocation failed");
         exit(1); // exit the program
     }
-    oi->ail = aiarray_init();
+    oi->ail = ailist_init();
 
     return oi;
 }
 
 
 void overlap_index_destroy(overlap_index_t *oi)
 {   /* Free overlap_index memory */
 
-    aiarray_destroy(oi->ail);
+    ailist_destroy(oi->ail);
     free(oi->indices);
     free(oi);
 }
 
 
 void overlap_index_add(overlap_index_t *oi, interval_t *i)
 {   /* Add interval to overlap_index */
@@ -58,9 +58,9 @@
     }
 
     // Increment size
     oi->size++;
 
     // Add new indices
     oi->indices[oi->size-1] = i->id_value;
-    aiarray_add(oi->ail, i->start, i->end);
+    ailist_add(oi->ail, i->start, i->end, i->id_value);
 }
```

### Comparing `ailist-1.0.4/ailist/src/utilities.h` & `ailist-2.0.2/ailist/src/utilities/utilities.h`

 * *Files identical despite different names*

