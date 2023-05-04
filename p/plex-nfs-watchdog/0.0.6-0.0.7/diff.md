# Comparing `tmp/plex-nfs-watchdog-0.0.6.tar.gz` & `tmp/plex-nfs-watchdog-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-nfs-watchdog-0.0.6.tar", last modified: Thu May  4 12:54:00 2023, max compression
+gzip compressed data, was "plex-nfs-watchdog-0.0.7.tar", last modified: Thu May  4 14:54:58 2023, max compression
```

## Comparing `plex-nfs-watchdog-0.0.6.tar` & `plex-nfs-watchdog-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/plex_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/plex_nfs_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.510978 plex-nfs-watchdog-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 14:54:58.510978 plex-nfs-watchdog-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 14:54:58.510978 plex-nfs-watchdog-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.502978 plex-nfs-watchdog-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.506978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.506978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.506978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/config/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.510978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/plex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/plex/plex_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.510978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 14:54:45.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/plex_nfs_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:58.506978 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:54:58.000000 plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/top_level.txt
```

### Comparing `plex-nfs-watchdog-0.0.6/LICENSE` & `plex-nfs-watchdog-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.6/PKG-INFO` & `plex-nfs-watchdog-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.6
+Version: 0.0.7
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.6 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.7 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.6/README.md` & `plex-nfs-watchdog-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.6/setup.cfg` & `plex-nfs-watchdog-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/plex_agent.py` & `plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/plex/plex_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class PlexAgent:
     __plex_config: dict[str, str] = {}
     __server: PlexServer = None
     __save_cache: bool = False
     __internal_paths: dict[str, tuple[str, str]] = {}
-    __notify_queue: set[tuple[str, str]] = set()
+    __notify_queue: list[tuple[str, str]] = list()
     __supported_ext: list[str] = [
         "3g2",
         "3gp",
         "amv",
         "asf",
         "ass",
         "avi",
@@ -185,15 +185,15 @@
         :return:
         """
         section_title, section_path = self.__internal_paths[section]
         plex_section = self.__server.library.section(section_title)
         if plex_section.refreshing:
             if shared.user_input.daemon:
                 logging.warning(f"Plex section {section_title} is already refreshing, re-scheduling...")
-                self.__notify_queue.add((section, item))
+                self.__notify_queue.append((section, item))
             else:
                 logging.warning(f"Plex section {section_title} is already refreshing, skipping...")
             return
         scan_path: Path = Path(f"{section_path}/{item}")
         logging.info(f"Requesting Plex to scan remote path {str(scan_path)}")
         if shared.user_input.dry_run:
             logging.info(f"Skipping Plex scan due to dry-run")
@@ -231,27 +231,27 @@
         section_child: Path | None = self.__find_section_child_of(event_path)
         if section_child is None:
             logging.error(f"Could not find Plex section for {event_path}")
             return
         section_scan = (section_child.parent.name, section_child.name)
         if section_scan not in self.__notify_queue:
             logging.info(f"Adding to queue ({event_type}): {section_child.name}")
-            self.__notify_queue.add(section_scan)
+            self.__notify_queue.append(section_scan)
 
     def start_service(self) -> ():
         """
         Start a thread to manage a queue of pending scans
         :return callable: A function to stop the thread
         """
         stopped = Event()
 
         def loop():
             while not stopped.wait(shared.user_input.interval):
                 if self.__notify_queue:
-                    section, item = self.__notify_queue.pop()
+                    section, item = self.__notify_queue.pop(0)
                     self._scan(section, item)
 
         Thread(target=loop).start()
         return stopped.set
 
 
 plex_agent_singleton = PlexAgent()
```

### Comparing `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py` & `plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/plex_nfs_watchdog.py` & `plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog/plex_nfs_watchdog.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/PKG-INFO` & `plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.6
+Version: 0.0.7
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.6 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.7 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/SOURCES.txt` & `plex-nfs-watchdog-0.0.7/src/plex_nfs_watchdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

