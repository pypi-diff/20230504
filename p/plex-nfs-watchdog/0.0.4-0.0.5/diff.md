# Comparing `tmp/plex-nfs-watchdog-0.0.4.tar.gz` & `tmp/plex-nfs-watchdog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-nfs-watchdog-0.0.4.tar", last modified: Tue Apr 25 13:01:11 2023, max compression
+gzip compressed data, was "plex-nfs-watchdog-0.0.5.tar", last modified: Thu May  4 09:35:22 2023, max compression
```

## Comparing `plex-nfs-watchdog-0.0.4.tar` & `plex-nfs-watchdog-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.335427 plex-nfs-watchdog-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/plex_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/plex_nfs_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/config/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/plex_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.123842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 09:35:07.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/plex_nfs_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:22.119842 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 09:35:22.000000 plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/top_level.txt
```

### Comparing `plex-nfs-watchdog-0.0.4/LICENSE` & `plex-nfs-watchdog-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.4/PKG-INFO` & `plex-nfs-watchdog-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.4
+Version: 0.0.5
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -122,27 +122,28 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Usage
 
 This utility requires the following arguments to work:
 
-| Argument                                     | Role                                                                                                                |
-|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
-| __--scan \| -s__                             | Manually triggers a partial-scan on the given paths                                                                 |
-| __--daemon \| -d__                           | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--inteval_ |
-| __--paths \| -p__ _\[PATHS...\]_             | A list of folder paths                                                                                             |
-| __--host \| -H__ _HOST_                      | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                |
-| __--token \| -t__ _TOKEN_                    | The token of the Plex server                                                                                        |
-| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The interval in seconds to wait between partial-scans                                                               |
+| Argument                                               | Role                                                                                                                                   |
+|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
+| __--scan \| -s__                                       | Manually triggers a partial-scan on the given paths                                                                                    |
+| __--daemon \| -d__                                     | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--interval_ and _--listeners_ |
+| __--paths \| -p__ _\[PATHS...\]_                       | A list of folder paths                                                                                                                 |
+| __--host \| -H__ _HOST_                                | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                                   |
+| __--token \| -t__ _TOKEN_                              | The token of the Plex server                                                                                                           |
+| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\]           | The interval in seconds to wait between partial-scans                                                                                  |
+| __--listeners \| -l__ _\[LISTENERS...\]_  \[OPTIONAL\] | The event type to watch: `move`, `modify`, `create`, `delete`, `io_close`, `io_open`                                                                                                        |
 
 - Manual Scan example:
     >`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --host http://localhost:32400 --token YOUR_TOKEN`
 - Daemon Scan example:
-  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150`
+  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150 --listeners move modify create delete`
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Notes
 
 After the first successful run, a cache config file containing Plex's host and token will be created in the user's home directory. This file will be used for subsequent runs, so you don't have to provide them every time.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.4 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.5 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
@@ -62,28 +62,31 @@
 can run the tool using: `plex-nfs-watchdog` - If you want to use the script
 directly: - Clone the repository anywhere on your pc: `git clone https://
 github.com/LightDestory/PlexNFSWatchdog` - Install the requirements using `pip`
 (create a `venv` if you want): `pip install -r requirements.txt` - Run directly
 from source: `python ./src/plex_nfs_watchdog/plex_nfs_watchdog.py`
                                                                   (back_to_top)
 ### Usage This utility requires the following arguments to work: | Argument |
-Role | |----------------------------------------------|------------------------
+Role | |--------------------------------------------------------|--------------
 -------------------------------------------------------------------------------
---------------| | __--scan \| -s__ | Manually triggers a partial-scan on the
-given paths | | __--daemon \| -d__ | Starts a watchdog daemon to automatically
-triggers a partial-scan on the given paths
-__Requires:__ _--inteval_ | | __--paths \| -p__ _\[PATHS...\]_ | A list of
-folder paths | | __--host \| -H__ _HOST_ | The host of the Plex server
+-------------------------------------------| | __--scan \| -s__ | Manually
+triggers a partial-scan on the given paths | | __--daemon \| -d__ | Starts a
+watchdog daemon to automatically triggers a partial-scan on the given paths
+__Requires:__ _--interval_ and _--listeners_ | | __--paths \| -p__ _\
+[PATHS...\]_ | A list of folder paths | | __--host \| -H__ _HOST_ | The host of
+the Plex server
 __Default:__ _http://localhost:32400_ | | __--token \| -t__ _TOKEN_ | The token
 of the Plex server | | __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The
