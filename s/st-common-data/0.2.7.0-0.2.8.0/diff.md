# Comparing `tmp/st_common_data-0.2.7.0.tar.gz` & `tmp/st_common_data-0.2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.7.0.tar", last modified: Fri Apr 28 11:58:27 2023, max compression
+gzip compressed data, was "st_common_data-0.2.8.0.tar", last modified: Thu May  4 08:33:06 2023, max compression
```

## Comparing `st_common_data-0.2.7.0.tar` & `st_common_data-0.2.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.7.0/LICENCE
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.7.0/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.7.0/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-28 11:58:27.039272 st_common_data-0.2.7.0/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-28 06:46:56.000000 st_common_data-0.2.7.0/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.7.0/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.7.0/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-25 17:38:18.000000 st_common_data-0.2.7.0/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.7.0/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.7.0/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    31811 2023-04-28 06:38:57.000000 st_common_data-0.2.7.0/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.7.0/st_common_data/nyse_holidays.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.7.0/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.7.0/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.7.0/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-28 11:58:27.035272 st_common_data-0.2.7.0/st_common_data.egg-info/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-28 11:58:27.000000 st_common_data-0.2.7.0/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-28 11:58:27.000000 st_common_data-0.2.7.0/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-28 11:58:27.000000 st_common_data-0.2.7.0/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-28 11:58:27.000000 st_common_data-0.2.7.0/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.095729 st_common_data-0.2.8.0/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.8.0/LICENCE
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-05-04 08:33:06.095729 st_common_data-0.2.8.0/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.8.0/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.8.0/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-05-04 08:33:06.095729 st_common_data-0.2.8.0/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.091728 st_common_data-0.2.8.0/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-05-03 07:55:35.000000 st_common_data-0.2.8.0/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.091728 st_common_data-0.2.8.0/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.8.0/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.8.0/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-25 17:38:18.000000 st_common_data-0.2.8.0/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.8.0/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.8.0/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    32775 2023-05-03 08:05:42.000000 st_common_data-0.2.8.0/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.8.0/st_common_data/nyse_holidays.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.091728 st_common_data-0.2.8.0/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.095729 st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.8.0/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.095729 st_common_data-0.2.8.0/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.8.0/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.8.0/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-05-04 08:33:06.091728 st_common_data-0.2.8.0/st_common_data.egg-info/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-05-04 08:33:06.000000 st_common_data-0.2.8.0/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-05-04 08:33:06.000000 st_common_data-0.2.8.0/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-05-04 08:33:06.000000 st_common_data-0.2.8.0/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-05-04 08:33:06.000000 st_common_data-0.2.8.0/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.7.0/LICENCE` & `st_common_data-0.2.8.0/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/PKG-INFO` & `st_common_data-0.2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.7.0
+Version: 0.2.8.0
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.7.0/README.md` & `st_common_data-0.2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/setup.cfg` & `st_common_data-0.2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/auth/django_auth.py` & `st_common_data-0.2.8.0/st_common_data/auth/django_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.8.0/st_common_data/auth/fastapi_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/auth/views.py` & `st_common_data-0.2.8.0/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/datum.py` & `st_common_data-0.2.8.0/st_common_data/datum.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,14 +494,44 @@
     response = defaultdict(list)
     for row in ticker_changes:
         response[row['eff_date']].append(row['old_ticker'])
         response[row['eff_date']].append(row['new_ticker'])
 
     return response
 
+
+def api_get_auctions(datum_api_url: str,
+                     service_auth0_token: str,
+                     start_date: str,
+                     end_date: str,
+                     ticker: str = None,
+                     auction: str = None):
+    """
+        ticker: optional, in query params, if it is null, endpoint returns auctions of active US stocks,
+                but in this case max date range of auction data is 5 days
+        auction: optional, in query params, can be: open/close/reopen
+                 if empty, endpoint returns all of the above auctions
+    """
+
+    params = {
+        'start_date': start_date,
+        'end_date': end_date,
+    }
+    if ticker is not None:
+        params.update({'ticker': ticker})
+    if auction is not None:
+        params.update({'auction': auction})
+
+    return datum_api_get_request(
+        url=f'{datum_api_url}/auctions',
+        service_auth0_token=service_auth0_token,
+        params=params
+    )
+
+
 # --------------------- End of Queries to Datum API ---------------------
 #
 # --------------------- Queries to Datum database: ---------------------
 
 
 def get_datum_data_by_ticker(db_creds, ticker, review_date):
     """Return data as of previous work day"""
```

### Comparing `st_common_data-0.2.7.0/st_common_data/nyse_holidays.py` & `st_common_data-0.2.8.0/st_common_data/nyse_holidays.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.8.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.8.0/st_common_data/trading_accounts/models.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.8.0/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data/utils/common.py` & `st_common_data-0.2.8.0/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.7.0/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.8.0/st_common_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-common-data
-Version: 0.2.7.0
+Version: 0.2.8.0
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.7.0/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.8.0/st_common_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

