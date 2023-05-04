# Comparing `tmp/SDTcloud-0.1.1.tar.gz` & `tmp/SDTcloud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.1.tar", last modified: Thu May  4 06:25:10 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.2.tar", last modified: Thu May  4 06:26:21 2023, max compression
```

## Comparing `SDTcloud-0.1.1.tar` & `SDTcloud-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:25:10.723526 SDTcloud-0.1.1/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:25:10.723317 SDTcloud-0.1.1/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.1/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:25:10.721496 SDTcloud-0.1.1/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.1/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    10543 2023-05-04 06:24:52.000000 SDTcloud-0.1.1/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:25:10.722660 SDTcloud-0.1.1/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:25:10.000000 SDTcloud-0.1.1/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 06:25:10.000000 SDTcloud-0.1.1/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 06:25:10.000000 SDTcloud-0.1.1/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 06:25:10.000000 SDTcloud-0.1.1/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 06:25:10.723562 SDTcloud-0.1.1/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 06:25:07.000000 SDTcloud-0.1.1/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.950447 SDTcloud-0.1.2/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:26:21.950311 SDTcloud-0.1.2/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.2/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.949254 SDTcloud-0.1.2/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.2/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    10543 2023-05-04 06:26:04.000000 SDTcloud-0.1.2/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 06:26:21.950092 SDTcloud-0.1.2/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 06:26:21.000000 SDTcloud-0.1.2/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 06:26:21.950485 SDTcloud-0.1.2/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 06:26:17.000000 SDTcloud-0.1.2/setup.py
```

### Comparing `SDTcloud-0.1.1/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.2/SDTcloud/sdtcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         respStatus, returnMessage = self.checkStatusCode(response.status_code)
 
         if respStatus == 0:
             exceptionHandle(response)
         
         result = json.loads(response.content)
 
-        self.userToken = f"Bearer {result["accessToken"]}"
+        self.userToken = f"Bearer {result['accessToken']}"
 
         print(returnMessage)
 
     # 스토리지 등록
     def create_storage(self, name, tag):
         """ Create storage in stackbase.
```

### Comparing `SDTcloud-0.1.1/setup.py` & `SDTcloud-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.1",
+    version="0.1.2",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

