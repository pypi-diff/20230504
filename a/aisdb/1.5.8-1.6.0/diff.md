# Comparing `tmp/aisdb-1.5.8-cp39-none-win_amd64.whl.zip` & `tmp/aisdb-1.6.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,67 +1,165 @@
-Zip file size: 2672058 bytes, number of entries: 65
--rw-r--r--  4.6 unx     5087 b- defN 23-Apr-09 01:05 aisdb-1.5.8.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Apr-09 01:05 aisdb-1.5.8.dist-info/WHEEL
--rw-r--r--  4.6 unx     5010 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/coarsetype.sql
--rw-r--r--  4.6 unx      372 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
--rw-r--r--  4.6 unx      114 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/createtable_griddata.sql
--rw-r--r--  4.6 unx      561 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/createtable_static.sql
--rw-r--r--  4.6 unx      270 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/createtable_static_aggregate.sql
--rw-r--r--  4.6 unx      384 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx       47 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/cte_aliases.sql
--rw-r--r--  4.6 unx       97 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/cte_coarsetype.sql
--rw-r--r--  4.6 unx      134 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      195 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/cte_static.sql
--rw-r--r--  4.6 unx      221 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/cte_static_aggregate.sql
--rw-r--r--  4.6 unx      247 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      424 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/insert_static.sql
--rw-r--r--  4.6 unx      790 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx      330 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/select_columns_static.sql
--rw-r--r--  4.6 unx      513 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
--rw-r--r--  4.6 unx      910 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/select_merged_all.sql
--rw-r--r--  4.6 unx      677 b- defN 23-Apr-09 01:05 aisdb/aisdb_sql/select_static_join_webdata.sql
--rw-r--r--  4.6 unx     5035 b- defN 23-Apr-09 01:05 aisdb/database/create_tables.py
--rw-r--r--  4.6 unx     6558 b- defN 23-Apr-09 01:05 aisdb/database/dbconn.py
--rw-r--r--  4.6 unx    11944 b- defN 23-Apr-09 01:05 aisdb/database/dbqry.py
--rw-r--r--  4.6 unx     9950 b- defN 23-Apr-09 01:05 aisdb/database/decoder.py
--rw-r--r--  4.6 unx     3272 b- defN 23-Apr-09 01:05 aisdb/database/sqlfcn.py
--rw-r--r--  4.6 unx     1795 b- defN 23-Apr-09 01:05 aisdb/database/sqlfcn_callbacks.py
--rw-r--r--  4.6 unx     4427 b- defN 23-Apr-09 01:05 aisdb/database/sql_query_strings.py
--rw-r--r--  4.6 unx        2 b- defN 23-Apr-09 01:05 aisdb/database/__init__.py
--rw-r--r--  4.6 unx    16588 b- defN 23-Apr-09 01:05 aisdb/gis.py
--rw-r--r--  4.6 unx     1655 b- defN 23-Apr-09 01:05 aisdb/interp.py
--rw-r--r--  4.6 unx    19317 b- defN 23-Apr-09 01:05 aisdb/network_graph.py
--rw-r--r--  4.6 unx     8306 b- defN 23-Apr-09 01:05 aisdb/proc_util.py
--rw-r--r--  4.6 unx     2534 b- defN 23-Apr-09 01:05 aisdb/receiver.py
--rw-r--r--  4.6 unx     3912 b- defN 23-Apr-09 01:05 aisdb/tests/create_testing_data.py
--rw-r--r--  4.6 unx    84630 b- defN 23-Apr-09 01:05 aisdb/tests/testdata/test_data_20211101.nm4
--rw-r--r--  4.6 unx    23613 b- defN 23-Apr-09 01:05 aisdb/tests/testdata/test_data_20211101.nm4.gz
--rw-r--r--  4.6 unx    23766 b- defN 23-Apr-09 01:05 aisdb/tests/testdata/test_data_20211101.nm4.zip
--rw-r--r--  4.6 unx     1454 b- defN 23-Apr-09 01:05 aisdb/tests/test_00_decode.py
--rw-r--r--  4.6 unx     2816 b- defN 23-Apr-09 01:05 aisdb/tests/test_01_createtables.py
--rw-r--r--  4.6 unx     3269 b- defN 23-Apr-09 01:05 aisdb/tests/test_02_dbqry.py
--rw-r--r--  4.6 unx     3034 b- defN 23-Apr-09 01:05 aisdb/tests/test_02_sqlfcn.py
--rw-r--r--  4.6 unx     2904 b- defN 23-Apr-09 01:05 aisdb/tests/test_03_gis.py
--rw-r--r--  4.6 unx     2381 b- defN 23-Apr-09 01:05 aisdb/tests/test_04_trackgen.py
--rw-r--r--  4.6 unx     4517 b- defN 23-Apr-09 01:05 aisdb/tests/test_05_proc_util.py
--rw-r--r--  4.6 unx     1124 b- defN 23-Apr-09 01:05 aisdb/tests/test_06_interp.py
--rw-r--r--  4.6 unx     1307 b- defN 23-Apr-09 01:05 aisdb/tests/test_07_bathymetry.py
--rw-r--r--  4.6 unx     1205 b- defN 23-Apr-09 01:05 aisdb/tests/test_07_shore_dist.py
--rw-r--r--  4.6 unx     2662 b- defN 23-Apr-09 01:05 aisdb/tests/test_08_marinetraffic.py
--rw-r--r--  4.6 unx     1757 b- defN 23-Apr-09 01:05 aisdb/tests/test_08_wsa.py
--rw-r--r--  4.6 unx     3627 b- defN 23-Apr-09 01:05 aisdb/tests/test_09_network_graph.py
--rw-r--r--  4.6 unx      810 b- defN 23-Apr-09 01:05 aisdb/tests/test_11_postgres.py
--rw-r--r--  4.6 unx       76 b- defN 23-Apr-09 01:05 aisdb/tests/test_rx.py
--rw-r--r--  4.6 unx   228241 b- defN 23-Apr-09 01:05 aisdb/tests/test_zones/test_zones.zip
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-09 01:05 aisdb/tests/__init__.py
--rw-r--r--  4.6 unx    15713 b- defN 23-Apr-09 01:05 aisdb/track_gen.py
--rw-r--r--  4.6 unx     5591 b- defN 23-Apr-09 01:05 aisdb/webdata/bathymetry.py
--rw-r--r--  4.6 unx     2520 b- defN 23-Apr-09 01:05 aisdb/webdata/load_raster.py
--rw-r--r--  4.6 unx    11326 b- defN 23-Apr-09 01:05 aisdb/webdata/marinetraffic.py
--rw-r--r--  4.6 unx     2758 b- defN 23-Apr-09 01:05 aisdb/webdata/shore_dist.py
--rw-r--r--  4.6 unx     2565 b- defN 23-Apr-09 01:05 aisdb/webdata/_scraper.py
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-09 01:05 aisdb/webdata/__init__.py
--rw-r--r--  4.6 unx     3959 b- defN 23-Apr-09 01:05 aisdb/wsa.py
--rw-r--r--  4.6 unx     1613 b- defN 23-Apr-09 01:05 aisdb/__init__.py
--rwxr-xr-x  4.6 unx  4933632 b- defN 23-Apr-09 01:05 aisdb/aisdb.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx     5695 b- defN 23-Apr-09 01:05 aisdb-1.5.8.dist-info/RECORD
-65 files, 5490338 bytes uncompressed, 2662968 bytes compressed:  51.5%
+Zip file size: 3478752 bytes, number of entries: 163
+-rw-r--r--  4.6 unx     5005 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     5010 b- defN 23-May-04 03:22 aisdb/aisdb_sql/coarsetype.sql
+-rw-r--r--  4.6 unx      372 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+-rw-r--r--  4.6 unx      114 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_griddata.sql
+-rw-r--r--  4.6 unx      561 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static.sql
+-rw-r--r--  4.6 unx      270 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static_aggregate.sql
+-rw-r--r--  4.6 unx      384 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx       47 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_aliases.sql
+-rw-r--r--  4.6 unx       97 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_coarsetype.sql
+-rw-r--r--  4.6 unx      134 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      195 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static.sql
+-rw-r--r--  4.6 unx      221 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static_aggregate.sql
+-rw-r--r--  4.6 unx      247 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      424 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_static.sql
+-rw-r--r--  4.6 unx      790 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      330 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_columns_static.sql
+-rw-r--r--  4.6 unx      513 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+-rw-r--r--  4.6 unx      910 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_merged_all.sql
+-rw-r--r--  4.6 unx      677 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_static_join_webdata.sql
+-rw-r--r--  4.6 unx     5035 b- defN 23-May-04 03:22 aisdb/database/create_tables.py
+-rw-r--r--  4.6 unx     6558 b- defN 23-May-04 03:22 aisdb/database/dbconn.py
+-rw-r--r--  4.6 unx    12239 b- defN 23-May-04 03:22 aisdb/database/dbqry.py
+-rw-r--r--  4.6 unx     9948 b- defN 23-May-04 03:22 aisdb/database/decoder.py
+-rw-r--r--  4.6 unx     3272 b- defN 23-May-04 03:22 aisdb/database/sqlfcn.py
+-rw-r--r--  4.6 unx     1795 b- defN 23-May-04 03:22 aisdb/database/sqlfcn_callbacks.py
+-rw-r--r--  4.6 unx     4318 b- defN 23-May-04 03:22 aisdb/database/sql_query_strings.py
+-rw-r--r--  4.6 unx        2 b- defN 23-May-04 03:22 aisdb/database/__init__.py
+-rw-r--r--  4.6 unx     7991 b- defN 23-May-04 03:22 aisdb/denoising_encoder.py
+-rw-r--r--  4.6 unx    19098 b- defN 23-May-04 03:22 aisdb/gis.py
+-rw-r--r--  4.6 unx     1655 b- defN 23-May-04 03:22 aisdb/interp.py
+-rw-r--r--  4.6 unx    19380 b- defN 23-May-04 03:22 aisdb/network_graph.py
+-rw-r--r--  4.6 unx     8306 b- defN 23-May-04 03:22 aisdb/proc_util.py
+-rw-r--r--  4.6 unx     2534 b- defN 23-May-04 03:22 aisdb/receiver.py
+-rw-r--r--  4.6 unx     3229 b- defN 23-May-04 03:22 aisdb/tests/create_testing_data.py
+-rw-r--r--  4.6 unx    84630 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4
+-rw-r--r--  4.6 unx    23613 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4.gz
+-rw-r--r--  4.6 unx    23766 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4.zip
+-rw-r--r--  4.6 unx     1454 b- defN 23-May-04 03:22 aisdb/tests/test_00_decode.py
+-rw-r--r--  4.6 unx     2816 b- defN 23-May-04 03:22 aisdb/tests/test_01_createtables.py
+-rw-r--r--  4.6 unx     2882 b- defN 23-May-04 03:22 aisdb/tests/test_02_dbqry.py
+-rw-r--r--  4.6 unx     3050 b- defN 23-May-04 03:22 aisdb/tests/test_02_sqlfcn.py
+-rw-r--r--  4.6 unx     3061 b- defN 23-May-04 03:22 aisdb/tests/test_03_gis.py
+-rw-r--r--  4.6 unx     2399 b- defN 23-May-04 03:22 aisdb/tests/test_04_trackgen.py
+-rw-r--r--  4.6 unx     4517 b- defN 23-May-04 03:22 aisdb/tests/test_05_proc_util.py
+-rw-r--r--  4.6 unx     1124 b- defN 23-May-04 03:22 aisdb/tests/test_06_interp.py
+-rw-r--r--  4.6 unx     1307 b- defN 23-May-04 03:22 aisdb/tests/test_07_bathymetry.py
+-rw-r--r--  4.6 unx     1173 b- defN 23-May-04 03:22 aisdb/tests/test_07_shore_dist.py
+-rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb/tests/test_08_marinetraffic.py
+-rw-r--r--  4.6 unx     1732 b- defN 23-May-04 03:22 aisdb/tests/test_08_wsa.py
+-rw-r--r--  4.6 unx     3722 b- defN 23-May-04 03:22 aisdb/tests/test_09_network_graph.py
+-rw-r--r--  4.6 unx      810 b- defN 23-May-04 03:22 aisdb/tests/test_11_postgres.py
+-rw-r--r--  4.6 unx       76 b- defN 23-May-04 03:22 aisdb/tests/test_rx.py
+-rw-r--r--  4.6 unx   228241 b- defN 23-May-04 03:22 aisdb/tests/test_zones/test_zones.zip
+-rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/tests/__init__.py
+-rw-r--r--  4.6 unx     7874 b- defN 23-May-04 03:22 aisdb/track_gen.py
+-rw-r--r--  4.6 unx     5590 b- defN 23-May-04 03:22 aisdb/webdata/bathymetry.py
+-rw-r--r--  4.6 unx     2520 b- defN 23-May-04 03:22 aisdb/webdata/load_raster.py
+-rw-r--r--  4.6 unx    11326 b- defN 23-May-04 03:22 aisdb/webdata/marinetraffic.py
+-rw-r--r--  4.6 unx     2758 b- defN 23-May-04 03:22 aisdb/webdata/shore_dist.py
+-rw-r--r--  4.6 unx     2565 b- defN 23-May-04 03:22 aisdb/webdata/_scraper.py
+-rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/webdata/__init__.py
+-rw-r--r--  4.6 unx     7200 b- defN 23-May-04 03:22 aisdb/web_interface.py
+-rw-r--r--  4.6 unx     3959 b- defN 23-May-04 03:22 aisdb/wsa.py
+-rw-r--r--  4.6 unx     1680 b- defN 23-May-04 03:22 aisdb/__init__.py
+-rw-r--r--  4.6 unx     1680 b- defN 23-May-04 03:22 aisdb/__init__.py
+-rw-r--r--  4.6 unx     7991 b- defN 23-May-04 03:22 aisdb/denoising_encoder.py
+-rw-r--r--  4.6 unx    19098 b- defN 23-May-04 03:22 aisdb/gis.py
+-rw-r--r--  4.6 unx     1655 b- defN 23-May-04 03:22 aisdb/interp.py
+-rw-r--r--  4.6 unx    19380 b- defN 23-May-04 03:22 aisdb/network_graph.py
+-rw-r--r--  4.6 unx     8306 b- defN 23-May-04 03:22 aisdb/proc_util.py
+-rw-r--r--  4.6 unx     2534 b- defN 23-May-04 03:22 aisdb/receiver.py
+-rw-r--r--  4.6 unx     7874 b- defN 23-May-04 03:22 aisdb/track_gen.py
+-rw-r--r--  4.6 unx     7200 b- defN 23-May-04 03:22 aisdb/web_interface.py
+-rw-r--r--  4.6 unx     3959 b- defN 23-May-04 03:22 aisdb/wsa.py
+-rw-r--r--  4.6 unx     5010 b- defN 23-May-04 03:22 aisdb/aisdb_sql/coarsetype.sql
+-rw-r--r--  4.6 unx      372 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+-rw-r--r--  4.6 unx      114 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_griddata.sql
+-rw-r--r--  4.6 unx      561 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static.sql
+-rw-r--r--  4.6 unx      270 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_static_aggregate.sql
+-rw-r--r--  4.6 unx      384 b- defN 23-May-04 03:22 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx       47 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_aliases.sql
+-rw-r--r--  4.6 unx       97 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_coarsetype.sql
+-rw-r--r--  4.6 unx      134 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      195 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static.sql
+-rw-r--r--  4.6 unx      221 b- defN 23-May-04 03:22 aisdb/aisdb_sql/cte_static_aggregate.sql
+-rw-r--r--  4.6 unx      247 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      424 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_static.sql
+-rw-r--r--  4.6 unx      790 b- defN 23-May-04 03:22 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      330 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_columns_static.sql
+-rw-r--r--  4.6 unx      513 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+-rw-r--r--  4.6 unx      910 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_merged_all.sql
+-rw-r--r--  4.6 unx      677 b- defN 23-May-04 03:22 aisdb/aisdb_sql/select_static_join_webdata.sql
+-rw-r--r--  4.6 unx        2 b- defN 23-May-04 03:22 aisdb/database/__init__.py
+-rw-r--r--  4.6 unx     5035 b- defN 23-May-04 03:22 aisdb/database/create_tables.py
+-rw-r--r--  4.6 unx     6558 b- defN 23-May-04 03:22 aisdb/database/dbconn.py
+-rw-r--r--  4.6 unx    12239 b- defN 23-May-04 03:22 aisdb/database/dbqry.py
+-rw-r--r--  4.6 unx     9948 b- defN 23-May-04 03:22 aisdb/database/decoder.py
+-rw-r--r--  4.6 unx     4318 b- defN 23-May-04 03:22 aisdb/database/sql_query_strings.py
+-rw-r--r--  4.6 unx     3272 b- defN 23-May-04 03:22 aisdb/database/sqlfcn.py
+-rw-r--r--  4.6 unx     1795 b- defN 23-May-04 03:22 aisdb/database/sqlfcn_callbacks.py
+-rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/tests/__init__.py
+-rw-r--r--  4.6 unx     3229 b- defN 23-May-04 03:22 aisdb/tests/create_testing_data.py
+-rw-r--r--  4.6 unx     1454 b- defN 23-May-04 03:22 aisdb/tests/test_00_decode.py
+-rw-r--r--  4.6 unx     2816 b- defN 23-May-04 03:22 aisdb/tests/test_01_createtables.py
+-rw-r--r--  4.6 unx     2882 b- defN 23-May-04 03:22 aisdb/tests/test_02_dbqry.py
+-rw-r--r--  4.6 unx     3050 b- defN 23-May-04 03:22 aisdb/tests/test_02_sqlfcn.py
+-rw-r--r--  4.6 unx     3061 b- defN 23-May-04 03:22 aisdb/tests/test_03_gis.py
+-rw-r--r--  4.6 unx     2399 b- defN 23-May-04 03:22 aisdb/tests/test_04_trackgen.py
+-rw-r--r--  4.6 unx     4517 b- defN 23-May-04 03:22 aisdb/tests/test_05_proc_util.py
+-rw-r--r--  4.6 unx     1124 b- defN 23-May-04 03:22 aisdb/tests/test_06_interp.py
+-rw-r--r--  4.6 unx     1307 b- defN 23-May-04 03:22 aisdb/tests/test_07_bathymetry.py
+-rw-r--r--  4.6 unx     1173 b- defN 23-May-04 03:22 aisdb/tests/test_07_shore_dist.py
+-rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb/tests/test_08_marinetraffic.py
+-rw-r--r--  4.6 unx     1732 b- defN 23-May-04 03:22 aisdb/tests/test_08_wsa.py
+-rw-r--r--  4.6 unx     3722 b- defN 23-May-04 03:22 aisdb/tests/test_09_network_graph.py
+-rw-r--r--  4.6 unx      810 b- defN 23-May-04 03:22 aisdb/tests/test_11_postgres.py
+-rw-r--r--  4.6 unx       76 b- defN 23-May-04 03:22 aisdb/tests/test_rx.py
+-rw-r--r--  4.6 unx  1258678 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20210701.csv
+-rw-r--r--  4.6 unx    84630 b- defN 23-May-04 03:22 aisdb/tests/testdata/test_data_20211101.nm4
+-rw-r--r--  4.6 unx        0 b- defN 23-May-04 03:22 aisdb/webdata/__init__.py
+-rw-r--r--  4.6 unx     2565 b- defN 23-May-04 03:22 aisdb/webdata/_scraper.py
+-rw-r--r--  4.6 unx     5590 b- defN 23-May-04 03:22 aisdb/webdata/bathymetry.py
+-rw-r--r--  4.6 unx     2520 b- defN 23-May-04 03:22 aisdb/webdata/load_raster.py
+-rw-r--r--  4.6 unx    11326 b- defN 23-May-04 03:22 aisdb/webdata/marinetraffic.py
+-rw-r--r--  4.6 unx     2758 b- defN 23-May-04 03:22 aisdb/webdata/shore_dist.py
+-rw-r--r--  4.6 unx    38050 b- defN 23-May-04 03:22 aisdb_lib/Cargo.lock
+-rw-r--r--  4.6 unx      990 b- defN 23-May-04 03:22 aisdb_lib/Cargo.toml
+-rw-r--r--  4.6 unx      139 b- defN 23-May-04 03:22 aisdb_lib/build.rs
+-rw-r--r--  4.6 unx     1672 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/OSM-113e35b9.js
+-rw-r--r--  4.6 unx    17519 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/TileImage-0791bc86.js
+-rw-r--r--  4.6 unx   152923 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/client_bg-7570c46f.wasm
+-rw-r--r--  4.6 unx      688 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/constants-9b7da064.js
+-rw-r--r--  4.6 unx     8224 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/index-f2c4f58e.css
+-rw-r--r--  4.6 unx     1185 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/livestream-ef9daf96.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/main-214e2e5c.js
+-rw-r--r--  4.6 unx   405642 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/map-b944464c.js
+-rw-r--r--  4.6 unx    15782 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/map-c04ede37.css
+-rw-r--r--  4.6 unx    16622 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/proj-3e4e3ac0.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/render-74985482.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/tileserver-bd7f89a4.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/url-91c1e158.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-May-04 03:22 aisdb_web/dist_map/assets/vessel_metadata-af75a617.js
+-rw-r--r--  4.6 unx    26223 b- defN 23-May-04 03:22 aisdb_web/dist_map/favicon.png
+-rw-r--r--  4.6 unx    21571 b- defN 23-May-04 03:22 aisdb_web/dist_map/favicon.svg
+-rw-r--r--  4.6 unx     2675 b- defN 23-May-04 03:22 aisdb_web/dist_map/index.html
+-rw-r--r--  4.6 unx   152923 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/client_bg-7570c46f.wasm
+-rw-r--r--  4.6 unx      616 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/constants-f1a52cc9.js
+-rw-r--r--  4.6 unx     8224 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
+-rw-r--r--  4.6 unx     1185 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/livestream-faa61b7f.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/main-b50358e6.js
+-rw-r--r--  4.6 unx    15782 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
+-rw-r--r--  4.6 unx   405242 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/map-e7b21464.js
+-rw-r--r--  4.6 unx    16622 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/render-0afdbaa3.js
+-rw-r--r--  4.6 unx    20179 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/tileserver-54834007.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/url-51dbde1e.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-ee9a20c1.js
+-rw-r--r--  4.6 unx    26223 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/favicon.png
+-rw-r--r--  4.6 unx    21571 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/favicon.svg
+-rw-r--r--  4.6 unx     2675 b- defN 23-May-04 03:22 aisdb_web/dist_map_bingmaps/index.html
+-rwxr-xr-x  4.6 unx  4936192 b- defN 23-May-04 03:22 aisdb/aisdb.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx    14775 b- defN 23-May-04 03:22 aisdb-1.6.0.dist-info/RECORD
+163 files, 8854155 bytes uncompressed, 3455216 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: aisdb-1.5.8.dist-info/METADATA
+Filename: aisdb-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: aisdb-1.5.8.dist-info/WHEEL
+Filename: aisdb-1.6.0.dist-info/WHEEL
 Comment: 
 
 Filename: aisdb/aisdb_sql/coarsetype.sql
 Comment: 
 
 Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
 Comment: 
