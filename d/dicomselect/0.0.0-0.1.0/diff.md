# Comparing `tmp/dicomselect-0.0.0.tar.gz` & `tmp/dicomselect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomselect-0.0.0.tar", last modified: Wed May  3 13:09:18 2023, max compression
+gzip compressed data, was "dicomselect-0.1.0.tar", last modified: Thu May  4 10:52:25 2023, max compression
```

## Comparing `dicomselect-0.0.0.tar` & `dicomselect-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:09:18.102313 dicomselect-0.0.0/
--rw-rw-rw-   0        0        0     1082 2023-04-18 16:33:48.000000 dicomselect-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      798 2023-05-03 13:09:18.102313 dicomselect-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-18 16:33:48.000000 dicomselect-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 13:09:18.081679 dicomselect-0.0.0/dicomselect/
--rw-rw-rw-   0        0        0       92 2023-05-02 16:40:21.000000 dicomselect-0.0.0/dicomselect/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-05-02 11:37:54.000000 dicomselect-0.0.0/dicomselect/constants.py
--rw-rw-rw-   0        0        0     5350 2023-05-03 08:13:30.000000 dicomselect-0.0.0/dicomselect/database.py
--rw-rw-rw-   0        0        0     2241 2023-05-02 16:40:02.000000 dicomselect-0.0.0/dicomselect/dicom.py
--rw-rw-rw-   0        0        0     1470 2023-05-01 13:30:45.000000 dicomselect-0.0.0/dicomselect/info.py
--rw-rw-rw-   0        0        0     8189 2023-05-02 16:40:16.000000 dicomselect-0.0.0/dicomselect/query.py
--rw-rw-rw-   0        0        0     2740 2023-05-02 16:40:11.000000 dicomselect-0.0.0/dicomselect/queryfactory.py
--rw-rw-rw-   0        0        0    15090 2023-05-02 16:40:07.000000 dicomselect-0.0.0/dicomselect/reader.py
--rw-rw-rw-   0        0        0   203115 2023-05-02 16:33:47.000000 dicomselect-0.0.0/dicomselect/tags_generated.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:09:18.101146 dicomselect-0.0.0/dicomselect.egg-info/
--rw-rw-rw-   0        0        0      798 2023-05-03 13:09:17.000000 dicomselect-0.0.0/dicomselect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-03 13:09:17.000000 dicomselect-0.0.0/dicomselect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:09:17.000000 dicomselect-0.0.0/dicomselect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 08:03:05.000000 dicomselect-0.0.0/dicomselect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      255 2023-05-03 13:09:17.000000 dicomselect-0.0.0/dicomselect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 13:09:17.000000 dicomselect-0.0.0/dicomselect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      930 2023-05-03 13:09:18.105819 dicomselect-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-01 07:59:57.000000 dicomselect-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.482298 dicomselect-0.1.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-18 16:33:48.000000 dicomselect-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      798 2023-05-04 10:52:25.482298 dicomselect-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-18 16:33:48.000000 dicomselect-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.463300 dicomselect-0.1.0/dicomselect/
+-rw-rw-rw-   0        0        0       92 2023-05-02 16:40:21.000000 dicomselect-0.1.0/dicomselect/__init__.py
+-rw-rw-rw-   0        0        0     1358 2023-05-02 11:37:54.000000 dicomselect-0.1.0/dicomselect/constants.py
+-rw-rw-rw-   0        0        0     5350 2023-05-03 08:13:30.000000 dicomselect-0.1.0/dicomselect/database.py
+-rw-rw-rw-   0        0        0     2239 2023-05-04 10:50:11.000000 dicomselect-0.1.0/dicomselect/dicom.py
+-rw-rw-rw-   0        0        0     1470 2023-05-01 13:30:45.000000 dicomselect-0.1.0/dicomselect/info.py
+-rw-rw-rw-   0        0        0     8189 2023-05-02 16:40:16.000000 dicomselect-0.1.0/dicomselect/query.py
+-rw-rw-rw-   0        0        0     2740 2023-05-02 16:40:11.000000 dicomselect-0.1.0/dicomselect/queryfactory.py
+-rw-rw-rw-   0        0        0    15090 2023-05-02 16:40:07.000000 dicomselect-0.1.0/dicomselect/reader.py
+-rw-rw-rw-   0        0        0   203115 2023-05-02 16:33:47.000000 dicomselect-0.1.0/dicomselect/tags_generated.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.480798 dicomselect-0.1.0/dicomselect.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 08:03:05.000000 dicomselect-0.1.0/dicomselect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      255 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      930 2023-05-04 10:52:25.486799 dicomselect-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-03 13:10:14.000000 dicomselect-0.1.0/setup.py
```

### Comparing `dicomselect-0.0.0/LICENSE` & `dicomselect-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/PKG-INFO` & `dicomselect-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.0.0
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author: 
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Platform: unix
```

### Comparing `dicomselect-0.0.0/dicomselect/constants.py` & `dicomselect-0.1.0/dicomselect/constants.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/database.py` & `dicomselect-0.1.0/dicomselect/database.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/dicom.py` & `dicomselect-0.1.0/dicomselect/dicom.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from dicomselect.tags_generated import tags_generated, version
 from dicomselect.constants import DEFAULT_DICOM_TAGS
 
 
 def convert_AS(value: str):
     t = value[3]
     value = int(value[:3])
