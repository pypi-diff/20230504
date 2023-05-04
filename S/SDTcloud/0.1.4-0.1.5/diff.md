# Comparing `tmp/SDTcloud-0.1.4.tar.gz` & `tmp/SDTcloud-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.4.tar", last modified: Thu May  4 07:44:18 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.5.tar", last modified: Thu May  4 07:45:17 2023, max compression
```

## Comparing `SDTcloud-0.1.4.tar` & `SDTcloud-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:44:18.291878 SDTcloud-0.1.4/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:44:18.291748 SDTcloud-0.1.4/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.4/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:44:18.290874 SDTcloud-0.1.4/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.4/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    11079 2023-05-04 07:44:06.000000 SDTcloud-0.1.4/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:44:18.291554 SDTcloud-0.1.4/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:44:18.000000 SDTcloud-0.1.4/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 07:44:18.000000 SDTcloud-0.1.4/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 07:44:18.000000 SDTcloud-0.1.4/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 07:44:18.000000 SDTcloud-0.1.4/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 07:44:18.291913 SDTcloud-0.1.4/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 07:44:15.000000 SDTcloud-0.1.4/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.789922 SDTcloud-0.1.5/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:45:17.789771 SDTcloud-0.1.5/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.5/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.788612 SDTcloud-0.1.5/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.5/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    11080 2023-05-04 07:45:04.000000 SDTcloud-0.1.5/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.789562 SDTcloud-0.1.5/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 07:45:17.789956 SDTcloud-0.1.5/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 07:45:14.000000 SDTcloud-0.1.5/setup.py
```

### Comparing `SDTcloud-0.1.4/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.5/SDTcloud/sdtcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             print("No Content!!!, Status: 204")
 
     def exceptionHandle(self, responseData, subtype):
         resp_dict = json.loads(responseData.content)
         if subtype == "500":
             errFormat = {
                 "timestamp": resp_dict['timestamp'],
-                "code": responseData.status_code
+                "code": responseData.status_code,
                 "error": resp_dict['error'],
                 "message": resp_dict['error']
             }
         else:
             errFormat = {
                 "timestamp": resp_dict['timestamp'],
                 "code": resp_dict['code'],
```

### Comparing `SDTcloud-0.1.4/setup.py` & `SDTcloud-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.4",
+    version="0.1.5",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

