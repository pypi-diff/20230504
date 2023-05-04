# Comparing `tmp/kmlb-0.0.91.tar.gz` & `tmp/kmlb-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmlb-0.0.91.tar", last modified: Thu Apr 27 00:43:00 2023, max compression
+gzip compressed data, was "kmlb-0.0.92.tar", last modified: Thu May  4 21:22:46 2023, max compression
```

## Comparing `kmlb-0.0.91.tar` & `kmlb-0.0.92.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 00:43:00.063889 kmlb-0.0.91/
--rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.91/LICENSE.md
--rw-rw-rw-   0        0        0    38527 2023-04-27 00:43:00.063889 kmlb-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 00:43:00.051889 kmlb-0.0.91/kmlb/
--rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.91/kmlb/__init__.py
--rw-rw-rw-   0        0        0    42713 2023-04-27 00:42:01.000000 kmlb-0.0.91/kmlb/base.py
--rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.91/kmlb/gis_basics.py
--rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.91/kmlb/shapes.py
-drwxrwxrwx   0        0        0        0 2023-04-27 00:43:00.062895 kmlb-0.0.91/kmlb.egg-info/
--rw-rw-rw-   0        0        0    38527 2023-04-27 00:43:00.000000 kmlb-0.0.91/kmlb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-27 00:43:00.000000 kmlb-0.0.91/kmlb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 00:43:00.000000 kmlb-0.0.91/kmlb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 00:43:00.000000 kmlb-0.0.91/kmlb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 00:43:00.063889 kmlb-0.0.91/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-27 00:42:01.000000 kmlb-0.0.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.059504 kmlb-0.0.92/
+-rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.92/LICENSE.md
+-rw-rw-rw-   0        0        0    38527 2023-05-04 21:22:46.058053 kmlb-0.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.92/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.034390 kmlb-0.0.92/kmlb/
+-rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.92/kmlb/__init__.py
+-rw-rw-rw-   0        0        0    43022 2023-05-04 21:17:54.000000 kmlb-0.0.92/kmlb/base.py
+-rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.92/kmlb/gis_basics.py
+-rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.92/kmlb/shapes.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.058053 kmlb-0.0.92/kmlb.egg-info/
+-rw-rw-rw-   0        0        0    38527 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 21:22:46.059504 kmlb-0.0.92/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-04 21:15:06.000000 kmlb-0.0.92/setup.py
```

### Comparing `kmlb-0.0.91/LICENSE.md` & `kmlb-0.0.92/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.91/PKG-INFO` & `kmlb-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.91
+Version: 0.0.92
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.91/README.md` & `kmlb-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.91/kmlb/base.py` & `kmlb-0.0.92/kmlb/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Functions for creating KML files.
 """
 
 import xml.etree.ElementTree as ET
 from pathlib import Path
 import zipfile
+import io
 
 
 def altitude_modes(altitude_mode='CTG'):
     """
     Expands an abbreviated altitude mode to its full length name.
 
     INPUT:
@@ -1196,15 +1197,15 @@
     # Image Default Camera Angle
     if camera is not None:
         overlay.append(camera)
 
     return overlay
 
 
-def kmz(kmz_name, kmls, path, files_as_bytes=None, **kwargs):
+def kmz(kmz_name, kmls, path=None, files_as_bytes=None, **kwargs):
     """
     Creates a KMZ file.
 
        OVERVIEW:
            Creates a KMZ file that can contain KMLs and files such as images.
 
        INPUTS:
@@ -1218,34 +1219,35 @@
                 Note: The file path should end '.kmz'
             files_as_bytes (Tuple) [Optional]:
                  (desitnation path of file within KMZ root, data as bytes)
             kwargs
                 Any argument accepted by the kml function
 
        OUTPUT:
-           kml_string (String):
-            xml string of kml file
+           kmz_buffer (Bytes):
+            KMZ file as bytes
 
        Parameters
        ----------
        kmz_name: str
        kmls: list[tuple]
        path: str
        files_as_bytes: list[tuple]
        kwargs
 
        Returns
        -------
-       network_link : element
+       kmz_buffer : Bytes
 
     """
 
     network_link_elements = list()
+    kmz_buffer = io.BytesIO()
 
-    with zipfile.ZipFile(path, 'w') as zf:
+    with zipfile.ZipFile(kmz_buffer, 'w') as zf:
         for count, doc in enumerate(kmls):
             name = doc[0]
             data = doc[1].encode()
             folder_type = doc[2]
             doc_path = f"kmls/doc_{count}.kml"
             zf.writestr(doc_path, data)
             nl = network_link(name, doc_path, folder_type=folder_type)
@@ -1255,7 +1257,18 @@
             for fb in files_as_bytes:
                 file_path = fb[0]
                 data = fb[1]
                 zf.writestr(file_path, data)
 
         index_k = kml(kmz_name, network_link_elements, **kwargs).encode()
         zf.writestr("doc.kml", index_k)
+
+    if path is not None:
+        filepath = Path(path)
+        filepath.parent.mkdir(parents=True, exist_ok=True)
+
+        with filepath.open('wb') as f:
+            f.write(kmz_buffer.getvalue())
+    else:
+        pass
+
+    return kmz_buffer.getvalue()
```

### Comparing `kmlb-0.0.91/kmlb/gis_basics.py` & `kmlb-0.0.92/kmlb/gis_basics.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.91/kmlb/shapes.py` & `kmlb-0.0.92/kmlb/shapes.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.91/kmlb.egg-info/PKG-INFO` & `kmlb-0.0.92/kmlb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.91
+Version: 0.0.92
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.91/setup.py` & `kmlb-0.0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmlb",
-    version="0.0.91",
+    version="0.0.92",
     author="HFM3",
     description="A Straightforward Google Earth KML Builder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HFM3/kmlb",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "images", "art"]),
     classifiers=[
```

