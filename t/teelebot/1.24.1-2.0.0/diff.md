# Comparing `tmp/teelebot-1.24.1-py3-none-any.whl.zip` & `tmp/teelebot-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 50682 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     3989 b- defN 23-Apr-19 01:18 teelebot/__init__.py
--rw-rw-rw-  2.0 fat      163 b- defN 21-Sep-11 03:28 teelebot/__main__.py
--rw-rw-rw-  2.0 fat     7352 b- defN 21-Sep-11 03:28 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    19354 b- defN 23-Apr-19 01:22 teelebot/handler.py
--rw-rw-rw-  2.0 fat     1808 b- defN 21-Sep-11 03:28 teelebot/logger.py
--rw-rw-rw-  2.0 fat      619 b- defN 22-Aug-14 05:17 teelebot/polling.py
--rw-rw-rw-  2.0 fat     4304 b- defN 23-Apr-11 13:55 teelebot/request.py
--rw-rw-rw-  2.0 fat     3876 b- defN 21-Sep-11 03:28 teelebot/schedule.py
--rw-rw-rw-  2.0 fat   126997 b- defN 23-Apr-27 17:02 teelebot/teelebot.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-27 17:01 teelebot/version.py
--rw-rw-rw-  2.0 fat     2665 b- defN 22-Aug-14 10:03 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    15118 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-27 17:15 teelebot-1.24.1.dist-info/RECORD
-18 files, 224112 bytes uncompressed, 48380 bytes compressed:  78.4%
+Zip file size: 38901 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     4126 b- defN 23-May-03 14:03 teelebot/__init__.py
+-rw-rw-rw-  2.0 fat      159 b- defN 23-May-03 15:15 teelebot/__main__.py
+-rw-rw-rw-  2.0 fat    28037 b- defN 23-May-04 03:39 teelebot/bot.py
+-rw-rw-rw-  2.0 fat     7366 b- defN 23-May-03 18:10 teelebot/buffer.py
+-rw-rw-rw-  2.0 fat    19342 b- defN 23-May-03 02:52 teelebot/handler.py
+-rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
+-rw-rw-rw-  2.0 fat      721 b- defN 23-May-03 00:01 teelebot/polling.py
+-rw-rw-rw-  2.0 fat     3696 b- defN 23-May-04 04:36 teelebot/request.py
+-rw-rw-rw-  2.0 fat     3880 b- defN 23-May-03 15:17 teelebot/schedule.py
+-rw-rw-rw-  2.0 fat      482 b- defN 23-May-03 00:01 teelebot/version.py
+-rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    15117 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1407 b- defN 23-May-04 05:09 teelebot-2.0.0.dist-info/RECORD
+18 files, 124774 bytes uncompressed, 36623 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: teelebot/__init__.py
 Comment: 
 
 Filename: teelebot/__main__.py
 Comment: 
 
+Filename: teelebot/bot.py
+Comment: 
+
 Filename: teelebot/buffer.py
 Comment: 
 
 Filename: teelebot/handler.py
 Comment: 
 
 Filename: teelebot/logger.py
@@ -18,38 +21,35 @@
 
 Filename: teelebot/request.py
 Comment: 
 
 Filename: teelebot/schedule.py
 Comment: 
 
-Filename: teelebot/teelebot.py
-Comment: 
-
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/LICENSE
+Filename: teelebot-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/METADATA
+Filename: teelebot-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/WHEEL
+Filename: teelebot-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/entry_points.txt
+Filename: teelebot-2.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/top_level.txt
+Filename: teelebot-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/zip-safe
+Filename: teelebot-2.0.0.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-1.24.1.dist-info/RECORD
+Filename: teelebot-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/__init__.py

