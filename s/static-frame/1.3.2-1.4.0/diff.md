# Comparing `tmp/static-frame-1.3.2.tar.gz` & `tmp/static-frame-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.3.2.tar", last modified: Tue May  2 23:46:44 2023, max compression
+gzip compressed data, was "static-frame-1.4.0.tar", last modified: Thu May  4 19:41:21 2023, max compression
```

## Comparing `static-frame-1.3.2.tar` & `static-frame-1.4.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.452348 static-frame-1.3.2/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.3.2/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.3.2/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-05-02 23:46:44.452348 static-frame-1.3.2/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23552 2023-05-02 20:45:20.000000 static-frame-1.3.2/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.3.2/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      362 2023-05-02 20:45:20.000000 static-frame-1.3.2/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       45 2023-05-02 20:45:20.000000 static-frame-1.3.2/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-02 23:46:44.452348 static-frame-1.3.2/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.3.2/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.432184 static-frame-1.3.2/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7595 2023-05-02 20:42:21.000000 static-frame-1.3.2/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.444283 static-frame-1.3.2/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   379745 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    57244 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21195 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107621 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24028 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   185868 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   128558 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.444283 static-frame-1.3.2/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.452348 static-frame-1.3.2/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   640988 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    63780 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1394 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41685 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19542 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16278 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23360 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47630 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.436217 static-frame-1.3.2/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      199 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.711680 static-frame-1.4.0/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.0/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.0/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-04 19:41:21.711680 static-frame-1.4.0/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-04 17:09:05.000000 static-frame-1.4.0/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.0/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-04 17:09:05.000000 static-frame-1.4.0/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-04 17:09:05.000000 static-frame-1.4.0/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-04 19:41:21.711680 static-frame-1.4.0/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.0/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.683680 static-frame-1.4.0/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-04 17:34:51.000000 static-frame-1.4.0/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.695680 static-frame-1.4.0/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   379744 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   185868 2023-05-03 15:14:12.000000 static-frame-1.4.0/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   128804 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.695680 static-frame-1.4.0/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.707680 static-frame-1.4.0/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.0/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   641142 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23361 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.0/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.4.0/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.4.0/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.4.0/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.0/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-04 19:41:21.683680 static-frame-1.4.0/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-04 19:41:21.000000 static-frame-1.4.0/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.3.2/LICENSE.txt` & `static-frame-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/PKG-INFO` & `static-frame-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.3.2
+Version: 1.4.0
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -45,15 +45,15 @@
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
-        - automap==0.6.2
+        - arraymap==0.1.7
         - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
```

### Comparing `static-frame-1.3.2/README.rst` & `static-frame-1.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 Dependencies
 --------------
 
 Core StaticFrame requires the following:
 
 - Python>=3.7
 - NumPy>=1.18.5
-- automap==0.6.2
+- arraymap==0.1.7
 - arraykit==0.3.4
 
 For extended input and output, the following packages are required:
 
 - pandas>=0.24.2
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
```

### Comparing `static-frame-1.3.2/setup.py` & `static-frame-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/__init__.py` & `static-frame-1.4.0/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 from static_frame.core.node_iter import IterNodeType as IterNodeType
 from static_frame.core.node_iter import IterNodeWindow
 from static_frame.core.node_re import InterfaceRe
 from static_frame.core.node_selector import InterfaceAssignQuartet
 from static_frame.core.node_selector import InterfaceAssignTrio
 from static_frame.core.node_selector import InterfaceAsType
 from static_frame.core.node_selector import InterfaceBatchAsType
+from static_frame.core.node_selector import InterfaceConsolidate
 from static_frame.core.node_selector import InterfaceGetItem as InterfaceGetItem
 from static_frame.core.node_selector import InterfaceSelectDuo
 from static_frame.core.node_selector import InterfaceSelectQuartet
 from static_frame.core.node_selector import InterfaceSelectTrio
 from static_frame.core.node_str import InterfaceBatchString
 from static_frame.core.node_str import InterfaceString
 from static_frame.core.node_transpose import InterfaceBatchTranspose
@@ -114,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.3.2'
+__version__ = '1.4.0'
```

### Comparing `static-frame-1.3.2/static_frame/__main__.py` & `static-frame-1.4.0/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/archive_npy.py` & `static-frame-1.4.0/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/axis_map.py` & `static-frame-1.4.0/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/batch.py` & `static-frame-1.4.0/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/bus.py` & `static-frame-1.4.0/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/container.py` & `static-frame-1.4.0/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/container_util.py` & `static-frame-1.4.0/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/display.py` & `static-frame-1.4.0/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/display_color.py` & `static-frame-1.4.0/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/display_config.py` & `static-frame-1.4.0/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/display_html_datatables.py` & `static-frame-1.4.0/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/display_visidata.py` & `static-frame-1.4.0/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/doc_str.py` & `static-frame-1.4.0/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/exception.py` & `static-frame-1.4.0/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/fill_value_auto.py` & `static-frame-1.4.0/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/frame.py` & `static-frame-1.4.0/static_frame/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,14 @@
                         index = index_to_frame,
                         index_constructor=index_constructor_to_frame,
                         columns=columns_to_frame,
                         columns_constructor=columns_constructor_to_frame,
                         ))
         own_index = False
         own_columns = False
