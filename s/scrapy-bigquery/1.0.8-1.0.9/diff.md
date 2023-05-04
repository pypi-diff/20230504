# Comparing `tmp/scrapy-bigquery-1.0.8.tar.gz` & `tmp/scrapy-bigquery-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-bigquery-1.0.8.tar", last modified: Fri Jan 21 01:42:26 2022, max compression
+gzip compressed data, was "scrapy-bigquery-1.0.9.tar", last modified: Fri Jan 21 22:31:28 2022, max compression
```

## Comparing `scrapy-bigquery-1.0.8.tar` & `scrapy-bigquery-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 01:42:26.833142 scrapy-bigquery-1.0.8/
--rw-r--r--   0 sackfield   (501) staff       (20)     1071 2021-08-06 06:28:47.000000 scrapy-bigquery-1.0.8/LICENSE
--rw-r--r--   0 sackfield   (501) staff       (20)       64 2021-08-06 08:39:11.000000 scrapy-bigquery-1.0.8/MANIFEST.in
--rw-r--r--   0 sackfield   (501) staff       (20)     3845 2022-01-21 01:42:26.833005 scrapy-bigquery-1.0.8/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)     2815 2021-09-15 11:59:57.000000 scrapy-bigquery-1.0.8/README.md
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 01:42:26.831800 scrapy-bigquery-1.0.8/bigquerypipeline/
--rw-r--r--   0 sackfield   (501) staff       (20)        0 2021-08-06 06:48:23.000000 scrapy-bigquery-1.0.8/bigquerypipeline/__init__.py
--rw-r--r--   0 sackfield   (501) staff       (20)     4083 2022-01-21 01:41:54.000000 scrapy-bigquery-1.0.8/bigquerypipeline/pipelines.py
--rw-r--r--   0 sackfield   (501) staff       (20)       75 2022-01-21 01:36:46.000000 scrapy-bigquery-1.0.8/requirements.txt
-drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 01:42:26.832819 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/
--rw-r--r--   0 sackfield   (501) staff       (20)     3845 2022-01-21 01:42:26.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 sackfield   (501) staff       (20)      346 2022-01-21 01:42:26.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2022-01-21 01:42:26.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 sackfield   (501) staff       (20)        1 2021-08-06 09:10:32.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 sackfield   (501) staff       (20)       75 2022-01-21 01:42:26.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/requires.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       17 2022-01-21 01:42:26.000000 scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/top_level.txt
--rw-r--r--   0 sackfield   (501) staff       (20)       38 2022-01-21 01:42:26.833183 scrapy-bigquery-1.0.8/setup.cfg
--rw-r--r--   0 sackfield   (501) staff       (20)     1310 2022-01-21 01:42:04.000000 scrapy-bigquery-1.0.8/setup.py
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 22:31:28.375535 scrapy-bigquery-1.0.9/
+-rw-r--r--   0 sackfield   (501) staff       (20)     1071 2021-08-06 06:28:47.000000 scrapy-bigquery-1.0.9/LICENSE
+-rw-r--r--   0 sackfield   (501) staff       (20)       64 2021-08-06 08:39:11.000000 scrapy-bigquery-1.0.9/MANIFEST.in
+-rw-r--r--   0 sackfield   (501) staff       (20)     3845 2022-01-21 22:31:28.375395 scrapy-bigquery-1.0.9/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)     2815 2021-09-15 11:59:57.000000 scrapy-bigquery-1.0.9/README.md
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 22:31:28.374226 scrapy-bigquery-1.0.9/bigquerypipeline/
+-rw-r--r--   0 sackfield   (501) staff       (20)        0 2021-08-06 06:48:23.000000 scrapy-bigquery-1.0.9/bigquerypipeline/__init__.py
+-rw-r--r--   0 sackfield   (501) staff       (20)     4244 2022-01-21 22:29:47.000000 scrapy-bigquery-1.0.9/bigquerypipeline/pipelines.py
+-rw-r--r--   0 sackfield   (501) staff       (20)       75 2022-01-21 01:36:46.000000 scrapy-bigquery-1.0.9/requirements.txt
+drwxr-xr-x   0 sackfield   (501) staff       (20)        0 2022-01-21 22:31:28.375184 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/
+-rw-r--r--   0 sackfield   (501) staff       (20)     3845 2022-01-21 22:31:28.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 sackfield   (501) staff       (20)      346 2022-01-21 22:31:28.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2022-01-21 22:31:28.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)        1 2021-08-06 09:10:32.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 sackfield   (501) staff       (20)       75 2022-01-21 22:31:28.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/requires.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       17 2022-01-21 22:31:28.000000 scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 sackfield   (501) staff       (20)       38 2022-01-21 22:31:28.375579 scrapy-bigquery-1.0.9/setup.cfg
+-rw-r--r--   0 sackfield   (501) staff       (20)     1310 2022-01-21 22:30:23.000000 scrapy-bigquery-1.0.9/setup.py
```

### Comparing `scrapy-bigquery-1.0.8/LICENSE` & `scrapy-bigquery-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-bigquery-1.0.8/PKG-INFO` & `scrapy-bigquery-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-bigquery
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scrapy pipeline to store items into BigQuery
 Home-page: https://github.com/8W9aG/scrapy-bigquery
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Description: # scrapy-bigquery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapy-bigquery Version: 1.0.8 Summary: Scrapy
+Metadata-Version: 2.1 Name: scrapy-bigquery Version: 1.0.9 Summary: Scrapy
 pipeline to store items into BigQuery Home-page: https://github.com/8W9aG/
 scrapy-bigquery Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Description: # scrapy-bigquery [PyPi] A Big Query pipeline to
 store items into [Google BigQuery](https://cloud.google.com/bigquery/). ##
 Dependencies :globe_with_meridians: * [Python 3.7](https://www.python.org/
 downloads/release/python-370/) * [Scrapy 2.4.0](https://scrapy.org/) * [Google
 Cloud Bigquery 2.23.2](https://pypi.org/project/google-cloud-bigquery/) *
```

### Comparing `scrapy-bigquery-1.0.8/README.md` & `scrapy-bigquery-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-bigquery-1.0.8/bigquerypipeline/pipelines.py` & `scrapy-bigquery-1.0.9/bigquerypipeline/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,17 @@
             )
         dataset = crawler.settings.get("BIGQUERY_DATASET")
         return cls(service_account_info=gcp_service_account, dataset_id=dataset)
 
     def process_item(self, item: typing.Dict, spider: scrapy.Spider) -> typing.Dict:
         table_id, item = self.table_id(item, spider)
         self.ensure_table_created(table_id, item, spider)
+        for item_key in item:
+            if isinstance(item[item_key], datetime.date):
+                item[item_key] = item[item_key].strftime("%Y-%m-%d")
         errors = self.client.insert_rows_json(table_id, [item])
         if errors:
             spider.logger.error(f"Error inserting rows to BigQuery: {errors}")
         return item
 
     def table_id(
         self, item: typing.Dict, spider: scrapy.Spider
@@ -72,15 +75,15 @@
         dataset = extract_and_delete(self.bigquery_dataset_key)
         table = extract_and_delete(self.bigquery_table_key)
         if spider.settings.get("BIGQUERY_ADD_SCRAPED_TIME", False):
             item["scraped_time"] = datetime.datetime.now()
         if spider.settings.get("BIGQUERY_ADD_SCRAPER_NAME", False):
             item["scraper"] = spider.name
         if spider.settings.get("BIGQUERY_ADD_SCRAPER_SESSION", False):
-            item["scraper_session_id"] = spider.name
+            item["scraper_session_id"] = self.session_id
         for key in item:
             if isinstance(item[key], datetime.datetime):
                 item[key] = str(item[key])
         return f"{self.project_id}.{dataset}.{table}", item
 
     def ensure_table_created(
         self, table_id: str, item: typing.Dict, spider: scrapy.Spider
```

### Comparing `scrapy-bigquery-1.0.8/scrapy_bigquery.egg-info/PKG-INFO` & `scrapy-bigquery-1.0.9/scrapy_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-bigquery
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scrapy pipeline to store items into BigQuery
 Home-page: https://github.com/8W9aG/scrapy-bigquery
 Author: Will Sackfield
 Author-email: will.sackfield@gmail.com
 License: MIT
 Description: # scrapy-bigquery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapy-bigquery Version: 1.0.8 Summary: Scrapy
+Metadata-Version: 2.1 Name: scrapy-bigquery Version: 1.0.9 Summary: Scrapy
 pipeline to store items into BigQuery Home-page: https://github.com/8W9aG/
 scrapy-bigquery Author: Will Sackfield Author-email: will.sackfield@gmail.com
 License: MIT Description: # scrapy-bigquery [PyPi] A Big Query pipeline to
 store items into [Google BigQuery](https://cloud.google.com/bigquery/). ##
 Dependencies :globe_with_meridians: * [Python 3.7](https://www.python.org/
 downloads/release/python-370/) * [Scrapy 2.4.0](https://scrapy.org/) * [Google
 Cloud Bigquery 2.23.2](https://pypi.org/project/google-cloud-bigquery/) *
```

### Comparing `scrapy-bigquery-1.0.8/setup.py` & `scrapy-bigquery-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             if not x.startswith(".") and not x.startswith("-e")
         ]
     return requires
 
 
 setup(
     name='scrapy-bigquery',
-    version='1.0.8',
+    version='1.0.9',
     description='Scrapy pipeline to store items into BigQuery',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Framework :: Scrapy',
```