```diff
@@ -1,22 +1,23 @@
 # -*- coding:utf-8 -*-
 """
 @creation date: 2019-08-23
-@last modification: 2023-04-19
+@last modification: 2023-05-03
 """
 import os
 import requests
 import urllib3
 
 from .polling import _runUpdates
 from .webhook import _runWebhook
-from .teelebot import Bot
+from .bot import Bot
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+
 name = "teelebot"
 __all__ = ['Bot']
 
 bot = Bot()
 VERSION = bot.version
 
 if bot._local_api_server != "False":
@@ -30,15 +31,15 @@
         "    __            __     __          __  " + "\n" + \
         "   / /____  ___  / /__  / /_  ____  / /_ " + "\n" + \
         "  / __/ _ \/ _ \/ / _ \/ __ \/ __ \/ __/ " + "\n" + \
         " / /_/  __/  __/ /  __/ /_/ / /_/ / /_   " + "\n" + \
         " \__/\___/\___/_/\___/_.___/\____/\__/   " + "\n"
     )
     print(" * Self-checking...", end="\r")
-    req = requests.post(url=bot._url + "getWebhookInfo", verify=False, proxies=bot.proxies)
+    req = requests.post(url=f'{bot._url}getWebhookInfo', verify=False, proxies=bot.proxies)
     if not req.json().get("ok"):
         if (req.json().get("error_code") == 401 and \
             req.json().get("description") == "Unauthorized"):
             print("\nif you already logout the bot from the cloud Bot API server,please wait at least 10 minutes and try again.")
         else:
             print("\nfailed to get running mode!")
         os._exit(0)
@@ -97,10 +98,17 @@
         print(" * The teelebot starts running",
               "\n * Version : v" + VERSION,
               "\n *    Mode : Polling",
               "\n *  Thread : " + str(bot._pool_size),
               "\n *  Server : " + api_server + "\n")
         if bot._drop_pending_updates == True and \
             pending_update_count != 0:
-            results = bot.getUpdates(allowed_updates=bot._allowed_updates)
+            results = bot.getUpdates(
+                offset=bot._offset,
+                limit=100,
+                timeout=bot._timeout,
+                allowed_updates=bot._allowed_updates
+            )
             messages = bot._washUpdates(results)
         _runUpdates(bot=bot)
+
+
```

## teelebot/__main__.py

```diff
@@ -1,9 +1,9 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-8-23
-@last modification: 2021-09-11
+@last modification: 2023-05-03
 '''
+import teelebot
 
 if __name__ == "__main__":
-    import teelebot
     teelebot.main()
```

## teelebot/buffer.py

```diff
@@ -1,25 +1,25 @@
 '''
 @creation date: 2021-04-25
-@last modification: 2021-09-11
+@last modification: 2023-05-03
 '''
 from __future__ import print_function
 from sys import getsizeof, stderr
 from itertools import chain
 from collections import deque
+from pathlib import Path
 try:
     from reprlib import repr
 except ImportError:
     pass
 
 import threading
 import inspect
 import os
 import copy
-from pathlib import Path
 
 
 class _Buffer(object):
     """
     数据暂存器类
     """
     def __init__(self, buffer_size, plugin_names, plugin_dir):
@@ -202,8 +202,11 @@
 
             for typ, handler in all_handlers.items():
                 if isinstance(o, typ):
                     s += sum(map(sizeof, handler(o)))
                     break
             return s
 
-        return sizeof(o)
+        return sizeof(o)
+    
+
+
```

