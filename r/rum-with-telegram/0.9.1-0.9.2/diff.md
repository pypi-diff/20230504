# Comparing `tmp/rum_with_telegram-0.9.1.tar.gz` & `tmp/rum_with_telegram-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.1.tar", last modified: Wed May  3 17:05:26 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.9.2.tar", last modified: Thu May  4 04:32:53 2023, max compression
```

## Comparing `rum_with_telegram-0.9.1.tar` & `rum_with_telegram-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.124428 rum_with_telegram-0.9.1/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-03 17:05:26.123430 rum_with_telegram-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.1/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.098176 rum_with_telegram-0.9.1/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-03 17:05:10.000000 rum_with_telegram-0.9.1/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.9.1/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25084 2023-05-03 17:04:42.000000 rum_with_telegram-0.9.1/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3411 2023-05-03 16:46:43.000000 rum_with_telegram-0.9.1/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-03 16:46:43.000000 rum_with_telegram-0.9.1/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:05:26.107908 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 17:05:26.000000 rum_with_telegram-0.9.1/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 17:05:26.124428 rum_with_telegram-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-03 17:05:10.000000 rum_with_telegram-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.413043 rum_with_telegram-0.9.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-04 04:32:53.410051 rum_with_telegram-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.2/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.395124 rum_with_telegram-0.9.2/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-04 04:32:01.000000 rum_with_telegram-0.9.2/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-03 14:40:44.000000 rum_with_telegram-0.9.2/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25084 2023-05-04 04:32:07.000000 rum_with_telegram-0.9.2/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3345 2023-05-04 04:27:01.000000 rum_with_telegram-0.9.2/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.2/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:32:53.408068 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 04:32:53.000000 rum_with_telegram-0.9.2/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 04:32:53.413043 rum_with_telegram-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-04 04:32:01.000000 rum_with_telegram-0.9.2/setup.py
```

### Comparing `rum_with_telegram-0.9.1/LICENSE` & `rum_with_telegram-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.1/PKG-INFO` & `rum_with_telegram-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.1
+Version: 0.9.2
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.1/rum_with_telegram/config.py` & `rum_with_telegram-0.9.2/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.1/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.9.2/rum_with_telegram/data_exchanger.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.1/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.9.2/rum_with_telegram/db_handle.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,10 +80,8 @@
             try:
                 session.commit()
             except Exception as err:
                 session.rollback()
                 logger.info(err)
 
     def update_user_export_at(self, userid):
-        with self.Session() as session:
-            session.query(User).filter_by(user_id=userid).update({"export_at": func.now()})
-            session.commit()
+        return self.add_or_update(User, {"user_id": userid, "export_at": func.now()}, "user_id")
```

### Comparing `rum_with_telegram-0.9.1/rum_with_telegram/module.py` & `rum_with_telegram-0.9.2/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.1/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.9.2/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.1
+Version: 0.9.2
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.1/setup.py` & `rum_with_telegram-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.1",
+    version="0.9.2",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

