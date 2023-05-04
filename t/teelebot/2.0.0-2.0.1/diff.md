# Comparing `tmp/teelebot-2.0.0-py3-none-any.whl.zip` & `tmp/teelebot-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 38901 bytes, number of entries: 18
+Zip file size: 38903 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat     4126 b- defN 23-May-03 14:03 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      159 b- defN 23-May-03 15:15 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    28037 b- defN 23-May-04 03:39 teelebot/bot.py
+-rw-rw-rw-  2.0 fat    28037 b- defN 23-May-04 05:25 teelebot/bot.py
 -rw-rw-rw-  2.0 fat     7366 b- defN 23-May-03 18:10 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat    19342 b- defN 23-May-03 02:52 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      721 b- defN 23-May-03 00:01 teelebot/polling.py
--rw-rw-rw-  2.0 fat     3696 b- defN 23-May-04 04:36 teelebot/request.py
+-rw-rw-rw-  2.0 fat     3702 b- defN 23-May-04 05:25 teelebot/request.py
 -rw-rw-rw-  2.0 fat     3880 b- defN 23-May-03 15:17 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      482 b- defN 23-May-03 00:01 teelebot/version.py
+-rw-rw-rw-  2.0 fat      482 b- defN 23-May-04 05:25 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    15117 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1407 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/RECORD
-18 files, 124774 bytes uncompressed, 36623 bytes compressed:  70.6%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    15117 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1407 b- defN 23-May-04 05:32 teelebot-2.0.1.dist-info/RECORD
+18 files, 124780 bytes uncompressed, 36625 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/LICENSE
+Filename: teelebot-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/METADATA
+Filename: teelebot-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/WHEEL
+Filename: teelebot-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/entry_points.txt
+Filename: teelebot-2.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/top_level.txt
+Filename: teelebot-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/zip-safe
+Filename: teelebot-2.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.0.0.dist-info/RECORD
+Filename: teelebot-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
 @last modification: 2023-05-03
 @author: Pluto (github:plutobell)
-@version: 2.0.0
+@version: 2.0.1
 """
 import time
 import sys
 import os
 import types
 import string
 import random
```

## teelebot/request.py

```diff
@@ -86,15 +86,15 @@
             elif isinstance(value, list):
                 data[key] = json.dumps(value)
             else:
                 data[key] = value
 
         # print(data, "\n", files)
         try:
-            with requests.post(url=f'{self.__url}{method_name}', data=data, files=files) as req:
+            with self.__session.post(url=f'{self.__url}{method_name}', data=data, files=files) as req:
                 self.__debug_info(method_name, req.json())
                 if req.json().get("ok", False):
                     return req.json().get("result")
                 else:
                     return req.json().get("ok")
         except Exception as e:
             print("error: " + str(e))
```

## teelebot/version.py

```diff
@@ -1,17 +1,17 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
 @last modification: 2023-05-03
 @author: Pluto (github:plutobell)
-@version: 2.0.0
+@version: 2.0.1
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-2.0.0.dist-info/LICENSE` & `teelebot-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.0.0.dist-info/METADATA` & `teelebot-2.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.0.0
+Version: 2.0.1
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.0.0 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.0.1 Summary: teelebot is a
 robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
 GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

## Comparing `teelebot-2.0.0.dist-info/RECORD` & `teelebot-2.0.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 teelebot/__init__.py,sha256=Tt_8Bw0m9xU1Q2_NZKUQ_j6uXC2tG9Xr4v3K28e6CVU,4126
 teelebot/__main__.py,sha256=s_E7-RSOfVOZx7c84WupirrRB3zuMwtNDqi6o2Ij0Ko,159
-teelebot/bot.py,sha256=mbi_feUSy0hRd8W5zgB6OHX9CV-Z4uFZEnBvSQtoAzw,28037
+teelebot/bot.py,sha256=6bbVSdUqy1G8Pb_js7D-rxDtmEEC2B1pmXox9kE001Q,28037
 teelebot/buffer.py,sha256=yn0CBGUbPBbXmERjMTuCeKZaM_y7H0gPsJbrxiRKliY,7366
 teelebot/handler.py,sha256=BFgQVpKcmQXeH8FTt812ARti9MJndnm0y06yDpG1fXQ,19342
 teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
 teelebot/polling.py,sha256=7lPDDeVInhk8MH-ZQhzGXYW-uI5t-F0XtMYkMrcEDEU,721
-teelebot/request.py,sha256=LI_L6V_ticTk-u5IIamzlFfMGf6OD17vfH3jwxj7P7s,3696
+teelebot/request.py,sha256=aSk7jw4RDf30D_B1gSh30hz1nD3Yu9quQT4IxsvjIFc,3702
 teelebot/schedule.py,sha256=NHo1Hx5DJZCrV1BY-VjjCVgwPKCM0LDuWIYfXrapKdw,3880
-teelebot/version.py,sha256=xd9duuU25Ittvtereq6Go1WU1o3aR4KSyc1YsqhL0qE,482
+teelebot/version.py,sha256=--kXKzY9wOVLknP2VkFMi54xtBmuDnZq3M7N4LvISs0,482
 teelebot/webhook.py,sha256=IomyaLxak_caDNYKNnLaTLtqkFToYq4sHWsD7kahV4Y,2665
-teelebot-2.0.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.0.0.dist-info/METADATA,sha256=SCvesgHASmJbUdF9VkikXKWjTueHB1f2bN77rheYbrk,15117
-teelebot-2.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-2.0.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.0.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.0.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.0.0.dist-info/RECORD,,
+teelebot-2.0.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.0.1.dist-info/METADATA,sha256=qyM2fp8bz-joeboJmVEO0gdpdzMwiEL_NiJMrBhXBDk,15117
+teelebot-2.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-2.0.1.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.0.1.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.0.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.0.1.dist-info/RECORD,,
```

