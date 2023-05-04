# Comparing `tmp/tsutils-8.0.2.tar.gz` & `tmp/tsutils-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsutils-8.0.2.tar", last modified: Tue Mar 14 02:45:41 2023, max compression
+gzip compressed data, was "tsutils-8.0.3.tar", last modified: Thu May  4 07:46:44 2023, max compression
```

## Comparing `tsutils-8.0.2.tar` & `tsutils-8.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.587494 tsutils-8.0.2/
--rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.2/LICENSE
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:45:41.587334 tsutils-8.0.2/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.2/README.md
--rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-03-14 02:45:41.587533 tsutils-8.0.2/setup.cfg
--rw-r--r--   0 chasehult   (501) staff       (20)      842 2023-03-14 02:42:36.000000 tsutils-8.0.2/setup.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.582239 tsutils-8.0.2/tsutils/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3920 2022-06-03 03:58:49.000000 tsutils-8.0.2/tsutils/cog_mixins.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/cog_settings.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.583380 tsutils-8.0.2/tsutils/cogs/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/cogs/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/cogs/donations.py
--rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/cogs/globaladmin.py
--rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/cogs/userpreferences.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.2/tsutils/emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.2/tsutils/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/errors.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.2/tsutils/formatting.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.2/tsutils/helper_classes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3286 2022-06-03 03:07:59.000000 tsutils-8.0.2/tsutils/helper_functions.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.2/tsutils/json_utils.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.584098 tsutils-8.0.2/tsutils/menu/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/menu/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.2/tsutils/menu/closable_embed_base.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.584801 tsutils-8.0.2/tsutils/menu/components/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.2/tsutils/menu/components/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.2/tsutils/menu/components/config.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1342 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/menu/components/footers.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.2/tsutils/menu/components/panes.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3348 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/menu/pad_view.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.2/tsutils/menu/simple_text.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.585481 tsutils-8.0.2/tsutils/menu/view/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.2/tsutils/menu/view/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/menu/view/closable_embed.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/menu/view/simple_text.py
--rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.2/tsutils/menu/view/view_state_base.py
--rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.2/tsutils/old_menu.py
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/pad.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.586241 tsutils-8.0.2/tsutils/query_settings/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.2/tsutils/query_settings/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.2/tsutils/query_settings/converters.py
--rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.2/tsutils/query_settings/enums.py
--rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.2/tsutils/query_settings/query_settings.py
--rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.2/tsutils/time.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.587041 tsutils-8.0.2/tsutils/tsubaki/
--rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.2/tsutils/tsubaki/__init__.py
--rw-r--r--   0 chasehult   (501) staff       (20)     4647 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/tsubaki/custom_emoji.py
--rw-r--r--   0 chasehult   (501) staff       (20)     3620 2023-03-14 02:42:07.000000 tsutils-8.0.2/tsutils/tsubaki/links.py
--rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-03-14 02:42:26.000000 tsutils-8.0.2/tsutils/tsubaki/monster_header.py
--rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.2/tsutils/user_interaction.py
-drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-03-14 02:45:41.582904 tsutils-8.0.2/tsutils.egg-info/
--rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:45:41.000000 tsutils-8.0.2/tsutils.egg-info/PKG-INFO
--rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-03-14 02:45:41.000000 tsutils-8.0.2/tsutils.egg-info/SOURCES.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-03-14 02:45:41.000000 tsutils-8.0.2/tsutils.egg-info/dependency_links.txt
--rw-r--r--   0 chasehult   (501) staff       (20)       61 2023-03-14 02:45:41.000000 tsutils-8.0.2/tsutils.egg-info/requires.txt
--rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-03-14 02:45:41.000000 tsutils-8.0.2/tsutils.egg-info/top_level.txt
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.972689 tsutils-8.0.3/
+-rw-r--r--   0 chasehult   (501) staff       (20)     1075 2021-09-27 07:51:44.000000 tsutils-8.0.3/LICENSE
+-rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-05-04 07:46:44.972562 tsutils-8.0.3/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)      174 2021-09-27 07:51:44.000000 tsutils-8.0.3/README.md
+-rw-r--r--   0 chasehult   (501) staff       (20)       38 2023-05-04 07:46:44.972730 tsutils-8.0.3/setup.cfg
+-rw-r--r--   0 chasehult   (501) staff       (20)      842 2023-04-14 01:13:39.000000 tsutils-8.0.3/setup.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.967604 tsutils-8.0.3/tsutils/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3920 2022-06-03 03:58:49.000000 tsutils-8.0.3/tsutils/cog_mixins.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1888 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cog_settings.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.968791 tsutils-8.0.3/tsutils/cogs/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      565 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/donations.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      761 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/globaladmin.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      523 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/cogs/userpreferences.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1220 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3436 2022-08-31 20:43:03.000000 tsutils-8.0.3/tsutils/emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1009 2022-03-02 22:25:01.000000 tsutils-8.0.3/tsutils/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1133 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/errors.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2456 2023-02-20 15:48:19.000000 tsutils-8.0.3/tsutils/formatting.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1942 2022-02-14 03:50:39.000000 tsutils-8.0.3/tsutils/helper_classes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3286 2022-06-03 03:07:59.000000 tsutils-8.0.3/tsutils/helper_functions.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2433 2022-11-11 00:42:14.000000 tsutils-8.0.3/tsutils/json_utils.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.969480 tsutils-8.0.3/tsutils/menu/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/menu/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      616 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/menu/closable_embed_base.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.970174 tsutils-8.0.3/tsutils/menu/components/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/components/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      604 2022-03-02 23:07:15.000000 tsutils-8.0.3/tsutils/menu/components/config.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1342 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/components/footers.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2320 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/components/panes.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3348 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/pad_view.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1624 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/menu/simple_text.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.970894 tsutils-8.0.3/tsutils/menu/view/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/view/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      429 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/view/closable_embed.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1790 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/menu/view/simple_text.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      597 2022-01-11 05:08:45.000000 tsutils-8.0.3/tsutils/menu/view/view_state_base.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     5868 2021-09-27 07:51:44.000000 tsutils-8.0.3/tsutils/old_menu.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/pad.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.971581 tsutils-8.0.3/tsutils/query_settings/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 22:16:59.000000 tsutils-8.0.3/tsutils/query_settings/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2017 2022-12-01 06:04:20.000000 tsutils-8.0.3/tsutils/query_settings/converters.py
+-rw-r--r--   0 chasehult   (501) staff       (20)      802 2022-11-11 00:42:14.000000 tsutils-8.0.3/tsutils/query_settings/enums.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     7507 2023-02-20 15:48:19.000000 tsutils-8.0.3/tsutils/query_settings/query_settings.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     1943 2022-06-03 03:07:59.000000 tsutils-8.0.3/tsutils/time.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.972305 tsutils-8.0.3/tsutils/tsubaki/
+-rw-r--r--   0 chasehult   (501) staff       (20)        0 2022-03-02 21:15:46.000000 tsutils-8.0.3/tsutils/tsubaki/__init__.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     4708 2023-05-04 07:35:57.000000 tsutils-8.0.3/tsutils/tsubaki/custom_emoji.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     3620 2023-03-14 02:42:07.000000 tsutils-8.0.3/tsutils/tsubaki/links.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     2736 2023-04-14 01:12:54.000000 tsutils-8.0.3/tsutils/tsubaki/monster_header.py
+-rw-r--r--   0 chasehult   (501) staff       (20)     6874 2022-08-31 20:46:20.000000 tsutils-8.0.3/tsutils/user_interaction.py
+drwxr-xr-x   0 chasehult   (501) staff       (20)        0 2023-05-04 07:46:44.968284 tsutils-8.0.3/tsutils.egg-info/
+-rw-r--r--   0 chasehult   (501) staff       (20)      670 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/PKG-INFO
+-rw-r--r--   0 chasehult   (501) staff       (20)     1260 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        1 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)       61 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/requires.txt
+-rw-r--r--   0 chasehult   (501) staff       (20)        8 2023-05-04 07:46:44.000000 tsutils-8.0.3/tsutils.egg-info/top_level.txt
```

### Comparing `tsutils-8.0.2/LICENSE` & `tsutils-8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/PKG-INFO` & `tsutils-8.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.2
+Version: 8.0.3
 Summary: A collection of helper commands for Red-DiscordBot
 Home-page: https://github.com/TsubakiBotPad/tsutils
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tsutils-8.0.2/setup.py` & `tsutils-8.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsutils",
-    version="8.0.2",
+    version="8.0.3",
     author="The Tsubotki Team",
     author_email="69992611+TsubakiBotPad@users.noreply.github.com",
     license="MIT",
     description="A collection of helper commands for Red-DiscordBot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TsubakiBotPad/tsutils",