-
         if not frame_seq:
             return cls(
                     index=index,
                     columns=columns,
                     name=name,
                     own_columns=own_columns,
                     own_index=own_index,
```

### Comparing `static-frame-1.3.2/static_frame/core/hloc.py` & `static-frame-1.4.0/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/index.py` & `static-frame-1.4.0/static_frame/core/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import numpy as np
 from arraykit import array_deepcopy
 from arraykit import immutable_filter
 from arraykit import mloc
 from arraykit import name_filter
 from arraykit import resolve_dtype
-from automap import AutoMap  # pylint: disable=E0611
-from automap import FrozenAutoMap  # pylint: disable=E0611
-from automap import NonUniqueError  # pylint: disable=E0611
+from arraymap import AutoMap  # pylint: disable=E0611
+from arraymap import FrozenAutoMap  # pylint: disable=E0611
+from arraymap import NonUniqueError  # pylint: disable=E0611
 
 from static_frame.core.container import ContainerOperand
 from static_frame.core.container_util import apply_binary_operator
 from static_frame.core.container_util import iter_component_signature_bytes
 from static_frame.core.container_util import key_from_container_key
 from static_frame.core.container_util import matmul
 from static_frame.core.container_util import sort_index_for_order
@@ -36,21 +36,21 @@
 from static_frame.core.node_re import InterfaceRe
 from static_frame.core.node_selector import InterfaceGetItem
 from static_frame.core.node_selector import InterfaceSelectDuo
 from static_frame.core.node_selector import TContainer
 from static_frame.core.node_str import InterfaceString
 from static_frame.core.node_values import InterfaceValues
 from static_frame.core.style_config import StyleConfig
+# from static_frame.core.util import DTYPE_OBJECTABLE_KINDS
 from static_frame.core.util import DEFAULT_SORT_KIND
 from static_frame.core.util import DTYPE_BOOL
 from static_frame.core.util import DTYPE_DATETIME_KIND
 from static_frame.core.util import DTYPE_INT_DEFAULT
 from static_frame.core.util import DTYPE_NA_KINDS
 from static_frame.core.util import DTYPE_OBJECT
-from static_frame.core.util import DTYPE_OBJECTABLE_KINDS
 from static_frame.core.util import EMPTY_ARRAY
 from static_frame.core.util import INT_TYPES
 from static_frame.core.util import KEY_ITERABLE_TYPES
 from static_frame.core.util import NAME_DEFAULT
 from static_frame.core.util import NULL_SLICE
 from static_frame.core.util import DepthLevelSpecifier
 from static_frame.core.util import DtypeSpecifier
@@ -198,15 +198,16 @@
             mapping: Can be None if loc_is_iloc.
             labels: might be an expired Generator, but if it is an immutable ndarray, we can use it without a copy.
         '''
         # pre-fetching labels for faster get_item construction
         if labels.__class__ is np.ndarray:
             if dtype is not None and dtype != labels.dtype: #type: ignore
                 raise ErrorInitIndex('invalid label dtype for this Index')
-            return immutable_filter(labels)
+            # NOTE: all labels arrays should be made immutable before this call
+            return labels
 
         # labels may be an expired generator, must use the mapping
         labels_src = labels if hasattr(labels, '__len__') else mapping
 
         if len(labels_src) == 0: #type: ignore
             if dtype is None:
                 labels = EMPTY_ARRAY
@@ -240,23 +241,27 @@
         '''
         Construct an ``Index`` from an iterable of labels, where each label is a hashable. Provided for a compatible interface to ``IndexHierarchy``.
         '''
         return cls(labels, name=name)
 
 
     @staticmethod
-    def _error_init_index_non_unique(labels: tp.Iterable[tp.Hashable]) -> ErrorInitIndexNonUnique:
+    def _error_init_index_non_unique(
+            labels: tp.Sequence[tp.Hashable],
+            ) -> ErrorInitIndexNonUnique:
+        '''Return an exception configured with an informative message.
+        '''
+        msg = ''
         labels_counter = Counter(labels)
         if len(labels_counter) == 0: # generator consumed
-            msg = 'Labels have non-unique values. Details from iterators not available.'
+            msg = 'Labels have non-unique values. Examples from iterators not are available.'
         else:
             labels_all = sum(labels_counter.values())
             labels_duplicated = [repr(p[0]) for p in labels_counter.most_common(10) if p[1] > 1]
             msg = f'Labels have {labels_all - len(labels_counter)} non-unique values, including {", ".join(labels_duplicated)}.'
-
         return ErrorInitIndexNonUnique(msg)
 
     #---------------------------------------------------------------------------
     @doc_inject(selector='index_init')
     def __init__(self,
             labels: IndexInitializer,
             *,
@@ -282,18 +287,18 @@
             if is_typed and dtype != self._DTYPE:
                 # NOTE: should never get to this branch, as derived Index classes that set _DTYPE remove dtype from __init__
                 raise ErrorInitIndex('invalid dtype argument for this Index', dtype, self._DTYPE) #pragma: no cover
             # self._DTYPE is None, passed dtype is not None, use dtype
             dtype_extract = dtype
 
         #-----------------------------------------------------------------------
-        # handle all Index subclasses
         if labels.__class__ is np.ndarray:
-            pass
+            labels = immutable_filter(labels)
         elif isinstance(labels, IndexBase):
+            # handle all Index subclasses
             if labels._recache:
                 labels._update_array_cache()
             if name is NAME_DEFAULT:
                 name = labels.name # immutable, so no copy necessary
 
             if labels.depth == 1: # not an IndexHierarchy
                 if (labels.STATIC and self.STATIC and dtype is None):
@@ -317,45 +322,34 @@
                 labels = array2d_to_tuples(array)
         # else: assume an iterable suitable for labels usage, we will identify strings later
 
         #-----------------------------------------------------------------------
         if is_typed:
             # do not need to check arrays, as will and checked to match dtype_extract in _extract_labels
             if not labels.__class__ is np.ndarray:
-                # for now, assume that if _DTYPE is defined, we have a date
+                # if is_typed, _DTYPE is defined, we have a date
                 labels = (to_datetime64(v, dtype_extract) for v in labels)
             # coerce to target type
             elif labels.dtype != dtype_extract: #type: ignore
                 labels = labels.astype(dtype_extract) #type: ignore
                 labels.flags.writeable = False #type: ignore
-            labels_for_automap = labels
 
         self._name = None if name is NAME_DEFAULT else name_filter(name)
 
         if self._map is None: # if _map not shared from another Index
             if not loc_is_iloc:
-                # PERF: calling tolist before initializing AutoMap is shown to be about 2x faster, but can only be done with NumPy dtypes that are equivalent after conversion to Python objects
-                if not is_typed:
-                    if labels.__class__ is np.ndarray and labels.dtype.kind in DTYPE_OBJECTABLE_KINDS: #type: ignore
-                        labels_for_automap = labels.tolist() #type: ignore
-                    elif isinstance(labels, str):
-                        # NOTE: this is necessary as otherwise a malformed Index will be created, whereby the _map will treat the string as an iterable of chars, while the labels will not and have a single string value. This is consisten as other elements (ints, Booleans) are rejected on instantiation of the AutoMap
-                        raise ErrorInitIndex('Cannot create an Index from a single string; provide an iterable of strings.')
-                    else:
-                        labels_for_automap = labels
-                else:
-                    labels_for_automap = labels
-
+                if isinstance(labels, str):
+                    # NOTE: this is necessary as otherwise a malformed Index will be created, whereby the _map will treat the string as an iterable of chars, while the labels will not and have a single string value. This is consisten as other elements (ints, Booleans) are rejected on instantiation of the AutoMap
+                    raise ErrorInitIndex('Cannot create an Index from a single string; provide an iterable of strings.')
                 try:
-                    self._map = FrozenAutoMap(labels_for_automap) if self.STATIC else AutoMap(labels_for_automap)
+                    self._map = FrozenAutoMap(labels) if self.STATIC else AutoMap(labels)
                 except NonUniqueError: # Automap will raise ValueError of non-unique values are encountered
-                    raise self._error_init_index_non_unique(labels_for_automap) from None
+                    raise self._error_init_index_non_unique(labels) from None
                 # must take length after map as might be iterator
                 size = len(self._map)
-
             else:
                 # if loc_is_iloc, labels must be positions and we assume that internal clients that provided loc_is_iloc will not give a generator
                 size = len(labels) #type: ignore
                 if positions is None:
                     positions = labels
         else: # map shared from another Index
             size = len(self._map)
@@ -1428,15 +1422,15 @@
             mapping: tp.Optional[tp.Dict[tp.Hashable, int]],
             labels: np.ndarray,
             dtype: tp.Optional[np.dtype] = None
             ) -> np.ndarray:
         '''Called in Index.__init__(). This creates and populates mutable storage as a side effect of array derivation; this storage will be grown as needed.
         '''
         labels = Index._extract_labels(mapping, labels, dtype)
-        self._labels_mutable = labels.tolist()
+        self._labels_mutable = labels.tolist() # must get a fresh list
         if len(labels):
             self._labels_mutable_dtype = labels.dtype
         else: # avoid setting to float default when labels is empty
             self._labels_mutable_dtype = None
         return labels
 
     def _extract_positions(self,
```

### Comparing `static-frame-1.3.2/static_frame/core/index_auto.py` & `static-frame-1.4.0/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/index_base.py` & `static-frame-1.4.0/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/index_correspondence.py` & `static-frame-1.4.0/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/index_datetime.py` & `static-frame-1.4.0/static_frame/core/index_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import typing as tp
 from functools import partial
 
 import numpy as np
-from automap import AutoMap  # pylint: disable = E0611
+from arraymap import AutoMap  # pylint: disable = E0611
 
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.exception import InvalidDatetime64Initializer
 from static_frame.core.exception import LocInvalid
 from static_frame.core.index import INDEX_GO_LEAF_SLOTS
 from static_frame.core.index import Index
 from static_frame.core.index import IndexGO
```

### Comparing `static-frame-1.3.2/static_frame/core/index_hierarchy.py` & `static-frame-1.4.0/static_frame/core/index_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,19 +379,19 @@
         indices = [] # store in a list, where index is depth
 
         index_constructors_iter = cls._build_index_constructors(
                 index_constructors=index_constructors,
                 depth=len(levels),
                 )
 
-        for lvl, constructor in zip(levels, index_constructors_iter):
-            if isinstance(lvl, Index):
-                indices.append(immutable_index_filter(lvl))
+        for level, constructor in zip(levels, index_constructors_iter):
+            if isinstance(level, Index):
+                indices.append(immutable_index_filter(level))
             else:
-                indices.append(constructor(lvl))
+                indices.append(constructor(level))
 
         if name is None:
             name = cls._build_name_from_indices(indices)
 
         indexers = build_indexers_from_product(list(map(len, indices)))
 
         return cls(
@@ -2286,17 +2286,20 @@
                 # Index could be [A, B, C]
                 # Indexers could be [2, 0, 0, 2, 1]
                 # This function return [C, A, B] -- shoutout to my initials
                 # get the outer level, or just the unique frame labels needed
                 labels = self.values_at_depth(pos)
                 label_indexes = ufunc_unique1d_positions(labels)[0]
                 label_indexes.sort()
-                return labels[label_indexes]
+                array = labels[label_indexes]
+            else:
+                array = self._indices[pos].values
 
-            return self._indices[pos].values
+            array.flags.writeable = False
+            return array
 
         if order_by_occurrence:
             raise NotImplementedError('order_by_occurrence not implemented for multiple depth levels.')
 
         return ufunc_unique(array2d_to_array1d(self.values_at_depth(sel)))
 
     @doc_inject()
```

### Comparing `static-frame-1.3.2/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.0/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/interface.py` & `static-frame-1.4.0/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/interface_meta.py` & `static-frame-1.4.0/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/join.py` & `static-frame-1.4.0/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/loc_map.py` & `static-frame-1.4.0/static_frame/core/loc_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import typing as tp
 from copy import deepcopy
 from functools import reduce
 
 import numpy as np
 from arraykit import array_deepcopy
 from arraykit import first_true_1d
-from automap import FrozenAutoMap  # pylint: disable = E0611
-from automap import NonUniqueError  # pylint: disable=E0611
+from arraymap import FrozenAutoMap  # pylint: disable = E0611
+from arraymap import NonUniqueError  # pylint: disable=E0611
 
 from static_frame.core.exception import ErrorInitIndexNonUnique
 from static_frame.core.exception import LocEmpty
 from static_frame.core.exception import LocInvalid
 from static_frame.core.util import DTYPE_BOOL
 from static_frame.core.util import DTYPE_DATETIME_KIND
 from static_frame.core.util import DTYPE_OBJECT
@@ -115,15 +115,15 @@
                 if field is SLICE_STOP_ATTR:
                     # loc selections are inclusive, so iloc gets one more
                     pos += 1
                 yield pos
 
     @classmethod
     def loc_to_iloc(cls, *,
-            label_to_pos: tp.Dict[tp.Hashable, int],
+            label_to_pos: FrozenAutoMap,
             labels: np.ndarray,
             positions: np.ndarray,
             key: GetItemKeyType,
             partial_selection: bool = False,
             ) -> GetItemKeyType:
         '''
         Note: all SF objects (Series, Index) need to be converted to basic types before being passed as `key` to this function.
@@ -136,15 +136,15 @@
         # NOTE: ILoc is handled prior to this call, in the Index._loc_to_iloc method
 
         if key.__class__ is slice:
             if key == NULL_SLICE:
                 return NULL_SLICE
             try:
                 return slice(*cls.map_slice_args(
-                        label_to_pos.get, #type: ignore
+                        label_to_pos.get,
                         key,
                         labels)
                         )
             except LocEmpty:
                 return EMPTY_SLICE
 
         labels_is_dt64 = labels.dtype.kind == DTYPE_DATETIME_KIND
@@ -183,21 +183,20 @@
                     key = reduce(OPERATORS['__or__'], (labels_ref == k for k in key)) # type: ignore
 
             if is_array and key.dtype == DTYPE_BOOL: #type: ignore
                 return positions[key]
 
             # map labels to integer positions, return a list of integer positions
             # NOTE: we may miss the opportunity to identify contiguous keys and extract a slice
-            # NOTE: we do more branching here to optimize performance
             if partial_selection:
-                return [label_to_pos[k] for k in key if k in label_to_pos] # type: ignore
-            return [label_to_pos[k] for k in key] # type: ignore
+                return label_to_pos.get_any(key)
+            return label_to_pos.get_all(key)
 
         # if a single element (an integer, string, or date, we just get the integer out of the map
-        return label_to_pos[key] #type: ignore
+        return label_to_pos[key]
 
 
 class HierarchicalLocMap:
     '''
     A utility utilized by IndexHierarchy in order to quickly map keys to ilocs.
     '''
```

### Comparing `static-frame-1.3.2/static_frame/core/memory_measure.py` & `static-frame-1.4.0/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_dt.py` & `static-frame-1.4.0/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_fill_value.py` & `static-frame-1.4.0/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_hashlib.py` & `static-frame-1.4.0/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_iter.py` & `static-frame-1.4.0/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_re.py` & `static-frame-1.4.0/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_selector.py` & `static-frame-1.4.0/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_str.py` & `static-frame-1.4.0/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_transpose.py` & `static-frame-1.4.0/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/node_values.py` & `static-frame-1.4.0/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/pivot.py` & `static-frame-1.4.0/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/platform.py` & `static-frame-1.4.0/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/protocol_dfi.py` & `static-frame-1.4.0/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.0/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/quilt.py` & `static-frame-1.4.0/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/rank.py` & `static-frame-1.4.0/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/series.py` & `static-frame-1.4.0/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store.py` & `static-frame-1.4.0/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_client_mixin.py` & `static-frame-1.4.0/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_config.py` & `static-frame-1.4.0/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_filter.py` & `static-frame-1.4.0/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_hdf5.py` & `static-frame-1.4.0/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_sqlite.py` & `static-frame-1.4.0/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_xlsx.py` & `static-frame-1.4.0/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/store_zip.py` & `static-frame-1.4.0/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/style_config.py` & `static-frame-1.4.0/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/type_blocks.py` & `static-frame-1.4.0/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/util.py` & `static-frame-1.4.0/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 import numpy as np
 from arraykit import column_2d_filter
 from arraykit import first_true_1d
 from arraykit import isna_element
 from arraykit import mloc
 from arraykit import resolve_dtype
-from automap import FrozenAutoMap  # pylint: disable = E0611
+from arraymap import FrozenAutoMap  # pylint: disable = E0611
 
 from static_frame.core.exception import ErrorNotTruthy
 from static_frame.core.exception import InvalidDatetime64Comparison
 from static_frame.core.exception import InvalidDatetime64Initializer
 from static_frame.core.exception import LocInvalid
 
 if tp.TYPE_CHECKING:
@@ -82,14 +82,21 @@
         DTYPE_FLOAT_KIND,
         DTYPE_COMPLEX_KIND,
         DTYPE_DATETIME_KIND,
         DTYPE_TIMEDELTA_KIND,
         DTYPE_OBJECT_KIND,
         ))
 