-interval in seconds to wait between partial-scans | - Manual Scan example:
->`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --
-host http://localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-
-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://
-localhost:32400 --token YOUR_TOKEN --interval 150`
+interval in seconds to wait between partial-scans | | __--listeners \| -l__ _\
+[LISTENERS...\]_ \[OPTIONAL\] | The event type to watch: `move`, `modify`,
+`create`, `delete`, `io_close`, `io_open` | - Manual Scan example: >`plex-nfs-
+watchdog --scan --paths /path/to/library_section1/section_chield1 --host http:/
+/localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-nfs-watchdog
+--daemon --paths /path/to/library_section1 --host http://localhost:32400 --
+token YOUR_TOKEN --interval 150 --listeners move modify create delete`
                                                                   (back_to_top)
 ### Notes After the first successful run, a cache config file containing Plex's
 host and token will be created in the user's home directory. This file will be
 used for subsequent runs, so you don't have to provide them every time.
                                                                   (back_to_top)
  ## :dizzy: Contributing If you are interested in contributing, please refer to
 [Contributing Guidelines](.github/CONTRIBUTING.md) for more information and
```

### Comparing `plex-nfs-watchdog-0.0.4/README.md` & `plex-nfs-watchdog-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -99,27 +99,28 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Usage
 
 This utility requires the following arguments to work:
 
-| Argument                                     | Role                                                                                                                |
-|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
-| __--scan \| -s__                             | Manually triggers a partial-scan on the given paths                                                                 |
-| __--daemon \| -d__                           | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--inteval_ |
-| __--paths \| -p__ _\[PATHS...\]_             | A list of folder paths                                                                                             |
-| __--host \| -H__ _HOST_                      | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                |
-| __--token \| -t__ _TOKEN_                    | The token of the Plex server                                                                                        |
-| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The interval in seconds to wait between partial-scans                                                               |
+| Argument                                               | Role                                                                                                                                   |
+|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
+| __--scan \| -s__                                       | Manually triggers a partial-scan on the given paths                                                                                    |
+| __--daemon \| -d__                                     | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--interval_ and _--listeners_ |
+| __--paths \| -p__ _\[PATHS...\]_                       | A list of folder paths                                                                                                                 |
+| __--host \| -H__ _HOST_                                | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                                   |
+| __--token \| -t__ _TOKEN_                              | The token of the Plex server                                                                                                           |
+| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\]           | The interval in seconds to wait between partial-scans                                                                                  |
+| __--listeners \| -l__ _\[LISTENERS...\]_  \[OPTIONAL\] | The event type to watch: `move`, `modify`, `create`, `delete`, `io_close`, `io_open`                                                                                                        |
 
 - Manual Scan example:
     >`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --host http://localhost:32400 --token YOUR_TOKEN`
 - Daemon Scan example:
-  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150`
+  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150 --listeners move modify create delete`
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Notes
 
 After the first successful run, a cache config file containing Plex's host and token will be created in the user's home directory. This file will be used for subsequent runs, so you don't have to provide them every time.
```

#### html2text {}

```diff
@@ -50,28 +50,31 @@
 can run the tool using: `plex-nfs-watchdog` - If you want to use the script
 directly: - Clone the repository anywhere on your pc: `git clone https://
 github.com/LightDestory/PlexNFSWatchdog` - Install the requirements using `pip`
 (create a `venv` if you want): `pip install -r requirements.txt` - Run directly
 from source: `python ./src/plex_nfs_watchdog/plex_nfs_watchdog.py`
                                                                   (back_to_top)
 ### Usage This utility requires the following arguments to work: | Argument |
-Role | |----------------------------------------------|------------------------
+Role | |--------------------------------------------------------|--------------
 -------------------------------------------------------------------------------
