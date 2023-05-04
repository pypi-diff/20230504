# Comparing `tmp/azuredol-0.1.2.tar.gz` & `tmp/azuredol-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuredol-0.1.2.tar", last modified: Tue Apr 11 19:50:04 2023, max compression
+gzip compressed data, was "azuredol-0.1.3.tar", last modified: Thu May  4 00:39:12 2023, max compression
```

## Comparing `azuredol-0.1.2.tar` & `azuredol-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:50:04.969126 azuredol-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 19:49:34.000000 azuredol-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 19:50:04.969126 azuredol-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 19:49:34.000000 azuredol-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:50:04.969126 azuredol-0.1.2/azuredol/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 19:49:34.000000 azuredol-0.1.2/azuredol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-11 19:49:34.000000 azuredol-0.1.2/azuredol/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:50:04.969126 azuredol-0.1.2/azuredol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 19:50:04.000000 azuredol-0.1.2/azuredol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 19:50:04.969126 azuredol-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 19:49:34.000000 azuredol-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:39:12.208368 azuredol-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 00:38:19.000000 azuredol-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 00:39:12.208368 azuredol-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 00:38:19.000000 azuredol-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:39:12.208368 azuredol-0.1.3/azuredol/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 00:38:19.000000 azuredol-0.1.3/azuredol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-04 00:39:10.000000 azuredol-0.1.3/azuredol/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:39:12.208368 azuredol-0.1.3/azuredol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 00:39:11.000000 azuredol-0.1.3/azuredol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 00:39:12.000000 azuredol-0.1.3/azuredol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:39:11.000000 azuredol-0.1.3/azuredol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:39:11.000000 azuredol-0.1.3/azuredol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 00:39:11.000000 azuredol-0.1.3/azuredol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 00:39:11.000000 azuredol-0.1.3/azuredol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 00:39:12.208368 azuredol-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 00:38:19.000000 azuredol-0.1.3/setup.py
```

### Comparing `azuredol-0.1.2/LICENSE` & `azuredol-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azuredol-0.1.2/setup.cfg` & `azuredol-0.1.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = azuredol
-version = 0.1.2
+version = 0.1.3
 url = https://github.com/i2mint/azuredol
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Azure Storage Data Object Layer
@@ -17,14 +17,14 @@
 display_name = AzureDOL
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	py2store
+	dol
 	azure-storage-blob
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