@@ -78,14 +78,17 @@
 
 Filename: aisdb/database/sql_query_strings.py
 Comment: 
 
 Filename: aisdb/database/__init__.py
 Comment: 
 
+Filename: aisdb/denoising_encoder.py
+Comment: 
+
 Filename: aisdb/gis.py
 Comment: 
 
 Filename: aisdb/interp.py
 Comment: 
 
 Filename: aisdb/network_graph.py
@@ -177,20 +180,311 @@
 
 Filename: aisdb/webdata/_scraper.py
 Comment: 
 
 Filename: aisdb/webdata/__init__.py
 Comment: 
 
+Filename: aisdb/web_interface.py
+Comment: 
+
 Filename: aisdb/wsa.py
 Comment: 
 
 Filename: aisdb/__init__.py
 Comment: 
 
+Filename: aisdb/__init__.py
+Comment: 
+
+Filename: aisdb/denoising_encoder.py
+Comment: 
+
+Filename: aisdb/gis.py
+Comment: 
+
+Filename: aisdb/interp.py
+Comment: 
+
+Filename: aisdb/network_graph.py
+Comment: 
+
+Filename: aisdb/proc_util.py
+Comment: 
+
+Filename: aisdb/receiver.py
+Comment: 
+
+Filename: aisdb/track_gen.py
+Comment: 
+
+Filename: aisdb/web_interface.py
+Comment: 
+
+Filename: aisdb/wsa.py
+Comment: 
+
+Filename: aisdb/aisdb_sql/coarsetype.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/createtable_griddata.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/createtable_static.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/cte_aliases.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/cte_coarsetype.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/cte_static.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/insert_static.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/select_columns_static.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/select_merged_all.sql
+Comment: 
+
+Filename: aisdb/aisdb_sql/select_static_join_webdata.sql
+Comment: 
+
+Filename: aisdb/database/__init__.py
+Comment: 
+
+Filename: aisdb/database/create_tables.py
+Comment: 
+
+Filename: aisdb/database/dbconn.py
+Comment: 
+
+Filename: aisdb/database/dbqry.py
+Comment: 
+
+Filename: aisdb/database/decoder.py
+Comment: 
+
+Filename: aisdb/database/sql_query_strings.py
+Comment: 
+
+Filename: aisdb/database/sqlfcn.py
+Comment: 
+
+Filename: aisdb/database/sqlfcn_callbacks.py
+Comment: 
+
+Filename: aisdb/tests/__init__.py
+Comment: 
+
+Filename: aisdb/tests/create_testing_data.py
+Comment: 
+
+Filename: aisdb/tests/test_00_decode.py
+Comment: 
+
+Filename: aisdb/tests/test_01_createtables.py
+Comment: 
+
+Filename: aisdb/tests/test_02_dbqry.py
+Comment: 
+
+Filename: aisdb/tests/test_02_sqlfcn.py
+Comment: 
+
+Filename: aisdb/tests/test_03_gis.py
+Comment: 
+
+Filename: aisdb/tests/test_04_trackgen.py
+Comment: 
+
+Filename: aisdb/tests/test_05_proc_util.py
+Comment: 
+
+Filename: aisdb/tests/test_06_interp.py
+Comment: 
+
+Filename: aisdb/tests/test_07_bathymetry.py
+Comment: 
+
+Filename: aisdb/tests/test_07_shore_dist.py
+Comment: 
+
+Filename: aisdb/tests/test_08_marinetraffic.py
+Comment: 
+
+Filename: aisdb/tests/test_08_wsa.py
+Comment: 
+
+Filename: aisdb/tests/test_09_network_graph.py
+Comment: 
+
+Filename: aisdb/tests/test_11_postgres.py
+Comment: 
+
+Filename: aisdb/tests/test_rx.py
+Comment: 
+
+Filename: aisdb/tests/testdata/test_data_20210701.csv
+Comment: 
+
+Filename: aisdb/tests/testdata/test_data_20211101.nm4
+Comment: 
+
+Filename: aisdb/webdata/__init__.py
+Comment: 
+
+Filename: aisdb/webdata/_scraper.py
+Comment: 
+
+Filename: aisdb/webdata/bathymetry.py
+Comment: 
+
+Filename: aisdb/webdata/load_raster.py
+Comment: 
+
+Filename: aisdb/webdata/marinetraffic.py
+Comment: 
+
+Filename: aisdb/webdata/shore_dist.py
+Comment: 
+
+Filename: aisdb_lib/Cargo.lock
+Comment: 
+
+Filename: aisdb_lib/Cargo.toml
+Comment: 
+
+Filename: aisdb_lib/build.rs
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/OSM-113e35b9.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/TileImage-0791bc86.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/client_bg-7570c46f.wasm
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/constants-9b7da064.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/index-f2c4f58e.css
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/livestream-ef9daf96.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/main-214e2e5c.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/map-b944464c.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/map-c04ede37.css
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/proj-3e4e3ac0.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/render-74985482.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/tileserver-bd7f89a4.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/url-91c1e158.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/vessel_metadata-af75a617.js
+Comment: 
+
+Filename: aisdb_web/dist_map/favicon.png
+Comment: 
+
+Filename: aisdb_web/dist_map/favicon.svg
+Comment: 
+
+Filename: aisdb_web/dist_map/index.html
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-7570c46f.wasm
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/constants-f1a52cc9.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/livestream-faa61b7f.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/main-b50358e6.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/map-e7b21464.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/render-0afdbaa3.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-54834007.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/url-51dbde1e.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-ee9a20c1.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/favicon.png
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/favicon.svg
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/index.html
+Comment: 
+
 Filename: aisdb/aisdb.cp39-win_amd64.pyd
 Comment: 
 
