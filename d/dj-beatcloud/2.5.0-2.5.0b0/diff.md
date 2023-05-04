# Comparing `tmp/dj_beatcloud-2.5.0.tar.gz` & `tmp/dj_beatcloud-2.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.0.tar", last modified: Thu May  4 18:30:43 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.0b0.tar", last modified: Wed May  3 03:53:24 2023, max compression
```

## Comparing `dj_beatcloud-2.5.0.tar` & `dj_beatcloud-2.5.0b0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.306432 dj_beatcloud-2.5.0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2691 2023-05-04 18:30:43.306516 dj_beatcloud-2.5.0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1408 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.294943 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2691 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1872 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-04 18:30:43.000000 dj_beatcloud-2.5.0/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.295605 dj_beatcloud-2.5.0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.297721 dj_beatcloud-2.5.0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1213 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13431 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5020 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.297936 dj_beatcloud-2.5.0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.301182 dj_beatcloud-2.5.0/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5334 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.302886 dj_beatcloud-2.5.0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5977 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.304296 dj_beatcloud-2.5.0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4710 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8276 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4324 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8707 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5000 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      880 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-04 18:30:43.306192 dj_beatcloud-2.5.0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      879 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3478 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9536 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8363 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-04 18:30:43.306820 dj_beatcloud-2.5.0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2206 2023-05-04 18:29:20.000000 dj_beatcloud-2.5.0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.217272 dj_beatcloud-2.5.0b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.0b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.217364 dj_beatcloud-2.5.0b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)      717 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.202279 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1872 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.203371 dj_beatcloud-2.5.0b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.206815 dj_beatcloud-2.5.0b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1213 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13431 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-03 01:35:47.000000 dj_beatcloud-2.5.0b0/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5020 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.207070 dj_beatcloud-2.5.0b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.210947 dj_beatcloud-2.5.0b0/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5334 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.212896 dj_beatcloud-2.5.0b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16576 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5977 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.214475 dj_beatcloud-2.5.0b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4710 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8276 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4324 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8707 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5000 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      880 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.216990 dj_beatcloud-2.5.0b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      879 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3478 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9526 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8363 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 19:26:48.000000 dj_beatcloud-2.5.0b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-03 03:53:24.217669 dj_beatcloud-2.5.0b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2223 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/setup.py
```

### Comparing `dj_beatcloud-2.5.0/LICENSE` & `dj_beatcloud-2.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/PKG-INFO` & `dj_beatcloud-2.5.0b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,169 +1,126 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 5f62  : 2.1.Name: dj_b
 00000020: 6561 7463 6c6f 7564 0a56 6572 7369 6f6e  eatcloud.Version