+DTYPE_NAN_NAT_KINDS = frozenset((
+        DTYPE_FLOAT_KIND,
+        DTYPE_COMPLEX_KIND,
+        DTYPE_DATETIME_KIND,
+        DTYPE_TIMEDELTA_KIND,
+        ))
+
 # this is all kinds except 'V'
 # DTYPE_FALSY_KINDS = frozenset((
 #         DTYPE_FLOAT_KIND,
 #         DTYPE_COMPLEX_KIND,
 #         DTYPE_DATETIME_KIND,
 #         DTYPE_TIMEDELTA_KIND,
 #         DTYPE_OBJECT_KIND,
@@ -236,15 +243,15 @@
         int,
         np.integer,
         slice,
         tp.List[tp.Any],
         None,
         'Index',
         'Series',
-        np.ndarray
+        np.ndarray,
         ]
 
 # keys that might include a multiple dimensions speciation; tuple is used to identify compound extraction
 GetItemKeyTypeCompound = tp.Union[
         tp.Tuple[tp.Any, ...],
         int,
         np.integer,
@@ -1155,17 +1162,17 @@
             return array
     else:
         array = np.sort(array)
 
     mask = np.empty(array.shape, dtype=DTYPE_BOOL)
     mask[:1] = True
     mask[1:] = array[1:] != array[:-1]
-
-    return array[mask]
-
+    array = array[mask]
+    array.flags.writeable = False
+    return array
 
 def ufunc_unique1d_indexer(array: np.ndarray,
         ) -> tp.Tuple[np.ndarray, np.ndarray]:
     '''
     Find the unique elements of an array. Optimized from NumPy implementation based on assumption of 1D array. Returns unique values as well as index positions of those values in the original array.
     '''
     positions = argsort_array(array)
@@ -1174,14 +1181,15 @@
     array = array[positions]
 
     mask = np.empty(array.shape, dtype=DTYPE_BOOL)
     mask[:1] = True
     mask[1:] = array[1:] != array[:-1]
 
     values = array[mask] # get unique values
+    values.flags.writeable = False
     if len(values) <= 1: # we have only one item
         return values, np.full(mask.shape, 0, dtype=DTYPE_INT_DEFAULT)
 
     indexer = np.empty(mask.shape, dtype=DTYPE_INT_DEFAULT)
     indexer[positions] = np.cumsum(mask) - 1
     indexer.flags.writeable = False
```

### Comparing `static-frame-1.3.2/static_frame/core/www.py` & `static-frame-1.4.0/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/core/yarn.py` & `static-frame-1.4.0/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/test_case.py` & `static-frame-1.4.0/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.0/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.0/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_batch.py` & `static-frame-1.4.0/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_bus.py` & `static-frame-1.4.0/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_container.py` & `static-frame-1.4.0/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.0/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_display.py` & `static-frame-1.4.0/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.0/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_doc.py` & `static-frame-1.4.0/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.0/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -9156,14 +9156,15 @@
                 (('p', (('w', 0), ('x', 2), ('z', 34))), ('q', (('w', False), ('x', False), ('z', False))), ('r', (('w', 'c'), ('x', 'd'), ('z', 'e'))), ('s', (('w', False), ('x', True), ('z', True))))
                 )
 
     def test_frame_from_concat_gg(self) -> None:
         # when explicitly named 0, we get the expected error when creting the index
         s1 = Series([1, 2, 3], name=0)
         s2 = s1.rename(np.datetime64('2022-01-01'))