-Filename: aisdb-1.5.8.dist-info/RECORD
+Filename: aisdb-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aisdb/database/dbqry.py

```diff
@@ -6,16 +6,18 @@
 from datetime import datetime, timedelta, date
 from functools import reduce
 import warnings
 
 import numpy as np
 
 from aisdb.database import sqlfcn, sqlfcn_callbacks
-from aisdb.database.create_tables import aggregate_static_msgs
-from aisdb.database.dbconn import DBConn, ConnectionType
+from aisdb.database.create_tables import (aggregate_static_msgs,
+                                          sqlite_createtable_dynamicreport,
+                                          sqlite_createtable_staticreport)
+from aisdb.database.dbconn import ConnectionType
 from aisdb.webdata.marinetraffic import VesselInfo
 
 
 class DBQuery(UserDict):
     ''' A database abstraction allowing the creation of SQL code via arguments
         passed to __init__(). Args are stored as a dictionary (UserDict).
 
@@ -47,15 +49,15 @@
         Alternatively, the database can also be queried directly, see
         DBConn.py for more info
 
         complete example:
 
         >>> import os
         >>> from datetime import datetime
-        >>> from aisdb import DBQuery, decode_msgs
+        >>> from aisdb import DBConn, DBQuery, decode_msgs
         >>> from aisdb.database.sqlfcn_callbacks import in_timerange_validmmsi
 
         >>> dbpath = './testdata/test.db'
         >>> start, end = datetime(2021, 7, 1), datetime(2021, 7, 7)
         >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
         ...              'aisdb/tests/testdata/test_data_20211101.nm4']
         >>> with DBConn() as dbconn:
@@ -206,18 +208,17 @@
 
                 # check if static tables exist
                 cur.execute(
                     f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
                     'WHERE type="table" AND name=?', [f'ais_{month}_static'])
                 if len(cur.fetchall()) == 0:
                     #sqlite_createtable_staticreport(self.dbconn, month, dbpath)
-                    warnings.warn(
-                        'No static data for selected time range! '
-                        f'{self.dbconn._get_dbname(dbpath)} {month=} '
-                        f'{rng_string}')
+                    warnings.warn('No static data for selected time range! '
+                                  f'{self.dbconn._get_dbname(dbpath)} '
+                                  f'{rng_string}')
 
                 # check if aggregate tables exist
                 cur.execute((
                     f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master '
                     'WHERE type="table" and name=?'),
                             [f'static_{month}_aggregate'])
                 res = cur.fetchall()
@@ -229,19 +230,21 @@
                     aggregate_static_msgs(self.dbconn, [month], verbose)
 
                 # check if dynamic tables exist
                 cur.execute(
                     f'SELECT * FROM {self.dbconn._get_dbname(dbpath)}.sqlite_master WHERE '
                     'type="table" and name=?', [f'ais_{month}_dynamic'])
                 if len(cur.fetchall()) == 0:  # pragma: no cover
-                    # sqlite_createtable_dynamicreport(self.dbconn, month, dbpath)
-                    warnings.warn(
-                        'No data for selected time range! '
-                        f'{self.dbconn._get_dbname(dbpath)} {month=} '
-                        f'{rng_string}')
+                    if isinstance(self.dbconn, ConnectionType.SQLITE.value):
+                        sqlite_createtable_dynamicreport(
+                            self.dbconn, month, dbpath)
+
+                    warnings.warn('No data for selected time range! '
+                                  f'{self.dbconn._get_dbname(dbpath)} '
+                                  f'{rng_string}')
 
             qry = fcn(dbpath=dbpath, **self.data)
             if verbose:
                 print(qry)
 
             # get 500k rows at a time, yield sets of rows for each unique MMSI
             mmsi_rows = []
@@ -251,15 +254,16 @@
             res = cur.fetchmany(10**5)
             delta = datetime.now() - dt
             if verbose:
                 print(
                     f'query time: {delta.total_seconds():.2f}s\nfetching rows...'
                 )
             if res == []:
-                raise SyntaxError(f'no results for query!\n{qry}')
+                # raise SyntaxError(f'no results for query!\n{qry}')
+                warnings.warn('No results for query!')
 
             while len(res) > 0:
                 mmsi_rows += res
                 ummsi_idx = np.where(
                     np.array(mmsi_rows)[:-1, 0] != np.array(mmsi_rows)[1:, 0]
                 )[0] + 1
                 ummsi_idx = reduce(np.append,
```

