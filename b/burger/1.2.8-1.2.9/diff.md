# Comparing `tmp/burger-1.2.8.tar.gz` & `tmp/burger-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burger-1.2.8.tar", last modified: Mon Feb 27 04:05:30 2023, max compression
+gzip compressed data, was "burger-1.2.9.tar", last modified: Thu May  4 03:47:43 2023, max compression
```

## Comparing `burger-1.2.8.tar` & `burger-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 04:05:30.838029 burger-1.2.8/
--rw-rw-rw-   0        0        0     1674 2022-02-04 19:15:29.000000 burger-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3085 2023-02-27 04:05:30.837029 burger-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1720 2021-11-15 06:20:17.000000 burger-1.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-27 04:05:30.828027 burger-1.2.8/burger/
--rw-rw-rw-   0        0        0     8960 2023-02-27 03:40:02.000000 burger-1.2.8/burger/__init__.py
--rw-rw-rw-   0        0        0     7608 2023-02-26 19:32:28.000000 burger-1.2.8/burger/_find_visual_studio.py
--rw-rw-rw-   0        0        0    14929 2022-12-25 00:26:46.000000 burger-1.2.8/burger/_find_win_sdks.py
--rw-rw-rw-   0        0        0     2196 2022-12-24 23:30:20.000000 burger-1.2.8/burger/_vsinstance.py
--rw-rw-rw-   0        0        0    21045 2022-12-26 18:04:26.000000 burger-1.2.8/burger/buildutils.py
--rw-rw-rw-   0        0        0     3859 2022-12-24 22:48:20.000000 burger-1.2.8/burger/cleanutils.py
--rw-rw-rw-   0        0        0    26226 2022-12-27 06:21:33.000000 burger-1.2.8/burger/fileutils.py
--rw-rw-rw-   0        0        0     8575 2022-12-28 21:50:01.000000 burger-1.2.8/burger/git.py
--rw-rw-rw-   0        0        0    22258 2023-02-27 03:47:59.000000 burger-1.2.8/burger/locators.py
--rw-rw-rw-   0        0        0    12662 2022-12-26 07:11:15.000000 burger-1.2.8/burger/perforce.py
--rw-rw-rw-   0        0        0    28209 2022-12-25 20:20:49.000000 burger-1.2.8/burger/strutils.py
--rw-rw-rw-   0        0        0    11710 2022-12-25 01:05:42.000000 burger-1.2.8/burger/validators.py
--rw-rw-rw-   0        0        0     2605 2022-12-25 00:31:52.000000 burger-1.2.8/burger/windowsutils.py
-drwxrwxrwx   0        0        0        0 2023-02-27 04:05:30.837029 burger-1.2.8/burger.egg-info/
--rw-rw-rw-   0        0        0     3085 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-27 04:05:30.000000 burger-1.2.8/burger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-27 04:05:30.838029 burger-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     4580 2022-12-25 19:15:30.000000 burger-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:47:43.611467 burger-1.2.9/
+-rw-rw-rw-   0        0        0     1674 2022-02-04 19:15:29.000000 burger-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3085 2023-05-04 03:47:43.610464 burger-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1720 2021-11-15 06:20:17.000000 burger-1.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 03:47:43.585806 burger-1.2.9/burger/
+-rw-rw-rw-   0        0        0     8960 2023-02-28 04:48:48.000000 burger-1.2.9/burger/__init__.py
+-rw-rw-rw-   0        0        0     7608 2023-02-26 19:32:28.000000 burger-1.2.9/burger/_find_visual_studio.py
+-rw-rw-rw-   0        0        0    14929 2022-12-25 00:26:46.000000 burger-1.2.9/burger/_find_win_sdks.py
+-rw-rw-rw-   0        0        0     2196 2022-12-24 23:30:20.000000 burger-1.2.9/burger/_vsinstance.py
+-rw-rw-rw-   0        0        0    21045 2022-12-26 18:04:26.000000 burger-1.2.9/burger/buildutils.py
+-rw-rw-rw-   0        0        0     3859 2022-12-24 22:48:20.000000 burger-1.2.9/burger/cleanutils.py
+-rw-rw-rw-   0        0        0    26237 2023-05-04 03:31:48.000000 burger-1.2.9/burger/fileutils.py
+-rw-rw-rw-   0        0        0     8575 2022-12-28 21:50:01.000000 burger-1.2.9/burger/git.py
+-rw-rw-rw-   0        0        0    22470 2023-02-28 04:47:19.000000 burger-1.2.9/burger/locators.py
+-rw-rw-rw-   0        0        0    12662 2022-12-26 07:11:15.000000 burger-1.2.9/burger/perforce.py
+-rw-rw-rw-   0        0        0    28209 2022-12-25 20:20:49.000000 burger-1.2.9/burger/strutils.py
+-rw-rw-rw-   0        0        0    11710 2022-12-25 01:05:42.000000 burger-1.2.9/burger/validators.py
+-rw-rw-rw-   0        0        0     2605 2022-12-25 00:31:52.000000 burger-1.2.9/burger/windowsutils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:47:43.609468 burger-1.2.9/burger.egg-info/
+-rw-rw-rw-   0        0        0     3085 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 03:47:43.000000 burger-1.2.9/burger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 03:47:43.611467 burger-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     4580 2022-12-25 19:15:30.000000 burger-1.2.9/setup.py
```

### Comparing `burger-1.2.8/LICENSE.txt` & `burger-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/PKG-INFO` & `burger-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burger
-Version: 1.2.8
+Version: 1.2.9
 Summary: Burger Becky's shared python library.
 Home-page: http://pyburger.readthedocs.io
 Author: Rebecca Ann Heineman
 Author-email: becky@burgerbecky.com
 License: MIT License
 Keywords: burger,perforce,burgerlib,development
 Platform: Any
