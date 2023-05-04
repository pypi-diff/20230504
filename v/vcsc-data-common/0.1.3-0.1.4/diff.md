# Comparing `tmp/vcsc_data_common-0.1.3.tar.gz` & `tmp/vcsc_data_common-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.3.tar", last modified: Fri Apr 21 06:19:37 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.4.tar", last modified: Thu May  4 06:36:44 2023, max compression
```

## Comparing `vcsc_data_common-0.1.3.tar` & `vcsc_data_common-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.871372 vcsc_data_common-0.1.3/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-21 06:19:37.871454 vcsc_data_common-0.1.3/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.3/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.3/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-21 06:19:37.871878 vcsc_data_common-0.1.3/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.868498 vcsc_data_common-0.1.3/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.3/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.869877 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870214 vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870542 vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870813 vcsc_data_common-0.1.3/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.3/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.871112 vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3444 2023-04-21 06:19:05.000000 vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.869268 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037602 vcsc_data_common-0.1.4/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-04 06:36:44.037682 vcsc_data_common-0.1.4/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.4/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.4/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-04 06:36:44.037976 vcsc_data_common-0.1.4/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.034777 vcsc_data_common-0.1.4/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.4/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036155 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036480 vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.036779 vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037066 vcsc_data_common-0.1.4/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.4/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.037358 vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3444 2023-04-21 06:19:05.000000 vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-04 06:36:44.035681 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-04 06:36:44.000000 vcsc_data_common-0.1.4/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.3/pyproject.toml` & `vcsc_data_common-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.4/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.4/vcsc_data_common/live_price_data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         actions_df = dt.get_add_actions().to_pandas()
         self.last_modification_time = actions_df.iloc[0]['modification_time']
         return self.last_modification_time
 
     def get_market_status(self) -> pd.DataFrame:
 
         response = requests.get(
-            'https://mt.vcsc.com.vn/api/price/marketStatus/getAll')
+            'https://mt.vietcap.com.vn/api/price/marketStatus/getAll')
         try:
 
             json_data = json.loads(response.text)
             arr = []
             for key in json_data:
                 arr.append(
                     {'marketCode': json_data[key]['marketCode'], 'status': json_data[key]['status']})
```

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.4/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.4/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.4/vcsc_data_common/portfolio_info/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.3/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.4/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