-00000030: 3a20 322e 352e 300a 5375 6d6d 6172 793a  : 2.5.0.Summary:
-00000040: 2044 4a20 546f 6f6c 7320 6973 2061 206c   DJ Tools is a l
-00000050: 6962 7261 7279 2066 6f72 206d 616e 6167  ibrary for manag
-00000060: 696e 6720 6120 636f 6c6c 6563 7469 6f6e  ing a collection
-00000070: 206f 6620 6d75 7369 6320 616e 6420 5265   of music and Re
-00000080: 6b6f 7264 626f 7820 584d 4c20 6669 6c65  kordbox XML file
-00000090: 732e 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
-000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000b0: 2f61 2d72 6963 682f 444a 2d74 6f6f 6c73  /a-rich/DJ-tools
-000000c0: 0a41 7574 686f 723a 2041 6c65 7820 5269  .Author: Alex Ri
-000000d0: 6368 6172 6473 0a41 7574 686f 722d 656d  chards.Author-em
-000000e0: 6169 6c3a 2061 6c65 782e 7269 6368 6172  ail: alex.richar
-000000f0: 6473 3030 3640 676d 6169 6c2e 636f 6d0a  ds006@gmail.com.
-00000100: 4c69 6365 6e73 653a 2047 4e55 2047 504c  License: GNU GPL
-00000110: 7633 0a4b 6579 776f 7264 733a 204d 5033  v3.Keywords: MP3
-00000120: 2052 656b 6f72 6462 6f78 2058 4d4c 2073   Rekordbox XML s
-00000130: 706f 7469 6679 2072 6564 6469 7420 6177  potify reddit aw
-00000140: 7320 7333 0a43 6c61 7373 6966 6965 723a  s s3.Classifier:
-00000150: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000160: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
-00000170: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-00000180: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000190: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-000001a0: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-000001b0: 2041 7564 6965 6e63 6520 3a3a 2045 6e64   Audience :: End
-000001c0: 2055 7365 7273 2f44 6573 6b74 6f70 0a43   Users/Desktop.C
-000001d0: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-000001e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000001f0: 4f74 6865 7220 4175 6469 656e 6365 0a43  Other Audience.C
-00000200: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000210: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000220: 6564 203a 3a20 474e 5520 4765 6e65 7261  ed :: GNU Genera
-00000230: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
-00000240: 2076 3320 2847 504c 7633 290a 436c 6173   v3 (GPLv3).Clas
-00000250: 7369 6669 6572 3a20 4e61 7475 7261 6c20  sifier: Natural 
-00000260: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
-00000270: 6973 680a 436c 6173 7369 6669 6572 3a20  ish.Classifier: 
-00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000290: 203a 3a20 4d61 634f 5320 3a3a 204d 6163   :: MacOS :: Mac
-000002a0: 4f53 2058 0a43 6c61 7373 6966 6965 723a  OS X.Classifier:
-000002b0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002c0: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
-000002d0: 3a20 5769 6e64 6f77 730a 436c 6173 7369  : Windows.Classi
-000002e0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-000002f0: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
-00000300: 3a3a 204c 696e 7578 0a43 6c61 7373 6966  :: Linux.Classif
-00000310: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000320: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000330: 686f 6e20 3a3a 2033 2e36 0a43 6c61 7373  hon :: 3.6.Class
-00000340: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000360: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
-00000370: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000380: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000390: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
-000003a0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000003b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000003c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000003d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000003e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000003f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000400: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
-00000410: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000420: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000430: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
-00000440: 723a 2054 6f70 6963 203a 3a20 4d75 6c74  r: Topic :: Mult
-00000450: 696d 6564 6961 203a 3a20 536f 756e 642f  imedia :: Sound/
-00000460: 4175 6469 6f0a 436c 6173 7369 6669 6572  Audio.Classifier
-00000470: 3a20 546f 7069 6320 3a3a 204f 7468 6572  : Topic :: Other
-00000480: 2f4e 6f6e 6c69 7374 6564 2054 6f70 6963  /Nonlisted Topic
-00000490: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000004a0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
-000004b0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000004c0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000004d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000004e0: 6c65 7665 6e73 6874 6569 6e0a 4c69 6365  levenshtein.Lice
-000004f0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-00000500: 450a 0a23 2044 4a20 546f 6f6c 730a 5b21  E..# DJ Tools.[!
-00000510: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
-00000520: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000530: 7970 692f 762f 646a 2d62 6561 7463 6c6f  ypi/v/dj-beatclo
-00000540: 7564 2e73 7667 295d 2868 7474 7073 3a2f  ud.svg)](https:/
-00000550: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000560: 742f 646a 2d62 6561 7463 6c6f 7564 2f29  t/dj-beatcloud/)
-00000570: 0a0a 506c 6561 7365 2073 6565 2074 6865  ..Please see the
-00000580: 205b 646f 6373 5d28 6874 7470 733a 2f2f   [docs](https://
-00000590: 612d 7269 6368 2e67 6974 6875 622e 696f  a-rich.github.io
-000005a0: 2f44 4a2d 546f 6f6c 732f 2920 666f 7220  /DJ-Tools/) for 
-000005b0: 7475 746f 7269 616c 732c 2068 6f77 2d74  tutorials, how-t
-000005c0: 6f20 6775 6964 6573 2c20 636f 6e63 6570  o guides, concep
-000005d0: 7475 616c 2067 7569 6465 732c 2061 6e64  tual guides, and
-000005e0: 2072 6566 6572 656e 6365 7321 0a0a 2320   references!..# 
-000005f0: 5265 6c65 6173 6520 506c 616e 0a2a 2032  Release Plan.* 2
-00000600: 2e35 2e31 0a20 2020 202d 205b 205d 205b  .5.1.    - [ ] [
-00000610: 5374 6162 696c 6974 7920 6973 7375 6573  Stability issues
-00000620: 2077 6974 6820 7265 7175 6573 7473 2074   with requests t
-00000630: 6f20 7468 6520 7365 6172 6368 2065 6e64  o the search end
-00000640: 706f 696e 7420 6f66 2074 6865 2053 706f  point of the Spo
-00000650: 7469 6679 2041 5049 5d28 6874 7470 733a  tify API](https:
-00000660: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
-00000670: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
-00000680: 7565 732f 3538 290a 2020 2020 2d20 5b20  ues/58).    - [ 
-00000690: 5d20 5b4d 616b 6520 5370 6f74 6966 7920  ] [Make Spotify 
-000006a0: 4150 4920 6361 6c6c 7320 6173 796e 6368  API calls asynch
-000006b0: 726f 6e6f 7573 5d28 6874 7470 733a 2f2f  ronous](https://
-000006c0: 6769 7468 7562 2e63 6f6d 2f61 2d72 6963  github.com/a-ric
-000006d0: 682f 444a 2d54 6f6f 6c73 2f69 7373 7565  h/DJ-Tools/issue
-000006e0: 732f 3338 290a 2020 2020 2d20 5b20 5d20  s/38).    - [ ] 
-000006f0: 5b44 6570 7265 6361 7465 2072 6567 6973  [Deprecate regis
-00000700: 7465 7265 645f 7573 6572 732e 7961 6d6c  tered_users.yaml
-00000710: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000720: 2e63 6f6d 2f61 2d72 6963 682f 444a 2d54  .com/a-rich/DJ-T
-00000730: 6f6f 6c73 2f69 7373 7565 732f 3939 290a  ools/issues/99).
-00000740: 2a20 322e 362e 300a 2020 2020 2d20 5b20  * 2.6.0.    - [ 
-00000750: 5d20 5b43 7265 6174 6520 7365 7269 616c  ] [Create serial
-00000760: 697a 6572 7320 7061 636b 6167 6520 666f  izers package fo
-00000770: 7220 636f 6e76 6572 7469 6e67 2064 6174  r converting dat
-00000780: 6162 6173 6520 6669 6c65 7320 6672 6f6d  abase files from
-00000790: 206f 7468 6572 2044 4a20 736f 6674 7761   other DJ softwa
-000007a0: 7265 2028 652e 672e 2053 6572 6174 6f2c  re (e.g. Serato,
-000007b0: 2054 7261 6b74 6f72 2c20 4465 6e6f 6e2c   Traktor, Denon,
-000007c0: 2065 7463 2e29 2073 6f20 7468 6174 206f   etc.) so that o
-000007d0: 7065 7261 7469 6f6e 7320 696e 2074 6865  perations in the
-000007e0: 2072 656b 6f72 6462 6f78 2070 6163 6b61   rekordbox packa
-000007f0: 6765 2063 616e 2062 6520 7573 6564 206f  ge can be used o
-00000800: 6e20 7468 656d 5d28 6874 7470 733a 2f2f  n them](https://
-00000810: 6769 7468 7562 2e63 6f6d 2f61 2d72 6963  github.com/a-ric
-00000820: 682f 444a 2d54 6f6f 6c73 2f69 7373 7565  h/DJ-Tools/issue
-00000830: 732f 3638 290a 2020 2020 2d20 5b20 5d20  s/68).    - [ ] 
-00000840: 5b49 6d70 726f 7665 2052 6564 6469 7420  [Improve Reddit 
-00000850: 7375 626d 6973 7369 6f6e 2074 6974 6c65  submission title
-00000860: 2070 6172 7369 6e67 2069 6e20 6f72 6465   parsing in orde
-00000870: 7220 746f 2069 6d70 726f 7665 2070 7265  r to improve pre
-00000880: 6369 7369 6f6e 2061 6e64 2072 6563 616c  cision and recal
-00000890: 6c20 6f66 2053 706f 7469 6679 2041 5049  l of Spotify API
-000008a0: 2073 6561 7263 6820 7265 7375 6c74 735d   search results]
-000008b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000008c0: 636f 6d2f 612d 7269 6368 2f44 4a2d 546f  com/a-rich/DJ-To
-000008d0: 6f6c 732f 6973 7375 6573 2f35 3929 0a20  ols/issues/59). 
-000008e0: 2020 202d 205b 205d 205b 5072 696e 7420     - [ ] [Print 
-000008f0: 4153 4349 4920 6869 7374 6f67 7261 6d20  ASCII histogram 
-00000900: 6f66 2074 6167 2073 7461 7469 7374 6963  of tag statistic
-00000910: 7320 666f 7220 436f 6d62 696e 6572 2070  s for Combiner p
-00000920: 6c61 796c 6973 7473 5d28 6874 7470 733a  laylists](https:
-00000930: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
-00000940: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
-00000950: 7565 732f 3837 290a 2020 2020 2d20 5b20  ues/87).    - [ 
-00000960: 5d20 5b50 6172 616d 6574 6572 697a 6520  ] [Parameterize 
-00000970: 6d75 7369 6320 666f 6c64 6572 2072 6f6f  music folder roo
-00000980: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000990: 622e 636f 6d2f 612d 7269 6368 2f44 4a2d  b.com/a-rich/DJ-
-000009a0: 546f 6f6c 732f 6973 7375 6573 2f39 3429  Tools/issues/94)
-000009b0: 0a20 2020 202d 205b 205d 205b 5061 7261  .    - [ ] [Para
-000009c0: 6d65 7465 7269 7a65 2077 6865 7468 6572  meterize whether
-000009d0: 2042 6561 7463 6c6f 7564 2074 7261 636b   Beatcloud track
-000009e0: 7320 7368 6f75 6c64 2062 6520 7265 6164  s should be read
-000009f0: 2061 7320 3c74 6974 6c65 3e20 2d20 3c61   as <title> - <a
-00000a00: 7274 6973 743e 206f 7220 7669 6365 2076  rtist> or vice v
-00000a10: 6572 7361 5d28 6874 7470 733a 2f2f 6769  ersa](https://gi
-00000a20: 7468 7562 2e63 6f6d 2f61 2d72 6963 682f  thub.com/a-rich/
-00000a30: 444a 2d54 6f6f 6c73 2f69 7373 7565 732f  DJ-Tools/issues/
-00000a40: 3935 290a 0a23 2043 6f6e 7472 6962 7574  95)..# Contribut
-00000a50: 696f 6e0a 506c 6561 7365 2073 6565 2074  ion.Please see t
-00000a60: 6865 205b 434f 4e54 5249 4255 5449 4e47  he [CONTRIBUTING
-00000a70: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
-00000a80: 6429 0a                                  d).
+00000030: 3a20 322e 352e 3062 300a 5375 6d6d 6172  : 2.5.0b0.Summar
+00000040: 793a 2044 4a20 546f 6f6c 7320 6973 2061  y: DJ Tools is a
+00000050: 206c 6962 7261 7279 2066 6f72 206d 616e   library for man
+00000060: 6167 696e 6720 6120 636f 6c6c 6563 7469  aging a collecti
+00000070: 6f6e 206f 6620 6d75 7369 6320 616e 6420  on of music and 
+00000080: 5265 6b6f 7264 626f 7820 584d 4c20 6669  Rekordbox XML fi
+00000090: 6c65 732e 0a48 6f6d 652d 7061 6765 3a20  les..Home-page: 
+000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000b0: 6f6d 2f61 2d72 6963 682f 444a 2d74 6f6f  om/a-rich/DJ-too
+000000c0: 6c73 0a41 7574 686f 723a 2041 6c65 7820  ls.Author: Alex 
+000000d0: 5269 6368 6172 6473 0a41 7574 686f 722d  Richards.Author-
+000000e0: 656d 6169 6c3a 2061 6c65 782e 7269 6368  email: alex.rich
+000000f0: 6172 6473 3030 3640 676d 6169 6c2e 636f  ards006@gmail.co
+00000100: 6d0a 4c69 6365 6e73 653a 2047 4e55 2047  m.License: GNU G
+00000110: 504c 7633 0a4b 6579 776f 7264 733a 204d  PLv3.Keywords: M
+00000120: 5033 2052 656b 6f72 6462 6f78 2058 4d4c  P3 Rekordbox XML
+00000130: 2073 706f 7469 6679 2072 6564 6469 7420   spotify reddit 
+00000140: 6177 7320 7333 0a43 6c61 7373 6966 6965  aws s3.Classifie
+00000150: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000160: 7461 7475 7320 3a3a 2034 202d 2042 6574  tatus :: 4 - Bet
+00000170: 610a 436c 6173 7369 6669 6572 3a20 496e  a.Classifier: In
+00000180: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000190: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+000001a0: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+000001b0: 6564 2041 7564 6965 6e63 6520 3a3a 2045  ed Audience :: E
+000001c0: 6e64 2055 7365 7273 2f44 6573 6b74 6f70  nd Users/Desktop
+000001d0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001f0: 3a20 4f74 6865 7220 4175 6469 656e 6365  : Other Audience
+00000200: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000210: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000220: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000230: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000240: 7365 2076 3320 2847 504c 7633 290a 436c  se v3 (GPLv3).Cl
+00000250: 6173 7369 6669 6572 3a20 4e61 7475 7261  assifier: Natura
+00000260: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
+00000270: 676c 6973 680a 436c 6173 7369 6669 6572  glish.Classifier
+00000280: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000290: 656d 203a 3a20 4d61 634f 5320 3a3a 204d  em :: MacOS :: M
+000002a0: 6163 4f53 2058 0a43 6c61 7373 6966 6965  acOS X.Classifie
+000002b0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002c0: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+000002d0: 203a 3a20 5769 6e64 6f77 730a 436c 6173   :: Windows.Clas
+000002e0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+000002f0: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
+00000300: 5820 3a3a 204c 696e 7578 0a43 6c61 7373  X :: Linux.Class
+00000310: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000320: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000330: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
+00000340: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00000370: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000380: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000390: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000003a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000003b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000003c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000003d0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+000003e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000400: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00000410: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000420: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000430: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00000440: 6965 723a 2054 6f70 6963 203a 3a20 4d75  ier: Topic :: Mu
+00000450: 6c74 696d 6564 6961 203a 3a20 536f 756e  ltimedia :: Soun
+00000460: 642f 4175 6469 6f0a 436c 6173 7369 6669  d/Audio.Classifi
+00000470: 6572 3a20 546f 7069 6320 3a3a 204f 7468  er: Topic :: Oth
+00000480: 6572 2f4e 6f6e 6c69 7374 6564 2054 6f70  er/Nonlisted Top
+00000490: 6963 0a52 6571 7569 7265 732d 5079 7468  ic.Requires-Pyth
+000004a0: 6f6e 3a20 3e3d 332e 360a 4465 7363 7269  on: >=3.6.Descri
+000004b0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+000004c0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+000004d0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
+000004e0: 3a20 6c65 7665 6e73 6874 6569 6e0a 4c69  : levenshtein.Li
+000004f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000500: 4e53 450a 0a23 2044 4a20 546f 6f6c 730a  NSE..# DJ Tools.
+00000510: 5b21 5b69 6d61 6765 5d28 6874 7470 733a  [![image](https:
+00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000530: 2f70 7970 692f 762f 646a 2d62 6561 7463  /pypi/v/dj-beatc
+00000540: 6c6f 7564 2e73 7667 295d 2868 7474 7073  loud.svg)](https
+00000550: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000560: 6563 742f 646a 2d62 6561 7463 6c6f 7564  ect/dj-beatcloud
+00000570: 2f29 0a0a 506c 6561 7365 2073 6565 2074  /)..Please see t
+00000580: 6865 205b 646f 6373 5d28 646f 6373 2f69  he [docs](docs/i
+00000590: 6e64 6578 2e6d 6429 2066 6f72 2074 7574  ndex.md) for tut
+000005a0: 6f72 6961 6c73 2c20 686f 772d 746f 2067  orials, how-to g
+000005b0: 7569 6465 732c 2063 6f6e 6365 7074 7561  uides, conceptua
+000005c0: 6c20 6775 6964 6573 2c20 616e 6420 7265  l guides, and re
+000005d0: 6665 7265 6e63 6573 210a 0a23 2052 656c  ferences!..# Rel
+000005e0: 6561 7365 2050 6c61 6e0a 2a20 322e 342e  ease Plan.* 2.4.
+000005f0: 310a 2020 2020 2d20 5b20 5d20 4d61 6b65  1.    - [ ] Make
+00000600: 2053 706f 7469 6679 2041 5049 2063 616c   Spotify API cal
+00000610: 6c73 2061 7379 6e63 6872 6f6e 6f75 730a  ls asynchronous.
+00000620: 2020 2020 2d20 5b20 5d20 496d 7072 6f76      - [ ] Improv
+00000630: 6564 2053 706f 7469 6679 2041 5049 2072  ed Spotify API r
+00000640: 6571 7565 7374 2073 7461 6269 6c69 7479  equest stability
+00000650: 200a 2020 2020 2d20 5b20 5d20 496d 7072   .    - [ ] Impr
+00000660: 6f76 6564 2052 6564 6469 7420 706f 7374  oved Reddit post
+00000670: 2070 6172 7369 6e67 2061 6e64 2053 706f   parsing and Spo
+00000680: 7469 6679 2073 6561 7263 6869 6e67 0a20  tify searching. 
+00000690: 2020 202d 205b 205d 204f 7074 696d 697a     - [ ] Optimiz
+000006a0: 6520 7079 7465 7374 2d63 6f76 2077 6f72  e pytest-cov wor
+000006b0: 6b66 6c6f 7720 616e 6420 6164 6420 5769  kflow and add Wi
+000006c0: 6e64 6f77 7320 7275 6e6e 6572 0a2a 2032  ndows runner.* 2
+000006d0: 2e35 2e30 0a20 2020 202d 205b 205d 2043  .5.0.    - [ ] C
+000006e0: 7265 6174 6520 7365 7269 616c 697a 6572  reate serializer
+000006f0: 7320 7061 636b 6167 6520 666f 7220 636f  s package for co
+00000700: 6e76 6572 7469 6e67 2064 6174 6162 6173  nverting databas
+00000710: 6520 6669 6c65 7320 6672 6f6d 206f 7468  e files from oth
+00000720: 6572 2044 4a20 736f 6674 7761 7265 2028  er DJ software (
+00000730: 652e 672e 2053 6572 6174 6f2c 2054 7261  e.g. Serato, Tra
+00000740: 6b74 6f72 2c20 4465 6e6f 6e2c 2065 7463  ktor, Denon, etc
+00000750: 2e29 2073 6f20 7468 6174 206f 7065 7261  .) so that opera
+00000760: 7469 6f6e 7320 696e 2074 6865 2072 656b  tions in the rek
+00000770: 6f72 6462 6f78 2070 6163 6b61 6765 2063  ordbox package c
+00000780: 616e 2062 6520 7573 6564 206f 6e20 7468  an be used on th
+00000790: 656d 0a0a 2320 436f 6e74 7269 6275 7469  em..# Contributi
+000007a0: 6f6e 0a50 6c65 6173 6520 7365 6520 7468  on.Please see th
+000007b0: 6520 5b43 4f4e 5452 4942 5554 494e 475d  e [CONTRIBUTING]
+000007c0: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
+000007d0: 290a                                     ).
```

### Comparing `dj_beatcloud-2.5.0/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,169 +1,126 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 2d62  : 2.1.Name: dj-b
 00000020: 6561 7463 6c6f 7564 0a56 6572 7369 6f6e  eatcloud.Version