+        # import ipdb; ipdb.set_trace()
         with self.assertRaises(InvalidDatetime64Initializer):
             _ = Frame.from_concat((s1, s2), axis=1, columns_constructor=sf.IndexDate)
 
         s1 = Series([1, 2, 3]) # happens implicitly, but here we make it explicit
         s2 = s1.rename(np.datetime64('2022-01-01'))
 
         with self.assertRaises(InvalidDatetime64Initializer):
@@ -13064,15 +13065,15 @@
         self.assertTrue(f2.equals(f3, compare_name=True, compare_dtype=True, compare_class=True))
         self.assertEqual(f2.to_pairs(),
                 ((0, (((0, 2), 129017), ((1, 0), 0), ((1, 1), 0), ((1, 2), 0), ((2, 0), 0))), (1, (((0, 2), 0), ((1, 0), 119909), ((1, 1), 0), ((1, 2), 166924), ((2, 0), 0))), (2, (((0, 2), 0), ((1, 0), 194224), ((1, 1), 172133), ((1, 2), 197228), ((2, 0), 35021))))
                 )
 
 
     def test_frame_pivot_y1(self) -> None:
-        f1 = ff.parse('s(10,4)|v(int)').assign[0].apply(
+        f1 = ff.parse('s(10,4)|v(int64)').assign[0].apply(
                 lambda x: x % 3).assign[1].apply(
                 lambda x: x % 3).assign[2].apply(
                 lambda x: x % 3)
 
         f2 = f1.pivot(index_fields=2, columns_fields=1, data_fields=[0, 3])
         self.assertEqual([(k, v.kind) for k, v in f2.dtypes.items()],
                 [((0, 0), 'f'), ((0, 3), 'f'), ((1, 0), 'f'), ((1, 3), 'f'), ((2, 0), 'i'), ((2, 3), 'i')])
@@ -13082,14 +13083,16 @@
                 fill_value=0)
         self.assertEqual(f3.index.name, 2)
         self.assertEqual(f3.columns.name, (1, 'values'))
         self.assertEqual(f3.to_pairs(),
                 (((0, 0), ((0, 0), (1, 1), (2, 4))), ((0, 3), ((0, 0), (1, 1), (2, 4))), ((1, 0), ((0, 0), (1, 0), (2, 1))), ((1, 3), ((0, 0), (1, 0), (2, 1))), ((2, 0), ((0, 1), (1, 1), (2, 2))), ((2, 3), ((0, 1), (1, 1), (2, 2))))
                 )
 