-    if t == 'Y':
-        value *= 365
+    if t == 'D':
+        value /= 365
     elif t == 'M':
-        value *= 30
+        value /= 12
     elif t == 'W':
-        value *= 7
+        value /= 52
     return value
 
 
 def convert_DT(value: str):
     value = value.replace(' ', '')
     r = re.search(r'^(\d{14}).?(\d+)?', value)
     return r.group()
 
 
 # https://dicom.nema.org/medical/dicom/current/output/chtml/part05/sect_6.2.html
 VR = {
-    "AS": ("INTEGER", convert_AS),
+    "AS": ("REAL", convert_AS),
     "DA": "INTEGER",
     "DT": ("REAL", convert_DT),
     "DS": "REAL",
     "FL": "REAL",
     "FD": "REAL",
     "IS": "INTEGER",
     "SL": "INTEGER",
```

### Comparing `dicomselect-0.0.0/dicomselect/info.py` & `dicomselect-0.1.0/dicomselect/info.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/query.py` & `dicomselect-0.1.0/dicomselect/query.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/queryfactory.py` & `dicomselect-0.1.0/dicomselect/queryfactory.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/reader.py` & `dicomselect-0.1.0/dicomselect/reader.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect/tags_generated.py` & `dicomselect-0.1.0/dicomselect/tags_generated.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/dicomselect.egg-info/PKG-INFO` & `dicomselect-0.1.0/dicomselect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.0.0
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author: 
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Platform: unix
```

### Comparing `dicomselect-0.0.0/dicomselect.egg-info/SOURCES.txt` & `dicomselect-0.1.0/dicomselect.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 ./dicomselect/query.py
 ./dicomselect/queryfactory.py
 ./dicomselect/reader.py
 ./dicomselect/tags_generated.py
 dicomselect/__init__.py
 dicomselect/constants.py
 dicomselect/database.py
+dicomselect/dicom.py
+dicomselect/info.py
 dicomselect/query.py
+dicomselect/queryfactory.py
 dicomselect/reader.py
+dicomselect/tags_generated.py
 dicomselect.egg-info/PKG-INFO
 dicomselect.egg-info/SOURCES.txt
 dicomselect.egg-info/dependency_links.txt
 dicomselect.egg-info/not-zip-safe
 dicomselect.egg-info/requires.txt
 dicomselect.egg-info/top_level.txt
```

### Comparing `dicomselect-0.0.0/setup.cfg` & `dicomselect-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dicomselect-0.0.0/setup.py` & `dicomselect-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name='dicomselect',
-        version='0.0.0',
+        version='0.1.0',
         author_email='Stan.Noordman@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/dicomselect',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dicomselect"
         },
```

