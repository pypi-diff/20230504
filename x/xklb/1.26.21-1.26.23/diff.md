# Comparing `tmp/xklb-1.26.21.tar.gz` & `tmp/xklb-1.26.23.tar.gz`

## Comparing `xklb-1.26.21.tar` & `xklb-1.26.23.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.21/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.21/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.21/Windows.md
--rw-r--r--   0        0        0   420713 2020-02-02 00:00:00.000000 xklb-1.26.21/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.21/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 xklb-1.26.21/.github/workflows/push.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/books.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/consts.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/dl_config.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/hn_extract.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/lb.py
--rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/playback.py
--rw-r--r--   0        0        0    26772 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/praw_extract.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.21/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.21/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.21/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.21/LICENSE
--rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.21/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.21/pyproject.toml
--rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.21/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.23/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.26.23/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.23/Windows.md
+-rw-r--r--   0        0        0   420713 2020-02-02 00:00:00.000000 xklb-1.26.23/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.23/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.23/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.23/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.23/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 xklb-1.26.23/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.26.23/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/books.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/consts.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/dl_config.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/lb.py
+-rw-r--r--   0        0        0    35723 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/playback.py
+-rw-r--r--   0        0        0    26772 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21844 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.23/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.23/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.23/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.23/LICENSE
+-rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.23/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.26.23/pyproject.toml
+-rw-r--r--   0        0        0    44039 2020-02-02 00:00:00.000000 xklb-1.26.23/PKG-INFO
```

### Comparing `xklb-1.26.21/Windows.md` & `xklb-1.26.23/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/pdm.lock` & `xklb-1.26.23/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/readme.py` & `xklb-1.26.23/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.23/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.23/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/.github/workflows/push.yaml` & `xklb-1.26.23/.github/workflows/push.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   test:
     strategy:
       fail-fast: false
       max-parallel: 8
       matrix:
-        nv: [ {os: windows-latest, py: 3.8}, {os: macos-latest, py: 3.9}, {os: ubuntu-latest, py: "3.11"} ]
+        nv: [ {os: ubuntu-latest, py: 3.8}, {os: macos-latest, py: 3.9}, {os: windows-latest, py: "3.10"}, {os: ubuntu-latest, py: "3.11"} ]
 
     runs-on: ${{ matrix.nv.os }}
     timeout-minutes: 20
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.nv.py }}
```

### Comparing `xklb-1.26.21/xklb/av.py` & `xklb-1.26.23/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/books.py` & `xklb-1.26.23/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/consts.py` & `xklb-1.26.23/xklb/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 
 def now():
     return int(datetime.now(tz=timezone.utc).timestamp())
 
 
 TEMP_DIR = gettempdir()
-FAKE_SUBTITLE = Path(TEMP_DIR) / "sub.srt"  # https://github.com/skorokithakis/catt/issues/393
-CAST_NOW_PLAYING = Path(TEMP_DIR) / "catt_playing"
-DEFAULT_MPV_SOCKET = Path(TEMP_DIR) / "mpv_socket"
+FAKE_SUBTITLE = str(Path(TEMP_DIR) / "sub.srt")  # https://github.com/skorokithakis/catt/issues/393
+CAST_NOW_PLAYING = str(Path(TEMP_DIR) / "catt_playing")
+DEFAULT_MPV_SOCKET = str(Path(TEMP_DIR) / "mpv_socket")
 DEFAULT_MPV_WATCH_LATER = str(Path("~/.config/mpv/watch_later/").expanduser().resolve())
-SUB_TEMP_DIR = Path(TEMP_DIR) / "library_temp_subtitles"
+SUB_TEMP_DIR = str(Path(TEMP_DIR) / "library_temp_subtitles")
 BLOCK_THE_CHANNEL = "__BLOCKLIST_ENTRY_"
 
 LOG_INFO = 1
 LOG_DEBUG = 2
 SIMILAR = 1
 SIMILAR_NO_FILTER = 2
 SIMILAR_NO_FILTER_NO_FTS = 2
```

### Comparing `xklb-1.26.21/xklb/db.py` & `xklb-1.26.23/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/dl_config.py` & `xklb-1.26.23/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/dl_extract.py` & `xklb-1.26.23/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/fs_extract.py` & `xklb-1.26.23/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/gui.py` & `xklb-1.26.23/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/hn_extract.py` & `xklb-1.26.23/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/lb.py` & `xklb-1.26.23/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/play_actions.py` & `xklb-1.26.23/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/playback.py` & `xklb-1.26.23/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/player.py` & `xklb-1.26.23/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/praw_extract.py` & `xklb-1.26.23/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/stats.py` & `xklb-1.26.23/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/subtitle.py` & `xklb-1.26.23/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/tabs_actions.py` & `xklb-1.26.23/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/tabs_extract.py` & `xklb-1.26.23/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/tube_backend.py` & `xklb-1.26.23/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/tube_extract.py` & `xklb-1.26.23/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/utils.py` & `xklb-1.26.23/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/__init__.py` & `xklb-1.26.23/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/bigdirs.py` & `xklb-1.26.23/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/christen.py` & `xklb-1.26.23/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/copy_play_counts.py` & `xklb-1.26.23/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/dedupe.py` & `xklb-1.26.23/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/merge_dbs.py` & `xklb-1.26.23/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/merge_online_local.py` & `xklb-1.26.23/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/move_list.py` & `xklb-1.26.23/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/optimize_db.py` & `xklb-1.26.23/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/redownload.py` & `xklb-1.26.23/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/relmv.py` & `xklb-1.26.23/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/scatter.py` & `xklb-1.26.23/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.23/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.23/xklb/scripts/mining/nfb_ca.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/mining/nouns.py` & `xklb-1.26.23/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/mining/pushshift.py` & `xklb-1.26.23/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.26.23/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/xklb/scripts/mining/words.py` & `xklb-1.26.23/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/assets/kotobago.png` & `xklb-1.26.23/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/.gitignore` & `xklb-1.26.23/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/LICENSE` & `xklb-1.26.23/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/README.md` & `xklb-1.26.23/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.021)
+    xk media library subcommands (v1.26.023)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.26.21/pyproject.toml` & `xklb-1.26.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.21/PKG-INFO` & `xklb-1.26.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.21
+Version: 1.26.23
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.021)
+    xk media library subcommands (v1.26.023)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