---------------| | __--scan \| -s__ | Manually triggers a partial-scan on the
-given paths | | __--daemon \| -d__ | Starts a watchdog daemon to automatically
-triggers a partial-scan on the given paths
-__Requires:__ _--inteval_ | | __--paths \| -p__ _\[PATHS...\]_ | A list of
-folder paths | | __--host \| -H__ _HOST_ | The host of the Plex server
+-------------------------------------------| | __--scan \| -s__ | Manually
+triggers a partial-scan on the given paths | | __--daemon \| -d__ | Starts a
+watchdog daemon to automatically triggers a partial-scan on the given paths
+__Requires:__ _--interval_ and _--listeners_ | | __--paths \| -p__ _\
+[PATHS...\]_ | A list of folder paths | | __--host \| -H__ _HOST_ | The host of
+the Plex server
 __Default:__ _http://localhost:32400_ | | __--token \| -t__ _TOKEN_ | The token
 of the Plex server | | __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The
-interval in seconds to wait between partial-scans | - Manual Scan example:
->`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --
-host http://localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-
-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://
-localhost:32400 --token YOUR_TOKEN --interval 150`
+interval in seconds to wait between partial-scans | | __--listeners \| -l__ _\
+[LISTENERS...\]_ \[OPTIONAL\] | The event type to watch: `move`, `modify`,
+`create`, `delete`, `io_close`, `io_open` | - Manual Scan example: >`plex-nfs-
+watchdog --scan --paths /path/to/library_section1/section_chield1 --host http:/
+/localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-nfs-watchdog
+--daemon --paths /path/to/library_section1 --host http://localhost:32400 --
+token YOUR_TOKEN --interval 150 --listeners move modify create delete`
                                                                   (back_to_top)
 ### Notes After the first successful run, a cache config file containing Plex's
 host and token will be created in the user's home directory. This file will be
 used for subsequent runs, so you don't have to provide them every time.
                                                                   (back_to_top)
  ## :dizzy: Contributing If you are interested in contributing, please refer to
 [Contributing Guidelines](.github/CONTRIBUTING.md) for more information and
```

### Comparing `plex-nfs-watchdog-0.0.4/setup.cfg` & `plex-nfs-watchdog-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/plex_agent.py` & `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/modules/plex/plex_agent.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/plex_nfs_watchdog.py` & `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog/plex_nfs_watchdog.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,22 @@
                         required=False)
     parser.add_argument("--dry-run", action='store_true',
                              help="Dry run mode, does not  send any request of partial-scans")
     parser.add_argument("--interval", "-i", help="The interval in seconds to wait between partial-scans",
                         action="store", type=int, required=False, default=None)
     parser.add_argument("--version", "-v", help="Prints the version of the application", action='version',
                         version=f"%(prog)s {shared.VERSION}")
+    parser.add_argument("--listeners", "-l", action="store", nargs='+', required=False, help="List of events to watch",
+                        type=str, choices=shared.listeners_type, default=None)
     shared.user_input = parser.parse_args()
     shared.user_input.paths = set(shared.user_input.paths)
     if shared.user_input.daemon and (shared.user_input.interval is None or shared.user_input.interval <= 0):
         parser.error("--interval is required when using --daemon. It must be a not zero positive integer")
+    if shared.user_input.daemon and shared.user_input.listeners is None:
+        parser.error("--listeners is required when using --daemon. It must be a valid event type")
     for given_path in shared.user_input.paths:
         if not given_path.exists() or not given_path.is_dir():
             parser.error(f"{given_path.resolve()} does not exist or it is not a folder!")
     if shared.user_input.token is None and not plex_agent_singleton.is_cache_loaded():
         parser.error("Plex host and token are missing!")
```

### Comparing `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/PKG-INFO` & `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.4
+Version: 0.0.5
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -122,27 +122,28 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Usage
 
 This utility requires the following arguments to work:
 
-| Argument                                     | Role                                                                                                                |
-|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
-| __--scan \| -s__                             | Manually triggers a partial-scan on the given paths                                                                 |
-| __--daemon \| -d__                           | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--inteval_ |
-| __--paths \| -p__ _\[PATHS...\]_             | A list of folder paths                                                                                             |
-| __--host \| -H__ _HOST_                      | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                |
-| __--token \| -t__ _TOKEN_                    | The token of the Plex server                                                                                        |
-| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The interval in seconds to wait between partial-scans                                                               |
+| Argument                                               | Role                                                                                                                                   |
+|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
+| __--scan \| -s__                                       | Manually triggers a partial-scan on the given paths                                                                                    |
+| __--daemon \| -d__                                     | Starts a watchdog daemon to automatically triggers a partial-scan on the given paths <br> __Requires:__ _--interval_ and _--listeners_ |
+| __--paths \| -p__ _\[PATHS...\]_                       | A list of folder paths                                                                                                                 |
+| __--host \| -H__ _HOST_                                | The host of the Plex server<br>__Default:__ _http://localhost:32400_                                                                   |
+| __--token \| -t__ _TOKEN_                              | The token of the Plex server                                                                                                           |
+| __--interval \| -i__ _INTERVAL_ \[OPTIONAL\]           | The interval in seconds to wait between partial-scans                                                                                  |
+| __--listeners \| -l__ _\[LISTENERS...\]_  \[OPTIONAL\] | The event type to watch: `move`, `modify`, `create`, `delete`, `io_close`, `io_open`                                                                                                        |
 
 - Manual Scan example:
     >`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --host http://localhost:32400 --token YOUR_TOKEN`
 - Daemon Scan example:
