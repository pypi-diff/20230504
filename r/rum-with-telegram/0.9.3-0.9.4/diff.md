# Comparing `tmp/rum_with_telegram-0.9.3.tar.gz` & `tmp/rum_with_telegram-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.3.tar", last modified: Thu May  4 04:54:58 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.4.tar", last modified: Thu May  4 05:07:42 2023, max compression
```

## Comparing `rum_with_telegram-0.9.3.tar` & `rum_with_telegram-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.133584 rum_with_telegram-0.9.3/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-04 04:54:58.131613 rum_with_telegram-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.3/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.085573 rum_with_telegram-0.9.3/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-04 04:48:20.000000 rum_with_telegram-0.9.3/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.3/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25286 2023-05-04 04:54:36.000000 rum_with_telegram-0.9.3/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.3/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.3/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:54:58.129593 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-04 04:54:57.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 04:54:57.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 04:54:58.000000 rum_with_telegram-0.9.3/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 04:54:58.133584 rum_with_telegram-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-04 04:48:20.000000 rum_with_telegram-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.920520 rum_with_telegram-0.9.4/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-04 05:07:42.919514 rum_with_telegram-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.4/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.904555 rum_with_telegram-0.9.4/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-04 05:01:32.000000 rum_with_telegram-0.9.4/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.4/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25343 2023-05-04 05:03:28.000000 rum_with_telegram-0.9.4/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.4/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.4/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:07:42.917518 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 05:07:42.000000 rum_with_telegram-0.9.4/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 05:07:42.921510 rum_with_telegram-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-04 05:01:32.000000 rum_with_telegram-0.9.4/setup.py
```

### Comparing `rum_with_telegram-0.9.3/LICENSE` & `rum_with_telegram-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.3/PKG-INFO` & `rum_with_telegram-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.3
+Version: 0.9.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.3/rum_with_telegram/config.py` & `rum_with_telegram-0.9.4/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.3/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.4/rum_with_telegram/data_exchanger.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             disable_web_page_preview=True,
             reply_to_message_id=reply_to_message_id,
         )
         logger.info("send reply done")
 
     async def handle_rum(self):
         if not self.config.RUM_TO_TG:
+            logger.warning("config.RUM_TO_TG is False")
             return
         if self.start_trx is None:
             trxs = self.rum.api.get_content(num=20, reverse=True)
             if trxs:
                 self.start_trx = trxs[-1]["TrxId"]
         _trx_id = self.start_trx
         while True:
```

### Comparing `rum_with_telegram-0.9.3/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.4/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.3/rum_with_telegram/module.py` & `rum_with_telegram-0.9.4/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.3/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.4/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.3
+Version: 0.9.4
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.3/setup.py` & `rum_with_telegram-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.3",
+    version="0.9.4",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

