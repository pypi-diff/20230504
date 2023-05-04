# Comparing `tmp/fc-guarder-0.4.3.tar.gz` & `tmp/fc-guarder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-guarder-0.4.3.tar", last modified: Wed Mar 22 02:13:30 2023, max compression
+gzip compressed data, was "dist/fc-guarder-0.5.0.tar", last modified: Thu May  4 03:24:10 2023, max compression
```

## Comparing `fc-guarder-0.4.3.tar` & `fc-guarder-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2022-08-17 07:02:28.000000 fc-guarder-0.4.3/README.rst
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2975 2022-03-07 07:28:36.000000 fc-guarder-0.4.3/fc_guarder/guarder.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      653 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       17 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      265 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      766 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       56 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       11 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/fc_guarder.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2022-03-07 07:28:36.000000 fc-guarder-0.4.3/LICENSE
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     3857 2023-03-22 02:13:00.000000 fc-guarder-0.4.3/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      766 2023-03-22 02:13:30.000000 fc-guarder-0.4.3/PKG-INFO
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-guarder-0.5.0/README.rst
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1928 2023-05-04 03:23:04.000000 fc-guarder-0.5.0/fc_guarder/guarder.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/setup.cfg
+drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       17 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/requires.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      265 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/PKG-INFO
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       56 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/entry_points.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       11 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/fc_guarder.egg-info/top_level.txt
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-guarder-0.5.0/LICENSE
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 03:23:04.000000 fc-guarder-0.5.0/setup.py
+-rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      716 2023-05-04 03:24:10.000000 fc-guarder-0.5.0/PKG-INFO
```

### Comparing `fc-guarder-0.4.3/README.rst` & `fc-guarder-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.4.3/setup.cfg` & `fc-guarder-0.5.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fc-guarder-0.4.3/LICENSE` & `fc-guarder-0.5.0/LICENSE`

 * *Files identical despite different names*

