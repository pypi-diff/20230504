# Comparing `tmp/nonebot_plugin_arktools-1.1.0.tar.gz` & `tmp/nonebot_plugin_arktools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arktools-1.1.0.tar", last modified: Sat Apr 15 08:12:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_arktools-1.2.0.tar", last modified: Thu May  4 05:16:30 2023, max compression
```

## Comparing `nonebot_plugin_arktools-1.1.0.tar` & `nonebot_plugin_arktools-1.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.253734 nonebot_plugin_arktools-1.1.0/
--rw-rw-rw-   0        0        0     1088 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    18443 2023-04-15 08:12:16.252735 nonebot_plugin_arktools-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    17876 2023-04-15 07:55:11.000000 nonebot_plugin_arktools-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.063719 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/
--rw-rw-rw-   0        0        0       20 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.094722 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/
--rw-rw-rw-   0        0        0      498 2023-04-14 10:56:53.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.117725 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/
--rw-rw-rw-   0        0        0      145 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/__init__.py
--rw-rw-rw-   0        0        0      295 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/draw_config.py
--rw-rw-rw-   0        0        0      279 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/ocr_config.py
--rw-rw-rw-   0        0        0     1003 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/path_config.py
--rw-rw-rw-   0        0        0      367 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/proxy_config.py
--rw-rw-rw-   0        0        0      729 2023-04-15 07:42:06.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/scheduler_config.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.125724 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/
--rw-rw-rw-   0        0        0       51 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.137726 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/
--rw-rw-rw-   0        0        0       58 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/__init__.py
--rw-rw-rw-   0        0        0    14379 2023-04-15 06:20:52.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py
--rw-rw-rw-   0        0        0     1897 2023-04-14 11:58:27.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py
--rw-rw-rw-   0        0        0    68752 2023-04-15 05:52:38.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/models_v3.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.140727 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/
--rw-rw-rw-   0        0        0     1413 2023-04-14 11:36:38.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.144725 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_draw_card/
--rw-rw-rw-   0        0        0      629 2023-04-07 10:02:31.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_draw_card/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.152728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/
--rw-rw-rw-   0        0        0     6382 2023-04-14 09:17:46.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py
--rw-rw-rw-   0        0        0     7194 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py
--rw-rw-rw-   0        0        0     1321 2023-04-14 10:56:39.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/help.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.160728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/
--rw-rw-rw-   0        0        0     1081 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.163728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/
--rw-rw-rw-   0        0        0     2839 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.173729 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/
--rw-rw-rw-   0        0        0     6874 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.181730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/
--rw-rw-rw-   0        0        0     5999 2023-04-15 07:49:18.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py
--rw-rw-rw-   0        0        0     5990 2023-04-15 07:48:53.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.189730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/
--rw-rw-rw-   0        0        0     3771 2023-04-14 09:06:35.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py
--rw-rw-rw-   0        0        0    11512 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.197729 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/
--rw-rw-rw-   0        0        0     1902 2023-03-28 04:16:27.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py
--rw-rw-rw-   0        0        0    19932 2023-04-08 12:40:58.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.202730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/
--rw-rw-rw-   0        0        0     5361 2023-04-14 09:13:06.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.222731 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/
--rw-rw-rw-   0        0        0     2172 2023-04-07 02:49:03.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/__init__.py
--rw-rw-rw-   0        0        0    17666 2023-04-15 08:05:19.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/database.py
--rw-rw-rw-   0        0        0     7997 2023-04-15 07:01:42.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/general.py
--rw-rw-rw-   0        0        0     1859 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/image.py
--rw-rw-rw-   0        0        0    13739 2023-04-15 02:39:41.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/update.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.247733 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/
--rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_database_utils.py
--rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_models.py
--rw-rw-rw-   0        0        0      613 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_open_recruitment.py
--rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_operator_info.py
--rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_update_utils.py
--rw-rw-rw-   0        0        0     2251 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.086723 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/
--rw-rw-rw-   0        0        0    18443 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2465 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      234 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 08:12:16.254736 nonebot_plugin_arktools-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-04-14 09:22:48.000000 nonebot_plugin_arktools-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.127291 nonebot_plugin_arktools-1.2.0/
+-rw-rw-rw-   0        0        0     1067 2022-07-09 04:15:32.000000 nonebot_plugin_arktools-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    19188 2023-05-04 05:16:30.126314 nonebot_plugin_arktools-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18621 2023-05-04 05:00:00.000000 nonebot_plugin_arktools-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.014888 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/
+-rw-rw-rw-   0        0        0       20 2023-02-10 14:33:50.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.033444 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/
+-rw-rw-rw-   0        0        0      498 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.046140 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/
+-rw-rw-rw-   0        0        0      145 2023-03-07 19:11:22.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-05-04 02:22:31.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/draw_config.py
+-rw-rw-rw-   0        0        0      279 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/ocr_config.py
+-rw-rw-rw-   0        0        0     1003 2023-03-07 19:11:22.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/path_config.py
+-rw-rw-rw-   0        0        0      367 2023-03-07 19:14:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/proxy_config.py
+-rw-rw-rw-   0        0        0      729 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/scheduler_config.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.051021 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/
+-rw-rw-rw-   0        0        0       51 2023-02-11 06:02:39.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.058834 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/
+-rw-rw-rw-   0        0        0       58 2023-02-11 20:30:55.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/__init__.py
+-rw-rw-rw-   0        0        0    14379 2023-05-04 04:12:06.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py
+-rw-rw-rw-   0        0        0     1897 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py
+-rw-rw-rw-   0        0        0    68765 2023-05-04 04:35:43.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/models_v3.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.060788 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/exceptions/
+-rw-rw-rw-   0        0        0     1643 2023-05-04 03:22:26.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.062742 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_draw_card/
+-rw-rw-rw-   0        0        0      629 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_draw_card/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.067624 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_guess_operator/
+-rw-rw-rw-   0        0        0     6382 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py
+-rw-rw-rw-   0        0        0     7194 2023-03-07 19:07:48.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/help.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.072507 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_monster_siren/
+-rw-rw-rw-   0        0        0     1081 2023-02-12 15:07:16.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-02-11 19:09:55.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.074460 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_operator_birthday/
+-rw-rw-rw-   0        0        0     3045 2023-05-04 05:00:00.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.080321 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_announce_push/
+-rw-rw-rw-   0        0        0     6874 2023-02-19 08:37:55.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-05-04 02:22:31.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.085203 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/
+-rw-rw-rw-   0        0        0     5999 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py
+-rw-rw-rw-   0        0        0     6057 2023-05-04 02:30:58.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.090086 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_open_recruitment/
+-rw-rw-rw-   0        0        0     3771 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py
+-rw-rw-rw-   0        0        0    11512 2023-03-09 00:44:32.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.094906 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_operator_info/
+-rw-rw-rw-   0        0        0     1902 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py
+-rw-rw-rw-   0        0        0    19932 2023-05-04 04:13:11.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.097839 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_sanity_notify/
+-rw-rw-rw-   0        0        0     5361 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.109554 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/
+-rw-rw-rw-   0        0        0     2617 2023-05-04 05:04:18.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/__init__.py
+-rw-rw-rw-   0        0        0    17669 2023-05-04 05:02:41.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/database.py
+-rw-rw-rw-   0        0        0     7997 2023-05-04 02:22:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/general.py
+-rw-rw-rw-   0        0        0     1859 2023-02-10 17:40:27.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/image.py
+-rw-rw-rw-   0        0        0    13799 2023-05-04 04:25:03.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/update.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.123385 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/
+-rw-rw-rw-   0        0        0        0 2023-02-11 05:40:06.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-11 05:39:33.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_database_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-11 05:39:51.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_models.py
+-rw-rw-rw-   0        0        0      613 2023-02-12 15:46:38.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_open_recruitment.py
+-rw-rw-rw-   0        0        0        0 2023-02-11 05:39:26.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_operator_info.py
+-rw-rw-rw-   0        0        0        0 2023-02-11 05:39:44.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_update_utils.py
+-rw-rw-rw-   0        0        0     2251 2023-02-11 05:58:04.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:16:30.028560 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/
+-rw-rw-rw-   0        0        0    19188 2023-05-04 05:16:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2465 2023-05-04 05:16:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 05:16:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2023-05-04 05:16:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 05:16:29.000000 nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 05:16:30.127291 nonebot_plugin_arktools-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-05-04 04:49:14.000000 nonebot_plugin_arktools-1.2.0/setup.py
```

### Comparing `nonebot_plugin_arktools-1.1.0/LICENSE` & `nonebot_plugin_arktools-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Number_Sir
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Number_Sir
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_arktools-1.1.0/PKG-INFO` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_arktools
-Version: 1.1.0
+Name: nonebot-plugin-arktools
+Version: 1.2.0
 Summary: 基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件
 Home-page: https://github.com/NumberSir/nonebot_plugin_arktools
 Author: Number_Sir
 Author-email: Number_Sir@126.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -161,14 +161,15 @@
 xxx/yyy 代表 xxx 或 yyy
 ```
 杂项
 ```text
 方舟帮助 / arkhelp   => 查看指令列表
 更新方舟素材          => 手动更新游戏数据(json)与图片
 更新方舟数据库        => 手动更新数据库
+更新方舟数据库 -D     => 删除原数据库各表并重新写入
 ```
 猜干员
 ```text
 猜干员    => 开始新游戏
 #[干员名] => 猜干员，如：#艾雅法拉
 提示      => 查看答案干员的信息
 结束      => 结束当前局游戏
@@ -254,29 +255,47 @@
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-481b-af92-71052a087670.png" width="500" />
 </div>
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-4295-982c-9498e0b880fb.png" width="500" />
 </div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-4e89-9cd0-dacc2cfe3c9c.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-4bd3-9aa5-3429bb0ecff9.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-4254-9689-f871af80b079.png" width="500" />
+</div>
 </details>
 
 
 # 感谢
  - __[yuanyan3060](https://github.com/yuanyan3060)__ 的 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__
- - __[Kengxxiao](https://github.com/Kengxxiao)__ 的 __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__
  - __[Aceship](https://github.com/Aceship)__ 的 __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__
  - __[AmiyaBot](https://github.com/AmiyaBot)__ 的 __[Amiya-bot](https://github.com/AmiyaBot/Amiya-Bot)__
  - __[Strelizia02](https://github.com/Strelizia02)__ 的 __[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__
  - __[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ 的 __[MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights)__
 
 # 更新日志
 <details>
 <summary>点击展开</summary>
 
+> 2023-05-04 v1.2.0
+> - 更换数据源 [@issue/42](https://github.com/NumberSir/nonebot_plugin_arktools/issues/42)
+> - 更新数据键值对
+> - 修复了使用 `ghproxy` 作为 github 镜像时无法获取数据的问题
+> - 添加了删表重写功能
+> - 修复了从 maa 作业站自动推送作业出错的问题
+> 
 > 2023-04-15 v1.1.0
 > - 公招查询、猜干员、理智提醒现在均可以私聊进行 (不推荐，私聊发消息可能导致风控)
 > - 简易修复了与其它同用 Tortoise-ORM 的插件初始化冲突的问题 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15)
 > - 添加在群聊查询、订阅、推送 [MAA 作业站](https://prts.plus)作业的功能
 > - 修复了更新数据库中某张表格时会删除所有表格的问题
 > 
 > 2023-04-08 v1.0.20
@@ -286,15 +305,15 @@
 > - 修复更新数据库命令不会强制覆盖更新的问题
 > 
 > 2023-04-06 v1.0.18
 > - 修复了舟舟更新数据结构导致的创建表单错误
 >
 > 2023-04-04 v1.0.17
 > - 添加数据库初始化检查，不再每次启动bot时重复创建
-> - 添加每次启动bot时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
+> - 添加每次启动 bot 时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
 >
 > 2023-03-28 v1.0.15
 > - 猜干员与干员信息功能可以使用干员昵称(可自行增删改查)
 > 
 > 2023-03-24 v1.0.14
 > - 修复阿米娅与近卫阿米娅冲突的问题 [@zx-issue/13](https://github.com/NumberSir/zhenxun_arktools/issues/13)
 >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_arktools Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arktools Version: 1.2.0 Summary:
 åºäº OneBot ééå¨ç NoneBot2 ææ¥æ¹èå°å·¥å·ç®±æä»¶ Home-page:
 https://github.com/NumberSir/nonebot_plugin_arktools Author: Number_Sir Author-
 email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -96,16 +96,17 @@
 4452-8959-04861087f4e8.png]
 ## å¹²åæµç§° ä½ç½®é»è®¤å¨ `data/arknights/processed_data/nicknames.json`
 é®ä¸ºå¹²åä¸­æåç§°ï¼å¼ä¸ºæµç§°ï¼å¯èªè¡ä¿®æ¹ã ## æä»¤
 ç¹å»å±å¼ ### è¯¦ç»æä»¤ ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼
 ```text æ ¼å¼ï¼ æä»¤ => å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy
 ``` æé¡¹ ```text æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨
 æ´æ°æ¹èç´ æ => æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç
-æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å
-=> å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
+æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº æ´æ°æ¹èæ°æ®åº -D =>
+å é¤åæ°æ®åºåè¡¨å¹¶éæ°åå¥ ``` çå¹²å ```text çå¹²å =>
+å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
 æ¥çç­æ¡å¹²åçä¿¡æ¯ ç»æ => ç»æå½åå±æ¸¸æ ``` ä»æ¥å¹²å
 ```text ä»æ¥å¹²å => æ¥çä»å¤©è¿çæ¥çå¹²å ``` å¡å£¬ç¹æ­ ```text
 å¡å£¬ç¹æ­ [å³é®å­] => ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åå°ç¾¤å ```
 å¹²åä¿¡æ¯ ```text å¹²å [å¹²åå] =>
 æ¥çå¹²åçç²¾è±åãæè½åçº§ãæè½ä¸ç²¾ãæ¨¡ç»è§£ééè¦çææ
 ``` å¬å¼æå ```text å¬æ [å¬æçé¢æªå¾] =>
 æ¥çæ ç­¾ç»ååå¯è½åºç°çå¹²å åå¤æªå¾ï¼å¬æ => åä¸
@@ -142,43 +143,51 @@
 4520-8632-544940a1cc96.png]
 [https://user-images.githubusercontent.com/52584526/218328344-2b9b0cda-3894-
 451b-9ea0-d7aeec7d200c.png]
 [https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-
 481b-af92-71052a087670.png]
 [https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-
 4295-982c-9498e0b880fb.png]
