# Comparing `tmp/ejtraderMT-3.12.tar.gz` & `tmp/ejtraderMT-3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderMT-3.12.tar", last modified: Thu Apr 27 19:08:32 2023, max compression
+gzip compressed data, was "ejtraderMT-3.13.tar", last modified: Thu May  4 04:58:28 2023, max compression
```

## Comparing `ejtraderMT-3.12.tar` & `ejtraderMT-3.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-27 19:08:19.000000 ejtraderMT-3.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 19:08:19.000000 ejtraderMT-3.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-04-27 19:08:32.212210 ejtraderMT-3.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-27 19:08:19.000000 ejtraderMT-3.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28732 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/api/mql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 19:08:19.000000 ejtraderMT-3.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 19:08:32.212210 ejtraderMT-3.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-27 19:08:19.000000 ejtraderMT-3.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:58:28.619589 ejtraderMT-3.13/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-04 04:58:17.000000 ejtraderMT-3.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 04:58:17.000000 ejtraderMT-3.13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-05-04 04:58:28.619589 ejtraderMT-3.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 04:58:17.000000 ejtraderMT-3.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:58:28.619589 ejtraderMT-3.13/ejtraderMT/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 04:58:17.000000 ejtraderMT-3.13/ejtraderMT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:58:28.619589 ejtraderMT-3.13/ejtraderMT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 04:58:17.000000 ejtraderMT-3.13/ejtraderMT/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28769 2023-05-04 04:58:17.000000 ejtraderMT-3.13/ejtraderMT/api/mql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:58:28.619589 ejtraderMT-3.13/ejtraderMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-05-04 04:58:28.000000 ejtraderMT-3.13/ejtraderMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 04:58:28.000000 ejtraderMT-3.13/ejtraderMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 04:58:28.000000 ejtraderMT-3.13/ejtraderMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 04:58:28.000000 ejtraderMT-3.13/ejtraderMT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 04:58:28.000000 ejtraderMT-3.13/ejtraderMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 04:58:17.000000 ejtraderMT-3.13/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 04:58:28.619589 ejtraderMT-3.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-04 04:58:17.000000 ejtraderMT-3.13/setup.py
```

### Comparing `ejtraderMT-3.12/LICENSE` & `ejtraderMT-3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.12/PKG-INFO` & `ejtraderMT-3.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.12
+Version: 3.13
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
-License: MIT License
+License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
 Project-URL: Source, https://github.com/traderpedroso/ejtraderMT
 Project-URL: Documentation, https://ejtrader.readthedocs.io/
 Keywords: metatrader,f-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -23,15 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+[![Release](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/releases/latest)  [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/blob/master/LICENSE)
 
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
```

### Comparing `ejtraderMT-3.12/README.md` & `ejtraderMT-3.13/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+[![Release](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/releases/latest)  [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/blob/master/LICENSE)
 
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
```

### Comparing `ejtraderMT-3.12/ejtraderMT/api/mql.py` & `ejtraderMT-3.13/ejtraderMT/api/mql.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,38 +268,38 @@
     
     
     
     def _calendar(self,data):
         symbol = self._symbol
         fromDate = self._fromDate 
         toDate = self._toDate
+        df = pd.DataFrame()
         # count data
         if not isinstance(fromDate, int):
             start_date = datetime.strptime(fromDate, "%d/%m/%Y")
         else:
             start_date = self.__brokerTimeDelta(fromDate)
         if not toDate:
             end_date = self.__brokerTimeDelta(0)
         else:
             end_date = datetime.strptime(toDate, "%d/%m/%Y")
         
-
         delta = timedelta(days=1)
         delta2 = timedelta(days=1)
         diff_days = start_date - end_date
         days_count = diff_days.days
         pbar = tqdm(total=abs(days_count))
         appended_data = []
-        
         while start_date <= end_date:
             pbar.update(delta.days)
             fromDate = start_date.strftime("%d/%m/%Y")
             toDate = start_date
             toDate +=  delta2
-            toDate = toDate.strftime("%d/%m/%Y")
+            toDate = toDate.strftime("%d/%m/%Y") 
+                
             if fromDate and toDate:
                 try:
                     df = self.__api.Command(action="CALENDAR", actionType="DATA", symbol=symbol, 
                                                     fromDate=self.__date_to_timestamp(fromDate), toDate=self.__date_to_timestamp(toDate))
                     
                 except:
                     pass
@@ -800,8 +800,8 @@
             q[f"{self.__active_name}"] = df
         else:
             try:
                 self.__set_utc_or_localtime_tz_df(df)
             except AttributeError:
                 pass
         if self.dbtype == "INFLUXDB":
-            self.__client.write_points(df, f"{self.__active_name}", protocol=self.protocol)
+            self.__client.write_points(df, f"{self.__active_name}", protocol=self.protocol)
```

### Comparing `ejtraderMT-3.12/ejtraderMT.egg-info/PKG-INFO` & `ejtraderMT-3.13/ejtraderMT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.12
+Version: 3.13
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
-License: MIT License
+License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
 Project-URL: Source, https://github.com/traderpedroso/ejtraderMT
 Project-URL: Documentation, https://ejtrader.readthedocs.io/
 Keywords: metatrader,f-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -23,15 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+[![Release](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/releases/latest)  [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderMT)](https://github.com/ejtraderLabs/ejtraderMT/blob/master/LICENSE)
 
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
```

### Comparing `ejtraderMT-3.12/setup.py` & `ejtraderMT-3.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderMT',
-    version='3.12',
+    version='3.13',
     packages=find_packages(),
     url='https://ejtraderMT.readthedocs.io/',
     download_url='https://ejtrader.com',
-    license='MIT License',
+    license='GPL-3.0',
     author='Emerson Pedroso',
     author_email='support@ejtrader.com',
     description='Metatrader API',
     long_description=readme(),
     long_description_content_type='text/markdown',
     install_requires=requirements(filename='requirements.txt'),
     include_package_data=True,
```

