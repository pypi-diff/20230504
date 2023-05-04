# Comparing `tmp/rum_with_telegram-0.9.2.tar.gz` & `tmp/rum_with_telegram-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.2.tar", last modified: Thu May  4 04:32:53 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.3.tar", last modified: Thu May  4 04:54:58 2023, max compression
```

## Comparing `rum_with_telegram-0.9.2.tar` & `rum_with_telegram-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.413043 rum_with_telegram-0.9.2/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-04 04:32:53.410051 rum_with_telegram-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.2/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.395124 rum_with_telegram-0.9.2/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-04 04:32:01.000000 rum_with_telegram-0.9.2/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.9.2/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25084 2023-05-04 04:32:07.000000 rum_with_telegram-0.9.2/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.2/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.2/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.408068 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 04:32:53.413043 rum_with_telegram-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-04 04:32:01.000000 rum_with_telegram-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.133584 rum_with_telegram-0.9.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-04 04:54:58.131613 rum_with_telegram-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.3/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.085573 rum_with_telegram-0.9.3/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-04 04:48:20.000000 rum_with_telegram-0.9.3/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.3/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25286 2023-05-04 04:54:36.000000 rum_with_telegram-0.9.3/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.3/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.3/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.129593 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-04 04:54:57.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 04:54:57.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 04:54:58.133584 rum_with_telegram-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-04 04:48:20.000000 rum_with_telegram-0.9.3/setup.py
```

### Comparing `rum_with_telegram-0.9.2/LICENSE` & `rum_with_telegram-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.2/PKG-INFO` & `rum_with_telegram-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.2
+Version: 0.9.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.2/rum_with_telegram/config.py` & `rum_with_telegram-0.9.3/rum_with_telegram/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     BLACK_LIST_TGIDS: list = None
     # whether to print sql statements
     DB_ECHO: bool = False
     # the default private key of this service to send trx
     ETH_PVTKEY: str = None
     RUM_DELAY_HOURS: int = -3
     RUM_POST_FOOTER: str = ""
+    RUM_TO_TG_TAG: str = ""
+    RUM_TO_TG: bool = True
     TG_REPLY_POSTURL: bool = True
     TG_USER_ID: int = None
     TG_CHANNEL_URL: str = None  # the url of telegram url
     TG_CHANNEL_ID: int = None
     TG_GROUP_ID: int = None
 
     def __post_init__(self):
```

### Comparing `rum_with_telegram-0.9.2/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.3/rum_with_telegram/data_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
             parse_mode="Markdown",
             disable_web_page_preview=True,
             reply_to_message_id=reply_to_message_id,
         )
         logger.info("send reply done")
 
     async def handle_rum(self):
+        if not self.config.RUM_TO_TG:
+            return
         if self.start_trx is None:
             trxs = self.rum.api.get_content(num=20, reverse=True)
             if trxs:
                 self.start_trx = trxs[-1]["TrxId"]
         _trx_id = self.start_trx
         while True:
             if self.start_trx != _trx_id:
@@ -137,14 +139,17 @@
         trxs = self.rum.api.get_content(num=20, start_trx=start_trx)
         for trx in trxs:
             start_trx = trx["TrxId"]
             if trx["SenderPubkey"] in self.config.BLACK_LIST_PUBKEYS:
                 continue
             if get_trx_type(trx) != "post":
                 continue
+            _tag = self.config.RUM_TO_TG_TAG
+            if _tag and _tag not in trx["Data"]["object"]["content"]:
+                continue
             trx_dt = util.get_published_datetime(trx)
             if trx_dt < datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
                 hours=self.config.RUM_DELAY_HOURS
             ):
                 continue
             origin_url = trx["Data"].get("origin", {}).get("url", "")
             if self.config.TG_CHANNEL_URL in origin_url:
@@ -432,16 +437,18 @@
         logger.info("start command_show_pvtkey %s", update.message.message_id)
         userid = update.message.from_user.id
         username = update.message.from_user.username
         user = self.db.init_user(userid, username)
         used = self.db.get_all(UsedKey, {"user_id": userid}, "user_id") or []
         if user:
             text = f"Your private key (please keep it safe) now is: \n```\n{user.pvtkey}\n```\nYour Address (can show to others)  now is:\n```\n{user.address}\n```"
-            for i in used:
-                text += f"\n\nUsed private key (please keep it safe) is: \n```\n{i.pvtkey}\n```\nUsed Address (can show to others) is:\n```\n{i.address}\n```"
+            if used:
+                text += "\n\nUsed private key (please keep it safe) is: \n"
+                for i in used:
+                    text += f"\n```\n{i.pvtkey}\n```\n"
         else:
             text = f"show_key error {userid}"
 
         await update.message.reply_text(text, parse_mode="Markdown")
 
     async def command_new_pvtkey(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start command_new_pvtkey %s", update.message.message_id)
```

### Comparing `rum_with_telegram-0.9.2/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.3/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.2/rum_with_telegram/module.py` & `rum_with_telegram-0.9.3/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.2/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.3/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.2
+Version: 0.9.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.2/setup.py` & `rum_with_telegram-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.2",
+    version="0.9.3",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

