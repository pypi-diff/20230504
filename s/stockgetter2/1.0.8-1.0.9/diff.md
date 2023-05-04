# Comparing `tmp/stockgetter2-1.0.8.tar.gz` & `tmp/stockgetter2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockgetter2-1.0.8.tar", last modified: Tue Jan 31 14:14:49 2023, max compression
+gzip compressed data, was "stockgetter2-1.0.9.tar", last modified: Tue Jan 31 14:36:27 2023, max compression
```

## Comparing `stockgetter2-1.0.8.tar` & `stockgetter2-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.592939 stockgetter2-1.0.8/
--rw-rw-rw-   0        0        0      881 2023-01-31 14:14:49.591941 stockgetter2-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       14 2022-11-17 12:26:32.000000 stockgetter2-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-01-31 14:14:49.592939 stockgetter2-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2724 2023-01-08 14:23:20.000000 stockgetter2-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.545067 stockgetter2-1.0.8/stockgetter2/
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.552048 stockgetter2-1.0.8/stockgetter2/Getter/
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.553047 stockgetter2-1.0.8/stockgetter2/Getter/Base/
--rw-rw-rw-   0        0        0     1406 2022-11-17 13:12:28.000000 stockgetter2-1.0.8/stockgetter2/Getter/Base/baseGetter.py
--rw-rw-rw-   0        0        0     4557 2023-01-09 02:04:09.000000 stockgetter2-1.0.8/stockgetter2/Getter/mstBrand.py
--rw-rw-rw-   0        0        0     6175 2023-01-26 13:48:12.000000 stockgetter2-1.0.8/stockgetter2/Getter/seleniumTest.py
--rw-rw-rw-   0        0        0    18810 2023-01-26 13:46:17.000000 stockgetter2-1.0.8/stockgetter2/Getter/trnDayStockPrice.py
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.573989 stockgetter2-1.0.8/stockgetter2/Library/
--rw-rw-rw-   0        0        0     6759 2023-01-08 13:35:23.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterConfig.py
--rw-rw-rw-   0        0        0      691 2023-01-03 10:35:46.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterConfiger.py
--rw-rw-rw-   0        0        0     1426 2023-01-03 10:19:06.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterController.py
--rw-rw-rw-   0        0        0      161 2022-12-20 13:27:33.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterDeclare.py
--rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterException.py
--rw-rw-rw-   0        0        0      558 2023-01-03 10:07:55.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterGlobals.py
--rw-rw-rw-   0        0        0     4729 2023-01-18 12:56:54.000000 stockgetter2-1.0.8/stockgetter2/Library/stockgetterMailer.py
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.575984 stockgetter2-1.0.8/stockgetter2/Models/
--rw-rw-rw-   0        0        0      915 2023-01-05 13:14:55.000000 stockgetter2-1.0.8/stockgetter2/Models/mstBrand.py
--rw-rw-rw-   0        0        0     1338 2023-01-05 13:24:41.000000 stockgetter2-1.0.8/stockgetter2/Models/trnDayStockPrice.py
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.589949 stockgetter2-1.0.8/stockgetter2/Register/
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.590945 stockgetter2-1.0.8/stockgetter2/Register/Base/
--rw-rw-rw-   0        0        0     3973 2023-01-09 09:19:16.000000 stockgetter2-1.0.8/stockgetter2/Register/Base/baseRegister.py
--rw-rw-rw-   0        0        0      444 2022-12-20 13:37:53.000000 stockgetter2-1.0.8/stockgetter2/Register/register_StockData.py
--rw-rw-rw-   0        0        0      265 2023-01-31 14:13:39.000000 stockgetter2-1.0.8/stockgetter2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 14:14:49.549057 stockgetter2-1.0.8/stockgetter2.egg-info/
--rw-rw-rw-   0        0        0      881 2023-01-31 14:14:48.000000 stockgetter2-1.0.8/stockgetter2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      833 2023-01-31 14:14:48.000000 stockgetter2-1.0.8/stockgetter2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 14:14:48.000000 stockgetter2-1.0.8/stockgetter2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      709 2023-01-31 14:14:48.000000 stockgetter2-1.0.8/stockgetter2.egg-info/requires.txt
--rw-rw-rw-   0        0        0      149 2023-01-31 14:14:48.000000 stockgetter2-1.0.8/stockgetter2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.191463 stockgetter2-1.0.9/
+-rw-rw-rw-   0        0        0      881 2023-01-31 14:36:27.191463 stockgetter2-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2022-11-17 12:26:32.000000 stockgetter2-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-31 14:36:27.191463 stockgetter2-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2724 2023-01-08 14:23:20.000000 stockgetter2-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.174980 stockgetter2-1.0.9/stockgetter2/
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.180964 stockgetter2-1.0.9/stockgetter2/Getter/
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.181495 stockgetter2-1.0.9/stockgetter2/Getter/Base/
+-rw-rw-rw-   0        0        0     1406 2022-11-17 13:12:28.000000 stockgetter2-1.0.9/stockgetter2/Getter/Base/baseGetter.py
+-rw-rw-rw-   0        0        0     4557 2023-01-09 02:04:09.000000 stockgetter2-1.0.9/stockgetter2/Getter/mstBrand.py
+-rw-rw-rw-   0        0        0     6270 2023-01-31 14:35:47.000000 stockgetter2-1.0.9/stockgetter2/Getter/seleniumTest.py
+-rw-rw-rw-   0        0        0    18810 2023-01-31 14:16:34.000000 stockgetter2-1.0.9/stockgetter2/Getter/trnDayStockPrice.py
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.187475 stockgetter2-1.0.9/stockgetter2/Library/
+-rw-rw-rw-   0        0        0     6759 2023-01-08 13:35:23.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterConfig.py
+-rw-rw-rw-   0        0        0      691 2023-01-03 10:35:46.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterConfiger.py
+-rw-rw-rw-   0        0        0     1426 2023-01-03 10:19:06.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterController.py
+-rw-rw-rw-   0        0        0      161 2022-12-20 13:27:33.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterDeclare.py
+-rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterException.py
+-rw-rw-rw-   0        0        0      558 2023-01-03 10:07:55.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterGlobals.py
+-rw-rw-rw-   0        0        0     4729 2023-01-18 12:56:54.000000 stockgetter2-1.0.9/stockgetter2/Library/stockgetterMailer.py
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.188472 stockgetter2-1.0.9/stockgetter2/Models/
+-rw-rw-rw-   0        0        0      915 2023-01-05 13:14:55.000000 stockgetter2-1.0.9/stockgetter2/Models/mstBrand.py
+-rw-rw-rw-   0        0        0     1338 2023-01-05 13:24:41.000000 stockgetter2-1.0.9/stockgetter2/Models/trnDayStockPrice.py
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.189468 stockgetter2-1.0.9/stockgetter2/Register/
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.190467 stockgetter2-1.0.9/stockgetter2/Register/Base/
+-rw-rw-rw-   0        0        0     3973 2023-01-09 09:19:16.000000 stockgetter2-1.0.9/stockgetter2/Register/Base/baseRegister.py
+-rw-rw-rw-   0        0        0      444 2022-12-20 13:37:53.000000 stockgetter2-1.0.9/stockgetter2/Register/register_StockData.py
+-rw-rw-rw-   0        0        0      265 2023-01-31 14:36:14.000000 stockgetter2-1.0.9/stockgetter2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-31 14:36:27.178969 stockgetter2-1.0.9/stockgetter2.egg-info/
+-rw-rw-rw-   0        0        0      881 2023-01-31 14:36:27.000000 stockgetter2-1.0.9/stockgetter2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2023-01-31 14:36:27.000000 stockgetter2-1.0.9/stockgetter2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-31 14:36:27.000000 stockgetter2-1.0.9/stockgetter2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      709 2023-01-31 14:36:27.000000 stockgetter2-1.0.9/stockgetter2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      149 2023-01-31 14:36:27.000000 stockgetter2-1.0.9/stockgetter2.egg-info/top_level.txt
```

### Comparing `stockgetter2-1.0.8/PKG-INFO` & `stockgetter2-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockgetter2
-Version: 1.0.8
+Version: 1.0.9
 Summary: stockgetter2 Package
 Home-page: https://github.com/kaioman/stockgetter2.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: stockgetter2
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stockgetter2-1.0.8/setup.py` & `stockgetter2-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Getter/Base/baseGetter.py` & `stockgetter2-1.0.9/stockgetter2/Getter/Base/baseGetter.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Getter/mstBrand.py` & `stockgetter2-1.0.9/stockgetter2/Getter/mstBrand.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Getter/seleniumTest.py` & `stockgetter2-1.0.9/stockgetter2/Getter/seleniumTest.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,15 +166,17 @@
             
             # 株価データmodel用意
             rsTrnDayStockPrice = recset[trnDayStockPrice](trnDayStockPrice)
 
             if rankingTables:
                 
                 # 戻り値を返す