## aisdb/database/decoder.py

```diff
@@ -67,15 +67,15 @@
                         'idx_map on hashmap(hash);')
 
     def insert_checksum(self, checksum):
         if isinstance(self.dbconn, SQLiteDBConn):
             dbconn = sqlite3.connect(self.dbconn.dbpaths[0])
         elif isinstance(self.dbconn, PostgresDBConn):
             dbconn = self.dbconn
-        dbconn.execute('INSERT INTO hashmap VALUES ($1,$2)',
+        dbconn.execute('INSERT INTO hashmap VALUES (?,?)',
                        [checksum, pickle.dumps(None)])
         dbconn.commit()
         if isinstance(self.dbconn, SQLiteDBConn):
             dbconn.close()
 
     def checksum_exists(self, checksum):
         # dbconn = sqlite3.connect(self.dbpath)
```

## aisdb/database/sql_query_strings.py

```diff
@@ -35,59 +35,59 @@
     assert ymin < ymax, f'got {ymin=} {ymax=}'
 
     if xmin == -180 and xmax == 180:
         return f'''({alias}.longitude >= {xmin} AND {alias}.longitude <= {xmax}) AND
     {alias}.latitude >= {ymin} AND
     {alias}.latitude <= {ymax}'''
 
-    if xmin < xmax:
-        #if xmin < -180 and xmax > 180:
-        #    raise ValueError(f'xmin, xmax are out of bounds! {xmin=} < -180,{xmax=} > 180')
-        #elif -180 <= xmin <= 180 and -180 <= xmax <= 180:
-        s = f'''{alias}.longitude >= {xmin} AND
-    {alias}.longitude <= {xmax} AND '''
-        """
-        elif xmin < -180:
-            s = f'''(
-        ({alias}.longitude >= -180 AND {alias}.longitude <= {xmax}) OR
-        ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmin])[0]})
-    ) AND '''
-        elif xmax > 180:
-            s = f'''(
-        ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmax])[0]}) OR
-        ({alias}.longitude >= -180 AND {alias}.longitude <= {xmin})
-    ) AND '''
-        else:
-            raise ValueError(
-                f'Error creating SQL query in longitude bounds {xmin=} {xmax=}'
-            )
-        """
+    #if xmin < xmax:
+    assert xmin < xmax
+    #if xmin < -180 and xmax > 180:
+    #    raise ValueError(f'xmin, xmax are out of bounds! {xmin=} < -180,{xmax=} > 180')
+    #elif -180 <= xmin <= 180 and -180 <= xmax <= 180:
+    s = f'''{alias}.longitude >= {xmin} AND
+            {alias}.longitude <= {xmax} AND '''
+    """
+    elif xmin < -180:
+        s = f'''(
+    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmax}) OR
+    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmin])[0]})
+) AND '''
+    elif xmax > 180:
+        s = f'''(
+    ({alias}.longitude <= 180 AND {alias}.longitude >= {shiftcoord([xmax])[0]}) OR
+    ({alias}.longitude >= -180 AND {alias}.longitude <= {xmin})
+) AND '''
+    else:
+        raise ValueError(
+            f'Error creating SQL query in longitude bounds {xmin=} {xmax=}'
+        )
+    """
 
-        query_args = f'''{s}
+    query_args = f'''{s}
     {alias}.latitude >= {ymin} AND
     {alias}.latitude <= {ymax}'''
-        return query_args
 
+    return query_args
+
+    #else:
+    '''
+    if xmin < -180:
+        x0 = shiftcoord([xmin])[0]
+    else:
+        x0 = xmin
+    if xmax > 180:
+        x1 = shiftcoord([xmax])[0]
     else:
-        '''
-        if xmin < -180:
-            x0 = shiftcoord([xmin])[0]
-        else:
-            x0 = xmin
-        if xmax > 180:
-            x1 = shiftcoord([xmax])[0]
-        else:
-            x1 = xmax
-        '''
+        x1 = xmax
+    '''
 
-        #assert x0 <= x1
+    #assert x0 <= x1
 
-        return f'''({alias}.longitude >= {xmin} OR {alias}.longitude <= {xmax}) AND
-    {alias}.latitude >= {ymin} AND
-    {alias}.latitude <= {ymax}'''
+    #return f'''({alias}.longitude >= {xmin} OR {alias}.longitude <= {xmax}) AND {alias}.latitude >= {ymin} AND {alias}.latitude <= {ymax}'''
 
 
 def in_timerange(*, alias, start, end, **_):
     ''' SQL callback restricting vessels in temporal range.
 
         args:
             alias (string)
```

## aisdb/gis.py

