# Comparing `tmp/mctools-1.2.1.tar.gz` & `tmp/mctools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctools-1.2.1.tar", last modified: Sat Apr  8 20:11:14 2023, max compression
+gzip compressed data, was "mctools-1.2.2.tar", last modified: Thu May  4 21:55:16 2023, max compression
```

## Comparing `mctools-1.2.1.tar` & `mctools-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.235259 mctools-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 20:10:58.000000 mctools-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 20:10:58.000000 mctools-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-04-08 20:11:14.235259 mctools-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-08 20:10:58.000000 mctools-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 20:10:58.000000 mctools-1.2.1/mcli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.231259 mctools-1.2.1/mctools/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/formattertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    32274 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/mclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.235259 mctools-1.2.1/mctools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:11:14.235259 mctools-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-04-08 20:10:58.000000 mctools-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:55:16.414484 mctools-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:54:58.000000 mctools-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 21:54:58.000000 mctools-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-04 21:55:16.414484 mctools-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-04 21:54:58.000000 mctools-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 21:54:58.000000 mctools-1.2.2/mcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:55:16.410484 mctools-1.2.2/mctools/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/formattertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32274 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/mclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-05-04 21:54:58.000000 mctools-1.2.2/mctools/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:55:16.414484 mctools-1.2.2/mctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 21:55:16.000000 mctools-1.2.2/mctools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:55:16.414484 mctools-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-04 21:54:58.000000 mctools-1.2.2/setup.py
```

### Comparing `mctools-1.2.1/LICENSE` & `mctools-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/PKG-INFO` & `mctools-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctools
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python implementations of common Minecraft protocols.
 Home-page: https://github.com/Owen-Cochell/mctools
 Author: Owen Cochell
 Author-email: owencochell@hotmail.com
 Project-URL: Bug Reports, https://github.com/Owen-Cochell/mctools/issues
 Project-URL: Source, https://github.com/Owen-Cochell/mctools
 Project-URL: Documentation, https://mctools.readthedocs.io/
@@ -163,14 +163,18 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+### 1.2.2
+
+Removed some debugging print statements.
+
 ## 1.2.1
 
 We now correctly disable length checking in RCONClient if specified by the user.
 
 The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
 This change applies to all clients, as they all use this method.
```

### Comparing `mctools-1.2.1/README.md` & `mctools-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,18 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+### 1.2.2
+
+Removed some debugging print statements.
+
 ## 1.2.1
 
 We now correctly disable length checking in RCONClient if specified by the user.
 
 The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
 This change applies to all clients, as they all use this method.
```

### Comparing `mctools-1.2.1/mctools/__main__.py` & `mctools-1.2.2/mctools/__main__.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/encoding.py` & `mctools-1.2.2/mctools/encoding.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/errors.py` & `mctools-1.2.2/mctools/errors.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/formattertools.py` & `mctools-1.2.2/mctools/formattertools.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/mclient.py` & `mctools-1.2.2/mctools/mclient.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/packet.py` & `mctools-1.2.2/mctools/packet.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.1/mctools/protocol.py` & `mctools-1.2.2/mctools/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,14 @@
 
         while len(byts) < length:
 
             last = self.sock.recv(length - len(byts))
 
             byts = byts + last
 
-            print(byts)
-
             if last == b'':
 
                 # We received nothing, lets close this connection:
 
                 self.stop()
 
                 # Raise the 'ConnectionClosed' exception:
```

### Comparing `mctools-1.2.1/mctools.egg-info/PKG-INFO` & `mctools-1.2.2/mctools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctools
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python implementations of common Minecraft protocols.
 Home-page: https://github.com/Owen-Cochell/mctools
 Author: Owen Cochell
 Author-email: owencochell@hotmail.com
 Project-URL: Bug Reports, https://github.com/Owen-Cochell/mctools/issues
 Project-URL: Source, https://github.com/Owen-Cochell/mctools
 Project-URL: Documentation, https://mctools.readthedocs.io/
@@ -163,14 +163,18 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+### 1.2.2
+
+Removed some debugging print statements.
+
 ## 1.2.1
 
 We now correctly disable length checking in RCONClient if specified by the user.
 
 The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
 This change applies to all clients, as they all use this method.
```

### Comparing `mctools-1.2.1/setup.py` & `mctools-1.2.2/setup.py`

 * *Files identical despite different names*