+[https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-
+4e89-9cd0-dacc2cfe3c9c.png]
+[https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-
+4bd3-9aa5-3429bb0ecff9.png]
+[https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-
+4254-9689-f871af80b079.png]
  # æè°¢ - __[yuanyan3060](https://github.com/yuanyan3060)__ ç __
 [ææ¥æ¹èå¸¸ç¨ç´ æåº](https://github.com/yuanyan3060/Arknights-Bot-
-Resource)__ - __[Kengxxiao](https://github.com/Kengxxiao)__ ç __
-[ãææ¥æ¹èãæ¸¸ææ°æ®åº](https://github.com/Kengxxiao/
-ArknightsGameData)__ - __[Aceship](https://github.com/Aceship)__ ç __
-[Arknight-Images](https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot]
-(https://github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/
-Amiya-Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __
-[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ - __
-[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ ç __[MAA]
-(https://github.com/MaaAssistantArknights/MaaAssistantArknights)__ #
-æ´æ°æ¥å¿  ç¹å»å±å¼ > 2023-04-15 v1.1.0 > -
+Resource)__ - __[Aceship](https://github.com/Aceship)__ ç __[Arknight-Images]
+(https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot](https://
+github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/Amiya-
+Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __[AngelinaBot]
+(https://github.com/Strelizia02/AngelinaBot)__ - __[MaaAssistantArknights]
+(https://github.com/MaaAssistantArknights)__ ç __[MAA](https://github.com/
+MaaAssistantArknights/MaaAssistantArknights)__ # æ´æ°æ¥å¿  ç¹å»å±å¼ >
+2023-05-04 v1.2.0 > - æ´æ¢æ°æ®æº [@issue/42](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/42) > - æ´æ°æ°æ®é®å¼å¯¹ > -
+ä¿®å¤äºä½¿ç¨ `ghproxy` ä½ä¸º github éåæ¶æ æ³è·åæ°æ®çé®é¢ >
+- æ·»å äºå è¡¨éååè½ > - ä¿®å¤äºä» maa
+ä½ä¸ç«èªå¨æ¨éä½ä¸åºéçé®é¢ > > 2023-04-15 v1.1.0 > -
 å¬ææ¥è¯¢ãçå¹²åãçæºæéç°å¨åå¯ä»¥ç§èè¿è¡
 (ä¸æ¨èï¼ç§èåæ¶æ¯å¯è½å¯¼è´é£æ§) > -
 ç®æä¿®å¤äºä¸å¶å®åç¨ Tortoise-ORM çæä»¶åå§åå²çªçé®é¢
 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15) > -
 æ·»å å¨ç¾¤èæ¥è¯¢ãè®¢éãæ¨é [MAA ä½ä¸ç«](https://
 prts.plus)ä½ä¸çåè½ > -
 ä¿®å¤äºæ´æ°æ°æ®åºä¸­æå¼ è¡¨æ ¼æ¶ä¼å é¤ææè¡¨æ ¼çé®é¢ > >
 2023-04-08 v1.0.20 > -
 ä¿®å¤å ç´ æåºæ´æ°æ»åå¯¼è´æ æ³æ¥çå¹²åçé®é¢ > > 2023-04-07
 v1.0.19 > - ä¿®å¤æ´æ°æ°æ®åºå½ä»¤ä¸ä¼å¼ºå¶è¦çæ´æ°çé®é¢ > >
 2023-04-06 v1.0.18 > -
 ä¿®å¤äºèèæ´æ°æ°æ®ç»æå¯¼è´çåå»ºè¡¨åéè¯¯ > > 2023-04-04
 v1.0.17 > -
 æ·»å æ°æ®åºåå§åæ£æ¥ï¼ä¸åæ¯æ¬¡å¯å¨botæ¶éå¤åå»º > -
-æ·»å æ¯æ¬¡å¯å¨botæ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/39]
-(https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-03-28
-v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
+æ·»å æ¯æ¬¡å¯å¨ bot æ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/
+39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-
+03-28 v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
 (å¯èªè¡å¢å æ¹æ¥) > > 2023-03-24 v1.0.14 > -
 ä¿®å¤é¿ç±³å¨ä¸è¿å«é¿ç±³å¨å²çªçé®é¢ [@zx-issue/13](https://
 github.com/NumberSir/zhenxun_arktools/issues/13) > > 2023-03-08 v1.0.12 > -
 æ·»å  rsshub ä»£çéç½®é¡¹ [@issue/34](https://github.com/NumberSir/
 nonebot_plugin_arktools/issues/34) > - ä¿®å¤å¬æå½ä»¤ä¸å¤ççé®é¢
 [@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35) > -
 æ·»å æ¹èç´ æ/èµæºè·¯å¾éç½®é¡¹ï¼ç°å¨é»è®¤å¨æºå¨äººæ ¹ç®å½ä¸
```

### Comparing `nonebot_plugin_arktools-1.1.0/README.md` & `nonebot_plugin_arktools-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 xxx/yyy 代表 xxx 或 yyy
 ```
 杂项
 ```text
 方舟帮助 / arkhelp   => 查看指令列表
 更新方舟素材          => 手动更新游戏数据(json)与图片
 更新方舟数据库        => 手动更新数据库
+更新方舟数据库 -D     => 删除原数据库各表并重新写入
 ```
 猜干员
 ```text
 猜干员    => 开始新游戏
 #[干员名] => 猜干员，如：#艾雅法拉
 提示      => 查看答案干员的信息
 结束      => 结束当前局游戏
@@ -238,29 +239,47 @@
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-481b-af92-71052a087670.png" width="500" />
 </div>
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-4295-982c-9498e0b880fb.png" width="500" />
 </div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-4e89-9cd0-dacc2cfe3c9c.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-4bd3-9aa5-3429bb0ecff9.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-4254-9689-f871af80b079.png" width="500" />
+</div>
 </details>
 
 
 # 感谢
  - __[yuanyan3060](https://github.com/yuanyan3060)__ 的 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__
- - __[Kengxxiao](https://github.com/Kengxxiao)__ 的 __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__
  - __[Aceship](https://github.com/Aceship)__ 的 __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__
  - __[AmiyaBot](https://github.com/AmiyaBot)__ 的 __[Amiya-bot](https://github.com/AmiyaBot/Amiya-Bot)__
  - __[Strelizia02](https://github.com/Strelizia02)__ 的 __[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__
  - __[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ 的 __[MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights)__
 
 # 更新日志
 <details>
 <summary>点击展开</summary>
 
+> 2023-05-04 v1.2.0
+> - 更换数据源 [@issue/42](https://github.com/NumberSir/nonebot_plugin_arktools/issues/42)
+> - 更新数据键值对
+> - 修复了使用 `ghproxy` 作为 github 镜像时无法获取数据的问题
+> - 添加了删表重写功能
+> - 修复了从 maa 作业站自动推送作业出错的问题
+> 
 > 2023-04-15 v1.1.0
 > - 公招查询、猜干员、理智提醒现在均可以私聊进行 (不推荐，私聊发消息可能导致风控)
 > - 简易修复了与其它同用 Tortoise-ORM 的插件初始化冲突的问题 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15)
 > - 添加在群聊查询、订阅、推送 [MAA 作业站](https://prts.plus)作业的功能
 > - 修复了更新数据库中某张表格时会删除所有表格的问题
 > 
 > 2023-04-08 v1.0.20
@@ -270,15 +289,15 @@
 > - 修复更新数据库命令不会强制覆盖更新的问题
 > 
 > 2023-04-06 v1.0.18
 > - 修复了舟舟更新数据结构导致的创建表单错误
 >
 > 2023-04-04 v1.0.17
 > - 添加数据库初始化检查，不再每次启动bot时重复创建
-> - 添加每次启动bot时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
+> - 添加每次启动 bot 时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
 >
 > 2023-03-28 v1.0.15
 > - 猜干员与干员信息功能可以使用干员昵称(可自行增删改查)
 > 
 > 2023-03-24 v1.0.14
 > - 修复阿米娅与近卫阿米娅冲突的问题 [@zx-issue/13](https://github.com/NumberSir/zhenxun_arktools/issues/13)
 >
```

#### html2text {}

```diff
@@ -88,16 +88,17 @@
 4452-8959-04861087f4e8.png]
 ## å¹²åæµç§° ä½ç½®é»è®¤å¨ `data/arknights/processed_data/nicknames.json`
 é®ä¸ºå¹²åä¸­æåç§°ï¼å¼ä¸ºæµç§°ï¼å¯èªè¡ä¿®æ¹ã ## æä»¤
 ç¹å»å±å¼ ### è¯¦ç»æä»¤ ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼
 ```text æ ¼å¼ï¼ æä»¤ => å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy
 ``` æé¡¹ ```text æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨
 æ´æ°æ¹èç´ æ => æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç
-æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å
-=> å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
+æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº æ´æ°æ¹èæ°æ®åº -D =>
+å é¤åæ°æ®åºåè¡¨å¹¶éæ°åå¥ ``` çå¹²å ```text çå¹²å =>
+å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
 æ¥çç­æ¡å¹²åçä¿¡æ¯ ç»æ => ç»æå½åå±æ¸¸æ ``` ä»æ¥å¹²å
 ```text ä»æ¥å¹²å => æ¥çä»å¤©è¿çæ¥çå¹²å ``` å¡å£¬ç¹æ­ ```text
 å¡å£¬ç¹æ­ [å³é®å­] => ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åå°ç¾¤å ```
 å¹²åä¿¡æ¯ ```text å¹²å [å¹²åå] =>
 æ¥çå¹²åçç²¾è±åãæè½åçº§ãæè½ä¸ç²¾ãæ¨¡ç»è§£ééè¦çææ
 ``` å¬å¼æå ```text å¬æ [å¬æçé¢æªå¾] =>
 æ¥çæ ç­¾ç»ååå¯è½åºç°çå¹²å åå¤æªå¾ï¼å¬æ => åä¸
@@ -134,43 +135,51 @@
 4520-8632-544940a1cc96.png]
 [https://user-images.githubusercontent.com/52584526/218328344-2b9b0cda-3894-
 451b-9ea0-d7aeec7d200c.png]
 [https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-
 481b-af92-71052a087670.png]
 [https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-
 4295-982c-9498e0b880fb.png]
+[https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-
+4e89-9cd0-dacc2cfe3c9c.png]
+[https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-
+4bd3-9aa5-3429bb0ecff9.png]
+[https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-
+4254-9689-f871af80b079.png]
  # æè°¢ - __[yuanyan3060](https://github.com/yuanyan3060)__ ç __
 [ææ¥æ¹èå¸¸ç¨ç´ æåº](https://github.com/yuanyan3060/Arknights-Bot-
-Resource)__ - __[Kengxxiao](https://github.com/Kengxxiao)__ ç __
-[ãææ¥æ¹èãæ¸¸ææ°æ®åº](https://github.com/Kengxxiao/
-ArknightsGameData)__ - __[Aceship](https://github.com/Aceship)__ ç __
-[Arknight-Images](https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot]
-(https://github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/
-Amiya-Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __
-[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ - __
-[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ ç __[MAA]
-(https://github.com/MaaAssistantArknights/MaaAssistantArknights)__ #
-æ´æ°æ¥å¿  ç¹å»å±å¼ > 2023-04-15 v1.1.0 > -
+Resource)__ - __[Aceship](https://github.com/Aceship)__ ç __[Arknight-Images]
+(https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot](https://
+github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/Amiya-
+Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __[AngelinaBot]
+(https://github.com/Strelizia02/AngelinaBot)__ - __[MaaAssistantArknights]
+(https://github.com/MaaAssistantArknights)__ ç __[MAA](https://github.com/
+MaaAssistantArknights/MaaAssistantArknights)__ # æ´æ°æ¥å¿  ç¹å»å±å¼ >
+2023-05-04 v1.2.0 > - æ´æ¢æ°æ®æº [@issue/42](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/42) > - æ´æ°æ°æ®é®å¼å¯¹ > -
+ä¿®å¤äºä½¿ç¨ `ghproxy` ä½ä¸º github éåæ¶æ æ³è·åæ°æ®çé®é¢ >
+- æ·»å äºå è¡¨éååè½ > - ä¿®å¤äºä» maa
+ä½ä¸ç«èªå¨æ¨éä½ä¸åºéçé®é¢ > > 2023-04-15 v1.1.0 > -
 å¬ææ¥è¯¢ãçå¹²åãçæºæéç°å¨åå¯ä»¥ç§èè¿è¡
 (ä¸æ¨èï¼ç§èåæ¶æ¯å¯è½å¯¼è´é£æ§) > -
 ç®æä¿®å¤äºä¸å¶å®åç¨ Tortoise-ORM çæä»¶åå§åå²çªçé®é¢
 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15) > -
 æ·»å å¨ç¾¤èæ¥è¯¢ãè®¢éãæ¨é [MAA ä½ä¸ç«](https://
 prts.plus)ä½ä¸çåè½ > -
 ä¿®å¤äºæ´æ°æ°æ®åºä¸­æå¼ è¡¨æ ¼æ¶ä¼å é¤ææè¡¨æ ¼çé®é¢ > >
 2023-04-08 v1.0.20 > -
 ä¿®å¤å ç´ æåºæ´æ°æ»åå¯¼è´æ æ³æ¥çå¹²åçé®é¢ > > 2023-04-07
 v1.0.19 > - ä¿®å¤æ´æ°æ°æ®åºå½ä»¤ä¸ä¼å¼ºå¶è¦çæ´æ°çé®é¢ > >
 2023-04-06 v1.0.18 > -
 ä¿®å¤äºèèæ´æ°æ°æ®ç»æå¯¼è´çåå»ºè¡¨åéè¯¯ > > 2023-04-04
 v1.0.17 > -
 æ·»å æ°æ®åºåå§åæ£æ¥ï¼ä¸åæ¯æ¬¡å¯å¨botæ¶éå¤åå»º > -
-æ·»å æ¯æ¬¡å¯å¨botæ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/39]
-(https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-03-28
-v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
+æ·»å æ¯æ¬¡å¯å¨ bot æ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/
+39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-
+03-28 v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
 (å¯èªè¡å¢å æ¹æ¥) > > 2023-03-24 v1.0.14 > -
 ä¿®å¤é¿ç±³å¨ä¸è¿å«é¿ç±³å¨å²çªçé®é¢ [@zx-issue/13](https://
 github.com/NumberSir/zhenxun_arktools/issues/13) > > 2023-03-08 v1.0.12 > -
 æ·»å  rsshub ä»£çéç½®é¡¹ [@issue/34](https://github.com/NumberSir/
 nonebot_plugin_arktools/issues/34) > - ä¿®å¤å¬æå½ä»¤ä¸å¤ççé®é¢
 [@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35) > -
 æ·»å æ¹èç´ æ/èµæºè·¯å¾éç½®é¡¹ï¼ç°å¨é»è®¤å¨æºå¨äººæ ¹ç®å½ä¸
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/path_config.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/path_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/scheduler_config.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/configs/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/models_v3.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/core/models_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1227,23 +1227,23 @@
     @property
     def level_up_cost_condition(self) -> List["SkillLevelUpCondition"]:
         """技能专精相关"""
         if not self._extra_data:
             raise NotImplementedError("未输入干员数据！")
         return [
             SkillLevelUpCondition(skill=self, data=d)
-            for d in self._extra_data["levelUpCostCond"]
+            for d in self._extra_data["specializeLevelUpData"]
         ]
 
     @property
     def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁(phase, level)"""
         if not self._extra_data:
             raise NotImplementedError("未输入干员数据！")
-        return CharacterUnlockCondition(data=self._extra_data["unlockCond"])
+        return CharacterUnlockCondition(data=self._extra_data["initialUnlockCond"])
 
     # 不在 arknights_skill_table 中的
     @property
     def icon(self) -> Image:
         """技能图标"""
         return Image.open(gameimage_path / "skill" / f"skill_icon_{self.icon_id or self.id}.png")
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/exceptions/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 
 class MAANoResultException(ArkBaseException):
     """没有作业"""
     def __init__(self, msg: str = "没有查询到结果！", details: str = ""):
         super().__init__(msg, details)
 
 
+class NoHandbookInfoException(ArkBaseException):
+    """没有档案"""
+    def __init__(self, msg: str = "干员没有档案！", details: str = ""):
+        super().__init__(msg, details)
+
+
 __all__ = [
     "NamedCharacterNotExistException",
     "NamedPoolNotExistException",
+    "NoHandbookInfoException",
 
     "MAAFailedResponseException",
     "MAANoResultException"
 ]
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_draw_card/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_draw_card/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/help.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List
 from datetime import datetime
 from PIL import Image, ImageFont
 from PIL.ImageDraw import Draw
 from io import BytesIO
 
 from ..core.models_v3 import Character
+from ..exceptions import NoHandbookInfoException
 from ..utils import text_border
 from ..configs.path_config import PathConfig
 
 
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
 font_path = Path(pcfg.arknights_font_path).absolute()
 
@@ -22,20 +23,23 @@
 today_birthday = on_command("今日干员")
 
 
 @today_birthday.handle()
 async def _():
     today = datetime.now().strftime("%m月%d日").strip("0").replace("月0", "月")
     characters = await Character.all()
+    try:
+        results: List["Character"] = [
+            cht
+            for cht in characters
+            if (await cht.get_handbook_info()).story_text_audio.birthday == today
+        ]
+    except NoHandbookInfoException as e:
+        await today_birthday.finish(f"嗯唔……干员的档案数据不全哦")
 
-    results: List["Character"] = [
-        cht
-        for cht in characters
-        if (await cht.get_handbook_info()).story_text_audio.birthday == today
-    ]
     if not results:
         await today_birthday.finish("哦呀？今天没有干员过生日哦……")
     try:
         main_background = Image.new("RGBA", (24*2+128*len(results)+16*(len(results)-1), 24*2+128+24), (0, 0, 0, 0))
         for idx, cht in enumerate(results):
             cht_bg = Image.new("RGBA", (128, 128+24), (150, 150, 150, 150))
             icon = cht.avatar.convert("RGBA").resize((128, 128))
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import random
 from io import BytesIO
+from datetime import datetime
 from typing import List, Dict, Tuple, Optional
 
 import httpx
 from nonebot import logger
 from nonebot_plugin_imageutils import text2image
 
 from ..core.database.plugin_sqlite import MAACopilotSubsModel
@@ -54,15 +55,15 @@
 
 
 async def process_works(works: List[Dict], keyword: str) -> Optional[Tuple[BytesIO, int, str]]:
     """判断最新、加进数据库，返回图片内容 + 关卡id"""
     work = works[0]
     local_data = await MAACopilotSubsModel.filter(sub_keyword=keyword).first()
     local_upload_time = local_data.latest_upload_time
-    latest_upload_time = work["upload_time"]
+    latest_upload_time = datetime.fromisoformat(work["upload_time"]).timestamp()
 
     if latest_upload_time <= local_upload_time:
         return None
 
     content = json.loads(work["content"])
     operators = content["opers"]
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/__init__.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """一些功能吧"""
 from .general import *
 from .image import *
 from .database import *
 from .update import *
 
 from nonebot import on_command, logger
+from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
+from nonebot.adapters.onebot.v11 import Message
 import httpx
 
 
 update_game_resource = on_command("更新方舟素材")
 init_db = on_command("更新方舟数据库")
 
 
@@ -26,28 +28,34 @@
         logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
         await update_game_resource.finish("下载方舟游戏素材请求出错或连接超时，请修改代理、重试或手动下载：\nhttps://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
     else:
         await update_game_resource.finish("游戏素材更新完成！")
 
 
 @init_db.handle()
-async def _():
+async def _(args: Message = CommandArg()):
     await update_game_resource.send("开始更新游戏数据库，视磁盘读写性能需1分钟左右……")
-    await ArknightsDB.init_data(force=True)
+    if args.extract_plain_text().strip() == "-D":
+        await ArknightsDB.drop_data()
+        await update_game_resource.send("已彻底删除原表，开始重新写入数据库……")
+        await ArknightsDB.init_db()
+    else:
+        await ArknightsDB.init_data(force=True)
     await update_game_resource.finish("游戏数据库更新完成！")
 
 
 __plugin_meta__ = PluginMetadata(
     name="杂项",
     description="查看指令列表、更新游戏素材、更新本地数据库",
     usage=(
         "命令:"
         "\n    方舟帮助 => 查看指令列表"
         "\n    更新方舟素材 => 从Github下载游戏素材(json数据与图片)"
         "\n    更新方舟数据库 => 更新本地sqlite数据库"
+        "\n    更新方舟数据库 -D => 删除原数据库各表并重新写入"
     ),
     extra={
         "name": "update_plugin_data",
         "author": "NumberSir<number_sir@126.com>",
         "version": "0.1.0"
     }
 )
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/database.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         async with aopen(gamedata_path / "excel" / "skill_table.json", "r", encoding="utf-8") as fp:
             data = await fp.read()
         data = json.loads(data)
         tasks = {
             SkillModel.update_or_create(
                 name=v["levels"][0]["name"],
                 skillType=v["levels"][0]["skillType"],
-                durationType=v["levels"][0]["skillType"],
+                durationType=v["levels"][0]["durationType"],
                 prefabId=v["levels"][0]["prefabId"],
                 **v
             )
             for _, v in data.items()
         }
         await asyncio.gather(*tasks)
         logger.info("\t- Skill data initiated")
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/general.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/general.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/image.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/update.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/src/utils/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 xcfg = ProxyConfig.parse_obj(get_driver().config.dict())
 BASE_URL_RAW = xcfg.github_raw  # 镜像
 BASE_URL_SITE = xcfg.github_site
 
 scfg = SchedulerConfig.parse_obj(get_driver().config.dict())
 
 REPOSITORIES = {
-    "gamedata": "/Kengxxiao/ArknightsGameData/master",
+    "gamedata": "/yuanyan3060/ArknightsGameResource/master",
     "gameimage_1": "/yuanyan3060/Arknights-Bot-Resource/master",
     "gameimage_2": "/Aceship/Arknight-Images/master",
 }
 
 FILES = {
     "gamedata": [
-        "zh_CN/gamedata/excel/building_data.json",          # 基建技能，制造配方
-        "zh_CN/gamedata/excel/char_patch_table.json",       # 升变阿米娅
-        "zh_CN/gamedata/excel/character_table.json",        # 干员表
-        "zh_CN/gamedata/excel/data_version.txt",            # 数据版本
-        "zh_CN/gamedata/excel/gamedata_const.json",         # 游戏常数
-        "zh_CN/gamedata/excel/gacha_table.json",            # 公招相关
-        "zh_CN/gamedata/excel/item_table.json",             # 物品表
-        "zh_CN/gamedata/excel/handbook_info_table.json",    # 档案表
-        "zh_CN/gamedata/excel/skill_table.json",            # 技能表
-        "zh_CN/gamedata/excel/uniequip_table.json",         # 模组表、子职业映射
-        "zh_CN/gamedata/excel/handbook_team_table.json",    # 干员阵营
-        "zh_CN/gamedata/excel/skin_table.json",             # 皮肤
-        "zh_CN/gamedata/excel/stage_table.json",            # 关卡
+        "gamedata/excel/building_data.json",          # 基建技能，制造配方
+        "gamedata/excel/char_patch_table.json",       # 升变阿米娅
+        "gamedata/excel/character_table.json",        # 干员表
+        "gamedata/excel/data_version.txt",            # 数据版本
+        "gamedata/excel/gamedata_const.json",         # 游戏常数
+        "gamedata/excel/gacha_table.json",            # 公招相关
+        "gamedata/excel/item_table.json",             # 物品表
+        "gamedata/excel/handbook_info_table.json",    # 档案表
+        "gamedata/excel/skill_table.json",            # 技能表
+        "gamedata/excel/uniequip_table.json",         # 模组表、子职业映射
+        "gamedata/excel/handbook_team_table.json",    # 干员阵营
+        "gamedata/excel/skin_table.json",             # 皮肤
+        "gamedata/excel/stage_table.json",            # 关卡
     ]
 }
 
 DIRS = {
     "gamedata": [
         "/zh_CN/gamedata/excel"
     ],
@@ -93,16 +93,16 @@
                 data = await fp.read()
         except FileNotFoundError as e:
             return ""
         return data.split(":")[-1].strip("\n").strip()
 
     async def get_latest_version(self) -> str:
         """获取最新版本"""
-        url = f"{self._url}/zh_CN/gamedata/excel/data_version.txt"
-        response = await self._client.get(url)
+        url = f"{self._url}/gamedata/excel/data_version.txt"
+        response = await self._client.get(url, follow_redirects=True)
         return response.text.split(":")[-1].strip("\n").strip()  # eg: "31.4.0"
 
     async def is_update_needed(self) -> bool:
         """是否要更新"""
         return await self.get_local_version() != await self.get_latest_version()
 
     async def download_files(self):
@@ -116,15 +116,15 @@
             for file in FILES['gamedata']
         ]
         await asyncio.gather(*tasks)
         logger.info("===== ARKNIGHTS GAMEDATA DOWNLOAD DONE ")
 
     async def save(self, url: str, file: str, tmp: Path):
         """异步gather用"""
-        content = (await self._client.get(f"{url}/{file}", timeout=100)).content
+        content = (await self._client.get(f"{url}/{file}", timeout=100, follow_redirects=True)).content
         async with aopen(tmp / file.split('/')[-1], "wb") as fp:
             await fp.write(content)
         logger.info(f"\t- Arknights-Data downloaded: {file.split('/')[-1]}")
 
 
 class ArknightsGameImage:
     def __init__(self, client: httpx.AsyncClient = None):
@@ -205,21 +205,21 @@
 
         tasks = [self.save(url, tmp) for url in self._urls if not (tmp / url.split('/master/')[-1]).exists()]
         await asyncio.gather(*tasks)
         logger.info("===== ARKNIGHTS GAMEIMAGE DOWNLOAD DONE ")
 
     async def get_htmls(self, url: str, dir_: str):
         """异步gather用"""
-        html = (await self._client.get(url, timeout=100)).text
+        html = (await self._client.get(url, timeout=100, follow_redirects=True)).text
         self._htmls[dir_] = (html, url)
 
     async def save(self, url: str, tmp: Path):
         """异步gather用"""
         # print(url)
-        content = (await self._client.get(quote(url, safe="/:"), timeout=100)).content
+        content = (await self._client.get(quote(url, safe="/:"), timeout=100, follow_redirects=True)).content
         if not url.endswith(".png"):
             return
         async with aopen(tmp / unquote(url).split('/master/')[-1], "wb") as fp:
             await fp.write(content)
         logger.info(f"\t- Arknights-Image downloaded: {unquote(url).split('/master/')[-1]}")
 
 
@@ -237,15 +237,15 @@
     logger.info("##### EXTRA FILES DOWNLOAD BEGIN")
     await aos.makedirs(data_path / "guess_character", exist_ok=True)
     await aos.makedirs(data_path / "arknights/processed_data", exist_ok=True)
     for url in urls:
         path = url.split("/data/")[-1]
         if (data_path / path).exists():
             continue
-        response = await client.get(url)
+        response = await client.get(url, follow_redirects=True)
         async with aopen(data_path / path, "wb") as fp:
             await fp.write(response.content)
             logger.info(f"\t- Extra file downloaded: {path}")
     await download_fonts(client)
     logger.info("===== EXTRA FILES DOWNLOAD DONE")
 
 
@@ -256,15 +256,15 @@
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/fonts/Arknights-zh.otf",
     ]
     await aos.makedirs(font_path, exist_ok=True)
     for url in urls:
         path = url.split("/")[-1]
         if (font_path / path).exists():
             continue
-        response = await client.get(url)
+        response = await client.get(url, follow_redirects=True)
         async with aopen(font_path / path, "wb") as fp:
             await fp.write(response.content)
             logger.info(f"\t- Font file downloaded: {path}")
 
 
 @driver.on_startup
 async def _init_game_files():
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_open_recruitment.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/test_open_recruitment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/utils.py` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools/test/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/PKG-INFO` & `nonebot_plugin_arktools-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-arktools
-Version: 1.1.0
+Name: nonebot_plugin_arktools
+Version: 1.2.0
 Summary: 基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件
 Home-page: https://github.com/NumberSir/nonebot_plugin_arktools
 Author: Number_Sir
 Author-email: Number_Sir@126.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -161,14 +161,15 @@
 xxx/yyy 代表 xxx 或 yyy
 ```
 杂项
 ```text
 方舟帮助 / arkhelp   => 查看指令列表
 更新方舟素材          => 手动更新游戏数据(json)与图片
 更新方舟数据库        => 手动更新数据库
+更新方舟数据库 -D     => 删除原数据库各表并重新写入
 ```
 猜干员
 ```text
 猜干员    => 开始新游戏
 #[干员名] => 猜干员，如：#艾雅法拉
 提示      => 查看答案干员的信息
 结束      => 结束当前局游戏
@@ -254,29 +255,47 @@
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-481b-af92-71052a087670.png" width="500" />
 </div>
 
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-4295-982c-9498e0b880fb.png" width="500" />
 </div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-4e89-9cd0-dacc2cfe3c9c.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-4bd3-9aa5-3429bb0ecff9.png" width="500" />
+</div>
+
+<div align="left">
+  <img src="https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-4254-9689-f871af80b079.png" width="500" />
+</div>
 </details>
 
 
 # 感谢
  - __[yuanyan3060](https://github.com/yuanyan3060)__ 的 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__
- - __[Kengxxiao](https://github.com/Kengxxiao)__ 的 __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__
  - __[Aceship](https://github.com/Aceship)__ 的 __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__
  - __[AmiyaBot](https://github.com/AmiyaBot)__ 的 __[Amiya-bot](https://github.com/AmiyaBot/Amiya-Bot)__
  - __[Strelizia02](https://github.com/Strelizia02)__ 的 __[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__
  - __[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ 的 __[MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights)__
 
 # 更新日志
 <details>
 <summary>点击展开</summary>
 
+> 2023-05-04 v1.2.0
+> - 更换数据源 [@issue/42](https://github.com/NumberSir/nonebot_plugin_arktools/issues/42)
+> - 更新数据键值对
+> - 修复了使用 `ghproxy` 作为 github 镜像时无法获取数据的问题
+> - 添加了删表重写功能
+> - 修复了从 maa 作业站自动推送作业出错的问题
+> 
 > 2023-04-15 v1.1.0
 > - 公招查询、猜干员、理智提醒现在均可以私聊进行 (不推荐，私聊发消息可能导致风控)
 > - 简易修复了与其它同用 Tortoise-ORM 的插件初始化冲突的问题 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15)
 > - 添加在群聊查询、订阅、推送 [MAA 作业站](https://prts.plus)作业的功能
 > - 修复了更新数据库中某张表格时会删除所有表格的问题
 > 
 > 2023-04-08 v1.0.20
@@ -286,15 +305,15 @@
 > - 修复更新数据库命令不会强制覆盖更新的问题
 > 
 > 2023-04-06 v1.0.18
 > - 修复了舟舟更新数据结构导致的创建表单错误
 >
 > 2023-04-04 v1.0.17
 > - 添加数据库初始化检查，不再每次启动bot时重复创建
-> - 添加每次启动bot时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
+> - 添加每次启动 bot 时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
 >
 > 2023-03-28 v1.0.15
 > - 猜干员与干员信息功能可以使用干员昵称(可自行增删改查)
 > 
 > 2023-03-24 v1.0.14
 > - 修复阿米娅与近卫阿米娅冲突的问题 [@zx-issue/13](https://github.com/NumberSir/zhenxun_arktools/issues/13)
 >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arktools Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_arktools Version: 1.2.0 Summary:
 åºäº OneBot ééå¨ç NoneBot2 ææ¥æ¹èå°å·¥å·ç®±æä»¶ Home-page:
 https://github.com/NumberSir/nonebot_plugin_arktools Author: Number_Sir Author-
 email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -96,16 +96,17 @@
 4452-8959-04861087f4e8.png]
 ## å¹²åæµç§° ä½ç½®é»è®¤å¨ `data/arknights/processed_data/nicknames.json`
 é®ä¸ºå¹²åä¸­æåç§°ï¼å¼ä¸ºæµç§°ï¼å¯èªè¡ä¿®æ¹ã ## æä»¤
 ç¹å»å±å¼ ### è¯¦ç»æä»¤ ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼
 ```text æ ¼å¼ï¼ æä»¤ => å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy
 ``` æé¡¹ ```text æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨
 æ´æ°æ¹èç´ æ => æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç
-æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å
-=> å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
+æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº æ´æ°æ¹èæ°æ®åº -D =>
+å é¤åæ°æ®åºåè¡¨å¹¶éæ°åå¥ ``` çå¹²å ```text çå¹²å =>
+å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
 æ¥çç­æ¡å¹²åçä¿¡æ¯ ç»æ => ç»æå½åå±æ¸¸æ ``` ä»æ¥å¹²å
 ```text ä»æ¥å¹²å => æ¥çä»å¤©è¿çæ¥çå¹²å ``` å¡å£¬ç¹æ­ ```text
 å¡å£¬ç¹æ­ [å³é®å­] => ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åå°ç¾¤å ```
 å¹²åä¿¡æ¯ ```text å¹²å [å¹²åå] =>
 æ¥çå¹²åçç²¾è±åãæè½åçº§ãæè½ä¸ç²¾ãæ¨¡ç»è§£ééè¦çææ
 ``` å¬å¼æå ```text å¬æ [å¬æçé¢æªå¾] =>
 æ¥çæ ç­¾ç»ååå¯è½åºç°çå¹²å åå¤æªå¾ï¼å¬æ => åä¸
@@ -142,43 +143,51 @@
 4520-8632-544940a1cc96.png]
 [https://user-images.githubusercontent.com/52584526/218328344-2b9b0cda-3894-
 451b-9ea0-d7aeec7d200c.png]
 [https://user-images.githubusercontent.com/52584526/218328356-a8a511c4-fa62-
 481b-af92-71052a087670.png]
 [https://user-images.githubusercontent.com/52584526/218328361-95ae9117-cd5e-
 4295-982c-9498e0b880fb.png]
+[https://user-images.githubusercontent.com/52584526/232200400-43d46da2-09a7-
+4e89-9cd0-dacc2cfe3c9c.png]
+[https://user-images.githubusercontent.com/52584526/232200403-275f5ef9-bcd3-
+4bd3-9aa5-3429bb0ecff9.png]
+[https://user-images.githubusercontent.com/52584526/232200407-b689d0af-e764-
+4254-9689-f871af80b079.png]
  # æè°¢ - __[yuanyan3060](https://github.com/yuanyan3060)__ ç __
 [ææ¥æ¹èå¸¸ç¨ç´ æåº](https://github.com/yuanyan3060/Arknights-Bot-
-Resource)__ - __[Kengxxiao](https://github.com/Kengxxiao)__ ç __
-[ãææ¥æ¹èãæ¸¸ææ°æ®åº](https://github.com/Kengxxiao/
-ArknightsGameData)__ - __[Aceship](https://github.com/Aceship)__ ç __
-[Arknight-Images](https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot]
-(https://github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/
-Amiya-Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __
-[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ - __
-[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ ç __[MAA]
-(https://github.com/MaaAssistantArknights/MaaAssistantArknights)__ #
-æ´æ°æ¥å¿  ç¹å»å±å¼ > 2023-04-15 v1.1.0 > -
+Resource)__ - __[Aceship](https://github.com/Aceship)__ ç __[Arknight-Images]
+(https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot](https://
+github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/Amiya-
+Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __[AngelinaBot]
+(https://github.com/Strelizia02/AngelinaBot)__ - __[MaaAssistantArknights]
+(https://github.com/MaaAssistantArknights)__ ç __[MAA](https://github.com/
+MaaAssistantArknights/MaaAssistantArknights)__ # æ´æ°æ¥å¿  ç¹å»å±å¼ >
+2023-05-04 v1.2.0 > - æ´æ¢æ°æ®æº [@issue/42](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/42) > - æ´æ°æ°æ®é®å¼å¯¹ > -
+ä¿®å¤äºä½¿ç¨ `ghproxy` ä½ä¸º github éåæ¶æ æ³è·åæ°æ®çé®é¢ >
+- æ·»å äºå è¡¨éååè½ > - ä¿®å¤äºä» maa
+ä½ä¸ç«èªå¨æ¨éä½ä¸åºéçé®é¢ > > 2023-04-15 v1.1.0 > -
 å¬ææ¥è¯¢ãçå¹²åãçæºæéç°å¨åå¯ä»¥ç§èè¿è¡
 (ä¸æ¨èï¼ç§èåæ¶æ¯å¯è½å¯¼è´é£æ§) > -
 ç®æä¿®å¤äºä¸å¶å®åç¨ Tortoise-ORM çæä»¶åå§åå²çªçé®é¢
 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15) > -
 æ·»å å¨ç¾¤èæ¥è¯¢ãè®¢éãæ¨é [MAA ä½ä¸ç«](https://
 prts.plus)ä½ä¸çåè½ > -
 ä¿®å¤äºæ´æ°æ°æ®åºä¸­æå¼ è¡¨æ ¼æ¶ä¼å é¤ææè¡¨æ ¼çé®é¢ > >
 2023-04-08 v1.0.20 > -
 ä¿®å¤å ç´ æåºæ´æ°æ»åå¯¼è´æ æ³æ¥çå¹²åçé®é¢ > > 2023-04-07
 v1.0.19 > - ä¿®å¤æ´æ°æ°æ®åºå½ä»¤ä¸ä¼å¼ºå¶è¦çæ´æ°çé®é¢ > >
 2023-04-06 v1.0.18 > -
 ä¿®å¤äºèèæ´æ°æ°æ®ç»æå¯¼è´çåå»ºè¡¨åéè¯¯ > > 2023-04-04
 v1.0.17 > -
 æ·»å æ°æ®åºåå§åæ£æ¥ï¼ä¸åæ¯æ¬¡å¯å¨botæ¶éå¤åå»º > -
-æ·»å æ¯æ¬¡å¯å¨botæ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/39]
-(https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-03-28
-v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
+æ·»å æ¯æ¬¡å¯å¨ bot æ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/
+39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-
+03-28 v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
 (å¯èªè¡å¢å æ¹æ¥) > > 2023-03-24 v1.0.14 > -
 ä¿®å¤é¿ç±³å¨ä¸è¿å«é¿ç±³å¨å²çªçé®é¢ [@zx-issue/13](https://
 github.com/NumberSir/zhenxun_arktools/issues/13) > > 2023-03-08 v1.0.12 > -
 æ·»å  rsshub ä»£çéç½®é¡¹ [@issue/34](https://github.com/NumberSir/
 nonebot_plugin_arktools/issues/34) > - ä¿®å¤å¬æå½ä»¤ä¸å¤ççé®é¢
 [@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35) > -
 æ·»å æ¹èç´ æ/èµæºè·¯å¾éç½®é¡¹ï¼ç°å¨é»è®¤å¨æºå¨äººæ ¹ç®å½ä¸
```

### Comparing `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/SOURCES.txt` & `nonebot_plugin_arktools-1.2.0/nonebot_plugin_arktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.1.0/setup.py` & `nonebot_plugin_arktools-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="nonebot_plugin_arktools",
-    version="1.1.0",
+    version="1.2.0",
     author="Number_Sir",
     author_email="Number_Sir@126.com",
     keywords=["pip", "nonebot2", "nonebot", "nonebot_plugin"],
     description="""基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NumberSir/nonebot_plugin_arktools",
```

