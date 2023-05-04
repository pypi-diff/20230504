# Comparing `tmp/hoyo_daily_logins_helper-1.0.1-py3-none-any.whl.zip` & `tmp/hoyo_daily_logins_helper-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 17947 bytes, number of entries: 15
+Zip file size: 18037 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 21:37 src/__init__.py
 -rw-r--r--  2.0 unx       33 b- defN 23-Apr-25 21:37 src/__main__.py
--rw-r--r--  2.0 unx      474 b- defN 23-Apr-26 01:31 src/config.py
+-rw-r--r--  2.0 unx      516 b- defN 23-May-04 07:09 src/config.py
 -rw-r--r--  2.0 unx     1685 b- defN 23-Apr-26 00:00 src/http.py
 -rw-r--r--  2.0 unx     2134 b- defN 23-Apr-26 00:01 src/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 21:50 src/games/__init__.py
 -rw-r--r--  2.0 unx      200 b- defN 23-Apr-26 01:31 src/games/genshin.py
--rw-r--r--  2.0 unx     2190 b- defN 23-Apr-26 01:41 src/games/hoyo_checkin.py
+-rw-r--r--  2.0 unx     2253 b- defN 23-May-04 07:09 src/games/hoyo_checkin.py
 -rw-r--r--  2.0 unx      207 b- defN 23-Apr-26 01:31 src/games/starrail.py
--rw-r--r--  2.0 unx    34227 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1781 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1237 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/RECORD
-15 files, 44323 bytes uncompressed, 15879 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx    34227 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1917 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1237 b- defN 23-May-04 07:11 hoyo_daily_logins_helper-1.1.0.dist-info/RECORD
+15 files, 44564 bytes uncompressed, 15969 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: src/games/hoyo_checkin.py
 Comment: 
 
 Filename: src/games/starrail.py
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/METADATA
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/WHEEL
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/entry_points.txt
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/top_level.txt
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.1.dist-info/RECORD
+Filename: hoyo_daily_logins_helper-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/config.py

```diff
@@ -1,17 +1,19 @@
 import os
 from typing import Optional
 
 _default_configs = {
     "USER_AGENT": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
                   "AppleWebKit/537.36 (KHTML, like Gecko) "
-                  "Chrome/74.0.3729.169 Safari/537.36"
+                  "Chrome/74.0.3729.169 Safari/537.36",
+    "LANG": "en-us"
 }
 
 CONFIG_USER_AGENT = "USER_AGENT"
+CONFIG_LANG = "LANG"
 
 
 def get_config(key: str) -> Optional[str]:
     if key not in os.environ:
         if key in _default_configs:
             return _default_configs[key]
         return None
```

## src/games/hoyo_checkin.py

```diff
@@ -1,24 +1,25 @@
 import json
 import random
 import time
 import logging
 
 from src.http import http_get_json, http_post_json
+from src.config import get_config, CONFIG_LANG
 
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
 
 def hoyo_checkin(
     event_base_url: str,
     act_id: str,
     cookie_str: str
 ):
-    lang = "en-us"
+    lang = get_config(CONFIG_LANG)
     referer_url = "https://act.hoyolab.com/"
     reward_url = f"{event_base_url}/home?lang={lang}" \
                  f"&act_id={act_id}"
     info_url = f"{event_base_url}/info?lang={lang}" \
                f"&act_id={act_id}"
     sign_url = f"{event_base_url}/sign?lang={lang}"
```

## Comparing `hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE` & `hoyo_daily_logins_helper-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hoyo_daily_logins_helper-1.0.1.dist-info/METADATA` & `hoyo_daily_logins_helper-1.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 1.0.1
+Version: 1.1.0
 Summary: Get hoyo daily login rewards automatically!
 Home-page: https://github.com/atomicptr/hoyo-daily-logins-helper
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
@@ -32,21 +32,31 @@
 4. Open a terminal with the command prepared and enter:
     ```bash
     $ hoyo-daily-logins-helper --cookie="your cookie string" --genshin
     ```
    (or ``--starrail`` for Honkai Star Rail)
 5. Done!
 
+## Installation
+
 ### Docker
 
 The command line options are also available via environment variables which
 allows you to easily run this script in Docker/Podman!
 
 ```bash
 $ docker run --rm --env GAME=starrail --env COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
 
+### pip
+
+```bash
+$ pip install hoyo-daily-logins-helper
+```
+
+PyPi: https://pypi.org/project/hoyo-daily-logins-helper/
+
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

