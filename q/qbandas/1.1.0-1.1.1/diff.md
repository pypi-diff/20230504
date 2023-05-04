# Comparing `tmp/qbandas-1.1.0.tar.gz` & `tmp/qbandas-1.1.1.tar.gz`

## Comparing `qbandas-1.1.0.tar` & `qbandas-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.1.0/requirements.txt
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/__main__.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/headers.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/pack.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/records.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/schema.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/util.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/data/field_types.json
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 qbandas-1.1.0/test/test_headers.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 qbandas-1.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.1.0/LICENSE
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.1.0/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 qbandas-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 qbandas-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.1.1/requirements.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qbandas-1.1.1/requirements_dev.txt
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/__main__.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/headers.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/pack.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/records.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/schema.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/util.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.1.1/qbandas/data/field_types.json
+-rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 qbandas-1.1.1/scripts/build.bat
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.1.1/scripts/doc-build.bat
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 qbandas-1.1.1/test/test_headers.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qbandas-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.1.1/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 qbandas-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 qbandas-1.1.1/PKG-INFO
```

### Comparing `qbandas-1.1.0/qbandas/__main__.py` & `qbandas-1.1.1/qbandas/__main__.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/qbandas/headers.py` & `qbandas-1.1.1/qbandas/headers.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/qbandas/pack.py` & `qbandas-1.1.1/qbandas/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     >>> qbandas.pack._pack_phonenum('<920>888.1234x553', format = '<###>###.####x###')
     {'value': '(920) 888-1234 x553'}
     >>> qbandas.pack._pack_phonenum(None) == None
     True
 
     """
     
-    if pd.isna(x):
+    if pd.isna(x) or not x:
         return None
     
     if not isinstance(x, str):
         raise Exception(f"type {type(x)} is invalid for value {x}, expected type str")
 
     # a str containing only the digits in order
     try:
```

### Comparing `qbandas-1.1.0/qbandas/records.py` & `qbandas-1.1.1/qbandas/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Functions that deal with sending records or information to a Quickbase 
 application.
 """
 
+import asyncio
 import json
 import os
-from datetime import datetime as dt
 from functools import partial
 from os.path import join
 from pathlib import Path
