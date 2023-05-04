# Comparing `tmp/ailist-2.0.2.tar.gz` & `tmp/ailist-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailist-2.0.2.tar", max compression
+gzip compressed data, was "ailist-2.1.0.tar", max compression
```

## Comparing `ailist-2.0.2.tar` & `ailist-2.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 ailist-2.0.2/LICENSE.md
--rwxr-xr-x   0        0        0     4923 2021-08-28 14:14:30.000000 ailist-2.0.2/README.md
--rw-r--r--   0        0        0   399968 2023-05-04 18:13:17.192103 ailist-2.0.2/ailist/AIList_core.cpython-310-darwin.so
--rwxr-xr-x   0        0        0    14968 2023-05-01 20:07:58.458938 ailist-2.0.2/ailist/AIList_core.pxd
--rwxr-xr-x   0        0        0    38543 2023-05-04 15:37:04.815831 ailist-2.0.2/ailist/AIList_core.pyx
--rw-r--r--   0        0        0    34745 2023-01-20 20:29:03.224385 ailist-2.0.2/ailist/IntervalArray_core.py
--rw-r--r--   0        0        0    83496 2023-05-04 18:13:17.191544 ailist-2.0.2/ailist/Interval_core.cpython-310-darwin.so
--rwxr-xr-x   0        0        0      721 2023-01-19 03:35:55.179175 ailist-2.0.2/ailist/Interval_core.pxd
--rwxr-xr-x   0        0        0     1452 2023-04-12 15:43:30.386933 ailist-2.0.2/ailist/Interval_core.pyx
--rw-r--r--   0        0        0   650384 2023-05-04 18:13:17.192531 ailist-2.0.2/ailist/LabeledIntervalArray_core.cpython-310-darwin.so
--rw-r--r--   0        0        0    28088 2023-04-24 14:57:56.149081 ailist-2.0.2/ailist/LabeledIntervalArray_core.pxd
--rw-r--r--   0        0        0    78595 2023-05-04 14:58:33.650745 ailist-2.0.2/ailist/LabeledIntervalArray_core.pyx
--rwxr-xr-x   0        0        0      536 2023-04-11 01:36:52.281521 ailist-2.0.2/ailist/__init__.py
--rw-r--r--   0        0        0    59928 2023-05-04 18:13:17.192770 ailist-2.0.2/ailist/array_query_core.cpython-310-darwin.so
--rwxr-xr-x   0        0        0     1086 2022-05-02 21:15:59.000000 ailist-2.0.2/ailist/array_query_core.pxd
--rwxr-xr-x   0        0        0     1304 2023-04-12 15:43:58.852105 ailist-2.0.2/ailist/array_query_core.pyx
--rw-r--r--   0        0        0     2228 2023-04-13 02:36:16.801973 ailist-2.0.2/ailist/src/ailist/ailist_add.c
--rw-r--r--   0        0        0     7229 2022-09-15 17:32:49.000000 ailist-2.0.2/ailist/src/ailist/ailist_construct.c
--rw-r--r--   0        0        0     5233 2023-02-10 20:43:05.058096 ailist-2.0.2/ailist/src/ailist/ailist_coverage.c
--rw-r--r--   0        0        0     1004 2021-02-01 19:00:33.000000 ailist-2.0.2/ailist/src/ailist/ailist_extract.c
--rw-r--r--   0        0        0     1582 2022-06-06 03:22:03.000000 ailist-2.0.2/ailist/src/ailist/ailist_filter.c
--rw-r--r--   0        0        0     2011 2022-06-16 14:20:03.000000 ailist-2.0.2/ailist/src/ailist/ailist_get_id.c
--rw-r--r--   0        0        0     3192 2022-07-28 20:03:17.000000 ailist-2.0.2/ailist/src/ailist/ailist_iter.c
--rw-r--r--   0        0        0     2009 2023-02-21 20:12:11.742021 ailist-2.0.2/ailist/src/ailist/ailist_merge.c
--rw-r--r--   0        0        0     2758 2022-09-07 00:38:08.000000 ailist-2.0.2/ailist/src/ailist/ailist_nhits.c
--rw-r--r--   0        0        0     5077 2023-05-04 15:00:47.219735 ailist-2.0.2/ailist/src/ailist/ailist_ops.c
--rw-r--r--   0        0        0    16745 2023-05-04 15:30:28.093848 ailist-2.0.2/ailist/src/ailist/ailist_query.c
--rw-r--r--   0        0        0     1066 2022-07-26 17:40:19.000000 ailist-2.0.2/ailist/src/ailist/ailist_simulate.c
--rw-r--r--   0        0        0     3612 2020-10-19 17:27:23.000000 ailist-2.0.2/ailist/src/ailist/ailist_wps.c
--rwxr-xr-x   0        0        0     2748 2022-09-15 14:07:25.000000 ailist-2.0.2/ailist/src/ailist/augmented_interval_list.c
--rwxr-xr-x   0        0        0    10932 2023-04-02 18:45:52.230047 ailist-2.0.2/ailist/src/ailist/augmented_interval_list.h
--rw-r--r--   0        0        0      804 2021-02-03 17:09:02.000000 ailist-2.0.2/ailist/src/ailist/interval.c
--rwxr-xr-x   0        0        0     1088 2021-02-03 17:08:42.000000 ailist-2.0.2/ailist/src/ailist/interval.h
--rwxr-xr-x   0        0        0     1714 2022-02-12 16:20:01.000000 ailist-2.0.2/ailist/src/ailist/overlap_index.c
--rwxr-xr-x   0        0        0      981 2023-01-26 15:09:47.831548 ailist-2.0.2/ailist/src/array_query/array_query_utilities.c
--rwxr-xr-x   0        0        0     2105 2023-01-26 15:08:56.094844 ailist-2.0.2/ailist/src/array_query/array_query_utilities.h
--rw-r--r--   0        0        0    21510 2021-04-26 19:06:11.000000 ailist-2.0.2/ailist/src/labeled_aiarray/khash.h
--rw-r--r--   0        0        0     2872 2023-01-25 18:17:24.561022 ailist-2.0.2/ailist/src/labeled_aiarray/kvec.h
--rw-r--r--   0        0        0     4759 2023-05-04 15:01:55.664279 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c
--rw-r--r--   0        0        0     1207 2023-05-01 20:57:05.670200 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_construct.c
--rw-r--r--   0        0        0     3846 2023-02-10 20:40:34.313629 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c
--rw-r--r--   0        0        0     1293 2022-05-11 19:58:25.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c
--rw-r--r--   0        0        0     2333 2023-02-01 22:05:01.741865 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c
--rw-r--r--   0        0        0     6944 2023-05-02 02:19:37.520386 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c
--rw-r--r--   0        0        0     6160 2023-02-09 21:43:40.683985 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c
--rw-r--r--   0        0        0     4160 2023-02-26 21:23:15.841726 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_iter.c
--rw-r--r--   0        0        0     9856 2023-05-02 02:17:46.112410 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_match.c
--rw-r--r--   0        0        0      937 2022-05-11 16:24:30.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_merge.c
--rw-r--r--   0        0        0     7199 2023-02-10 20:45:56.368299 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c
--rw-r--r--   0        0        0     2424 2023-05-04 14:53:06.390402 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_ops.c
--rw-r--r--   0        0        0     1956 2023-02-26 21:24:15.672922 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c
--rw-r--r--   0        0        0     5350 2023-01-26 15:10:01.828428 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c
--rw-r--r--   0        0        0     4338 2023-05-02 02:17:29.334654 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c
--rw-r--r--   0        0        0     6240 2023-01-25 16:50:52.952858 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c
--rw-r--r--   0        0        0     1013 2022-07-26 19:33:03.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c
--rw-r--r--   0        0        0     2210 2023-03-22 14:45:22.854467 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_sort.c
--rw-r--r--   0        0        0     1299 2022-05-02 16:48:19.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_wps.c
--rw-r--r--   0        0        0     5281 2022-09-14 17:13:56.000000 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.c
--rwxr-xr-x   0        0        0    20345 2023-05-02 02:18:45.419047 ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.h
--rwxr-xr-x   0        0        0     2298 2023-05-02 02:18:32.335127 ailist-2.0.2/ailist/src/labeled_aiarray/overlap_label_index.c
--rwxr-xr-x   0        0        0     3103 2021-02-20 22:03:14.000000 ailist-2.0.2/ailist/src/utilities/utilities.h
--rw-r--r--   0        0        0     3447 2023-04-12 15:10:52.847444 ailist-2.0.2/build.py
--rw-r--r--   0        0        0     2109 2023-04-13 02:24:05.892680 ailist-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ailist-2.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 ailist-2.1.0/LICENSE.md
+-rwxr-xr-x   0        0        0     4923 2021-08-28 14:14:30.000000 ailist-2.1.0/README.md
+-rw-r--r--   0        0        0   399968 2023-05-04 19:22:21.913054 ailist-2.1.0/ailist/AIList_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0    14968 2023-05-01 20:07:58.458938 ailist-2.1.0/ailist/AIList_core.pxd
+-rwxr-xr-x   0        0        0    38543 2023-05-04 15:37:04.815831 ailist-2.1.0/ailist/AIList_core.pyx
+-rw-r--r--   0        0        0    34745 2023-01-20 20:29:03.224385 ailist-2.1.0/ailist/IntervalArray_core.py
+-rw-r--r--   0        0        0    83496 2023-05-04 19:22:21.912564 ailist-2.1.0/ailist/Interval_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0      721 2023-01-19 03:35:55.179175 ailist-2.1.0/ailist/Interval_core.pxd
+-rwxr-xr-x   0        0        0     1452 2023-04-12 15:43:30.386933 ailist-2.1.0/ailist/Interval_core.pyx
+-rw-r--r--   0        0        0   650384 2023-05-04 19:22:21.913549 ailist-2.1.0/ailist/LabeledIntervalArray_core.cpython-310-darwin.so
+-rw-r--r--   0        0        0    28088 2023-04-24 14:57:56.149081 ailist-2.1.0/ailist/LabeledIntervalArray_core.pxd
+-rw-r--r--   0        0        0    78595 2023-05-04 14:58:33.650745 ailist-2.1.0/ailist/LabeledIntervalArray_core.pyx
+-rwxr-xr-x   0        0        0      536 2023-05-04 19:31:37.426820 ailist-2.1.0/ailist/__init__.py
+-rw-r--r--   0        0        0    59928 2023-05-04 19:22:21.913772 ailist-2.1.0/ailist/array_query_core.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0     1086 2022-05-02 21:15:59.000000 ailist-2.1.0/ailist/array_query_core.pxd
+-rwxr-xr-x   0        0        0     1304 2023-04-12 15:43:58.852105 ailist-2.1.0/ailist/array_query_core.pyx
+-rw-r--r--   0        0        0     2228 2023-04-13 02:36:16.801973 ailist-2.1.0/ailist/src/ailist/ailist_add.c
+-rw-r--r--   0        0        0     7229 2022-09-15 17:32:49.000000 ailist-2.1.0/ailist/src/ailist/ailist_construct.c
+-rw-r--r--   0        0        0     5233 2023-02-10 20:43:05.058096 ailist-2.1.0/ailist/src/ailist/ailist_coverage.c
+-rw-r--r--   0        0        0     1004 2021-02-01 19:00:33.000000 ailist-2.1.0/ailist/src/ailist/ailist_extract.c
+-rw-r--r--   0        0        0     1582 2022-06-06 03:22:03.000000 ailist-2.1.0/ailist/src/ailist/ailist_filter.c
+-rw-r--r--   0        0        0     2011 2022-06-16 14:20:03.000000 ailist-2.1.0/ailist/src/ailist/ailist_get_id.c
+-rw-r--r--   0        0        0     3192 2022-07-28 20:03:17.000000 ailist-2.1.0/ailist/src/ailist/ailist_iter.c
+-rw-r--r--   0        0        0     2009 2023-02-21 20:12:11.742021 ailist-2.1.0/ailist/src/ailist/ailist_merge.c
+-rw-r--r--   0        0        0     2758 2022-09-07 00:38:08.000000 ailist-2.1.0/ailist/src/ailist/ailist_nhits.c
+-rw-r--r--   0        0        0     5077 2023-05-04 15:00:47.219735 ailist-2.1.0/ailist/src/ailist/ailist_ops.c
+-rw-r--r--   0        0        0    16745 2023-05-04 15:30:28.093848 ailist-2.1.0/ailist/src/ailist/ailist_query.c
+-rw-r--r--   0        0        0     1066 2022-07-26 17:40:19.000000 ailist-2.1.0/ailist/src/ailist/ailist_simulate.c
+-rw-r--r--   0        0        0     3612 2020-10-19 17:27:23.000000 ailist-2.1.0/ailist/src/ailist/ailist_wps.c
+-rwxr-xr-x   0        0        0     2748 2022-09-15 14:07:25.000000 ailist-2.1.0/ailist/src/ailist/augmented_interval_list.c
+-rwxr-xr-x   0        0        0    10932 2023-04-02 18:45:52.230047 ailist-2.1.0/ailist/src/ailist/augmented_interval_list.h
+-rw-r--r--   0        0        0      804 2021-02-03 17:09:02.000000 ailist-2.1.0/ailist/src/ailist/interval.c
+-rwxr-xr-x   0        0        0     1088 2021-02-03 17:08:42.000000 ailist-2.1.0/ailist/src/ailist/interval.h
+-rwxr-xr-x   0        0        0     1714 2022-02-12 16:20:01.000000 ailist-2.1.0/ailist/src/ailist/overlap_index.c
+-rwxr-xr-x   0        0        0      981 2023-01-26 15:09:47.831548 ailist-2.1.0/ailist/src/array_query/array_query_utilities.c
+-rwxr-xr-x   0        0        0     2105 2023-01-26 15:08:56.094844 ailist-2.1.0/ailist/src/array_query/array_query_utilities.h
+-rw-r--r--   0        0        0    21510 2021-04-26 19:06:11.000000 ailist-2.1.0/ailist/src/labeled_aiarray/khash.h
+-rw-r--r--   0        0        0     2872 2023-01-25 18:17:24.561022 ailist-2.1.0/ailist/src/labeled_aiarray/kvec.h
+-rw-r--r--   0        0        0     4759 2023-05-04 15:01:55.664279 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_add.c
+-rw-r--r--   0        0        0     1207 2023-05-01 20:57:05.670200 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_construct.c
+-rw-r--r--   0        0        0     3846 2023-02-10 20:40:34.313629 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c
+-rw-r--r--   0        0        0     1293 2022-05-11 19:58:25.000000 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_extract.c
+-rw-r--r--   0        0        0     2333 2023-02-01 22:05:01.741865 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_filter.c
+-rw-r--r--   0        0        0     6944 2023-05-02 02:19:37.520386 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_get.c
+-rw-r--r--   0        0        0     6160 2023-02-09 21:43:40.683985 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_index.c
+-rw-r--r--   0        0        0     4160 2023-02-26 21:23:15.841726 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_iter.c
+-rw-r--r--   0        0        0     9856 2023-05-02 02:17:46.112410 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_match.c
+-rw-r--r--   0        0        0      937 2022-05-11 16:24:30.000000 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_merge.c
+-rw-r--r--   0        0        0     7199 2023-02-10 20:45:56.368299 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c
+-rw-r--r--   0        0        0     2424 2023-05-04 14:53:06.390402 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_ops.c
+-rw-r--r--   0        0        0     1956 2023-02-26 21:24:15.672922 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_percent.c
+-rw-r--r--   0        0        0     5350 2023-01-26 15:10:01.828428 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c
+-rw-r--r--   0        0        0     4338 2023-05-02 02:17:29.334654 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c
+-rw-r--r--   0        0        0     6240 2023-01-25 16:50:52.952858 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c
+-rw-r--r--   0        0        0     1013 2022-07-26 19:33:03.000000 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c
+-rw-r--r--   0        0        0     2210 2023-03-22 14:45:22.854467 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_sort.c
+-rw-r--r--   0        0        0     1299 2022-05-02 16:48:19.000000 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_wps.c
+-rw-r--r--   0        0        0     5281 2022-09-14 17:13:56.000000 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_augmented_array.c
+-rwxr-xr-x   0        0        0    20345 2023-05-02 02:18:45.419047 ailist-2.1.0/ailist/src/labeled_aiarray/labeled_augmented_array.h
+-rwxr-xr-x   0        0        0     2298 2023-05-02 02:18:32.335127 ailist-2.1.0/ailist/src/labeled_aiarray/overlap_label_index.c
+-rwxr-xr-x   0        0        0     3103 2021-02-20 22:03:14.000000 ailist-2.1.0/ailist/src/utilities/utilities.h
+-rw-r--r--   0        0        0     3447 2023-04-12 15:10:52.847444 ailist-2.1.0/build.py
+-rw-r--r--   0        0        0     2109 2023-05-04 19:31:43.816043 ailist-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ailist-2.1.0/PKG-INFO
```

### Comparing `ailist-2.0.2/LICENSE.md` & `ailist-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/README.md` & `ailist-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/AIList_core.cpython-310-darwin.so` & `ailist-2.1.0/ailist/AIList_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/AIList_core.pxd` & `ailist-2.1.0/ailist/AIList_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/AIList_core.pyx` & `ailist-2.1.0/ailist/AIList_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/IntervalArray_core.py` & `ailist-2.1.0/ailist/IntervalArray_core.py`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/Interval_core.cpython-310-darwin.so` & `ailist-2.1.0/ailist/Interval_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/Interval_core.pxd` & `ailist-2.1.0/ailist/Interval_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/Interval_core.pyx` & `ailist-2.1.0/ailist/Interval_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/LabeledIntervalArray_core.cpython-310-darwin.so` & `ailist-2.1.0/ailist/LabeledIntervalArray_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/LabeledIntervalArray_core.pxd` & `ailist-2.1.0/ailist/LabeledIntervalArray_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/LabeledIntervalArray_core.pyx` & `ailist-2.1.0/ailist/LabeledIntervalArray_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/__init__.py` & `ailist-2.1.0/ailist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 from .AIList_core import AIList
 from .IntervalArray_core import IntervalArray
 from .Interval_core import Interval
 from .LabeledIntervalArray_core import LabeledIntervalArray, LabeledInterval, get_include
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '2.0.1'
+__version__ = '2.1.0'
 __author__ = "Kyle S. Smith"
 
 
 __doc__ = """\
 API
 ======
```