+    # NOTE: this is failing on old Python, windows with Windows fatal exception: access violation
+    @skip_win
     def test_frame_pivot_y2(self) -> None:
         f1 = ff.parse('s(10,4)|v(int)').assign[0].apply(
                 lambda x: x % 3).assign[1].apply(
                 lambda x: x % 3).assign[2].apply(
                 lambda x: x % 3)
 
         f2 = f1.pivot(index_fields=2,
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.0/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.0/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index.py` & `static-frame-1.4.0/static_frame/test/unit/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,26 @@
         with self.assertRaises(ErrorInitIndex):
             _ = Index('bar')
 
     def test_index_init_m(self) -> None:
         with self.assertRaises(ErrorInitIndex):
             _ = Index(np.array(('2021-02', '2022-04'), dtype=np.datetime64))
 
+    def test_index_init_n(self) -> None:
+        a1 = np.array((np.nan, np.nan, 3), dtype=np.float64)
+        a2 = a1.astype(np.float16)
+        a2.flags.writeable = False
+        idx = Index(a2)
+        self.assertEqual(idx.loc_to_iloc(3), 2)
+
+    def test_index_init_o(self) -> None:
+        a1 = np.array((10, 40, 20))
+        idx = Index(a1) # permit a mutable array
+        self.assertEqual(idx.values.tolist(), [10, 40, 20])
+
 
     #---------------------------------------------------------------------------
 
     def test_index_loc_to_iloc_a(self) -> None:
 
         idx = Index(('a', 'b', 'c', 'd'))
 
@@ -169,15 +181,15 @@
         self.assertEqual(idx._loc_to_iloc(slice('c',)), slice(None, 3, None))
         self.assertEqual(idx._loc_to_iloc(slice('b','d')), slice(1, 4, None))
         self.assertEqual(idx._loc_to_iloc('d'), 3)
 
     def test_index_loc_to_iloc_b(self) -> None:
         idx = Index(('a', 'b', 'c', 'd'))
         post = idx._loc_to_iloc(Series(['b', 'c']))
-        self.assertEqual(post, [1, 2])
+        self.assertEqual(post.tolist(), [1, 2]) #type: ignore
 
     def test_index_loc_to_iloc_c(self) -> None:
         idx = Index(('a', 'b', 'c', 'd'))
         with self.assertRaises(KeyError):
             _ = idx._loc_to_iloc(['c', 'd', 'e'])
 
         post = idx._loc_to_iloc(['c', 'd', 'e'], partial_selection=True)
@@ -191,15 +203,15 @@
         with self.assertRaises(KeyError):
             _ = idx1.loc_to_iloc('g')
 
         self.assertEqual(idx1.loc_to_iloc(slice('b', 'd')), slice(1, 4, None))
         with self.assertRaises(LocInvalid):
             _ = idx1.loc_to_iloc(slice('x', 'y'))
 
-        self.assertEqual(idx1.loc_to_iloc(['d', 'a']), [3, 0])
+        self.assertEqual(idx1.loc_to_iloc(['d', 'a']).tolist(), [3, 0]) #type: ignore
         with self.assertRaises(KeyError):
             _ = idx1.loc_to_iloc(['d', 'x'])
 
         self.assertEqual(idx1.loc_to_iloc(np.array([False, True, True, False])).tolist(), [1, 2]) #type: ignore [union-attr]
         with self.assertRaises(IndexError):
             _ = idx1.loc_to_iloc(np.array([False, True, False]))
 
@@ -243,15 +255,15 @@
                 1
                 )
         # NOTE: this fails as we only see a list of dt64s and cannot match them in the AutoMap dictionary unless we were to directly examine and conert each element
         with self.assertRaises(KeyError):
             _ = idx1.loc_to_iloc([dt64(d) for d in reversed(idx1)])
 
         post = idx1.loc_to_iloc(np.array([dt64(d) for d in reversed(idx1)]))