-  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150`
+  >`plex-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://localhost:32400 --token YOUR_TOKEN --interval 150 --listeners move modify create delete`
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Notes
 
 After the first successful run, a cache config file containing Plex's host and token will be created in the user's home directory. This file will be used for subsequent runs, so you don't have to provide them every time.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.4 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.5 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
@@ -62,28 +62,31 @@
 can run the tool using: `plex-nfs-watchdog` - If you want to use the script
 directly: - Clone the repository anywhere on your pc: `git clone https://
 github.com/LightDestory/PlexNFSWatchdog` - Install the requirements using `pip`
 (create a `venv` if you want): `pip install -r requirements.txt` - Run directly
 from source: `python ./src/plex_nfs_watchdog/plex_nfs_watchdog.py`
                                                                   (back_to_top)
 ### Usage This utility requires the following arguments to work: | Argument |
-Role | |----------------------------------------------|------------------------
+Role | |--------------------------------------------------------|--------------
 -------------------------------------------------------------------------------
---------------| | __--scan \| -s__ | Manually triggers a partial-scan on the
-given paths | | __--daemon \| -d__ | Starts a watchdog daemon to automatically
-triggers a partial-scan on the given paths
-__Requires:__ _--inteval_ | | __--paths \| -p__ _\[PATHS...\]_ | A list of
-folder paths | | __--host \| -H__ _HOST_ | The host of the Plex server
+-------------------------------------------| | __--scan \| -s__ | Manually
+triggers a partial-scan on the given paths | | __--daemon \| -d__ | Starts a
+watchdog daemon to automatically triggers a partial-scan on the given paths
+__Requires:__ _--interval_ and _--listeners_ | | __--paths \| -p__ _\
+[PATHS...\]_ | A list of folder paths | | __--host \| -H__ _HOST_ | The host of
+the Plex server
 __Default:__ _http://localhost:32400_ | | __--token \| -t__ _TOKEN_ | The token
 of the Plex server | | __--interval \| -i__ _INTERVAL_ \[OPTIONAL\] | The
-interval in seconds to wait between partial-scans | - Manual Scan example:
->`plex-nfs-watchdog --scan --paths /path/to/library_section1/section_chield1 --
-host http://localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-
-nfs-watchdog --daemon --paths /path/to/library_section1 --host http://
-localhost:32400 --token YOUR_TOKEN --interval 150`
+interval in seconds to wait between partial-scans | | __--listeners \| -l__ _\
+[LISTENERS...\]_ \[OPTIONAL\] | The event type to watch: `move`, `modify`,
+`create`, `delete`, `io_close`, `io_open` | - Manual Scan example: >`plex-nfs-
+watchdog --scan --paths /path/to/library_section1/section_chield1 --host http:/
+/localhost:32400 --token YOUR_TOKEN` - Daemon Scan example: >`plex-nfs-watchdog
+--daemon --paths /path/to/library_section1 --host http://localhost:32400 --
+token YOUR_TOKEN --interval 150 --listeners move modify create delete`
                                                                   (back_to_top)
 ### Notes After the first successful run, a cache config file containing Plex's
 host and token will be created in the user's home directory. This file will be
 used for subsequent runs, so you don't have to provide them every time.
                                                                   (back_to_top)
  ## :dizzy: Contributing If you are interested in contributing, please refer to
 [Contributing Guidelines](.github/CONTRIBUTING.md) for more information and
```

### Comparing `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/SOURCES.txt` & `plex-nfs-watchdog-0.0.5/src/plex_nfs_watchdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