```diff
@@ -1,10 +1,12 @@
 '''Geometry and GIS utilities'''
 
 import os
+import pathlib
+import tempfile
 from datetime import datetime, timedelta
 from functools import partial
 
 import numpy as np
 import shapely.ops
 import shapely.geometry
 import warnings
@@ -172,15 +174,14 @@
             point latitude
         z1 (float)
             point depth (metres)
         colname (string)
             track dictionary key for which depth values will be set.
             by default, distances are appended to the 'distance_metres'
             key
-
     '''
     for track in tracks:
         track['dynamic'] = track['dynamic'].union(set([colname]))
         dists = [
             distance3D(x1=x1, y1=y1, x2=x, y2=y, depth_metres=z1)
             for x, y in zip(track['lon'], track['lat'])
         ]
@@ -236,14 +237,15 @@
             self.name
             self.zones
             self.boundary
             self.minX
             self.minY
             self.maxX
             self.maxY
+
     '''
 
     _meridian = LineString(
         np.array((
             (-180, -180, 180, 180),
             (-90, 90, 90, -90),
         )).T)
@@ -252,84 +254,154 @@
         ''' computes the maximum distance to the centroid '''
         return np.max([
             haversine(geom.centroid.x, geom.centroid.y, x2, y2)
             for x2, y2 in zip(zone_x, zone_y)
         ])
 
     def _add_zone(self, name, x, y):
-        if name[-2:] == '_b' and (x0b := np.min(x)) < self.minX_b:
-            self.minX_b = x0b
-        elif name[-2:] != '_c' and (x0c := np.min(x)) > self.minX:
-            self.minX = x0c
-
-        if name[-2:] == '_c' and (x1b := np.max(x)) < self.maxX_c:
-            self.maxX_c = x1b
-        elif name[-2:] != '_b' and (x1c := np.max(x)) > self.maxX:
-            self.maxX = x1c
+        '''
+        if name[-2:] == '_b':
+            if (x0b := np.min(x)) < self.minX_b:
+                self.minX_b = x0b
+            if (x0c := np.min(x)) > self.minX:
+                self.minX = x0c
+
+        elif name[-2:] == '_c':
+            if (x1b := np.max(x)) < self.maxX_c:
+                self.maxX_c = x1b
+            if (x1c := np.max(x)) > self.maxX:
+                self.maxX = x1c
+
+        else:
+        '''
+        if ((x0a := np.min(x)) < self.minX):
+            self.minX = x0a
+        if ((x1a := np.max(x)) > self.maxX):
+            self.maxX = x1a
 
         if np.min(y) < self.minY:
             self.minY = np.min(y)
         if np.max(y) > self.maxY:
             self.maxY = np.max(y)
+        '''
+        if np.min(x) < self.minX:
+            self.minX = np.min(x)
+        if np.max(x) > self.maxX:
+            self.maxX = np.max(x)
+        '''
 
+        assert self.minX < self.maxX
+        assert self.minY < self.maxY
         assert -180 <= self.minX <= 180 and -180 <= self.maxX <= 180
         assert -90 <= self.minY <= 90 and -90 <= self.maxY <= 90
 
         geom = Polygon(zip(x, y))
-        maxradius = self._zone_max_radius(geom, x, y)
 
-        self.zones.update({name: {'geometry': geom, 'maxradius': maxradius}})
+        self.zones.update({
+            name: {
+                'geometry': geom,
+                'maxradius': self._zone_max_radius(geom, x, y)
+            }
+        })
 
         return
 
+    def _handle_outofbounds_zone(self, zone, zones_dir):
+        zones_west = zones_dir / 'west'
+        zones_east = zones_dir / 'east'
+        zones_corr = zones_dir / 'corr'
+        stringify = lambda x, y: map(
+            ','.join, zip(map(str, x), map(lambda y: y + '\n', map(str, y))))
+
+        for g in self.split_geom(zone):
+            if g.centroid.x < -180:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_west):
+                    os.mkdir(zones_west)
+                with open(os.path.join(zones_west, zone['name'] + '_west.txt'),
+                          'w') as w:
+                    w.writelines(stringify(shiftcoord(x), y))
+            elif g.centroid.x > 180:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_east):
+                    os.mkdir(zones_east)
+                with open(os.path.join(zones_east, zone['name'] + '_east.txt'),
+                          'w') as w:
+                    w.writelines(stringify(shiftcoord(x), y))
+            else:
+                x, y = np.array(g.boundary.coords.xy)
+                if not os.path.isdir(zones_corr):
+                    os.mkdir(zones_corr)
+                with open(os.path.join(zones_corr, zone['name'] + '_corr.txt'),
+                          'w') as w:
+                    w.writelines(stringify(x, y))
+
     def __init__(self, name, zones=[], **kw):
-        ''' Initialize the domain from zone geometries, dividing along the 180th meridian '''
+        ''' Initialize the domain from zone geometries '''
+
         if len(zones) == 0:
             raise ValueError(
                 'domain needs to have atleast one polygon geometry')
         self.name = name
         self.zones = {}
         self.minX, self.maxX = 180, -180
-        self.minX_b = 180
+        # self.minX_b = 180
         self.minY, self.maxY = 90, -90
-        self.maxX_c = -180
+        # self.maxX_c = -180
+
+        valid_domain = True
+        zones_dir = pathlib.Path(tempfile.mkdtemp(prefix='aisdb_zones_'))
 
         for zone in zones:
-            assert 'name' in zone.keys(), f'{zone=}'
-            assert 'geometry' in zone.keys(), f'{zone=}'
+            if 'name' not in zone.keys():
+                raise KeyError(f'Zone missing \'name\' key: {zone=}')
+            if 'geometry' not in zone.keys():
+                raise KeyError(f'Zone missing \'geometry\' key: {zone=}')
+
             x, y = zone['geometry'].boundary.coords.xy
             if not (np.min(x) >= -180 and np.max(x) <= 180):
-                warnings.warn(f'dividing geometry... {zone["name"]}')
-                for g in self.split_geom(zone):
-                    if g.centroid.x < -180:
-                        x, y = np.array(g.boundary.coords.xy)
-                        self._add_zone(zone['name'] + '_b', shiftcoord(x), y)
-                    elif g.centroid.x > 180:
-                        x, y = np.array(g.boundary.coords.xy)
-                        self._add_zone(zone['name'] + '_c', shiftcoord(x), y)
-                    else:
-                        x, y = np.array(g.boundary.coords.xy)
-                        self._add_zone(zone['name'] + '_a', x, y)
+                #warnings.warn(f'dividing geometry... {zone["name"]}')
+                valid_domain = False
+                self._handle_outofbounds_zone(zone, zones_dir)
             else:
                 self._add_zone(zone['name'], x, y)
 
+        if not valid_domain:
+            '''
+            if not os.path.isdir(os.path.dirname(
+                    zones_corr)) or not os.path.isdir(zones_corr):
+                print('Creating new output directory in ',
+                      os.path.dirname(zones_dir))
+                os.makedirs(zones_dir, exist_ok=True)
+            '''
+
+            for zonename, zone in self.zones.items():
+                zone['name'] = zonename
+                self._handle_outofbounds_zone(zone, zones_dir)
+
+            raise ValueError(
+                'Invalid zone geometry! '
+                'Exceeds longitude range -180 to 180. '
+                'If you want to query a bounding box spanning 180 degrees '
+                'longitude, consider querying multiple times instead.\n'
+                f'Saved modified geometries in {str(zones_dir)}, try using these corrected domains:\n'
+                f'\tdomain1 = aisdb.DomainFromTxts(domainName=\'{name}_corr\', folder={str(zones_dir)}{os.path.sep}corrected)\n'
+                f'\tdomain2 = aisdb.DomainFromTxts(domainName=\'{name}_west\', folder={str(zones_dir)}{os.path.sep}west))\n'
+                f'\tdomain3 = aisdb.DomainFromTxts(domainName=\'{name}_east\', folder={str(zones_dir)}{os.path.sep}east))\n'
+            )
+
+        assert self.minX < self.maxX
+        assert self.minY < self.maxY
+
         self.boundary = {
             'xmin': self.minX,
             'xmax': self.maxX,
             'ymin': self.minY,
             'ymax': self.maxY
         }
-        if self.minX_b != 180 and self.boundary['xmin'] % 180 != 0:
-            assert self.minX_b >= self.boundary[
-                'xmin'], f'{self.boundary=} {self.minX_b=}'
-            self.boundary.update({'xmin': self.minX_b, 'xmin_alt': self.minX})
-        if self.maxX_c != -180 and self.boundary['xmax'] % 180 != 0:
-            assert self.maxX_c <= self.boundary[
-                'xmax'], f'{self.boundary=} {self.maxX_c=}'
-            self.boundary.update({'xmax': self.maxX_c, 'xmax_alt': self.maxX})
 
     def nearest_polygons_to_point(self, x, y):
         ''' compute great circle distance for this point to each polygon
             centroid, subtracting the maximum polygon radius.
             returns all zones with distances less than zero meters, sorted by
             nearest first
         '''
```

## aisdb/network_graph.py