-        self.assertEqual(post, [2, 1, 0])
+        self.assertEqual(post.tolist(), [2, 1, 0]) #type: ignore
 
     def test_index_loc_to_iloc_g(self) -> None:
         dt = datetime.date
         dt64 = np.datetime64
 
         idx1 = IndexYear(('2021', '2018', '2001'))
 
@@ -404,15 +416,15 @@
 
         self.assertEqual(idx[2:].values.tolist(), ['c', 'd']) #type: ignore
 
         self.assertEqual(idx.loc['b':].values.tolist(), ['b', 'c', 'd'])  # type: ignore  # https://github.com/python/typeshed/pull/3024
 
         self.assertEqual(idx.loc['b':'d'].values.tolist(), ['b', 'c', 'd'])  # type: ignore  # https://github.com/python/typeshed/pull/3024
 
-        self.assertEqual(idx._loc_to_iloc(['b', 'b', 'c']), [1, 1, 2])
+        self.assertEqual(idx._loc_to_iloc(['b', 'b', 'c']).tolist(), [1, 1, 2]) #type: ignore
 
         self.assertEqual(idx.loc['c'], 'c')
 
         idxgo = IndexGO(('a', 'b', 'c', 'd'))
         self.assertEqual(idxgo.values.tolist(), ['a', 'b', 'c', 'd'])
 
         idxgo.append('e')
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_correspondence.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
         self.assertFalse(ic.is_subset)
         self.assertTrue(ic.has_common)
         # this is an array, due to loc_is_iloc being True
         assert isinstance(ic.iloc_src, np.ndarray)
         self.assertEqual(ic.iloc_src.tolist(),
                 [0, 1, 2, 3, 4]
                 )