```

### Comparing `tsutils-8.0.2/tsutils/cog_mixins.py` & `tsutils-8.0.3/tsutils/cog_mixins.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/cog_settings.py` & `tsutils-8.0.3/tsutils/cog_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/cogs/donations.py` & `tsutils-8.0.3/tsutils/cogs/donations.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/cogs/globaladmin.py` & `tsutils-8.0.3/tsutils/cogs/globaladmin.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/cogs/userpreferences.py` & `tsutils-8.0.3/tsutils/cogs/userpreferences.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/converters.py` & `tsutils-8.0.3/tsutils/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/emoji.py` & `tsutils-8.0.3/tsutils/emoji.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/enums.py` & `tsutils-8.0.3/tsutils/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/errors.py` & `tsutils-8.0.3/tsutils/errors.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/formatting.py` & `tsutils-8.0.3/tsutils/formatting.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/helper_classes.py` & `tsutils-8.0.3/tsutils/helper_classes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/helper_functions.py` & `tsutils-8.0.3/tsutils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/json_utils.py` & `tsutils-8.0.3/tsutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/closable_embed_base.py` & `tsutils-8.0.3/tsutils/menu/closable_embed_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/components/config.py` & `tsutils-8.0.3/tsutils/menu/components/config.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/components/footers.py` & `tsutils-8.0.3/tsutils/menu/components/footers.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/components/panes.py` & `tsutils-8.0.3/tsutils/menu/components/panes.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/pad_view.py` & `tsutils-8.0.3/tsutils/menu/pad_view.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/simple_text.py` & `tsutils-8.0.3/tsutils/menu/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/view/simple_text.py` & `tsutils-8.0.3/tsutils/menu/view/simple_text.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/menu/view/view_state_base.py` & `tsutils-8.0.3/tsutils/menu/view/view_state_base.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/old_menu.py` & `tsutils-8.0.3/tsutils/old_menu.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/pad.py` & `tsutils-8.0.3/tsutils/pad.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/query_settings/converters.py` & `tsutils-8.0.3/tsutils/query_settings/converters.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/query_settings/enums.py` & `tsutils-8.0.3/tsutils/query_settings/enums.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/query_settings/query_settings.py` & `tsutils-8.0.3/tsutils/query_settings/query_settings.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/time.py` & `tsutils-8.0.3/tsutils/time.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/tsubaki/custom_emoji.py` & `tsutils-8.0.3/tsutils/tsubaki/custom_emoji.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,16 @@
     100: 'oe_water_super',
     101: 'oe_wood_super',
     102: 'oe_light_super',
     103: 'oe_dark_super',
     104: 'oe_heart_super',
     105: 'misc_sb_minus',
     106: 'misc_levitate',
