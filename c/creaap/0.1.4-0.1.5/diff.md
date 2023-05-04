# Comparing `tmp/creaap-0.1.4.tar.gz` & `tmp/creaap-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creaap-0.1.4.tar", last modified: Wed Apr 26 12:30:20 2023, max compression
+gzip compressed data, was "creaap-0.1.5.tar", last modified: Thu May  4 13:47:27 2023, max compression
```

## Comparing `creaap-0.1.4.tar` & `creaap-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     1051 2023-04-26 12:29:40.000000 creaap-0.1.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       39 2023-04-26 12:29:40.000000 creaap-0.1.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)    11746 2023-04-26 12:30:20.087722 creaap-0.1.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11047 2023-04-26 12:29:40.000000 creaap-0.1.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap/
--rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3797 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/formats.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1690 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/io.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5784 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap/spatial/
--rw-r--r--   0 vsts      (1001) docker     (123)      271 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/spatial/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    49041 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts0
--rw-r--r--   0 vsts      (1001) docker     (123)    80472 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts1
--rw-r--r--   0 vsts      (1001) docker     (123)   126320 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts2
--rw-r--r--   0 vsts      (1001) docker     (123)   288809 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts3
--rw-r--r--   0 vsts      (1001) docker     (123)    10355 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/match.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7559 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/storage/
--rw-r--r--   0 vsts      (1001) docker     (123)      197 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8318 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/blob.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6705 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9152 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/table.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9799 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/users/aad.py
--rw-r--r--   0 vsts      (1001) docker     (123)      743 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)    11746 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      146 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        7 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-26 12:30:20.087722 creaap-0.1.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-04-26 12:29:40.000000 creaap-0.1.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.301768 creaap-0.1.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1051 2023-05-04 13:46:39.000000 creaap-0.1.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       39 2023-05-04 13:46:39.000000 creaap-0.1.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)    11797 2023-05-04 13:47:27.301768 creaap-0.1.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11047 2023-05-04 13:46:39.000000 creaap-0.1.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.297768 creaap-0.1.5/creaap/
+-rw-r--r--   0 vsts      (1001) docker     (123)      450 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3797 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/formats.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1690 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/io.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5784 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.297768 creaap-0.1.5/creaap/spatial/
+-rw-r--r--   0 vsts      (1001) docker     (123)      271 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.297768 creaap-0.1.5/creaap/spatial/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   114975 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/data/nuts0
+-rw-r--r--   0 vsts      (1001) docker     (123)   169486 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/data/nuts1
+-rw-r--r--   0 vsts      (1001) docker     (123)   236333 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/data/nuts2
+-rw-r--r--   0 vsts      (1001) docker     (123)   456454 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/data/nuts3
+-rw-r--r--   0 vsts      (1001) docker     (123)    10414 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7579 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/spatial/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.301768 creaap-0.1.5/creaap/storage/
+-rw-r--r--   0 vsts      (1001) docker     (123)      197 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8318 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/storage/blob.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6705 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/storage/file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9152 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/storage/table.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.301768 creaap-0.1.5/creaap/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9799 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/users/aad.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      743 2023-05-04 13:46:39.000000 creaap-0.1.5/creaap/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 13:47:27.297768 creaap-0.1.5/creaap.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11797 2023-05-04 13:47:27.000000 creaap-0.1.5/creaap.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-05-04 13:47:27.000000 creaap-0.1.5/creaap.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 13:47:27.000000 creaap-0.1.5/creaap.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      146 2023-05-04 13:47:27.000000 creaap-0.1.5/creaap.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        7 2023-05-04 13:47:27.000000 creaap-0.1.5/creaap.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-04 13:47:27.301768 creaap-0.1.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-04 13:46:39.000000 creaap-0.1.5/setup.py
```

### Comparing `creaap-0.1.4/LICENSE` & `creaap-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/PKG-INFO` & `creaap-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.4
+Version: 0.1.5
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CREA Applications in Python kit
```

### Comparing `creaap-0.1.4/README.md` & `creaap-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/formats.py` & `creaap-0.1.5/creaap/formats.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/io.py` & `creaap-0.1.5/creaap/io.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/models.py` & `creaap-0.1.5/creaap/models.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/spatial/match.py` & `creaap-0.1.5/creaap/spatial/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         -------
         None
         
         '''
         self.g=[]
         if shapefile:
             for s in shapefile.shapes():
-                self.g.append(wkt.loads(pygeoif.geometry.as_shape(s).wkt))
+                self.g.append(shape(s))
         else:
             if geometries is not None:
                 for gm in geometries:
                     if isinstance(gm, str):
                         try: 
                             self.g.append(wkt.loads(gm))
                         except:
@@ -83,14 +83,16 @@
                     else:
                         raise TypeError("geometries must be either WKT strings or Shapely geometries, found " + str(type(gm)))
         # build the index
         self.index = STRtree(self.g)
         if isinstance(labels, str):
             for record in shapefile.records():
                 self.labels.append(record.as_dict()[labels])
+        elif isinstance (labels, list):
+            self.labels = labels
         elif isinstance(labels, Iterable) or isinstance(labels, Collection):
             self.labels = list(labels)
         else:
             raise TypeError("labels can be either a field in the Shapefile or a list of values")
               
 
     def get_intersection(self, geometry_wkt):
@@ -107,16 +109,17 @@
         list
             labels of intersecting geometries
         '''
         query_geom =wkt.loads(geometry_wkt)
         result = self.index.query(query_geom)
         out_idxs=[]
         for r in result:
