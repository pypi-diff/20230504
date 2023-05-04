# Comparing `tmp/pyowletapi-2023.5.4.tar.gz` & `tmp/pyowletapi-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.5.4.tar", last modified: Wed May  3 14:50:57 2023, max compression
+gzip compressed data, was "pyowletapi-2023.5.5.tar", last modified: Wed May  3 15:01:48 2023, max compression
```

## Comparing `pyowletapi-2023.5.4.tar` & `pyowletapi-2023.5.5.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.462345 pyowletapi-2023.5.4/
--rw-rw-rw-   0        0        0     2175 2023-05-03 14:50:57.463343 pyowletapi-2023.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.415345 pyowletapi-2023.5.4/pyowletapi/
-drwxrwxrwx   0        0        0        0 2023-05-03 14:50:57.460345 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     2175 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:50:57.000000 pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-03 14:50:57.465343 pyowletapi-2023.5.4/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-05-03 14:50:49.000000 pyowletapi-2023.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.721639 pyowletapi-2023.5.5/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 15:01:48.721639 pyowletapi-2023.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-03 15:01:48.724639 pyowletapi-2023.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-03 15:00:29.000000 pyowletapi-2023.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.624933 pyowletapi-2023.5.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.651932 pyowletapi-2023.5.5/src/pyowletapi/
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/src/pyowletapi/__init__.py
+-rw-rw-rw-   0        0        0    10013 2023-05-03 10:53:08.000000 pyowletapi-2023.5.5/src/pyowletapi/api.py
+-rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.5/src/pyowletapi/exceptions.py
+-rw-rw-rw-   0        0        0     4281 2023-05-03 14:32:12.000000 pyowletapi-2023.5.5/src/pyowletapi/owlet.py
+-rw-rw-rw-   0        0        0     6935 2023-05-02 14:41:49.000000 pyowletapi-2023.5.5/src/pyowletapi/sock.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.718638 pyowletapi-2023.5.5/src/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     2175 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/top_level.txt
```

### Comparing `pyowletapi-2023.5.4/PKG-INFO` & `pyowletapi-2023.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.4
+Version: 2023.5.5
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

### Comparing `pyowletapi-2023.5.4/README.md` & `pyowletapi-2023.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.4/pyowletapi/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.5.5/src/pyowletapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.4
+Version: 2023.5.5
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

### Comparing `pyowletapi-2023.5.4/setup.py` & `pyowletapi-2023.5.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    
     name="pyowletapi",
-    version="2023.05.4",
+    version="2023.05.5",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
     classifiers=[ 
         "License :: OSI Approved :: MIT License",        
         "Programming Language :: Python :: 3.9",
     ],
     
     keywords="owlet, api, baby",
-    package_dir={"": "pyowletapi"}, 
-    packages=find_packages(where="pyowletapi"), 
+    package_dir={"": "src"}, 
+    packages=find_packages(where="src"), 
     python_requires=">=3.9",
     
     install_requires=["aiohttp"], 
 )
```

