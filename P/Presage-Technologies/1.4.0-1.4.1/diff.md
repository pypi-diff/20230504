# Comparing `tmp/Presage Technologies-1.4.0.tar.gz` & `tmp/Presage Technologies-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Presage Technologies-1.4.0.tar", last modified: Fri Feb 24 17:43:59 2023, max compression
+gzip compressed data, was "dist/Presage Technologies-1.4.1.tar", last modified: Thu May  4 13:34:34 2023, max compression
```

## Comparing `Presage Technologies-1.4.0.tar` & `Presage Technologies-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     8080 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8080 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       49 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/Presage_Technologies.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6579 2023-02-24 17:42:06.000000 Presage Technologies-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/presage_technologies/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-02-24 17:42:06.000000 Presage Technologies-1.4.0/presage_technologies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7507 2023-02-24 17:42:06.000000 Presage Technologies-1.4.0/presage_technologies/physiology.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-24 17:42:06.000000 Presage Technologies-1.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-02-24 17:43:59.000000 Presage Technologies-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-02-24 17:43:57.000000 Presage Technologies-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/Presage_Technologies.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6579 2023-05-04 13:32:11.000000 Presage Technologies-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/presage_technologies/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-04 13:32:11.000000 Presage Technologies-1.4.1/presage_technologies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-05-04 13:32:11.000000 Presage Technologies-1.4.1/presage_technologies/physiology.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-04 13:32:11.000000 Presage Technologies-1.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-04 13:34:34.000000 Presage Technologies-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-04 13:34:33.000000 Presage Technologies-1.4.1/setup.py
```

### Comparing `Presage Technologies-1.4.0/PKG-INFO` & `Presage Technologies-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage Technologies
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python client to interface with Presage Technologies' API services.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_technologies/issues
 Description: # presage_technologies
```

### Comparing `Presage Technologies-1.4.0/Presage_Technologies.egg-info/PKG-INFO` & `Presage Technologies-1.4.1/Presage_Technologies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage-Technologies
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python client to interface with Presage Technologies' API services.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_technologies/issues
 Description: # presage_technologies
```

### Comparing `Presage Technologies-1.4.0/README.md` & `Presage Technologies-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Presage Technologies-1.4.0/presage_technologies/physiology.py` & `Presage Technologies-1.4.1/presage_technologies/physiology.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,22 +54,22 @@
                 self.base_api_url + "/retrieve-data",
                 headers={"x-api-key": self.api_key},
                 json={"id": id},
             )
             if response.status_code == 200:
                 return response.json()
             elif response.status_code == 201:
-                time.sleep(5)
+                time.sleep(1)
             elif response.status_code == 401:
                 logging.warning(
                     "Unauthorized error! Please make sure your API key is correct."
                 )
                 return
             else:
-                time.sleep(30)
+                time.sleep(1)
         return None
 
     def process_loop(self, video_path, preprocess, compress, type, trace=None):
         parts = []
         vid_id = None
         upload_id = None
         urls = []
```

### Comparing `Presage Technologies-1.4.0/setup.py` & `Presage Technologies-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 requirements = ['requests', 'presage_physiology_preprocessing==1.2.1']
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 
 setup(
     name='Presage Technologies',
     version=__version__,
     packages=['presage_technologies'],
     author="Presage Technologies",
     author_email="support@presagetech.com",
```