## teelebot/handler.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-04-19
+@last modification: 2023-05-03
 '''
 import configparser
 import argparse
 import os
 import sys
 import shutil
 import requests
@@ -425,15 +425,15 @@
 
 if args.close and args.logout:
     print("only one of logout and close can be used at the same time.")
     os._exit(0)
 
 elif args.logout and not args.close:
     config = _config()
-    logout_url = cloud_api_server + "bot" + config["key"] + "/logOut"
+    logout_url = f'{cloud_api_server}bot{config["key"]}/logOut'
     try:
         req = requests.post(url=logout_url, verify=False)
     except:
         print("error request the cloud Bot API server.")
         os._exit(0)
     if req.json().get("ok"):
         print("successfully logout from the cloud Bot API server.")
@@ -446,15 +446,15 @@
 
 elif args.close and not args.logout:
     config = _config()
     if config["local_api_server"] == "False":
         print("close can only be used when local_api_server is configured.")
         os._exit(0)
 
-    close_url = config["local_api_server"] + "bot" + config["key"] + "/close"
+    close_url = f'{config["local_api_server"]}bot{config["key"]}/close'
     try:
         req = requests.post(url=close_url, verify=False)
     except:
         print("error request the the local API server.")
         os._exit(0)
     if req.json().get("ok"):
         print("successfully close from the local API server.")
```

## teelebot/logger.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2021-09-11
+@last modification: 2023-05-03
 '''
 import logging
 
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
 
 RESET_SEQ = "\033[0m"
@@ -42,15 +42,15 @@
         return logging.Formatter.format(self, record)
 
 
 class ColoredLogger(logging.Logger):
     FORMAT = "[$BOLD%(asctime)s][$RESET%(levelname)s] %(message)s"
     COLOR_FORMAT = formatter_message(FORMAT, True)
     def __init__(self, name):
-        logging.Logger.__init__(self, name, logging.DEBUG)
+        logging.Logger.__init__(self, name, logging.INFO)
 
         color_formatter = ColoredFormatter(self.COLOR_FORMAT)
 
         console = logging.StreamHandler()
         console.setFormatter(color_formatter)
 
         self.addHandler(console)
```

## teelebot/polling.py

```diff
@@ -1,22 +1,26 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2020-06-23
-@last modification: 2021-09-11
+@last modification: 2023-05-03
 '''
-import time
 import os
 import signal
 
 
 def _runUpdates(bot):
 
     signal.signal(signal.SIGINT, __exit)
     while True:
-        results = bot.getUpdates(allowed_updates=bot._allowed_updates)  # 获取消息队列messages
+        results = bot.getUpdates(
+            offset=bot._offset,
+            limit=100,
+            timeout=bot._timeout,
+            allowed_updates=bot._allowed_updates
+        ) # 获取消息队列messages
         messages = bot._washUpdates(results)
         if messages is None or not messages:
             continue
         for message in messages:  # 获取单条消息message
             bot._pluginRun(bot, message)
```

## teelebot/request.py

```diff
@@ -1,19 +1,18 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2023-04-11
+@last modification: 2023-05-04
 '''
-import os
-
+import json
 import requests
-import inspect
 from .logger import _logger
 from traceback import extract_stack
 
+
 class _Request(object):
     """
     接口请求类
     """
     def __init__(self, thread_pool_size, url, debug=False, proxies={"all": None}):
         self.__url = url
         self.__debug = debug
@@ -39,79 +38,66 @@
         adapter = requests.adapters.HTTPAdapter(pool_connections=pool_connections,
                                                 pool_maxsize=pool_maxsize, max_retries=max_retries)
         session.mount('http://', adapter)
         session.mount('https://', adapter)
 
         return session
 
-    def __debug_info(self, result):
+    def __debug_info(self, method_name, result):
         """
         debug模式
         """
         if self.__debug and not result.get("ok"):
             stack_info = extract_stack()
             if len(stack_info) > 8:  # 插件内
-                os.system("")  # "玄学"解决Windows下颜色显示失效的问题...
-                _logger.debug("\033[1;31m" + \
-                            "Request failed" + " - " + \
-                            "From:" + stack_info[-3][2] + " - " + \
-                            "Path:" + stack_info[5][0] + " - " + \
-                            "Line:" + str(stack_info[5][1]) + " - " + \
-                            "Method:" + stack_info[6][2] + " - " + \
-                            "Result:" + str(result) + \
-                            "\033[0m")
+                _logger.error(
+                    "Request failed" + " - " + \
+                    "From:" + stack_info[-3][2] + " - " + \
+                    "Path:" + stack_info[5][0] + " - " + \
+                    "Line:" + str(stack_info[5][1]) + " - " + \
+                    "Method:" + method_name + " - " + \
+                    "Result:" + str(result)) # function name: stack_info[6][2]
             elif len(stack_info) > 3:  # 外部调用
