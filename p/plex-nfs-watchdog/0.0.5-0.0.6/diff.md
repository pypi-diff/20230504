# Comparing `tmp/plex-nfs-watchdog-0.0.5.tar.gz` & `tmp/plex-nfs-watchdog-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-nfs-watchdog-0.0.5.tar", last modified: Thu May  4 09:35:22 2023, max compression
+gzip compressed data, was "plex-nfs-watchdog-0.0.6.tar", last modified: Thu May  4 12:54:00 2023, max compression
```

## Comparing `plex-nfs-watchdog-0.0.5.tar` & `plex-nfs-watchdog-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/plex_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/plex_nfs_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/config/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/plex_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 12:53:48.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/plex_nfs_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:54:00.837244 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 12:54:00.000000 plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/top_level.txt
```

### Comparing `plex-nfs-watchdog-0.0.5/LICENSE` & `plex-nfs-watchdog-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.5/PKG-INFO` & `plex-nfs-watchdog-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.5 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.6 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.5/README.md` & `plex-nfs-watchdog-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.5/setup.cfg` & `plex-nfs-watchdog-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/plex_agent.py` & `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/plex/plex_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,24 +220,25 @@
 
     def parse_event(self, event) -> None:
         """
         Parses the given event and adds it to the queue
         :param event: The event to parse
         :return:
         """
-        event_path = Path(event.src_path)
+        event_type: str = event.event_type
+        event_path: Path = Path(event.src_path) if event_type != 'moved' else Path(event.dest_path)
         if event_path.name in self.__internal_paths.keys():
             return
         section_child: Path | None = self.__find_section_child_of(event_path)
         if section_child is None:
             logging.error(f"Could not find Plex section for {event_path}")
             return
         section_scan = (section_child.parent.name, section_child.name)
         if section_scan not in self.__notify_queue:
-            logging.info(f"Adding to queue ({event.event_type}): {section_child.name}")
+            logging.info(f"Adding to queue ({event_type}): {section_child.name}")
             self.__notify_queue.add(section_scan)
 
     def start_service(self) -> ():
         """
         Start a thread to manage a queue of pending scans
         :return callable: A function to stop the thread
         """
```

### Comparing `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py` & `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/plex_nfs_watchdog.py` & `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog/plex_nfs_watchdog.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/PKG-INFO` & `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.5 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.6 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/SOURCES.txt` & `plex-nfs-watchdog-0.0.6/src/plex_nfs_watchdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