-            if r.intersects(query_geom):
-                out_idxs.append(self.g.index(r))
+            res_geom = self.g[r]
+            if res_geom.intersects(query_geom):
+                out_idxs.append(r)
         return [self.labels[i] for i in out_idxs]
     
     def get_intersection_percentages(self, geometry_wkt, areas=None):
         '''
         Returns the labels of the indexed geometries which intesrect the query geometry
         and their intersection percentages.
 
@@ -160,15 +163,15 @@
         Returns
         -------
         string
             label of the nearest geometry
         '''
         query_geom =wkt.loads(geometry_wkt)
         result = self.index.nearest(query_geom)
-        return self.labels[self.g.index(result)]
+        return self.labels[result]
     
     def save(self, path):
         '''serializes the SpatialMatcher instance to a file
         
         Parameters
         ----------
         path: string
@@ -291,9 +294,9 @@
     ----------
     nuts_shapefile: a shapefile object
     '''
     shapes, names = _get_nuts_level(nuts_shapefile, nuts_level, attribute) # get correct level shapefile
     shp , _ , dbf = convert_goem(shapes,input_projection, output_projection, names, flip_coords=False)
     wgs84_shapes = shapefile.Reader(shp=shp, dbf=dbf)
     matcher = SpatialMatcher()
-    matcher.build_spatial_index(wgs84_shapes, names)
+    matcher.build_spatial_index(wgs84_shapes, labels = names)
     return matcher
```

### Comparing `creaap-0.1.4/creaap/spatial/utils.py` & `creaap-0.1.5/creaap/spatial/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         if names is None:
             wgs_shp.record(str(idx))
         else:
             wgs_shp.record([names[idx]])
     wgs_shp.close()
     return shp , shx , dbf
 
-def read_shape_from_zip(package, name):
+def read_shape_from_zip(package:zipfile.ZipFile, name:str):
 	'''SHP files are often packaged as ZIP files, so this function extracts
 	Shapes from Zipfiles.
     
     Parameters
     ----------
     package: zipfile.ZipFile
         the zip file, already openend with the zipfile package
```

### Comparing `creaap-0.1.4/creaap/storage/blob.py` & `creaap-0.1.5/creaap/storage/blob.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/storage/file.py` & `creaap-0.1.5/creaap/storage/file.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/storage/table.py` & `creaap-0.1.5/creaap/storage/table.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/users/aad.py` & `creaap-0.1.5/creaap/users/aad.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap/utils.py` & `creaap-0.1.5/creaap/utils.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/creaap.egg-info/PKG-INFO` & `creaap-0.1.5/creaap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.4
+Version: 0.1.5
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CREA Applications in Python kit
```

### Comparing `creaap-0.1.4/creaap.egg-info/SOURCES.txt` & `creaap-0.1.5/creaap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creaap-0.1.4/setup.py` & `creaap-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
    name='creaap',
-   version='0.1.4',
+   version='0.1.5',
    description='CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.',
    author='CREA',
    author_email='dario.denart@crea.gov.it',
    packages=['creaap', 'creaap.spatial', 'creaap.storage', 'creaap.users'],
    classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        #"Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
-   install_requires=['azure-storage-blob','azure-storage-file-share','azure-data-tables','Shapely==1.8.4','pytz','pygeoif',
+   install_requires=['azure-storage-blob','azure-storage-file-share','azure-data-tables','Shapely>=2.0.0','pytz','pygeoif',
                      'numpy','scipy','scikit-learn','numpy','pyshp','pandas','pyproj', 'msal'], #external packages as dependencies
    include_package_data=True, # to be able to access data files
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit"
 )
```