-                os.system("")  # "玄学"解决Windows下颜色显示失效的问题...
-                _logger.debug("\033[1;31m" + \
-                            "Request failed" + " - " + \
-                            "From:" + stack_info[0][0] + " - " + \
-                            "Path:" + stack_info[1][0] + " - " + \
-                            "Line:" + str(stack_info[0][1]) + " - " + \
-                            "Method:" + stack_info[1][2] + " - " + \
-                            "Result:" + str(result) + \
-                            "\033[0m")
-
-    def post(self, addr):
-        try:
-            with self.__session.post(self.__url + addr) as req:
-                self.__debug_info(req.json())
-                if req.json().get("ok"):
-                    return req.json().get("result")
-                elif not req.json().get("ok"):
-                    return req.json().get("ok")
-        except:
-            return False
-
-    def postFile(self, addr, file_data):
-        try:
-            with self.__session.post(self.__url + addr, files=file_data) as req:
-                self.__debug_info(req.json())
-                if req.json().get("ok"):
-                    return req.json().get("result")
-                elif not req.json().get("ok"):
-                    return req.json().get("ok")
-        except:
-            return False
-
-    def postJson(self, addr, json):
-        try:
-            with self.__session.get(self.__url + addr, json=json) as req:
-                self.__debug_info(req.json())
-                if req.json().get("ok"):
-                    return req.json().get("result")
-                elif not req.json().get("ok"):
-                    return req.json().get("ok")
-        except:
-            return False
+                _logger.error(
+                    "Request failed" + " - " + \
+                    "From:" + stack_info[0][0] + " - " + \
+                    "Path:" + stack_info[1][0] + " - " + \
+                    "Line:" + str(stack_info[0][1]) + " - " + \
+                    "Method:" + method_name + " - " + \
+                    "Result:" + str(result)) # function name: stack_info[6][2]
+
+    def postEverything(self, method_name, **kwargs):
+
+        inputmedia_methods = ["sendMediaGroup", "editMessageMedia"]
+        is_inputmedia = False
+        inputmedia_param_name = "files"
+        if method_name in inputmedia_methods:
+            is_inputmedia = True
+
+        data, files = {}, {}
+        for key, value in kwargs.items():
+            if not is_inputmedia and key == inputmedia_param_name:
+                pass
+            elif is_inputmedia and key == inputmedia_param_name:
+                files = value
+            elif isinstance(value, bytes):
+                files[key] = value
+            elif isinstance(value, dict):
+                data[key] = json.dumps(value)
+            elif isinstance(value, list):
+                data[key] = json.dumps(value)
+            else:
+                data[key] = value
 
-    def get(self, addr):
+        # print(data, "\n", files)
         try:
-            with self.__session.get(self.__url + addr) as req:
-                self.__debug_info(req.json())
-                if req.json().get("ok"):
+            with requests.post(url=f'{self.__url}{method_name}', data=data, files=files) as req:
+                self.__debug_info(method_name, req.json())
+                if req.json().get("ok", False):
                     return req.json().get("result")
-                elif not req.json().get("ok"):
+                else:
                     return req.json().get("ok")
-        except:
+        except Exception as e:
+            print("error: " + str(e))
             return False
```

## teelebot/schedule.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2021-09-11
+@last modification: 2023-05-03
 '''
 import threading
 from uuid import uuid4
 
 class _Schedule(object):
     """
     周期性任务类
@@ -126,7 +126,9 @@
 
                 with self.__queue_mutex:
                     self.__queue.clear()
 
                 return True, "Cleared"
             except Exception as e:
                 return False, str(e)
+
+
```

