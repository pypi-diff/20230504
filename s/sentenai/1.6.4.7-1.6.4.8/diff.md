# Comparing `tmp/sentenai-1.6.4.7.tar.gz` & `tmp/sentenai-1.6.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentenai-1.6.4.7.tar", last modified: Thu May  4 20:21:49 2023, max compression
+gzip compressed data, was "dist/sentenai-1.6.4.8.tar", last modified: Thu May  4 20:28:42 2023, max compression
```

## Comparing `sentenai-1.6.4.7.tar` & `sentenai-1.6.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.7/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.7/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     8918 2023-04-30 01:51:32.000000 sentenai-1.6.4.7/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.7/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.4.7/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.7/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.7/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    19914 2023-05-04 20:20:46.000000 sentenai-1.6.4.7/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-05-04 20:21:23.000000 sentenai-1.6.4.7/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.8/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.8/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     8918 2023-04-30 01:51:32.000000 sentenai-1.6.4.8/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.8/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.4.8/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.8/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.8/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    19900 2023-05-04 20:27:36.000000 sentenai-1.6.4.8/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:28:41.000000 sentenai-1.6.4.8/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-05-04 20:28:41.000000 sentenai-1.6.4.8/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-05-04 20:28:12.000000 sentenai-1.6.4.8/setup.py
```

### Comparing `sentenai-1.6.4.7/LICENSE` & `sentenai-1.6.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/PKG-INFO` & `sentenai-1.6.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.7
+Version: 1.6.4.8
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.7/README.md` & `sentenai-1.6.4.8/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/sentenai/__init__.py` & `sentenai-1.6.4.8/sentenai/__init__.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/sentenai/api.py` & `sentenai-1.6.4.8/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/sentenai/stream/events.py` & `sentenai-1.6.4.8/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/sentenai/stream/metadata.py` & `sentenai-1.6.4.8/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.7/sentenai/stream/streams.py` & `sentenai-1.6.4.8/sentenai/stream/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                     json=data, headers={'Content-Type': 'application/cbor'}, raw=True)
         except:
             counter += 1
             sleep(.1)
         else:
             if resp.status_code > 204:
                 resp.close()
-                raise Exception(f"failed on row {i}, column {k}")
+                raise Exception(f"failed on index")
             resp.close()
             break
 
 
 class Database(API):
     def __init__(self, parent, name, origin):
         self._parent = parent
```

### Comparing `sentenai-1.6.4.7/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.8/sentenai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.7
+Version: 1.6.4.8
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.7/setup.py` & `sentenai-1.6.4.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.7',
+    version='1.6.4.8',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