+    107: 'misc_comboboost_super',
+    108: 'l_attack_super',
 }
 
 AWAKENING_RESTRICTED_LATENT_VALUE_TO_EMOJI_NAME_MAP = {
     606: 'unmatchable_clear',
     607: 'spinner_clear',
     608: 'absorb_pierce',
 }
```

### Comparing `tsutils-8.0.2/tsutils/tsubaki/links.py` & `tsutils-8.0.3/tsutils/tsubaki/links.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils/tsubaki/monster_header.py` & `tsutils-8.0.3/tsutils/tsubaki/monster_header.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             '\N{REGIONAL INDICATOR SYMBOL LETTER U}\N{REGIONAL INDICATOR SYMBOL LETTER S}' if m.server_priority == Server.NA else '',
             cls._maybe_tsubaki(m, is_tsubaki=is_tsubaki, is_jp_buffed=bool(is_jp_buffed))))
 
     @classmethod
     def box_with_emoji(cls, m, *, link=True, prefix=None,
                        qs: Optional[QuerySettings] = None):
         msg = f"{m.monster_no} - {m.name_en}"
-        suffix = cls._jp_suffix(m, False, False)
+        suffix = cls._server_suffix(m, False, False)
         return Box(
             prefix,
             Text(get_attribute_emoji_by_monster(m)),
             LinkedText(msg, MonsterLink.header_link(m, qs=qs)) if link else Text(msg),
             Text(suffix) if suffix else None,
             delimiter=' '
         )
@@ -35,26 +35,34 @@
     @classmethod
     def text_with_emoji(cls, m, *, prefix=None,
                         qs: Optional[QuerySettings] = None):
         return cls.box_with_emoji(m, link=False, prefix=prefix,
                                   qs=qs).to_markdown()
 
     @classmethod
-    def _jp_suffix(cls, m, is_jp_buffed=False, subname_on_override=True):
+    def _server_suffix(cls, m, is_jp_buffed=False, subname_on_override=True):
         suffix = ""
         if m.roma_subname and (subname_on_override or m.name_en_override is None):
             suffix += ' [{}]'.format(m.roma_subname)
         if not m.on_na:
-            suffix += ' (JP only)'
+            if m.reskin_id is not None:
+                suffix += ' (Has reskin)'
+            else:
+                suffix += ' (JP only)'
+        elif not m.on_jp:
+            if m.reskin_id is not None:
+                suffix += ' (Is reskin)'
+            else:
+                suffix += ' (NA only)'
         if is_jp_buffed:
             suffix += ' (JP buffed)'
         return suffix
 
     @classmethod
     def _maybe_tsubaki(cls, m, is_tsubaki, is_jp_buffed=False):
         """Returns the monster name as well as an `!` if the monster is Tsubaki
 
         To celebrate 1000 issues/PRs in our main Tsubaki repo, we added this easter egg! Yay!
         """
         tsubaki_punctuation = '!' if is_tsubaki else ''
-        suffix = cls._jp_suffix(m, is_jp_buffed)
+        suffix = cls._server_suffix(m, is_jp_buffed)
         return f'[{m.monster_no}] {m.name_en}{tsubaki_punctuation}{suffix}'
```

### Comparing `tsutils-8.0.2/tsutils/user_interaction.py` & `tsutils-8.0.3/tsutils/user_interaction.py`

 * *Files identical despite different names*

### Comparing `tsutils-8.0.2/tsutils.egg-info/PKG-INFO` & `tsutils-8.0.3/tsutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsutils
-Version: 8.0.2
+Version: 8.0.3
 Summary: A collection of helper commands for Red-DiscordBot
 Home-page: https://github.com/TsubakiBotPad/tsutils
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tsutils-8.0.2/tsutils.egg-info/SOURCES.txt` & `tsutils-8.0.3/tsutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