```

### Comparing `burger-1.2.8/README.rst` & `burger-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/__init__.py` & `burger-1.2.9/burger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 else:
     from io import StringIO
 
 ########################################
 
 
 # Numeric version
-__numversion__ = (1, 2, 8)
+__numversion__ = (1, 2, 9)
 
 # Current version of the library
 __version__ = ".".join([str(num) for num in __numversion__])
 
 # Author's name
 __author__ = "Rebecca Ann Heineman"
```

### Comparing `burger-1.2.8/burger/_find_visual_studio.py` & `burger-1.2.9/burger/_find_visual_studio.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/_find_win_sdks.py` & `burger-1.2.9/burger/_find_win_sdks.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/_vsinstance.py` & `burger-1.2.9/burger/_vsinstance.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/buildutils.py` & `burger-1.2.9/burger/buildutils.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/cleanutils.py` & `burger-1.2.9/burger/cleanutils.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/fileutils.py` & `burger-1.2.9/burger/fileutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,16 @@
     if IS_MACOSX:
         exename = os.path.join(tool_folder, "macosx", tool_name)
 
     # Windows supports 32 and 64 bit Intel
     elif IS_WINDOWS_HOST:
         exename = os.path.join(
             tool_folder,
-            "windows_" + get_windows_host_type(True),
+            "windows",
+           	get_windows_host_type(True),
             tool_name + ".exe")
 
     # Linux is currently just 64 bit Intel, will have to update
     # as more platforms are supported
     elif IS_LINUX:
         exename = os.path.join(tool_folder, "linux", tool_name)
```

### Comparing `burger-1.2.8/burger/git.py` & `burger-1.2.9/burger/git.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/locators.py` & `burger-1.2.9/burger/locators.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,15 +598,15 @@
 
     # Can't find it
     return None
 
 ########################################
 
 
-def where_is_visual_studio(vs_version, tool_name=None):
+def where_is_visual_studio(vs_version, tool_name=None, cpu=None):
     """
     Locate devenv.com for a specific version of Visual Studio.
 
     Given a specific version by year, check for the appropriate environment
     variable that contains the path to the executable of the IDE
 
     Note:
@@ -615,60 +615,66 @@
     Examples:
         >>> burger.where_is_visual_studio(2010)
         "C:\\Program Files (x86)\\Microsoft Visual Studio 10.0\\Common7\\ide\\devenv.com"
 
     Args:
         vs_version: Version year as number
         tool_name: Return the path to this tool, None becomes ``devenv.com``
+        cpu: String of the cpu type of the tool requested, ``x86``, ``x64``
 
     Returns:
         Path to devenv.com for the IDE or None.
     """
 
     # pylint: disable=too-many-branches
 
     # Test if running on a windows host
     host_type = get_windows_host_type(True)
     if not host_type:
         return None
 
-    # Check if it's even in the table
+    # Check if the version is even in the table
     table_item = _VS_TABLE.get(vs_version, None)
     if not table_item:
         return None
 
     # Tool to locate, use default if not supplied
     if not tool_name:
         tool_name = "devenv.com"
 
     # Table of cputypes to check
     cputable = []
 
-    # If already x86, or .com skip extra cpus
-    if host_type != "x86" and not tool_name.endswith(".com"):
+    # Only check this one
+    if cpu:
+        cputable.append(cpu)
+
+    else:
+        # If already x86, or .com skip extra cpus
+        if host_type != "x86" and not tool_name.endswith(".com"):
+
+            # Prioritize the native CPU
+            cputable.append(host_type)
+
+            # If ARM, allow x64 for the emulation layer
+            if host_type in ("arm", "arm64"):
+                cputable.append("x64")
 
-        # Prioritize the native CPU
-        cputable.append(host_type)
-
-        # If ARM, allow x64 for the emulation layer
-        if host_type in ("arm", "arm64"):
-            cputable.append("x64")
-
-    # Always use x86
-    cputable.append("x86")
+        # Always use x86
+        cputable.append("x86")
 
     # Try the registry first
     for item in find_visual_studios():
 
         # Is this the version of Visual Studio requested?
         if item.version_info[0] == table_item[2]:
 
             # Check with CPUs and find a match
-            for cpu in cputable:
-                vstudiopath = item.known_paths.get(tool_name + "_" + cpu, None)
+            for i in cputable:
+                vstudiopath = item.known_paths.get(tool_name + "_" + i, None)
                 if vstudiopath:
                     return vstudiopath
 
     # Try the environment variable next
     vstudio_paths = []
     vstudiopath = os.getenv(table_item[0], default=None)
     if vstudiopath:
```

### Comparing `burger-1.2.8/burger/perforce.py` & `burger-1.2.9/burger/perforce.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/strutils.py` & `burger-1.2.9/burger/strutils.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/validators.py` & `burger-1.2.9/burger/validators.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger/windowsutils.py` & `burger-1.2.9/burger/windowsutils.py`

 * *Files identical despite different names*

### Comparing `burger-1.2.8/burger.egg-info/PKG-INFO` & `burger-1.2.9/burger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burger
-Version: 1.2.8
+Version: 1.2.9
 Summary: Burger Becky's shared python library.
 Home-page: http://pyburger.readthedocs.io
 Author: Rebecca Ann Heineman
 Author-email: becky@burgerbecky.com
 License: MIT License
 Keywords: burger,perforce,burgerlib,development
 Platform: Any
```

### Comparing `burger-1.2.8/setup.py` & `burger-1.2.9/setup.py`

 * *Files identical despite different names*