-        self.assertEqual(ic.iloc_dst,
+        self.assertEqual(ic.iloc_dst.tolist(), #type: ignore
                 [0, 1, 2, 3, 4]
                 )
 
     def test_index_correspondence_b(self) -> None:
         # issue found with a hypothesis test
 
         idx = Index([False], loc_is_iloc=False)
         ic = IndexCorrespondence.from_correspondence(idx, idx)
         self.assertTrue(ic.is_subset)
         self.assertTrue(ic.has_common)
         self.assertEqual(ic.size, 1)
         self.assertEqual(ic.iloc_src, [0]) # this is as list in this use case
-        self.assertEqual(ic.iloc_dst.tolist(), [0]) # type: ignore
+        self.assertEqual(ic.iloc_dst.tolist(), [0]) #type: ignore
 
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,18 @@
     def test_index_date_q(self) -> None:
         index = IndexDate(('2017-12-30', '2017-12-31', '2018-01-05'))
         s1 = Series(range(len(index)), index=index)
         # a range beyond the observed values cannot determine a match,
         self.assertEqual(s1[:'2019'].shape, (0,)) # type: ignore
         self.assertEqual(s1['2016':].shape, (0,)) # type: ignore
 
+    def test_index_date_r(self) -> None:
+        with self.assertRaises(InvalidDatetime64Initializer):
+            _ = IndexDate((0,))
+
     #---------------------------------------------------------------------------
 
     def test_index_datetime_init_a(self) -> None:
 
         dates = [datetime.date(*x) for x in product((2017,), (4,5,), range(1, 4))]
         s1 = Series(range(len(dates)), index=IndexDate(dates))
 
@@ -849,15 +853,15 @@
 
     #---------------------------------------------------------------------------
 
     def test_index_datetime_loc_to_iloc_a(self) -> None:
         dt64 = np.datetime64
         idx = IndexDate.from_date_range('2020-01-01', '2020-01-31')
 
-        self.assertEqual(idx.loc_to_iloc(['2020-01-15', '2020-01-29']),
+        self.assertEqual(idx.loc_to_iloc(['2020-01-15', '2020-01-29']).tolist(), #type: ignore
                 [14, 28])
 
         self.assertEqual(idx.loc_to_iloc(idx == dt64('2020-01-13')).tolist(), #type: ignore [union-attr]
                 [12])
         self.assertEqual(idx.loc_to_iloc(slice('2020-01-15', '2020-01-29')),
                 slice(14, 29, None))
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.0/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_interface.py` & `static-frame-1.4.0/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.0/static_frame/test/unit/test_loc_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from static_frame.core.loc_map import LocMap
 from static_frame.core.util import DTYPE_UINT_DEFAULT
 from static_frame.core.util import NULL_SLICE
 from static_frame.core.util import PositionsAllocator
 from static_frame.test.test_case import TestCase
 
 
+def np_arange(*args: int) -> np.ndarray:
+    a = np.arange(*args)
+    a.flags.writeable = False
+    return a
+
 class TestLocMapUnit(TestCase):
 
     def test_loc_map_a(self) -> None:
         idx = Index(['a', 'b', 'c'])
         post1 = LocMap.loc_to_iloc(
                 label_to_pos=idx._map,
                 labels=idx._labels,
@@ -43,15 +48,15 @@
         post1 = LocMap.loc_to_iloc(
                 label_to_pos=idx._map,
                 labels=idx._labels,
                 positions=idx._positions,
                 key=['b', 'd'],
                 partial_selection=False,
                 )
-        self.assertEqual(post1, [1, 3])
+        self.assertEqual(post1.tolist(), [1, 3]) #type: ignore
 
     def test_loc_map_slice_a(self) -> None:
         dt64 = np.datetime64
         idx = IndexDate.from_date_range('1985-01-01', '1985-01-08')
 
         post1 = LocMap.loc_to_iloc(
                 label_to_pos=idx._map,
@@ -113,15 +118,15 @@
 
 class TestHierarchicalLocMapUnit(TestCase):
 
     #---------------------------------------------------------------------------
 
     def test_init_a(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -287,21 +292,21 @@
         self.assertTrue(HierarchicalLocMap.is_single_element(1.0023))
         self.assertTrue(HierarchicalLocMap.is_single_element(np.nan))
         self.assertTrue(HierarchicalLocMap.is_single_element(()))
         self.assertTrue(HierarchicalLocMap.is_single_element((1, 2, 3)))
 
         self.assertFalse(HierarchicalLocMap.is_single_element([False]))
         self.assertFalse(HierarchicalLocMap.is_single_element([2.3, 8878.33]))
-        self.assertFalse(HierarchicalLocMap.is_single_element(np.arange(5)))
+        self.assertFalse(HierarchicalLocMap.is_single_element(np_arange(5)))
 
     #---------------------------------------------------------------------------
 
     def test_loc_to_iloc_a(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -319,15 +324,15 @@
         self.assertEqual(hlmap.loc_to_iloc(([3, 0], 'E'), indices), [0, 9])
         self.assertEqual(hlmap.loc_to_iloc(([3, 0], ['E']), indices), [0, 9])
 
         self.assertEqual(hlmap.loc_to_iloc(np.array([0, 'E'], dtype=object), indices), 9)
 
     def test_loc_to_iloc_b(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -344,33 +349,32 @@
         with self.assertRaises(KeyError):
             hlmap.loc_to_iloc(([0, 1, 2], ['A', 'B', 'C']), indices)
 
     #---------------------------------------------------------------------------
 
     def test_nbytes_a(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
         )
 
         hlmap = HierarchicalLocMap(indices=indices, indexers=indexers)
-
-        self.assertIn(hlmap.nbytes, (720 + 8 + 8 + 25, 721, 705)) # automap + 2 uint64 bit offsets + PyBool
+        self.assertTrue(hlmap.nbytes > 0)
 
     #---------------------------------------------------------------------------
 
     def test_deepcopy_a(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -387,15 +391,15 @@
         self.assertNotEqual(id(hlmap.bit_offset_encoders), id(hlmap_copy.bit_offset_encoders))
         self.assertNotEqual(id(hlmap.encoded_indexer_map), id(hlmap_copy.encoded_indexer_map))
 
     #---------------------------------------------------------------------------
 
     def test_indexers_to_iloc_invalid_input(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -413,15 +417,15 @@
 
         # Invliad dtype
         with self.assertRaises(AssertionError):
             hlmap.indexers_to_iloc(np.array([[0, 1]]).astype(object))
 
     def test_indexers_to_iloc_a(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -430,15 +434,15 @@
         hlmap = HierarchicalLocMap(indices=indices, indexers=indexers)
 
         post = hlmap.indexers_to_iloc(indexers.T.astype(DTYPE_UINT_DEFAULT))
         self.assertListEqual(post, list(range(10)))
 
     def test_indexers_to_iloc_b(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
@@ -450,15 +454,15 @@
 
         for subset in subsets:
             post = hlmap.indexers_to_iloc(indexers.T.astype(DTYPE_UINT_DEFAULT)[subset])
             self.assertListEqual(post, subset)
 
     def test_indexers_to_iloc_c(self) -> None:
         indices = [
-                Index(np.arange(5)),
+                Index(np_arange(5)),
                 Index(tuple('ABCDE')),
                 ]
         indexers = np.array(
             [
                 [3, 3, 0, 1, 4, 0, 3, 2, 2, 0],
                 [4, 2, 1, 0, 3, 0, 3, 2, 0, 4],
             ]
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.0/static_frame/test/unit/test_memory_measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from sys import getsizeof
 
 import frame_fixtures as ff
 import numpy as np
-from automap import FrozenAutoMap  # pylint: disable=E0611
+from arraymap import FrozenAutoMap  # pylint: disable=E0611
 
 from static_frame.core.memory_measure import MaterializedArray
 from static_frame.core.memory_measure import MeasureFormat
 from static_frame.core.memory_measure import MemoryDisplay
 from static_frame.core.memory_measure import MemoryMeasure
 from static_frame.core.memory_measure import memory_total
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.0/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as tp
 import unittest
 from sys import getsizeof
 
 import frame_fixtures as ff
 import numpy as np
-from automap import FrozenAutoMap  # pylint: disable=E0611
+from arraymap import FrozenAutoMap  # pylint: disable=E0611
 
 from static_frame import Bus
 from static_frame import Frame
 from static_frame import Index
 from static_frame import IndexDateGO
 from static_frame import IndexGO
 from static_frame import IndexHierarchy
```

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.0/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.0/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.0/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_rank.py` & `static-frame-1.4.0/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_series.py` & `static-frame-1.4.0/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.0/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store.py` & `static-frame-1.4.0/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.0/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.0/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.0/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.0/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.0/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.0/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.0/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_util.py` & `static-frame-1.4.0/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_www.py` & `static-frame-1.4.0/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.2/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.0/static_frame/test/unit/test_yarn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1133,15 +1133,17 @@
         f5 = ff.parse('s(4,4)').rename('f5')
         f6 = ff.parse('s(6,4)').rename('f6')
 
         b1 = Bus.from_frames((f1, f2, f3))
         b2 = Bus.from_frames((f4,))
         b3 = Bus.from_frames((f5, f6))
 
-        y1 = Yarn((b1, b2, b3), index=IndexHierarchy.from_product(('a', 'b'), np.array((1, 2, 3), dtype=np.int64)))
+        a1 = np.array((1, 2, 3), dtype=np.int64)
+        a1.flags.writeable = False
+        y1 = Yarn((b1, b2, b3), index=IndexHierarchy.from_product(('a', 'b'), a1))
 
         bytes1 = y1._to_signature_bytes(include_name=False)
         self.assertEqual(sha256(bytes1).hexdigest(),
             '0a6978231ec671903449e39ae465747a68a0da8492e9b5b5fcf4dc98afb8143e')
 
     def test_yarn_to_signature_bytes_b(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
@@ -1151,15 +1153,17 @@
         f5 = ff.parse('s(4,4)').rename('f5')
         f6 = ff.parse('s(6,4)').rename('f6')
 
         b1 = Bus.from_frames((f1, f2, f3))
         b2 = Bus.from_frames((f4,))
         b3 = Bus.from_frames((f5, f6))
 
-        y1 = Yarn((b1, b2, b3), index=IndexHierarchy.from_product(('a', 'b'), np.array((1, 2, 3), dtype=np.int64)))
+        a1 = np.array((1, 2, 3), dtype=np.int64)
+        a1.flags.writeable = False
+        y1 = Yarn((b1, b2, b3), index=IndexHierarchy.from_product(('a', 'b'), a1))
         bytes1 = y1._to_signature_bytes(include_name=False)
 
         y2 = Yarn((b1, b2, b3))
         bytes2 = y2._to_signature_bytes(include_name=False)
 
         self.assertNotEqual(sha256(bytes1).hexdigest(), sha256(bytes2).hexdigest())
```

### Comparing `static-frame-1.3.2/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.0/static_frame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.3.2
+Version: 1.4.0
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -45,15 +45,15 @@
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
-        - automap==0.6.2
+        - arraymap==0.1.7
         - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
```

### Comparing `static-frame-1.3.2/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.0/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

