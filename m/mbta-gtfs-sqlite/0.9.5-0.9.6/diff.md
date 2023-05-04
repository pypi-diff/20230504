# Comparing `tmp/mbta-gtfs-sqlite-0.9.5.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.5.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.6.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.5.tar` & `mbta-gtfs-sqlite-0.9.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     2265 2023-05-02 03:05:44.353658 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      312 2023-04-30 02:20:13.261136 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     4110 2023-05-02 12:21:38.720435 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6281 2023-05-01 18:28:34.679685 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1970 2023-05-02 13:18:10.062598 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-02 13:18:57.459477 mbta-gtfs-sqlite-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-02 13:19:12.908566 mbta-gtfs-sqlite-0.9.5/setup.py
--rw-r--r--   0        0        0      494 2023-05-02 13:19:12.908792 mbta-gtfs-sqlite-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     4302 2023-05-04 05:02:09.173183 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6281 2023-05-03 21:20:38.555719 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     1970 2023-05-02 13:18:10.062598 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-04 14:36:14.832754 mbta-gtfs-sqlite-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-04 14:37:04.412120 mbta-gtfs-sqlite-0.9.6/setup.py
+-rw-r--r--   0        0        0      494 2023-05-04 14:37:04.412383 mbta-gtfs-sqlite-0.9.6/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/build.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
-from os import path, remove
-from shutil import copy
+from os import path, remove, listdir
+from shutil import copy, rmtree
 from zipfile import ZipFile
 from hashlib import md5
 
 
 import requests
 
 from .reader import GtfsReader
@@ -24,14 +24,21 @@
         for data in response.iter_content(block_size):
             file.write(data)
 
 
 def unzip_feed(zip_path: str, target_path: str):
     zf = ZipFile(zip_path)
     zf.extractall(target_path)
+    items = listdir(target_path)
+    if len(items) == 1:
+        inner_dir = items[0]
+        inner_dir_path = path.join(target_path, inner_dir)
+        for file in listdir(inner_dir_path):
+            copy(path.join(inner_dir_path, file), target_path)
+        rmtree(inner_dir_path)
 
 
 def get_zip_checksum(zip_path: str) -> str:
     with open(zip_path, "rb") as file:
         chunk_size = 4096
         hasher = md5()
         while chunk := file.read(chunk_size):
@@ -43,40 +50,59 @@
 def ingest_feed_to_sqlite(
     feed_path: str,
     db_path: str,
     compact_db_path: str,
     result: GtfsFeedDownloadResult,
 ):
     from .ingest import ingest_gtfs_csv_into_db
-    from .compact import make_compact_db
     from .session import create_sqlalchemy_session
 
     try:
         reader = GtfsReader(feed_path)
         session = create_sqlalchemy_session(db_path)
         ingest_gtfs_csv_into_db(session, result, reader)
-        copy(db_path, compact_db_path)
-        compact_session = create_sqlalchemy_session(compact_db_path)
-        make_compact_db(compact_session)
     except Exception as ex:
         try:
             remove(db_path)
+        except FileNotFoundError:
+            pass
+        raise ex
+
+
+def compress_sqlite_feed(db_path: str, compact_db_path: str):
+    from .compact import make_compact_db
+    from .session import create_sqlalchemy_session
+
+    try:
+        copy(db_path, compact_db_path)
+        session = create_sqlalchemy_session(compact_db_path)
+        make_compact_db(session)
+    except Exception as ex:
+        try:
             remove(compact_db_path)
         except FileNotFoundError:
             pass
         raise ex
 
 
-def build_local_feed_entry(feed: GtfsFeed, compact_only=False):
+def build_local_feed_entry(
+    feed: GtfsFeed,
+    compact_only=False,
+    rebuild_db=True,
+    rebuild_compact_db=True,
+):
     (zip_path, feed_path, db_path, compact_db_path) = (
         path.join(feed.local_subdirectory, entity)
         for entity in ("data.zip", "feed", "gtfs.sqlite3", "gtfs_compact.sqlite3")
     )
     download_feed_zip(feed.url, zip_path)
     unzip_feed(zip_path, feed_path)
     result = GtfsFeedDownloadResult(
         url=feed.url,
         zip_md5_checksum=get_zip_checksum(zip_path),
     )
-    ingest_feed_to_sqlite(feed_path, db_path, compact_db_path, result)
+    if not path.exists(db_path) or rebuild_db:
+        ingest_feed_to_sqlite(feed_path, db_path, compact_db_path, result)
+    if not path.exists(compact_db_path) or rebuild_compact_db:
+        compress_sqlite_feed(db_path, compact_db_path)
     if compact_only:
         remove(db_path)
```

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/feed.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,19 +56,24 @@
         except RuntimeError:
             return False
         for file in self.required_feed_files():
             if not any(obj.key.endswith(file) for obj in remote_objects):
                 return False
         return True
 
-    def build_locally(self):
+    def build_locally(self, rebuild_compact_db: bool = True, rebuild_db: bool = True):
         from .build import build_local_feed_entry
 
         self.ensure_subdirectory()
-        build_local_feed_entry(self, self.compact_only)
+        build_local_feed_entry(
+            self,
+            compact_only=self.compact_only,
+            rebuild_compact_db=rebuild_compact_db,
+            rebuild_db=rebuild_db,
+        )
 
     def download_from_s3(self):
         if not self.exists_remotely():
             raise RuntimeError("Feed does not exist remotely")
         self.ensure_subdirectory()
         for file in self.required_feed_files():
             self.archive.s3_bucket.download_file(
```

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/ingest.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/models/trips.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/indexes.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.6/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.5/setup.py` & `mbta-gtfs-sqlite-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

