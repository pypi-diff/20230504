# Comparing `tmp/onionrequests-0.0.1.tar.gz` & `tmp/onionrequests-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onionrequests-0.0.1.tar", last modified: Thu May  4 06:44:58 2023, max compression
+gzip compressed data, was "onionrequests-0.0.2.tar", last modified: Thu May  4 17:13:13 2023, max compression
```

## Comparing `onionrequests-0.0.1.tar` & `onionrequests-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 06:44:58.099187 onionrequests-0.0.1/
--rw-rw-r--   0 esamford  (1000) esamford  (1000)     1070 2023-05-03 22:31:31.000000 onionrequests-0.0.1/LICENSE
--rw-rw-r--   0 esamford  (1000) esamford  (1000)      128 2023-05-03 23:26:01.000000 onionrequests-0.0.1/MANIFEST.in
--rw-rw-r--   0 esamford  (1000) esamford  (1000)    12737 2023-05-04 06:44:58.099187 onionrequests-0.0.1/PKG-INFO
--rw-rw-r--   0 esamford  (1000) esamford  (1000)    12387 2023-05-04 06:18:44.000000 onionrequests-0.0.1/README.md
-drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 06:44:58.095185 onionrequests-0.0.1/onionrequests/
--rw-rw-r--   0 esamford  (1000) esamford  (1000)    12099 2023-04-25 06:52:15.000000 onionrequests-0.0.1/onionrequests/OnionQueue.py
--rwxrwxr-x   0 esamford  (1000) esamford  (1000)     1236 2023-04-20 22:03:29.000000 onionrequests-0.0.1/onionrequests/OnionSession.py
--rwxrwxr-x   0 esamford  (1000) esamford  (1000)       74 2023-05-04 06:09:07.000000 onionrequests-0.0.1/onionrequests/__init__.py
--rw-rw-r--   0 esamford  (1000) esamford  (1000)     3276 2023-04-27 15:51:14.000000 onionrequests-0.0.1/onionrequests/tests.py
-drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 06:44:58.099187 onionrequests-0.0.1/onionrequests.egg-info/
--rw-rw-r--   0 esamford  (1000) esamford  (1000)    12737 2023-05-04 06:44:58.000000 onionrequests-0.0.1/onionrequests.egg-info/PKG-INFO
--rw-rw-r--   0 esamford  (1000) esamford  (1000)      362 2023-05-04 06:44:58.000000 onionrequests-0.0.1/onionrequests.egg-info/SOURCES.txt
--rw-rw-r--   0 esamford  (1000) esamford  (1000)        1 2023-05-04 06:44:58.000000 onionrequests-0.0.1/onionrequests.egg-info/dependency_links.txt
--rw-rw-r--   0 esamford  (1000) esamford  (1000)       16 2023-05-04 06:44:58.000000 onionrequests-0.0.1/onionrequests.egg-info/requires.txt
--rw-rw-r--   0 esamford  (1000) esamford  (1000)       14 2023-05-04 06:44:58.000000 onionrequests-0.0.1/onionrequests.egg-info/top_level.txt
--rw-rw-r--   0 esamford  (1000) esamford  (1000)      103 2023-05-04 06:42:44.000000 onionrequests-0.0.1/pyproject.toml
--rwxrwxr-x   0 esamford  (1000) esamford  (1000)       27 2023-04-20 22:03:29.000000 onionrequests-0.0.1/requirements.txt
--rw-rw-r--   0 esamford  (1000) esamford  (1000)      480 2023-05-04 06:44:58.099187 onionrequests-0.0.1/setup.cfg
+drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 17:13:13.027988 onionrequests-0.0.2/
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)     1070 2023-05-03 22:31:31.000000 onionrequests-0.0.2/LICENSE
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)      128 2023-05-03 23:26:01.000000 onionrequests-0.0.2/MANIFEST.in
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)    12737 2023-05-04 17:13:13.027988 onionrequests-0.0.2/PKG-INFO
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)    12387 2023-05-04 06:18:44.000000 onionrequests-0.0.2/README.md
+drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 17:13:13.015988 onionrequests-0.0.2/onionrequests/
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)    12099 2023-04-25 06:52:15.000000 onionrequests-0.0.2/onionrequests/OnionQueue.py
+-rwxrwxr-x   0 esamford  (1000) esamford  (1000)     1015 2023-05-04 17:11:59.000000 onionrequests-0.0.2/onionrequests/OnionSession.py
+-rwxrwxr-x   0 esamford  (1000) esamford  (1000)       74 2023-05-04 06:09:07.000000 onionrequests-0.0.2/onionrequests/__init__.py
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)     3276 2023-04-27 15:51:14.000000 onionrequests-0.0.2/onionrequests/tests.py
+drwxrwxr-x   0 esamford  (1000) esamford  (1000)        0 2023-05-04 17:13:13.027988 onionrequests-0.0.2/onionrequests.egg-info/
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)    12737 2023-05-04 17:13:12.000000 onionrequests-0.0.2/onionrequests.egg-info/PKG-INFO
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)      362 2023-05-04 17:13:12.000000 onionrequests-0.0.2/onionrequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)        1 2023-05-04 17:13:12.000000 onionrequests-0.0.2/onionrequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)       16 2023-05-04 17:13:12.000000 onionrequests-0.0.2/onionrequests.egg-info/requires.txt
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)       14 2023-05-04 17:13:12.000000 onionrequests-0.0.2/onionrequests.egg-info/top_level.txt
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)      103 2023-05-04 06:42:44.000000 onionrequests-0.0.2/pyproject.toml
+-rwxrwxr-x   0 esamford  (1000) esamford  (1000)       27 2023-04-20 22:03:29.000000 onionrequests-0.0.2/requirements.txt
+-rw-rw-r--   0 esamford  (1000) esamford  (1000)      480 2023-05-04 17:13:13.027988 onionrequests-0.0.2/setup.cfg
```

### Comparing `onionrequests-0.0.1/LICENSE` & `onionrequests-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onionrequests-0.0.1/PKG-INFO` & `onionrequests-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onionrequests
-Version: 0.0.1
+Version: 0.0.2
 Summary: Anonymous HTTP requests via TOR
 Author: Ethan Samford
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `onionrequests-0.0.1/README.md` & `onionrequests-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `onionrequests-0.0.1/onionrequests/OnionQueue.py` & `onionrequests-0.0.2/onionrequests/OnionQueue.py`

 * *Files identical despite different names*

### Comparing `onionrequests-0.0.1/onionrequests/tests.py` & `onionrequests-0.0.2/onionrequests/tests.py`

 * *Files identical despite different names*

### Comparing `onionrequests-0.0.1/onionrequests.egg-info/PKG-INFO` & `onionrequests-0.0.2/onionrequests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onionrequests
-Version: 0.0.1
+Version: 0.0.2
 Summary: Anonymous HTTP requests via TOR
 Author: Ethan Samford
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