-from typing import NoReturn
 
 import pandas as pd
 import requests
 
 from . import FIELD_TYPES, headers
 
 
 def upload(df: pd.DataFrame, table_name: str, directory: Path|str = None,
-            **kwargs) -> NoReturn: 
+            **kwargs): 
     """
     Send a table of records (rows) to a table on QuickBase.
 
     If no errors are thrown, the data was successfully uploaded to 
     QuickBase. If an error occurs when sending the data, it is possible 
     that only _some_ of your records will have been uploaded to 
     QuickBase. If that is an issue, please fix the data, and send it 
@@ -111,27 +110,32 @@
     body = {"to": schema['_DBID_']}
 
     # look for optinal arguments to include from kwargs
     for option in ["fieldsToReturn", 'mergeFieldId']:
         if option in kwargs:
             body[option] = kwargs[option]
 
-    # send the data one batch a time
-    batch_size = kwargs["Payload-Size"] if "Payload-Size" in kwargs else 20_000
-    for i in range(0, len(records), batch_size):
-        body["data"] = records[i:i+batch_size]
-        r = requests.post(
-            'https://api.quickbase.com/v1/records', 
-            headers = headers_, 
-            json = body
-        )
-        if debug:
-            print(str_resp(r))
-        r.raise_for_status()
-        
+    # send the data all at once
+
+    async def main():
+        batch_size = 5
+        jobs = list()
+        for i in range(0, len(records), batch_size):
+            async def job():
+                body["data"] = records[i : i + batch_size]
+                r = requests.post('https://api.quickbase.com/v1/records', 
+                    headers = headers_, json = body)
+                if debug: print(str_resp(r))
+                r.raise_for_status()
+                print('RAN THAT YE YEE')
+            jobs.append(job())
+        await asyncio.gather(*jobs)
+    asyncio.run(main())
+    
+    
 
 def fetch(table_name: str, *columns, where: str = None, order: list = None, 
             group_by: list = None, skip: int = 0, limit: int = None, 
             directory: Path|str = None, **kwargs) -> pd.DataFrame:
     '''
     Fetch a table of records from a QuickBase app
 
@@ -181,15 +185,15 @@
         
     body = {
         'from': table_name,
         'select': [schema[c]['id'] for c in columns],
         "options": {
             "skip": skip if skip else 0,
             "top": limit if limit else -1,
-            "compareWithAppLocalTime": False
+            "compareWithAppLocalTime": True
         }
     }
     
     # are we sorting?
     if order:
         order = list(order)
         for i, item in enumerate(order.copy()):
@@ -221,11 +225,14 @@
     # assemble dataframe
     for i, record in enumerate(data.copy()):
         data[i] = {k: v['value'] for k, v in record.items()}
     df = pd.DataFrame(data)
     # data typing... builtins didn't work for me
     for id, type_ in type_map.items():
         if type_ in ['timestamp', 'date']:
-            df[id] = pd.to_datetime(df[id])
+            import datetime as dt
+
+            # WARNNG:: OFFSET FOR US CENTRAL TIME
+            df[id] = pd.to_datetime(df[id]) - dt.timedelta(hours=5)
     df.rename(columns = name_map, inplace = True)
     
     return df
```

### Comparing `qbandas-1.1.0/qbandas/schema.py` & `qbandas-1.1.1/qbandas/schema.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/qbandas/util.py` & `qbandas-1.1.1/qbandas/util.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/qbandas/data/field_types.json` & `qbandas-1.1.1/qbandas/data/field_types.json`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/test/test_headers.py` & `qbandas-1.1.1/test/test_headers.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/LICENSE` & `qbandas-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/README.md` & `qbandas-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qbandas-1.1.0/pyproject.toml` & `qbandas-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
-00000010: 7265 7175 6972 6573 203d 205b 0d0a 2020  requires = [..  
-00000020: 2268 6174 6368 6c69 6e67 222c 200d 0a20  "hatchling", .. 
-00000030: 2022 7061 6e64 6173 3d3d 312e 342e 3322   "pandas==1.4.3"
-00000040: 2c0d 0a20 2022 7265 7175 6573 7473 3d3d  ,..  "requests==
-00000050: 322e 3238 2e31 220d 0a20 205d 0d0a 6275  2.28.1"..  ]..bu
-00000060: 696c 642d 6261 636b 656e 6420 3d20 2268  ild-backend = "h
-00000070: 6174 6368 6c69 6e67 2e62 7569 6c64 220d  atchling.build".
-00000080: 0a0d 0a5b 7072 6f6a 6563 745d 0d0a 6e61  ...[project]..na
-00000090: 6d65 203d 2022 7162 616e 6461 7322 0d0a  me = "qbandas"..
-000000a0: 7665 7273 696f 6e20 3d20 2231 2e31 2e30  version = "1.1.0
-000000b0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
-000000c0: 2020 7b20 6e61 6d65 3d22 4a6f 7368 7561    { name="Joshua
-000000d0: 2048 6f70 776f 6f64 2220 7d2c 0d0a 5d0d   Hopwood" },..].
-000000e0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
-000000f0: 496e 7465 6772 6174 6573 2074 6865 2070  Integrates the p
-00000100: 6f70 756c 6172 2064 6174 6120 6861 6e64  opular data hand
-00000110: 6c69 6e67 206c 6962 7261 7279 2050 616e  ling library Pan
-00000120: 6461 7320 616e 6420 7468 6520 5175 6963  das and the Quic
-00000130: 6b42 6173 6520 4150 4922 0d0a 7265 6164  kBase API"..read
-00000140: 6d65 203d 2022 5245 4144 4d45 2e6d 6422  me = "README.md"
-00000150: 0d0a 7265 7175 6972 6573 2d70 7974 686f  ..requires-pytho
-00000160: 6e20 3d20 223e 3d33 2e37 220d 0a63 6c61  n = ">=3.7"..cla
-00000170: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
-00000180: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001a0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
-000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001d0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
-000001e0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001f0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000200: 222c 0d0a 5d0d 0a0d 0a5b 7072 6f6a 6563  ",..]....[projec
-00000210: 742e 7572 6c73 5d0d 0a22 486f 6d65 7061  t.urls].."Homepa
-00000220: 6765 2220 3d20 2268 7474 7073 3a2f 2f67  ge" = "https://g
-00000230: 6974 6875 622e 636f 6d2f 6a68 6f70 776f  ithub.com/jhopwo
-00000240: 6f64 2d6a 6a6b 2f71 4261 6e64 6173 22    od-jjk/qBandas"
+00000010: 7265 7175 6972 6573 203d 205b 2022 6861  requires = [ "ha
+00000020: 7463 686c 696e 6722 205d 0d0a 6275 696c  tchling" ]..buil
+00000030: 642d 6261 636b 656e 6420 3d20 2268 6174  d-backend = "hat
+00000040: 6368 6c69 6e67 2e62 7569 6c64 220d 0a0d  chling.build"...
+00000050: 0a5b 7072 6f6a 6563 745d 0d0a 6e61 6d65  .[project]..name
+00000060: 203d 2022 7162 616e 6461 7322 0d0a 7665   = "qbandas"..ve
+00000070: 7273 696f 6e20 3d20 2231 2e31 2e31 220d  rsion = "1.1.1".
+00000080: 0a61 7574 686f 7273 203d 205b 0d0a 2020  .authors = [..  
+00000090: 7b20 6e61 6d65 203d 2022 4a6f 7368 7561  { name = "Joshua
+000000a0: 2048 6f70 776f 6f64 2220 7d2c 0d0a 5d0d   Hopwood" },..].
+000000b0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+000000c0: 496e 7465 6772 6174 6573 2074 6865 2070  Integrates the p
+000000d0: 6f70 756c 6172 2064 6174 6120 6861 6e64  opular data hand
+000000e0: 6c69 6e67 206c 6962 7261 7279 2050 616e  ling library Pan
+000000f0: 6461 7320 616e 6420 7468 6520 5175 6963  das and the Quic
+00000100: 6b42 6173 6520 4150 4922 0d0a 6465 7065  kBase API"..depe
+00000110: 6e64 656e 6369 6573 203d 205b 0d0a 2020  ndencies = [..  
+00000120: 2270 616e 6461 733d 3d31 2e34 2e33 222c  "pandas==1.4.3",
+00000130: 0d0a 2020 2272 6571 7565 7374 733d 3d32  ..  "requests==2
+00000140: 2e32 382e 3122 0d0a 5d0d 0a72 6561 646d  .28.1"..]..readm
+00000150: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
+00000160: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
+00000170: 203d 2022 3e3d 332e 3722 0d0a 636c 6173   = ">=3.7"..clas
+00000180: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
+00000190: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+000001a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001b0: 203a 3a20 3322 2c0d 0a20 2020 2022 4c69   :: 3",..    "Li
+000001c0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001d0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000001e0: 656e 7365 222c 0d0a 2020 2020 224f 7065  ense",..    "Ope
+000001f0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000200: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
+00000210: 2c0d 0a5d 0d0a 0d0a 5b70 726f 6a65 6374  ,..]....[project
+00000220: 2e75 726c 735d 0d0a 686f 6d65 7061 6765  .urls]..homepage
+00000230: 203d 2022 6874 7470 733a 2f2f 7079 7069   = "https://pypi
+00000240: 2e6f 7267 2f70 726f 6a65 6374 2f71 6261  .org/project/qba
+00000250: 6e64 6173 2f22 0d0a 7265 706f 7369 746f  ndas/"..reposito
+00000260: 7279 203d 2022 6874 7470 733a 2f2f 6769  ry = "https://gi
+00000270: 7468 7562 2e63 6f6d 2f6a 686f 7077 6f6f  thub.com/jhopwoo
+00000280: 642d 6a6a 6b2f 7142 616e 6461 7322 0d0a  d-jjk/qBandas"..
+00000290: 646f 6375 6d65 6e74 6174 696f 6e20 3d20  documentation = 
+000002a0: 2268 7474 7073 3a2f 2f6a 686f 7077 6f6f  "https://jhopwoo
+000002b0: 642d 6a6a 6b2e 6769 7468 7562 2e69 6f2f  d-jjk.github.io/
+000002c0: 7162 616e 6461 732f 22                   qbandas/"
```

### Comparing `qbandas-1.1.0/PKG-INFO` & `qbandas-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: qbandas
-Version: 1.1.0
+Version: 1.1.1
 Summary: Integrates the popular data handling library Pandas and the QuickBase API
-Project-URL: Homepage, https://github.com/jhopwood-jjk/qBandas
+Project-URL: homepage, https://pypi.org/project/qbandas/
+Project-URL: repository, https://github.com/jhopwood-jjk/qBandas
+Project-URL: documentation, https://jhopwood-jjk.github.io/qbandas/
 Author: Joshua Hopwood
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: pandas==1.4.3
+Requires-Dist: requests==2.28.1
 Description-Content-Type: text/markdown
 
 # qBandas
 
 qBandas (QuickBase + Pandas) is a Python package designed to effeciently transfer tabular data between QuickBase applications and the popular Python data handling library Pandas. If you are new to Pandas, you can read more about it [here](https://pandas.pydata.org/).
 
 The advantages of this approach over a QuickBase pipeline are:
```

