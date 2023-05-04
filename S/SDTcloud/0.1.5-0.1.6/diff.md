# Comparing `tmp/SDTcloud-0.1.5.tar.gz` & `tmp/SDTcloud-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.5.tar", last modified: Thu May  4 07:45:17 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.6.tar", last modified: Thu May  4 07:52:30 2023, max compression
```

## Comparing `SDTcloud-0.1.5.tar` & `SDTcloud-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.789922 SDTcloud-0.1.5/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:45:17.789771 SDTcloud-0.1.5/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.5/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.788612 SDTcloud-0.1.5/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.5/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    11080 2023-05-04 07:45:04.000000 SDTcloud-0.1.5/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:45:17.789562 SDTcloud-0.1.5/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 07:45:17.000000 SDTcloud-0.1.5/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 07:45:17.789956 SDTcloud-0.1.5/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 07:45:14.000000 SDTcloud-0.1.5/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:52:30.903010 SDTcloud-0.1.6/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:52:30.902868 SDTcloud-0.1.6/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.6/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:52:30.901834 SDTcloud-0.1.6/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.6/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    11112 2023-05-04 07:51:55.000000 SDTcloud-0.1.6/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 07:52:30.902671 SDTcloud-0.1.6/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 07:52:30.000000 SDTcloud-0.1.6/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 07:52:30.000000 SDTcloud-0.1.6/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 07:52:30.000000 SDTcloud-0.1.6/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 07:52:30.000000 SDTcloud-0.1.6/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 07:52:30.903047 SDTcloud-0.1.6/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 07:52:28.000000 SDTcloud-0.1.6/setup.py
```

### Comparing `SDTcloud-0.1.5/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.6/SDTcloud/sdtcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     def successMessage(self, codeValue):
         if codeValue == 1:
             print("Ok!!!, Status: 200")
         elif codeValue == 2:
             print("Created!!!, Status: 201")
         elif codeValue == 3:
             print("No Content!!!, Status: 204")
+            exit()
+            
 
     def exceptionHandle(self, responseData, subtype):
         resp_dict = json.loads(responseData.content)
         if subtype == "500":
             errFormat = {
                 "timestamp": resp_dict['timestamp'],
                 "code": responseData.status_code,
```

### Comparing `SDTcloud-0.1.5/setup.py` & `SDTcloud-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.5",
+    version="0.1.6",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