-00000030: 3a20 322e 352e 300a 5375 6d6d 6172 793a  : 2.5.0.Summary:
-00000040: 2044 4a20 546f 6f6c 7320 6973 2061 206c   DJ Tools is a l
-00000050: 6962 7261 7279 2066 6f72 206d 616e 6167  ibrary for manag
-00000060: 696e 6720 6120 636f 6c6c 6563 7469 6f6e  ing a collection
-00000070: 206f 6620 6d75 7369 6320 616e 6420 5265   of music and Re
-00000080: 6b6f 7264 626f 7820 584d 4c20 6669 6c65  kordbox XML file
-00000090: 732e 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
-000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000b0: 2f61 2d72 6963 682f 444a 2d74 6f6f 6c73  /a-rich/DJ-tools
-000000c0: 0a41 7574 686f 723a 2041 6c65 7820 5269  .Author: Alex Ri
-000000d0: 6368 6172 6473 0a41 7574 686f 722d 656d  chards.Author-em
-000000e0: 6169 6c3a 2061 6c65 782e 7269 6368 6172  ail: alex.richar
-000000f0: 6473 3030 3640 676d 6169 6c2e 636f 6d0a  ds006@gmail.com.
-00000100: 4c69 6365 6e73 653a 2047 4e55 2047 504c  License: GNU GPL
-00000110: 7633 0a4b 6579 776f 7264 733a 204d 5033  v3.Keywords: MP3
-00000120: 2052 656b 6f72 6462 6f78 2058 4d4c 2073   Rekordbox XML s
-00000130: 706f 7469 6679 2072 6564 6469 7420 6177  potify reddit aw
-00000140: 7320 7333 0a43 6c61 7373 6966 6965 723a  s s3.Classifier:
-00000150: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000160: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
-00000170: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-00000180: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000190: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-000001a0: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-000001b0: 2041 7564 6965 6e63 6520 3a3a 2045 6e64   Audience :: End
-000001c0: 2055 7365 7273 2f44 6573 6b74 6f70 0a43   Users/Desktop.C
-000001d0: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-000001e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000001f0: 4f74 6865 7220 4175 6469 656e 6365 0a43  Other Audience.C
-00000200: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000210: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000220: 6564 203a 3a20 474e 5520 4765 6e65 7261  ed :: GNU Genera
-00000230: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
-00000240: 2076 3320 2847 504c 7633 290a 436c 6173   v3 (GPLv3).Clas
-00000250: 7369 6669 6572 3a20 4e61 7475 7261 6c20  sifier: Natural 
-00000260: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
-00000270: 6973 680a 436c 6173 7369 6669 6572 3a20  ish.Classifier: 
-00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000290: 203a 3a20 4d61 634f 5320 3a3a 204d 6163   :: MacOS :: Mac
-000002a0: 4f53 2058 0a43 6c61 7373 6966 6965 723a  OS X.Classifier:
-000002b0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002c0: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
-000002d0: 3a20 5769 6e64 6f77 730a 436c 6173 7369  : Windows.Classi
-000002e0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-000002f0: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
-00000300: 3a3a 204c 696e 7578 0a43 6c61 7373 6966  :: Linux.Classif
-00000310: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000320: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000330: 686f 6e20 3a3a 2033 2e36 0a43 6c61 7373  hon :: 3.6.Class
-00000340: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000360: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
-00000370: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000380: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000390: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
-000003a0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000003b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000003c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000003d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000003e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000003f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000400: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
-00000410: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000420: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000430: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
-00000440: 723a 2054 6f70 6963 203a 3a20 4d75 6c74  r: Topic :: Mult
-00000450: 696d 6564 6961 203a 3a20 536f 756e 642f  imedia :: Sound/
-00000460: 4175 6469 6f0a 436c 6173 7369 6669 6572  Audio.Classifier
-00000470: 3a20 546f 7069 6320 3a3a 204f 7468 6572  : Topic :: Other
-00000480: 2f4e 6f6e 6c69 7374 6564 2054 6f70 6963  /Nonlisted Topic
-00000490: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000004a0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
-000004b0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000004c0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000004d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000004e0: 6c65 7665 6e73 6874 6569 6e0a 4c69 6365  levenshtein.Lice
-000004f0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-00000500: 450a 0a23 2044 4a20 546f 6f6c 730a 5b21  E..# DJ Tools.[!
-00000510: 5b69 6d61 6765 5d28 6874 7470 733a 2f2f  [image](https://
-00000520: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000530: 7970 692f 762f 646a 2d62 6561 7463 6c6f  ypi/v/dj-beatclo
-00000540: 7564 2e73 7667 295d 2868 7474 7073 3a2f  ud.svg)](https:/
-00000550: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000560: 742f 646a 2d62 6561 7463 6c6f 7564 2f29  t/dj-beatcloud/)
-00000570: 0a0a 506c 6561 7365 2073 6565 2074 6865  ..Please see the
-00000580: 205b 646f 6373 5d28 6874 7470 733a 2f2f   [docs](https://
-00000590: 612d 7269 6368 2e67 6974 6875 622e 696f  a-rich.github.io
-000005a0: 2f44 4a2d 546f 6f6c 732f 2920 666f 7220  /DJ-Tools/) for 
-000005b0: 7475 746f 7269 616c 732c 2068 6f77 2d74  tutorials, how-t
-000005c0: 6f20 6775 6964 6573 2c20 636f 6e63 6570  o guides, concep
-000005d0: 7475 616c 2067 7569 6465 732c 2061 6e64  tual guides, and
-000005e0: 2072 6566 6572 656e 6365 7321 0a0a 2320   references!..# 
-000005f0: 5265 6c65 6173 6520 506c 616e 0a2a 2032  Release Plan.* 2
-00000600: 2e35 2e31 0a20 2020 202d 205b 205d 205b  .5.1.    - [ ] [
-00000610: 5374 6162 696c 6974 7920 6973 7375 6573  Stability issues
-00000620: 2077 6974 6820 7265 7175 6573 7473 2074   with requests t
-00000630: 6f20 7468 6520 7365 6172 6368 2065 6e64  o the search end
-00000640: 706f 696e 7420 6f66 2074 6865 2053 706f  point of the Spo
-00000650: 7469 6679 2041 5049 5d28 6874 7470 733a  tify API](https:
-00000660: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
-00000670: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
-00000680: 7565 732f 3538 290a 2020 2020 2d20 5b20  ues/58).    - [ 
-00000690: 5d20 5b4d 616b 6520 5370 6f74 6966 7920  ] [Make Spotify 
-000006a0: 4150 4920 6361 6c6c 7320 6173 796e 6368  API calls asynch
-000006b0: 726f 6e6f 7573 5d28 6874 7470 733a 2f2f  ronous](https://
-000006c0: 6769 7468 7562 2e63 6f6d 2f61 2d72 6963  github.com/a-ric
-000006d0: 682f 444a 2d54 6f6f 6c73 2f69 7373 7565  h/DJ-Tools/issue
-000006e0: 732f 3338 290a 2020 2020 2d20 5b20 5d20  s/38).    - [ ] 
-000006f0: 5b44 6570 7265 6361 7465 2072 6567 6973  [Deprecate regis
-00000700: 7465 7265 645f 7573 6572 732e 7961 6d6c  tered_users.yaml
-00000710: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000720: 2e63 6f6d 2f61 2d72 6963 682f 444a 2d54  .com/a-rich/DJ-T
-00000730: 6f6f 6c73 2f69 7373 7565 732f 3939 290a  ools/issues/99).
-00000740: 2a20 322e 362e 300a 2020 2020 2d20 5b20  * 2.6.0.    - [ 
-00000750: 5d20 5b43 7265 6174 6520 7365 7269 616c  ] [Create serial
-00000760: 697a 6572 7320 7061 636b 6167 6520 666f  izers package fo
-00000770: 7220 636f 6e76 6572 7469 6e67 2064 6174  r converting dat
-00000780: 6162 6173 6520 6669 6c65 7320 6672 6f6d  abase files from
-00000790: 206f 7468 6572 2044 4a20 736f 6674 7761   other DJ softwa
-000007a0: 7265 2028 652e 672e 2053 6572 6174 6f2c  re (e.g. Serato,
-000007b0: 2054 7261 6b74 6f72 2c20 4465 6e6f 6e2c   Traktor, Denon,
-000007c0: 2065 7463 2e29 2073 6f20 7468 6174 206f   etc.) so that o
-000007d0: 7065 7261 7469 6f6e 7320 696e 2074 6865  perations in the
-000007e0: 2072 656b 6f72 6462 6f78 2070 6163 6b61   rekordbox packa
-000007f0: 6765 2063 616e 2062 6520 7573 6564 206f  ge can be used o
-00000800: 6e20 7468 656d 5d28 6874 7470 733a 2f2f  n them](https://
-00000810: 6769 7468 7562 2e63 6f6d 2f61 2d72 6963  github.com/a-ric
-00000820: 682f 444a 2d54 6f6f 6c73 2f69 7373 7565  h/DJ-Tools/issue
-00000830: 732f 3638 290a 2020 2020 2d20 5b20 5d20  s/68).    - [ ] 
-00000840: 5b49 6d70 726f 7665 2052 6564 6469 7420  [Improve Reddit 
-00000850: 7375 626d 6973 7369 6f6e 2074 6974 6c65  submission title
-00000860: 2070 6172 7369 6e67 2069 6e20 6f72 6465   parsing in orde
-00000870: 7220 746f 2069 6d70 726f 7665 2070 7265  r to improve pre
-00000880: 6369 7369 6f6e 2061 6e64 2072 6563 616c  cision and recal
-00000890: 6c20 6f66 2053 706f 7469 6679 2041 5049  l of Spotify API
-000008a0: 2073 6561 7263 6820 7265 7375 6c74 735d   search results]
-000008b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000008c0: 636f 6d2f 612d 7269 6368 2f44 4a2d 546f  com/a-rich/DJ-To
-000008d0: 6f6c 732f 6973 7375 6573 2f35 3929 0a20  ols/issues/59). 
-000008e0: 2020 202d 205b 205d 205b 5072 696e 7420     - [ ] [Print 
-000008f0: 4153 4349 4920 6869 7374 6f67 7261 6d20  ASCII histogram 
-00000900: 6f66 2074 6167 2073 7461 7469 7374 6963  of tag statistic
-00000910: 7320 666f 7220 436f 6d62 696e 6572 2070  s for Combiner p
-00000920: 6c61 796c 6973 7473 5d28 6874 7470 733a  laylists](https:
-00000930: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
-00000940: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
-00000950: 7565 732f 3837 290a 2020 2020 2d20 5b20  ues/87).    - [ 
-00000960: 5d20 5b50 6172 616d 6574 6572 697a 6520  ] [Parameterize 
-00000970: 6d75 7369 6320 666f 6c64 6572 2072 6f6f  music folder roo
-00000980: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000990: 622e 636f 6d2f 612d 7269 6368 2f44 4a2d  b.com/a-rich/DJ-
-000009a0: 546f 6f6c 732f 6973 7375 6573 2f39 3429  Tools/issues/94)
-000009b0: 0a20 2020 202d 205b 205d 205b 5061 7261  .    - [ ] [Para
-000009c0: 6d65 7465 7269 7a65 2077 6865 7468 6572  meterize whether
-000009d0: 2042 6561 7463 6c6f 7564 2074 7261 636b   Beatcloud track
-000009e0: 7320 7368 6f75 6c64 2062 6520 7265 6164  s should be read
-000009f0: 2061 7320 3c74 6974 6c65 3e20 2d20 3c61   as <title> - <a
-00000a00: 7274 6973 743e 206f 7220 7669 6365 2076  rtist> or vice v
-00000a10: 6572 7361 5d28 6874 7470 733a 2f2f 6769  ersa](https://gi
-00000a20: 7468 7562 2e63 6f6d 2f61 2d72 6963 682f  thub.com/a-rich/
-00000a30: 444a 2d54 6f6f 6c73 2f69 7373 7565 732f  DJ-Tools/issues/
-00000a40: 3935 290a 0a23 2043 6f6e 7472 6962 7574  95)..# Contribut
-00000a50: 696f 6e0a 506c 6561 7365 2073 6565 2074  ion.Please see t
-00000a60: 6865 205b 434f 4e54 5249 4255 5449 4e47  he [CONTRIBUTING
-00000a70: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
-00000a80: 6429 0a                                  d).
+00000030: 3a20 322e 352e 3062 300a 5375 6d6d 6172  : 2.5.0b0.Summar
+00000040: 793a 2044 4a20 546f 6f6c 7320 6973 2061  y: DJ Tools is a
+00000050: 206c 6962 7261 7279 2066 6f72 206d 616e   library for man
+00000060: 6167 696e 6720 6120 636f 6c6c 6563 7469  aging a collecti
+00000070: 6f6e 206f 6620 6d75 7369 6320 616e 6420  on of music and 
+00000080: 5265 6b6f 7264 626f 7820 584d 4c20 6669  Rekordbox XML fi
+00000090: 6c65 732e 0a48 6f6d 652d 7061 6765 3a20  les..Home-page: 
+000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000b0: 6f6d 2f61 2d72 6963 682f 444a 2d74 6f6f  om/a-rich/DJ-too
+000000c0: 6c73 0a41 7574 686f 723a 2041 6c65 7820  ls.Author: Alex 
+000000d0: 5269 6368 6172 6473 0a41 7574 686f 722d  Richards.Author-
+000000e0: 656d 6169 6c3a 2061 6c65 782e 7269 6368  email: alex.rich
+000000f0: 6172 6473 3030 3640 676d 6169 6c2e 636f  ards006@gmail.co
+00000100: 6d0a 4c69 6365 6e73 653a 2047 4e55 2047  m.License: GNU G
+00000110: 504c 7633 0a4b 6579 776f 7264 733a 204d  PLv3.Keywords: M
+00000120: 5033 2052 656b 6f72 6462 6f78 2058 4d4c  P3 Rekordbox XML
+00000130: 2073 706f 7469 6679 2072 6564 6469 7420   spotify reddit 
+00000140: 6177 7320 7333 0a43 6c61 7373 6966 6965  aws s3.Classifie
+00000150: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000160: 7461 7475 7320 3a3a 2034 202d 2042 6574  tatus :: 4 - Bet
+00000170: 610a 436c 6173 7369 6669 6572 3a20 496e  a.Classifier: In
+00000180: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000190: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+000001a0: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+000001b0: 6564 2041 7564 6965 6e63 6520 3a3a 2045  ed Audience :: E
+000001c0: 6e64 2055 7365 7273 2f44 6573 6b74 6f70  nd Users/Desktop
+000001d0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001f0: 3a20 4f74 6865 7220 4175 6469 656e 6365  : Other Audience
+00000200: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000210: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000220: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000230: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000240: 7365 2076 3320 2847 504c 7633 290a 436c  se v3 (GPLv3).Cl
+00000250: 6173 7369 6669 6572 3a20 4e61 7475 7261  assifier: Natura
+00000260: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
+00000270: 676c 6973 680a 436c 6173 7369 6669 6572  glish.Classifier
+00000280: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000290: 656d 203a 3a20 4d61 634f 5320 3a3a 204d  em :: MacOS :: M
+000002a0: 6163 4f53 2058 0a43 6c61 7373 6966 6965  acOS X.Classifie
+000002b0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002c0: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+000002d0: 203a 3a20 5769 6e64 6f77 730a 436c 6173   :: Windows.Clas
+000002e0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+000002f0: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
+00000300: 5820 3a3a 204c 696e 7578 0a43 6c61 7373  X :: Linux.Class
+00000310: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000320: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000330: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
+00000340: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00000370: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000380: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000390: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000003a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000003b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000003c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000003d0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+000003e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000400: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00000410: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000420: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000430: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00000440: 6965 723a 2054 6f70 6963 203a 3a20 4d75  ier: Topic :: Mu
+00000450: 6c74 696d 6564 6961 203a 3a20 536f 756e  ltimedia :: Soun
+00000460: 642f 4175 6469 6f0a 436c 6173 7369 6669  d/Audio.Classifi
+00000470: 6572 3a20 546f 7069 6320 3a3a 204f 7468  er: Topic :: Oth
+00000480: 6572 2f4e 6f6e 6c69 7374 6564 2054 6f70  er/Nonlisted Top
+00000490: 6963 0a52 6571 7569 7265 732d 5079 7468  ic.Requires-Pyth
+000004a0: 6f6e 3a20 3e3d 332e 360a 4465 7363 7269  on: >=3.6.Descri
+000004b0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+000004c0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+000004d0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
+000004e0: 3a20 6c65 7665 6e73 6874 6569 6e0a 4c69  : levenshtein.Li
+000004f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000500: 4e53 450a 0a23 2044 4a20 546f 6f6c 730a  NSE..# DJ Tools.
+00000510: 5b21 5b69 6d61 6765 5d28 6874 7470 733a  [![image](https:
+00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000530: 2f70 7970 692f 762f 646a 2d62 6561 7463  /pypi/v/dj-beatc
+00000540: 6c6f 7564 2e73 7667 295d 2868 7474 7073  loud.svg)](https
+00000550: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000560: 6563 742f 646a 2d62 6561 7463 6c6f 7564  ect/dj-beatcloud
+00000570: 2f29 0a0a 506c 6561 7365 2073 6565 2074  /)..Please see t
+00000580: 6865 205b 646f 6373 5d28 646f 6373 2f69  he [docs](docs/i
+00000590: 6e64 6578 2e6d 6429 2066 6f72 2074 7574  ndex.md) for tut
+000005a0: 6f72 6961 6c73 2c20 686f 772d 746f 2067  orials, how-to g
+000005b0: 7569 6465 732c 2063 6f6e 6365 7074 7561  uides, conceptua
+000005c0: 6c20 6775 6964 6573 2c20 616e 6420 7265  l guides, and re
+000005d0: 6665 7265 6e63 6573 210a 0a23 2052 656c  ferences!..# Rel
+000005e0: 6561 7365 2050 6c61 6e0a 2a20 322e 342e  ease Plan.* 2.4.
+000005f0: 310a 2020 2020 2d20 5b20 5d20 4d61 6b65  1.    - [ ] Make
+00000600: 2053 706f 7469 6679 2041 5049 2063 616c   Spotify API cal
+00000610: 6c73 2061 7379 6e63 6872 6f6e 6f75 730a  ls asynchronous.
+00000620: 2020 2020 2d20 5b20 5d20 496d 7072 6f76      - [ ] Improv
+00000630: 6564 2053 706f 7469 6679 2041 5049 2072  ed Spotify API r
+00000640: 6571 7565 7374 2073 7461 6269 6c69 7479  equest stability
+00000650: 200a 2020 2020 2d20 5b20 5d20 496d 7072   .    - [ ] Impr
+00000660: 6f76 6564 2052 6564 6469 7420 706f 7374  oved Reddit post
+00000670: 2070 6172 7369 6e67 2061 6e64 2053 706f   parsing and Spo
+00000680: 7469 6679 2073 6561 7263 6869 6e67 0a20  tify searching. 
+00000690: 2020 202d 205b 205d 204f 7074 696d 697a     - [ ] Optimiz
+000006a0: 6520 7079 7465 7374 2d63 6f76 2077 6f72  e pytest-cov wor
+000006b0: 6b66 6c6f 7720 616e 6420 6164 6420 5769  kflow and add Wi
+000006c0: 6e64 6f77 7320 7275 6e6e 6572 0a2a 2032  ndows runner.* 2
+000006d0: 2e35 2e30 0a20 2020 202d 205b 205d 2043  .5.0.    - [ ] C
+000006e0: 7265 6174 6520 7365 7269 616c 697a 6572  reate serializer
+000006f0: 7320 7061 636b 6167 6520 666f 7220 636f  s package for co
+00000700: 6e76 6572 7469 6e67 2064 6174 6162 6173  nverting databas
+00000710: 6520 6669 6c65 7320 6672 6f6d 206f 7468  e files from oth
+00000720: 6572 2044 4a20 736f 6674 7761 7265 2028  er DJ software (
+00000730: 652e 672e 2053 6572 6174 6f2c 2054 7261  e.g. Serato, Tra
+00000740: 6b74 6f72 2c20 4465 6e6f 6e2c 2065 7463  ktor, Denon, etc
+00000750: 2e29 2073 6f20 7468 6174 206f 7065 7261  .) so that opera
+00000760: 7469 6f6e 7320 696e 2074 6865 2072 656b  tions in the rek
+00000770: 6f72 6462 6f78 2070 6163 6b61 6765 2063  ordbox package c
+00000780: 616e 2062 6520 7573 6564 206f 6e20 7468  an be used on th
+00000790: 656d 0a0a 2320 436f 6e74 7269 6275 7469  em..# Contributi
+000007a0: 6f6e 0a50 6c65 6173 6520 7365 6520 7468  on.Please see th
+000007b0: 6520 5b43 4f4e 5452 4942 5554 494e 475d  e [CONTRIBUTING]
+000007c0: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
+000007d0: 290a                                     ).
```

### Comparing `dj_beatcloud-2.5.0/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/__main__.py` & `dj_beatcloud-2.5.0b0/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/config.py` & `dj_beatcloud-2.5.0b0/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/config.yaml` & `dj_beatcloud-2.5.0b0/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/config.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,21 +345,21 @@
     playlist_name: str,
     playlist_ids: Dict[str, str],
     spotify_username: str,
     spotify: spotipy.Spotify,
     tracks: List[Tuple[str]],
     playlist_limit: Optional[int] = sys.maxsize,
     verbosity: Optional[int] = 0,