-                return rsTrnDayStockPrice.getDataFrame()
+                df = rsTrnDayStockPrice.getDataFrame()
+                print('brandcd={} count={}'.format(brandCd),len(df))
+                return df
 
     class beautifulSoup(browserContainer.beautifulSoup):
         
         """
         ブラウザコンテナ:beautifulSoup
         """
```

### Comparing `stockgetter2-1.0.8/stockgetter2/Getter/trnDayStockPrice.py` & `stockgetter2-1.0.9/stockgetter2/Getter/trnDayStockPrice.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterConfig.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterConfig.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterConfiger.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterConfiger.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterController.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterController.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterException.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterException.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterGlobals.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterGlobals.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Library/stockgetterMailer.py` & `stockgetter2-1.0.9/stockgetter2/Library/stockgetterMailer.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Models/mstBrand.py` & `stockgetter2-1.0.9/stockgetter2/Models/mstBrand.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Models/trnDayStockPrice.py` & `stockgetter2-1.0.9/stockgetter2/Models/trnDayStockPrice.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2/Register/Base/baseRegister.py` & `stockgetter2-1.0.9/stockgetter2/Register/Base/baseRegister.py`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2.egg-info/PKG-INFO` & `stockgetter2-1.0.9/stockgetter2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockgetter2
-Version: 1.0.8
+Version: 1.0.9
 Summary: stockgetter2 Package
 Home-page: https://github.com/kaioman/stockgetter2.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: stockgetter2
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stockgetter2-1.0.8/stockgetter2.egg-info/SOURCES.txt` & `stockgetter2-1.0.9/stockgetter2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stockgetter2-1.0.8/stockgetter2.egg-info/requires.txt` & `stockgetter2-1.0.9/stockgetter2.egg-info/requires.txt`

 * *Files identical despite different names*