```diff
@@ -19,18 +19,18 @@
 from aisdb.gis import (
     delta_knots,
     delta_meters,
     epoch_2_dt,
 )
 from aisdb.track_gen import (
     TrackGen,
-    encode_greatcircledistance,
     fence_tracks,
     split_timedelta,
 )
+from aisdb.denoising_encoder import encode_greatcircledistance
 from aisdb.database.dbconn import ConnectionType
 from aisdb.interp import interp_time
 from aisdb.proc_util import _sanitize
 from aisdb.proc_util import _segment_rng
 from aisdb.webdata.bathymetry import Gebco
 from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
 from aisdb.webdata.shore_dist import ShoreDist, PortDist
@@ -319,40 +319,40 @@
                 filepath for resulting CSV output
             maxdelta (datetime.timedelta)
                 maximum time between vessel messages before considering
                 it to be part of a new trajectory. See
                 :func:`aisdb.track_gen.split_timedelta` for more info
             speed_threshold (int, float)
                 maximum speed in knots for encoder segmentation. See
-                :func:`aisdb.track_gen.encode_greatcircledistance` for
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
                 more info
             distance_threshold (int, float)
                 maximum distance in meters for encoder segmentation. See
-                :func:`aisdb.track_gen.encode_greatcircledistance` for
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
                 more info
             interp_delta (timedelta)
                 track positions will be interpolated to the given sample rate
             minscore (float)
                 minimum score for segments to be considered sequential. See
-                :func:`aisdb.track_gen.encode_greatcircledistance` for
+                :func:`aisdb.denoising_encoder.encode_greatcircledistance` for
                 more info
 
         Network graph activity is computed following these steps:
 
             - Create database query with
               :meth:`aisdb.database.dbqry.DBQuery.gen_qry`, and supply
               resulting generator as rowgen arg. Define a domain
               (:class:`aisdb.gis.Domain`) in which to compute movements
             - Vectorize tracks using :py:func:`aisdb.track_gen.TrackGen`
             - Append vessel metadata to track vessels with
               :func:`aisdb.webdata.marinetraffic.vessel_info`
             - Segment track vectors where time between messages exceeds
               maxdelta using :func:`aisdb.track_gen.split_timedelta`
             - Segment track vectors as encoded by
-              :py:func:`aisdb.track_gen.encode_greatcircledistance`
+              :py:func:`aisdb.denoising_encoder.encode_greatcircledistance`
             - Perform geofencing on track segments using
               :py:func:`aisdb.track_gen.fence_tracks` to determine zone
               containment
             - Check where zone boundaries are transited and serialize results
               to ``outputfile``. Additional metrics per zone activity is also
               aggregated at this step.
```

## aisdb/tests/create_testing_data.py

```diff
@@ -24,36 +24,29 @@
     )
     dbconn.execute(
         'INSERT OR IGNORE INTO ais_200001_dynamic (mmsi, time, longitude, latitude, cog, sog) VALUES (000000001, 946702840, -60.994833, 47.434647238127695, -1, -1)'
     )
     dbconn.commit()
 
 
-def sample_random_polygon(xscale=10, yscale=10):
-    vertices = 6
+def sample_random_polygon(xscale=50, yscale=50):
+    vertices = 5
 
     x, y = [0, 0, 0], [0, 0, 0]
     while not Polygon(zip(x, y)).is_valid:
-        x = (np.random.random(vertices) * xscale) + (180 *
-                                                     (np.random.random() - .5))
-        y = (np.random.random(vertices) * yscale) + (90 *
-                                                     (np.random.random() - .5))
-
-    return x, y
-
-
-def sample_invalid_polygon(xscale=10, yscale=10):
-    vertices = 6
-
-    x, y = [0, 0, 0], [0, 0, 0]
-    while not Polygon(zip(x, y)).is_valid:
-        x = (np.random.random(vertices) * xscale) + (3600 *
-                                                     (np.random.random() - .5))
-        y = (np.random.random(vertices) * yscale) + (1800 *
-                                                     (np.random.random() - .5))
+        x = np.random.random(vertices) * xscale
+        x += np.random.randint(360 - xscale)
+        x -= 180
+        y = np.random.random(vertices) * yscale
+        y += np.random.randint(180 - yscale)
+        y -= 90
+        assert min(x) >= -180, min(x)
+        assert max(x) <= 180, max(x)
+        assert min(y) >= -90, min(y)
+        assert max(y) <= 90, max(y)
 
     return x, y
 
 
 def sample_gulfstlawrence_bbox():
     gulfstlawrence_bbox_xy = np.array([
         (-71.64440346704974, 43.18445256159233),
@@ -62,37 +55,24 @@
         (-50.345262703792734, 42.95158299927571),
         (-71.64440346704974, 43.18445256159233),
     ])
     return gulfstlawrence_bbox_xy.T
 
 
 def random_polygons_domain(count=10):
-    return Domain(
-        'testdomain', [{
-            'name': f'random_{i:03}',
-            'geometry': Polygon(zip(*sample_random_polygon()))
-        } for i in range(count)] + [
-            {
-                'name':
-                'outofbounds0',
-                'geometry':
-                Polygon(zip([-200, -170, -170, -200, -200],
-                            [90, 90, 0, 0, 90]))
-            },
-            {
-                'name':
-                'outofbounds1',
-                'geometry':
-                Polygon(zip([200, 170, 170, 200, 200], [-90, -90, 0, 0, -90]))
-            },
-        ])
+    return Domain('testdomain',
+                  [{
+                      'name': f'random_{i:03}',
+                      'geometry': Polygon(zip(*sample_random_polygon()))
+                  } for i in range(count)])
 
 
 def sample_database_file(dbpath):
     ''' test data for date 2021-11-01 '''
+    assert os.path.isdir(os.path.join(os.path.dirname(__file__), 'testdata'))
     datapath_csv = os.path.join(os.path.dirname(__file__), 'testdata',
                                 'test_data_20210701.csv')
     # no static data in nm4
     datapath_nm4 = os.path.join(os.path.dirname(__file__), 'testdata',
                                 'test_data_20211101.nm4')
     months = ["202107", "202111"]
     with DBConn() as dbconn:
```

## aisdb/tests/test_02_dbqry.py

```diff
@@ -22,20 +22,15 @@
             dbpath=dbpath,
             start=datetime(2021, 1, 1),
             end=datetime(2021, 1, 7),
             callback=sqlfcn_callbacks.in_timerange_validmmsi,
         )
         sqlite_createtable_dynamicreport(dbconn, month='202101', dbpath=dbpath)
         rows = q.gen_qry(reaggregate_static=True)
-        try:
-            next(rows)
-        except StopIteration:
-            pass
-        except Exception as err:
-            raise err
+        assert list(rows) == []
 
 
 def test_prepare_qry_domain(tmpdir):
 
     testdbpath = os.path.join(tmpdir, 'test_prepare_qry_domain.db')
     months = sample_database_file(testdbpath)
     start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
@@ -47,20 +42,15 @@
             dbconn=aisdatabase,
             dbpath=testdbpath,
             start=start,
             end=end,
             **domain.boundary,
             callback=sqlfcn_callbacks.in_timerange,
         ).gen_qry(reaggregate_static=True)
-        try:
-            next(rowgen)
-        except SyntaxError:
-            pass
-        except Exception as err:
-            raise err
+        next(rowgen)
 
 
 def test_sql_query_strings(tmpdir):
     testdbpath = os.path.join(tmpdir, 'test_sql_query_strings.db')
     months = sample_database_file(testdbpath)
     start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
     end = start + timedelta(weeks=4)
@@ -82,14 +72,8 @@
                 start=start,
                 end=end,
                 **domain.boundary,
                 callback=callback,
                 mmsi=316000000,
                 mmsis=[316000000, 316000001],
             ).gen_qry(fcn=sqlfcn.crawl_dynamic_static)
-            try:
-                next(rowgen)
-            except SyntaxError:
-                pass
-            except Exception as err:
-                raise err
-    return
+            next(rowgen)
```

## aisdb/tests/test_02_sqlfcn.py

```diff
@@ -71,16 +71,16 @@
             sqlfcn_callbacks.in_time_bbox_validmmsi,
             sqlfcn_callbacks.in_time_mmsi,
             sqlfcn_callbacks.in_timerange,
             sqlfcn_callbacks.in_timerange_hasmmsi,
             sqlfcn_callbacks.in_timerange_inmmsi,
             sqlfcn_callbacks.in_timerange_validmmsi,
     ]:
-        box_x = np.random.random(2) * 360 - 180
-        box_y = np.random.random(2) * 180 - 90
+        box_x = sorted(np.random.random(2) * 360 - 180)
+        box_y = sorted(np.random.random(2) * 180 - 90)
         kwargs = dict(
             start=start,
             end=start + timedelta(days=7),
             xmin=box_x[0],
             xmax=box_x[1],
             ymin=min(box_y),
             ymax=max(box_y),
```

## aisdb/tests/test_03_gis.py