-) -> Dict[str, str]:
+):
     """Inserts tracks into either a new playlist or an existing one.
 
     Args:
         playlist_name: Name of the playlist.
         playlist_ids: Lookup of playlist IDs.
-        spotify_username: Spotify user's username.
+        spotify_username: Spotify users's username.
         spotify: Spotify client.
         tracks: List of tracks.
         playlist_limit: Maximum number of tracks allowed in a playlist.
         verbosity: Logging verbosity level.
 
     Returns:
         Updated playlist IDs.
```

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/config.py` & `dj_beatcloud-2.5.0b0/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/test_main.py` & `dj_beatcloud-2.5.0b0/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/config.py` & `dj_beatcloud-2.5.0b0/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from itertools import product
 import logging
 import logging.config
 import os
 from pathlib import Path
 from subprocess import check_output
 import tempfile
-from typing import Any, Dict, IO, List, Optional, Set, Tuple
+from typing import Any, Dict, List, Optional, Set, Tuple
 from unittest import mock
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
@@ -38,15 +38,15 @@
     ):
         self._user_a = user_a
         self._user_b = user_b
         self._files = files
         self._content = content
         self._write_only = write_only
 
-    def open(self, *args, **kwargs) -> IO:
+    def open(self, *args, **kwargs):
         """Function to replace the builtin open function.
 
         Returns:
             File handler.
         """
         file_name = os.path.basename(args[0])
         if file_name in self._files:
```

### Comparing `dj_beatcloud-2.5.0/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/djtools/utils/url_download.py` & `dj_beatcloud-2.5.0b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0/setup.py` & `dj_beatcloud-2.5.0b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Setup 'djtools' package.
 """
-from setuptools import setup
+from setuptools import find_packages, setup
 
 
 with open('README.md', encoding='utf-8') as _file:
     LONG_DESCRIPTION = _file.read()
 
 REQUIREMENTS = [
     "asyncpraw==7.6.1",
@@ -44,15 +44,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.5.0',
+    version='2.5.0b0',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