### Comparing `ailist-2.0.2/ailist/array_query_core.cpython-310-darwin.so` & `ailist-2.1.0/ailist/array_query_core.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/array_query_core.pxd` & `ailist-2.1.0/ailist/array_query_core.pxd`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/array_query_core.pyx` & `ailist-2.1.0/ailist/array_query_core.pyx`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_add.c` & `ailist-2.1.0/ailist/src/ailist/ailist_add.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_construct.c` & `ailist-2.1.0/ailist/src/ailist/ailist_construct.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_coverage.c` & `ailist-2.1.0/ailist/src/ailist/ailist_coverage.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_extract.c` & `ailist-2.1.0/ailist/src/ailist/ailist_extract.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_filter.c` & `ailist-2.1.0/ailist/src/ailist/ailist_filter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_get_id.c` & `ailist-2.1.0/ailist/src/ailist/ailist_get_id.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_iter.c` & `ailist-2.1.0/ailist/src/ailist/ailist_iter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_merge.c` & `ailist-2.1.0/ailist/src/ailist/ailist_merge.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_nhits.c` & `ailist-2.1.0/ailist/src/ailist/ailist_nhits.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_ops.c` & `ailist-2.1.0/ailist/src/ailist/ailist_ops.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_query.c` & `ailist-2.1.0/ailist/src/ailist/ailist_query.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_simulate.c` & `ailist-2.1.0/ailist/src/ailist/ailist_simulate.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/ailist_wps.c` & `ailist-2.1.0/ailist/src/ailist/ailist_wps.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/augmented_interval_list.c` & `ailist-2.1.0/ailist/src/ailist/augmented_interval_list.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/augmented_interval_list.h` & `ailist-2.1.0/ailist/src/ailist/augmented_interval_list.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/interval.c` & `ailist-2.1.0/ailist/src/ailist/interval.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/interval.h` & `ailist-2.1.0/ailist/src/ailist/interval.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/ailist/overlap_index.c` & `ailist-2.1.0/ailist/src/ailist/overlap_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/array_query/array_query_utilities.c` & `ailist-2.1.0/ailist/src/array_query/array_query_utilities.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/array_query/array_query_utilities.h` & `ailist-2.1.0/ailist/src/array_query/array_query_utilities.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/khash.h` & `ailist-2.1.0/ailist/src/labeled_aiarray/khash.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/kvec.h` & `ailist-2.1.0/ailist/src/labeled_aiarray/kvec.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_add.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_add.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_construct.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_construct.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_extract.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_extract.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_filter.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_filter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_get.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_get.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_index.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_iter.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_iter.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_match.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_match.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_merge.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_merge.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_ops.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_ops.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_percent.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_percent.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_sort.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_sort.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_aiarray_wps.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_aiarray_wps.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_augmented_array.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/labeled_augmented_array.h` & `ailist-2.1.0/ailist/src/labeled_aiarray/labeled_augmented_array.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/labeled_aiarray/overlap_label_index.c` & `ailist-2.1.0/ailist/src/labeled_aiarray/overlap_label_index.c`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/ailist/src/utilities/utilities.h` & `ailist-2.1.0/ailist/src/utilities/utilities.h`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/build.py` & `ailist-2.1.0/build.py`

 * *Files identical despite different names*

### Comparing `ailist-2.0.2/pyproject.toml` & `ailist-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailist"
-version = "2.0.2"
+version = "2.1.0"
 description = "Python package for Augmented Interval List"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/ailist"
 documentation = "https://www.biosciencestack.com/static/ailist/docs/index.html"
 keywords = ["cython", "interval", "ailist", "c"]
 readme = 'README.md'
```

### Comparing `ailist-2.0.2/PKG-INFO` & `ailist-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailist
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python package for Augmented Interval List
 Home-page: https://github.com/kylessmith/ailist
 License: GPL-2.0-or-later
 Keywords: cython,interval,ailist,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
```