```diff
@@ -1,18 +1,45 @@
 import os
 
 from shapely.geometry import Polygon
 import numpy as np
 import zipfile
 
-from aisdb.gis import Domain, DomainFromTxts, DomainFromPoints, shiftcoord, distance3D
+from aisdb.gis import (
+    Domain,
+    DomainFromPoints,
+    DomainFromTxts,
+    distance3D,
+    shiftcoord,
+)
 from aisdb.tests.create_testing_data import random_polygons_domain
 from aisdb.tests.create_testing_data import sample_gulfstlawrence_bbox
 
 
+def test_invalid_domain():
+    try:
+        Domain('errordomain', [{
+            'name':
+            'outofbounds0',
+            'geometry':
+            Polygon(zip([-200, -170, -170, -200, -200], [90, 90, 0, 0, 90]))
+        }, {
+            'name':
+            'outofbounds1',
+            'geometry':
+            Polygon(zip([200, 170, 170, 200, 200], [-90, -90, 0, 0, -90]))
+        }])
+    except ValueError:
+        return
+    except Exception as e:
+        raise (e)
+
+    raise RuntimeError('This test should fail with a ValueError')
+
+
 def test_domain():
     domain = random_polygons_domain(count=10)
     dist_to_centroids = domain.nearest_polygons_to_point(-64, 45)
 
     print(dist_to_centroids)
 
     for name, zone in domain.zones.items():
@@ -48,36 +75,22 @@
 
 
 def test_domain_points_in_polygon():
     lon, lat = sample_gulfstlawrence_bbox()
     z1 = Polygon(zip(lon, lat))
     z2 = Polygon(zip(lon - 145, lat))
     z3 = Polygon(zip(lon, lat - 45))
-    domain = Domain('gulf domain',
-                    zones=[
-                        {
-                            'name': 'z1',
-                            'geometry': z1
-                        },
-                        {
-                            'name': 'z2',
-                            'geometry': z2
-                        },
-                        {
-                            'name': 'z3',
-                            'geometry': z3
-                        },
-                    ])
+    domain1 = Domain('gulf domain', zones=[{'name': 'z1', 'geometry': z1}])
 
     xx = [z1.centroid.x, z2.centroid.x, z3.centroid.x]
     yy = [z1.centroid.y, z2.centroid.y, z3.centroid.y]
-    test = [domain.point_in_polygon(x, y) for x, y in zip(xx, yy)]
+    test = [domain1.point_in_polygon(x, y) for x, y in zip(xx, yy)]
     assert test[0] == 'z1'
     assert test[1] == 'Z0'
-    assert test[2] == 'z3'
+    assert test[2] == 'Z0'
 
 
 def test_shiftcoord():
     x = np.array([-360, -270, -180, -90, 0, 90, 180, 270, 360])
     xshift = shiftcoord(x)
     assert sum(xshift == np.array([0, 90, 180, -90, 0, 90, -180, -90, 0])) == 9
```

## aisdb/tests/test_04_trackgen.py

```diff
@@ -3,15 +3,16 @@
 
 import numpy as np
 
 from aisdb import track_gen, sqlfcn_callbacks
 from aisdb.gis import vesseltrack_3D_dist, mask_in_radius_2D
 from aisdb.database.dbconn import DBConn
 from aisdb.database.dbqry import DBQuery
-from aisdb.track_gen import encode_greatcircledistance, min_speed_filter
+from aisdb import encode_greatcircledistance
+from aisdb.track_gen import min_speed_filter
 from aisdb.tests.create_testing_data import sample_database_file
 
 
 def test_TrackGen(tmpdir):
     dbpath = os.path.join(tmpdir, 'test_trackgen.db')
     months = sample_database_file(dbpath)
     start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
```

## aisdb/tests/test_07_shore_dist.py

```diff
@@ -1,35 +1,36 @@
 import os
 
 import numpy as np
 
 from aisdb.webdata.shore_dist import ShoreDist, PortDist
 
 data_dir = os.environ.get(
-        'AISDBDATADIR',
-        os.path.join(
-            os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
-            'testdata',
-            ),
-        )
+    'AISDBDATADIR',
+    os.path.join(
+        os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
+        'testdata',
+    ),
+)
 
 y1, x1 = 48.271185186388735, -61.10595523571155
 
 tracks_short = [
-        dict(
-            lon=np.array([x1]),
-            lat=np.array([y1]),
-            time=[0],
-            dynamic=set(['time']),
-            )
-        ]
+    dict(
+        lon=np.array([x1]),
+        lat=np.array([y1]),
+        time=[0],
+        dynamic=set(['time']),
+    )
+]
 
 
 def test_ShoreDist():
     imgpath = os.path.join(data_dir, 'distance-from-shore.tif')
+    assert os.path.isfile(imgpath)
     with ShoreDist(data_dir=data_dir) as sdist:
         for track in sdist.get_distance(tracks_short):
             assert 'km_from_shore' in track.keys()
             assert 'km_from_shore' in track['dynamic']
 
 
 def test_PortDist():
```

## aisdb/tests/test_08_wsa.py

```diff
@@ -1,15 +1,14 @@
 import os
 from datetime import datetime, timedelta
-import pickle
 
 import warnings
 
 from aisdb import track_gen, DBQuery, sqlfcn_callbacks, DBConn
-from aisdb.track_gen import encode_greatcircledistance
+from aisdb import encode_greatcircledistance
 from aisdb.wsa import wetted_surface_area
 from aisdb.database import sqlfcn
 from aisdb.webdata.marinetraffic import vessel_info, VesselInfo
 
 from aisdb.tests.create_testing_data import sample_database_file
 
 testdir = os.environ.get(
```

## aisdb/tests/test_09_network_graph.py

```diff
@@ -6,15 +6,16 @@
 import os
 from datetime import datetime, timedelta
 
 from shapely.geometry import Polygon
 import warnings
 
 from aisdb.database import sqlfcn, sqlfcn_callbacks
-from aisdb.database.dbqry import DBQuery, DBConn
+from aisdb.database.dbqry import DBQuery
+from aisdb.database.dbconn import DBConn
 from aisdb.gis import Domain
 from aisdb.network_graph import graph
 from aisdb.tests.create_testing_data import (
     sample_database_file,
     sample_gulfstlawrence_bbox,
 )
 
@@ -32,34 +33,35 @@
         os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
         'testdata',
     ),
 )
 
 lon, lat = sample_gulfstlawrence_bbox()
 z1 = Polygon(zip(lon, lat))
-z2 = Polygon(zip(lon - 145, lat))
+z2 = Polygon(zip(lon - 45, lat))
 z3 = Polygon(zip(lon, lat - 45))
-domain = Domain('gulf domain',
-                zones=[
-                    {
-                        'name': 'z1',
-                        'geometry': z1
-                    },
-                    {
-                        'name': 'z2',
-                        'geometry': z2
-                    },
-                    {
-                        'name': 'z3',
-                        'geometry': z3
-                    },
-                ])
 
 
 def test_graph_minimal(tmpdir):
+    domain = Domain('gulf domain',
+                    zones=[
+                        {
+                            'name': 'z1',
+                            'geometry': z1
+                        },
+                        {
+                            'name': 'z2',
+                            'geometry': z2
+                        },
+                        {
+                            'name': 'z3',
+                            'geometry': z3
+                        },
+                    ])
+
     testdbpath = os.path.join(tmpdir, 'test_graph_minimal.db')
 
     months = sample_database_file(testdbpath)
     start = datetime(int(months[0][0:4]), int(months[0][4:6]), 1)
     end = start + timedelta(weeks=1)
 
     with DBConn() as aisdatabase:
```

## aisdb/track_gen.py