## teelebot/version.py

```diff
@@ -1,15 +1,17 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-04-28
+@last modification: 2023-05-03
 @author: Pluto (github:plutobell)
-@version: 1.24.1
+@version: 2.0.0
 """
 
-__version__ = "1.24.1"
+__version__ = "2.0.0"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
-__description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
+__description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
+
+
```

## teelebot/webhook.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2020-6-12
-@last modification: 2022-08-14
+@last modification: 2023-05-03
 '''
-from http.server import HTTPServer, BaseHTTPRequestHandler
 #from socketserver import ThreadingMixIn
+from http.server import HTTPServer, BaseHTTPRequestHandler
 import ssl
 import os
 import json
 
 
 def __MakeRequestHandler(bot):
     class RequestHandler(BaseHTTPRequestHandler):
```

## Comparing `teelebot-1.24.1.dist-info/LICENSE` & `teelebot-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-1.24.1.dist-info/METADATA` & `teelebot-2.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 1.24.1
+Version: 2.0.0
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <h1 align="center">
   <br>
   <a href="#" alt="logo" ><img src="./LOGO.png" width="150"/></a>
@@ -90,15 +90,15 @@
 
 ## 环境要求 ##
 
 ### Python版本
 
 teelebot 只支持 Python3.x，不支持Python2.x。
 
-本项目在 Python 3.5 及以上版本测试通过。
+本项目在 Python 3.6 及以上版本测试通过。
 
 
 
 
 
 ## 安装 ##
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: teelebot Version: 1.24.1 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.0.0 Summary: teelebot is a
 robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
 GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Requires-Python: >=3.5 Description-Content-Type: text/markdown
+v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
                                     ******
                                  [./LOGO.png]
                                    teelebot
                                      ******
                           *** Pythonå®ç°çTelegram
 Botæºå¨äººæ¡æ¶ï¼å·ææä»¶ç³»ç»ï¼æä»¶æ¯æç­æ´æ°åç­è£è½½ã
@@ -28,15 +28,15 @@
 ## * **[æ´æ°æ¥å¿](./CHANGELOG.md)** ## æ¹æ³åè¡¨ ## * **[æ¹æ³åè¡¨]
 (./FUNCTION.md)** ## Demo ## * **Telegram Groupï¼[teelebot official](https://
 t.me/teelebot_official)ï¼t.me/teelebot_officialï¼** * **Bot : [teelebotBot]
 (https://t.me/teelebotBot)ï¼t.me/teelebotBotï¼** * ~~Telegram Groupï¼
 [teelebotä½éªç¾¤](http://t.me/teelebot_chat)ï¼t.me/teelebot_chatï¼~~ *
 ~~Bot : [teelebot](http://t.me/teelebot)ï¼t.me/teelebotï¼~~ ## ç¯å¢è¦æ±
 ## ### Pythonçæ¬ teelebot åªæ¯æ Python3.xï¼ä¸æ¯æPython2.xã
-æ¬é¡¹ç®å¨ Python 3.5 åä»¥ä¸çæ¬æµè¯éè¿ã ## å®è£ ## **1.Pip**
+æ¬é¡¹ç®å¨ Python 3.6 åä»¥ä¸çæ¬æµè¯éè¿ã ## å®è£ ## **1.Pip**
 ```bash pip install teelebot ```
 **æ­¤æ¹å¼æ¨èä½¿ç¨Pythonèæç¯å¢å®è£** **2.Docker** ```bash #
 æ ä»£ç docker run -it \ --name teelebot \ --restart always \ -v /path/to/
 teelebot/config:/config \ -v /path/to/teelebot/plugins:/plugins \ ghcr.io/
 plutobell/teelebot:latest # æä»£ç docker run -it \ --name teelebot \ --
 restart always \ --network host \ -e http_proxy="http://ip:port" \ -
 e https_proxy="http://ip:port" \ -v /path/to/teelebot/config:/config \ -v /
```

## Comparing `teelebot-1.24.1.dist-info/RECORD` & `teelebot-2.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-teelebot/__init__.py,sha256=EllxG9NIQvaLa3cFBHh4_uTWcPDiHKV8mD_-oEuy8pM,3989
-teelebot/__main__.py,sha256=SRKzFAyri9IQ-2Ox_xM3h_o9KrU4Qb2SikEGl-fhun8,163
-teelebot/buffer.py,sha256=YFYDSt7wQzko4Fuzg16PdwyjpXLpvBIK_ZHenv5gD4s,7352
-teelebot/handler.py,sha256=JPF71of7h1DBxDzjHfcjqPieO3lZh4cLMZXoo1oEjjs,19354
-teelebot/logger.py,sha256=WALHg4p9zKuBTuI9ciND-8z-dZ04kVIwgdBmQx2lk0M,1808
-teelebot/polling.py,sha256=KyfGkXHUpPBkDzB2bQRZ8btJm0EOOXoTFZpRZS0b4nM,619
-teelebot/request.py,sha256=WntfQMyHqjGFtiekGx6O-YOZV9Ljqayvr0D1hsruNs8,4304
-teelebot/schedule.py,sha256=K5eecKJD-M9h_ZXqXMlgXlo3Bq8h6unqmTWt37LZhXg,3876
-teelebot/teelebot.py,sha256=1SWCr3tOSYrCCE8uao8dLKmSmLOunk37aXAEzF9EjX4,126997
-teelebot/version.py,sha256=hmltT1CZJ1m25LJnKEjn4lRCPJ4P6ypvMjOC9ajcRX4,478
-teelebot/webhook.py,sha256=LQ51F722XOJW1mdErKw-rA9AhotGJnsvR8RStDotpVM,2665
-teelebot-1.24.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-1.24.1.dist-info/METADATA,sha256=X-6ukNJJ1L9fP17wlpoaFIIN-nc8lSClOGX93StLCKU,15118
-teelebot-1.24.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-1.24.1.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-1.24.1.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-1.24.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-1.24.1.dist-info/RECORD,,
+teelebot/__init__.py,sha256=Tt_8Bw0m9xU1Q2_NZKUQ_j6uXC2tG9Xr4v3K28e6CVU,4126
+teelebot/__main__.py,sha256=s_E7-RSOfVOZx7c84WupirrRB3zuMwtNDqi6o2Ij0Ko,159
+teelebot/bot.py,sha256=mbi_feUSy0hRd8W5zgB6OHX9CV-Z4uFZEnBvSQtoAzw,28037
+teelebot/buffer.py,sha256=yn0CBGUbPBbXmERjMTuCeKZaM_y7H0gPsJbrxiRKliY,7366
+teelebot/handler.py,sha256=BFgQVpKcmQXeH8FTt812ARti9MJndnm0y06yDpG1fXQ,19342
+teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
+teelebot/polling.py,sha256=7lPDDeVInhk8MH-ZQhzGXYW-uI5t-F0XtMYkMrcEDEU,721
+teelebot/request.py,sha256=LI_L6V_ticTk-u5IIamzlFfMGf6OD17vfH3jwxj7P7s,3696
+teelebot/schedule.py,sha256=NHo1Hx5DJZCrV1BY-VjjCVgwPKCM0LDuWIYfXrapKdw,3880
+teelebot/version.py,sha256=xd9duuU25Ittvtereq6Go1WU1o3aR4KSyc1YsqhL0qE,482
+teelebot/webhook.py,sha256=IomyaLxak_caDNYKNnLaTLtqkFToYq4sHWsD7kahV4Y,2665
+teelebot-2.0.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.0.0.dist-info/METADATA,sha256=SCvesgHASmJbUdF9VkikXKWjTueHB1f2bN77rheYbrk,15117
+teelebot-2.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-2.0.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.0.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.0.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.0.0.dist-info/RECORD,,
```