```diff
@@ -2,18 +2,17 @@
 
 from functools import reduce
 from datetime import timedelta
 import sqlite3
 import types
 
 import numpy as np
-import warnings
 
-from aisdb.aisdb import simplify_linestring_idx, encoder_score_fcn
-from aisdb.gis import delta_knots, delta_meters
+from aisdb.aisdb import simplify_linestring_idx
+from aisdb.gis import delta_knots
 from aisdb.proc_util import _segment_rng
 from aisdb import Domain
 
 staticcols = set([
     'mmsi', 'vessel_name', 'ship_type', 'ship_type_txt', 'dim_bow',
     'dim_stern', 'dim_port', 'dim_star', 'imo', 'draught'
 ])
@@ -99,20 +98,18 @@
             static data (e.g. mmsi, name, geometry) will be stored as
             scalar values
 
         >>> import os
         >>> from datetime import datetime
         >>> from aisdb import DBConn, DBQuery, TrackGen, decode_msgs
         >>> from aisdb.database import sqlfcn_callbacks
-
         >>> # create example database file
         >>> dbpath = 'track_gen_test.db'
         >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
         ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-
         >>> with DBConn() as dbconn:
         ...     decode_msgs(filepaths=filepaths, dbconn=dbconn, dbpath=dbpath,
         ...     source='TESTING')
         ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
         ...             dbconn=dbconn,
         ...             dbpath=dbpath,
         ...             start=datetime(2021, 7, 1),
@@ -154,221 +151,22 @@
     for track in tracks:
         for rng in _segment_rng(track, maxdelta):
             assert len(rng) > 0
             yield dict(
                 **{k: track[k]
                    for k in track['static']},
                 **{
-                    k: np.array(track[k], dtype=object)[rng]
+                    k: np.array(track[k], dtype=type(track[k][0]))[rng]
                     for k in track['dynamic']
                 },
                 static=track['static'],
                 dynamic=track['dynamic'],
             )
 
 
-def _score_idx(scores):
-    ''' Returns indices of score array where value at index is equal to the
-        highest score. In tie cases, the last index will be selected
-    '''
-    assert len(scores) > 0
-    return np.where(scores == np.max(scores))[0][-1]
-
-
-def _segments_idx(track, distance_threshold, speed_threshold, **_):
-    segments_idx1 = reduce(
-        np.append, ([0], np.where(delta_knots(track) > speed_threshold)[0] + 1,
-                    [track['time'].size]))
-    segments_idx2 = reduce(
-        np.append,
-        ([0], np.where(delta_meters(track) > distance_threshold)[0] + 1,
-         [track['time'].size]))
-
-    return reduce(np.union1d, (segments_idx1, segments_idx2))
-
-
-def _scoresarray(track, *, pathways, i, segments_idx, distance_threshold,
-                 speed_threshold, minscore):
-    scores = np.array(
-        [
-            encoder_score_fcn(
-                x1=pathway['lon'][-1],
-                y1=pathway['lat'][-1],
-                t1=pathway['time'][-1],
-                x2=track['lon'][segments_idx[i]],
-                y2=track['lat'][segments_idx[i]],
-                t2=track['time'][segments_idx[i]],
-                dist_thresh=distance_threshold,
-                speed_thresh=speed_threshold,
-            ) for pathway in pathways
-        ],
-        dtype=np.float32,
-    )
-    highscore = (scores[np.where(
-        scores == np.max(scores))[0][0]] if scores.size > 0 else minscore)
-    return scores, highscore
-
-
-def _append_highscore(track, *, highscoreidx, pathways, i, segments_idx):
-    return dict(
-        **{k: track[k]
-           for k in track['static']},
-        **{
-            k: np.append(pathways[highscoreidx][k],
-                         track[k][segments_idx[i]:segments_idx[i + 1]])
-            for k in track['dynamic']
-        },
-        static=track['static'],
-        dynamic=track['dynamic'],
-    )
-
-
-def _split_pathway(track, *, i, segments_idx):
-    path = dict(
-        **{k: track[k]
-           for k in track['static']},
-        **{
-            k: track[k][segments_idx[i]:segments_idx[i + 1]]
-            for k in track['dynamic']
-        },
-        static=track['static'],
-        dynamic=track['dynamic'],
-    )
-    return path
-
-
-def encode_score(track, distance_threshold, speed_threshold, minscore):
-    ''' Encodes likelihood of persistent track membership when given distance,
-        speed, and score thresholds, using track speed deltas computed using
-        distance computed by haversine function divided by elapsed time
-
-        A higher distance threshold will increase the maximum distance in
-        meters allowed between pings for same trajectory membership. A higher
-        speed threshold will allow vessels travelling up to this value in knots
-        to be kconsidered for persistent track membership.
-        The minscore assigns a minimum score needed to be considered for
-        membership, typically 0 or very close to 0 such as 1e-5.
-
-        For example: a vessel travelling at a lower speed with short intervals
-        between pings will have a higher likelihood of persistence.
-        A trajectory with higher average speed or long intervals between
-        pings may indicate two separate trajectories and will be segmented
-        forming alternate trajectories according to highest likelihood of
-        membership.
-    '''
-    assert 'time' in track.keys()
-    assert len(track['time']) > 0
-    params = dict(distance_threshold=distance_threshold,
-                  speed_threshold=speed_threshold,
-                  minscore=minscore)
-    segments_idx = _segments_idx(track, **params)
-    pathways = []
-    warned = False
-    for i in range(segments_idx.size - 1):
-        if len(pathways) == 0:
-            path = _split_pathway(track, i=i, segments_idx=segments_idx)
-            assert path is not None
-            pathways.append(path)
-            continue
-        elif not warned and len(pathways) > 100:
-            warnings.warn(
-                f'excessive number of pathways! mmsi={track["mmsi"]}')
-            warned = True
-        assert len(track['time']) > 0, f'{track=}'
-
-        scores, highscore = _scoresarray(track,
-                                         pathways=pathways,
-                                         i=i,
-                                         segments_idx=segments_idx,
-                                         **params)
-        assert len(scores) > 0, f'{track}'
-        if (highscore >= minscore):
-            highscoreidx = _score_idx(scores)
-            pathways[highscoreidx] = _append_highscore(
-                track,
-                highscoreidx=highscoreidx,
-                pathways=pathways,
-                i=i,
-                segments_idx=segments_idx)
-        else:
-            path = _split_pathway(track, i=i, segments_idx=segments_idx)
-            assert path is not None
-            pathways.append(path.copy())
-
-    for pathway, label in zip(pathways, range(len(pathways))):
-        pathway['label'] = label
-        pathway['static'] = set(pathway['static']).union({'label'})
-        assert 'label' in pathway.keys()
-        assert 'time' in pathway.keys(), f'{pathway=}'
-        yield pathway
-
-
-def encode_greatcircledistance(
-    tracks,
-    *,
-    distance_threshold,
-    speed_threshold=50,
-    minscore=1e-6,
-):
-    ''' partitions tracks where delta speeds exceed speed_threshold or
-        delta_meters exceeds distance_threshold.
-        concatenates track segments with the highest likelihood of being
-        sequential, as encoded by the encode_score function
-
-        args:
-            tracks (aisdb.track_gen.TrackGen)
-                track vectors generator
-            distance_threshold (int)
-                distance in meters that will be used as a
-                speed score numerator
-            time_threshold (datetime.timedelta)
-            minscore (float)
-                minimum score threshold at which to allow track
-                segments to be linked
-
-        >>> import os
-        >>> from datetime import datetime, timedelta
-        >>> from aisdb import DBConn, DBQuery, TrackGen
-        >>> from aisdb import decode_msgs, encode_greatcircledistance, sqlfcn_callbacks
-
-        >>> # create example database file
-        >>> dbpath = 'encoder_test.db'
-        >>> filepaths = ['aisdb/tests/testdata/test_data_20210701.csv',
-        ...              'aisdb/tests/testdata/test_data_20211101.nm4']
-        >>> with DBConn() as dbconn:
-        ...     decode_msgs(filepaths=filepaths, dbconn=dbconn,
-        ...     dbpath=dbpath, source='TESTING')
-
-        >>> with DBConn() as dbconn:
-        ...     q = DBQuery(callback=sqlfcn_callbacks.in_timerange_validmmsi,
-        ...             dbconn=dbconn,
-        ...             dbpath=dbpath,
-        ...             start=datetime(2021, 7, 1),
-        ...             end=datetime(2021, 7, 7))
-        ...     tracks = TrackGen(q.gen_qry(), decimate=True)
-        ...     for track in encode_greatcircledistance(
-        ...             tracks,
-        ...             distance_threshold=250000,  # metres
-        ...             speed_threshold=50,  # knots
-        ...             minscore=0):
-        ...         print(track['mmsi'])
-        ...         print(track['lon'], track['lat'])
-        ...         break
-        204242000
-        [-8.931666] [41.45]
-        >>> os.remove(dbpath)
-
-    '''
-    for track in tracks:
-        assert isinstance(track, dict), f'got {type(track)} {track}'
-        for path in encode_score(track, distance_threshold, speed_threshold,
-                                 minscore):
-            yield path
-
-
 def fence_tracks(tracks, domain):
     ''' compute points-in-polygons for vessel positions within domain polygons
 
         yields track dictionaries
 
         Also see zone_mask()
     '''
```

## aisdb/webdata/bathymetry.py

```diff
@@ -128,15 +128,15 @@
         for track in tracks:
             # mapping of filepaths to the corresponding boundary region
             raster_keys = np.array(list(self._check_in_bounds(track)),
                                    dtype=object)
 
             # ensure that each vector time slice has a value
             if len(raster_keys) != len(track['time']):
-                raise ValueError(f'no rasters found for track')
+                raise ValueError('no rasters found for track')
             bathy_segments = np.append(
                 np.append([0],
                           np.where(raster_keys[:-1] != raster_keys[:1])[0]),
                 [len(raster_keys)],
             )
             track['depth_metres'] = reduce(np.append, [
                 self.rasterfiles[raster_keys[i]]
```

## aisdb/__init__.py

```diff
@@ -7,14 +7,16 @@
         or (sqlite3.sqlite_version_info[0] <= 3
             and sqlite3.sqlite_version_info[1] < 8)):
     warnings.warn(
         f"An outdated version of SQLite was found ({sqlite3.sqlite_version})")
 
 sqlpath = os.path.abspath(os.path.join(os.path.dirname(__file__), 'aisdb_sql'))
 
+import aisdb.web_interface
+
 from .database.create_tables import (
     aggregate_static_msgs,
     sqlite_createtable_dynamicreport,
     sqlite_createtable_staticreport,
 )
 
 from .database.dbconn import DBConn, SQLiteDBConn, PostgresDBConn
@@ -57,14 +59,16 @@
     write_csv,
 )
 
 from .track_gen import (
     TrackGen,
     split_timedelta,
     fence_tracks,
+)
+from .denoising_encoder import (
     encode_score,
     encode_greatcircledistance,
 )
 
 LOGLEVEL = os.environ.get('LOGLEVEL', 'INFO')
 logging.basicConfig(format='%(message)s',
                     level=LOGLEVEL,
```

## Comparing `aisdb-1.5.8.dist-info/METADATA` & `aisdb-1.6.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdb
-Version: 1.5.8
+Version: 1.6.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,35 +21,34 @@
 Requires-Dist: pillow
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: shapely
 Requires-Dist: tqdm
 Requires-Dist: numpy
 Requires-Dist: webdriver-manager
+Requires-Dist: psycopg
 Requires-Dist: psycopg[binary]
+Requires-Dist: orjson
+Requires-Dist: websockets
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-dotenv; extra == 'test'
-Requires-Dist: psycopg; extra == 'devel'
-Requires-Dist: orjson; extra == 'web_api'
-Requires-Dist: websockets; extra == 'web_api'
-Requires-Dist: sphinx; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme; extra == 'docs'
+Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: devel
-Provides-Extra: web_api
-Provides-Extra: docs
 Summary: AIS Database and Processing Utils
 Author-email: Matthew Smith <matthew.smith@dal.ca>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
+Project-URL: documentation, https://aisdb.meridian.cs.dal.ca/doc/readme.html
 Project-URL: repository, https://git-dev.cs.dal.ca/meridian/aisdb
 Project-URL: homepage, https://aisdb.meridian.cs.dal.ca/
-Project-URL: documentation, https://aisdb.meridian.cs.dal.ca/doc/readme.html
 
 Readme
 ======
 
 .. image:: https://git-dev.cs.dal.ca/meridian/aisdb/badges/master/pipeline.svg
 
 .. image:: https://img.shields.io/gitlab/coverage/meridian/aisdb/master?gitlab_url=https%3A%2F%2Fgit-dev.cs.dal.ca&job_name=python-test
```

