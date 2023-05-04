# Comparing `tmp/pylipd-1.3.1.tar.gz` & `tmp/pylipd-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.3.1.tar", last modified: Thu Apr 20 10:42:32 2023, max compression
+gzip compressed data, was "pylipd-1.3.2.tar", last modified: Thu May  4 15:21:37 2023, max compression
```

## Comparing `pylipd-1.3.1.tar` & `pylipd-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.584532 pylipd-1.3.1/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.1/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:42:32.584582 pylipd-1.3.1/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.1/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.582030 pylipd-1.3.1/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-20 10:37:56.000000 pylipd-1.3.1/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.583072 pylipd-1.3.1/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.1/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.1/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)     7357 2023-04-20 09:59:20.000000 pylipd-1.3.1/pylipd/globals/queries.py
--rw-r--r--   0 varun      (502) staff       (20)    14792 2023-04-20 09:57:33.000000 pylipd-1.3.1/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.1/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.1/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    28453 2023-04-20 10:40:15.000000 pylipd-1.3.1/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)     3349 2023-04-20 10:37:20.000000 pylipd-1.3.1/pylipd/lipd_series.py
--rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.1/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     3009 2023-04-20 07:46:48.000000 pylipd-1.3.1/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)     9324 2023-04-20 10:34:40.000000 pylipd-1.3.1/pylipd/rdf_graph.py
--rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.1/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.583417 pylipd-1.3.1/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.1/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.1/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.1/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     6004 2023-04-20 10:15:46.000000 pylipd-1.3.1/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)      928 2023-04-20 10:13:54.000000 pylipd-1.3.1/pylipd/usage_parallel.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.1/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-20 10:42:32.584433 pylipd-1.3.1/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      689 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.1/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       40 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-20 10:42:32.000000 pylipd-1.3.1/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.1/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      699 2023-04-20 10:42:32.584840 pylipd-1.3.1/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-20 10:37:46.000000 pylipd-1.3.1/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.676397 pylipd-1.3.2/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.2/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-04 15:21:37.676469 pylipd-1.3.2/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.2/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.673875 pylipd-1.3.2/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-21 04:14:36.000000 pylipd-1.3.2/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.674850 pylipd-1.3.2/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.2/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.2/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     7417 2023-05-04 15:18:49.000000 pylipd-1.3.2/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    15000 2023-04-21 04:08:45.000000 pylipd-1.3.2/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.2/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.2/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    29337 2023-05-04 15:18:49.000000 pylipd-1.3.2/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)     3349 2023-04-20 10:37:20.000000 pylipd-1.3.2/pylipd/lipd_series.py
+-rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.2/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     3089 2023-05-04 14:42:24.000000 pylipd-1.3.2/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)     9324 2023-04-20 10:34:40.000000 pylipd-1.3.2/pylipd/rdf_graph.py
+-rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.2/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.675215 pylipd-1.3.2/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.2/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.2/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.2/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     6073 2023-04-21 04:13:57.000000 pylipd-1.3.2/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     1095 2023-05-04 14:37:41.000000 pylipd-1.3.2/pylipd/usage_parallel.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.2/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.676292 pylipd-1.3.2/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      689 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.2/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       40 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.2/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      699 2023-05-04 15:21:37.676756 pylipd-1.3.2/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-21 04:14:43.000000 pylipd-1.3.2/setup.py
```

### Comparing `pylipd-1.3.1/LICENSE` & `pylipd-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/PKG-INFO` & `pylipd-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.1/README.md` & `pylipd-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/globals/queries.py` & `pylipd-1.3.2/pylipd/globals/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,23 @@
 QUERY_DSID = """
     SELECT ?dsid WHERE {
         ?ds a le:Dataset .
         OPTIONAL{?ds le:datasetId ?dsid}
     }
 """
 
+QUERY_UNIQUE_ARCHIVE_TYPE = """
+    SELECT distinct ?archiveType WHERE {
+        ?ds a le:Dataset .
+        ?ds le:proxyArchiveType ?archiveType .
+    }
+"""
+
 QUERY_ENSEMBLE_TABLE_SHORT = """
     PREFIX le: <http://linked.earth/ontology#>
-    PREFIX wgs: <http://www.w3.org/2003/01/geo/wgs84_pos#>
 
     SELECT ?datasetName ?ensembleTable ?ensembleVariableName ?ensembleVariableValues ?ensembleVariableUnits ?ensembleDepthName ?ensembleDepthValues ?ensembleDepthUnits ?notes 
     WHERE {
         ?ds a le:Dataset .
         ?ds le:name ?datasetName .
             FILTER regex(?datasetName, "[dsname].*", "i").
     
@@ -41,17 +47,16 @@
         ?ensdepthvar le:hasValues ?ensembleDepthValues .
             OPTIONAL{?ensdepthvar le:hasUnits ?ensembleDepthUnits .}
     }
 """
 
 QUERY_ENSEMBLE_TABLE = """
     PREFIX le: <http://linked.earth/ontology#>
-    PREFIX wgs: <http://www.w3.org/2003/01/geo/wgs84_pos#>
 
-    SELECT ?datasetName ?ensembleTable ?ensembleVariableName ?ensembleVariableValues ?ensembleVariableUnits ?ensembleDepthName ?ensembleDepthValues ?ensembleDepthUnits ?notes
+    SELECT ?datasetName ?ensembleTable ?ensembleVariableName ?ensembleVariableValues ?ensembleVariableUnits ?ensembleDepthName ?ensembleDepthValues ?ensembleDepthUnits ?notes ?methodobj ?methods
     WHERE {
         ?ds a le:Dataset .
         ?ds le:name ?datasetName .
             FILTER regex(?datasetName, "[dsname].*", "i").
     
         ?ds le:includesChronData ?chron .
         ?chron le:chronModeledBy ?model .
```

### Comparing `pylipd-1.3.1/pylipd/globals/schema.py` & `pylipd-1.3.2/pylipd/globals/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             'multiple': True,
             'schema': 'Model',
             'category': 'ChronModel'
         }
     },
     'Model': {
         '@id': ['{@parent.@id}', '.Model', '{@index}'],
-        'method': { 
+        'methods': { 
             'name': 'hasCode', 
             'schema': 'SoftwareCode' 
         },
         'summaryTable': {
             'name': 'foundInSummaryTable',
             'multiple': True,
             'schema': 'DataTable'
@@ -217,28 +217,37 @@
             'multiple': True,
             'schema': 'DataTable'
         }
     },
     'SoftwareCode': {
         '@id': {
             '{@parent.@id}',
-            '.',
+            '.Method',
             '{name|software}'
         },
-        'runCommand': { 
-            'name': 'hasExecutionCommand' 
+        'method': {
+            'type': 'string' 
         },
-        'runEnv': { 
-            'name': 'hasExecutionEnvironment' 
+        'version': {
+            'type': 'string' 
+        },
+        'algorithm': {
+            'type': 'string' 
         },
         'parameters': { 
             'type': 'string' 
         },
+        'runCommand': { 
+            'name': 'hasExecutionCommand' 
+        },            
+        'runEnv': { 
+            'name': 'hasExecutionEnvironment' 
+        },
         'software': { 
-            'name': 'name' 
+            'type': 'string' 
         }
     },
     'DataTable': {
         '@id': ['{filename}', '_trunc(4)'],
         '@fromJson': ['_set_inter_variable_links'],
         'filename': { 
             'name': 'hasFileName'
```

### Comparing `pylipd-1.3.1/pylipd/legacy_utils.py` & `pylipd-1.3.2/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/lipd.py` & `pylipd-1.3.2/pylipd/lipd.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pandas as pd
 import random
 import string
 import io
 
 from rdflib import ConjunctiveGraph, URIRef
 from tqdm import tqdm
-from pylipd.globals.queries import QUERY_ALL_VARIABLES_GRAPH, QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE, QUERY_ENSEMBLE_TABLE_SHORT, QUERY_FILTER_ARCHIVE_TYPE, QUERY_FILTER_GEO, QUERY_VARIABLE, QUERY_VARIABLE_GRAPH
+from pylipd.globals.queries import QUERY_ALL_VARIABLES_GRAPH, QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE, QUERY_ENSEMBLE_TABLE_SHORT, QUERY_FILTER_ARCHIVE_TYPE, QUERY_FILTER_GEO, QUERY_VARIABLE, QUERY_VARIABLE_GRAPH, QUERY_UNIQUE_ARCHIVE_TYPE
 from pylipd.lipd_series import LiPDSeries
 from pylipd.multi_processing import multi_convert_to_rdf, multi_load_lipd
 from pylipd.rdf_graph import RDFGraph
 
 from pylipd.rdf_to_lipd import RDFToLiPD
 from pylipd.legacy_utils import LiPD_Legacy
 from pylipd.utils import sanitizeId
@@ -174,22 +174,22 @@
 
         filemap = {}
         for path in os.listdir(lipd_dir):
             fullpath = os.path.join(lipd_dir, path)
             tmp_rdf_file = tempfile.NamedTemporaryFile().name
             filemap[fullpath] = tmp_rdf_file
         
-        print(f"Starting conversion of {len(filemap.keys())} LiPD files")
+        print(f"Converting {len(filemap.keys())} LiPD files to RDF..")
 
         multi_convert_to_rdf(filemap, parallel)
         
         print("Conversion to RDF done..")
 
         print("Writing to main RDF file..")
-        with open(rdf_file, "a") as fout:
+        with open(rdf_file, "w") as fout:
             for lipdfile in filemap.keys():
                 tmp_rdf_file = filemap[lipdfile]
                 if os.path.exists(tmp_rdf_file):
                     fin = open(tmp_rdf_file, "r")
                     data = fin.read();
                     fin.close()
                     fout.write(data)
@@ -703,14 +703,47 @@
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             print(lipd.get_all_dataset_ids())
         '''
         qres, qres_df = self.query(QUERY_DSID)
         return [sanitizeId(row.dsid) for row in qres]
+    
+    def get_all_archiveTypes(self):
+        '''
+        Returns a list of all the unique archiveTypes present in the LiPD object
+
+        Returns
+        -------
+        list
+            A list of archiveTypes
+            
+        Examples
+        --------
+        
+        .. ipython:: python
+            :okwarning:
+            :okexcept:
+
+            from pylipd.lipd import LiPD
+
+            # Fetch LiPD data from remote RDF Graph
+            lipd = LiPD()
+            lipd.load([
+                "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
+                "../examples/data/MD98_2181.Stott.2007.lpd"
+            ])
+            print(lipd.get_all_archiveTypes())
+
+        '''
+        
+        qres, qres_df = self.query(QUERY_UNIQUE_ARCHIVE_TYPE)
+        return [sanitizeId(row.archiveType) for row in qres]
+        
+        
 
 
     def get_ensemble_tables(self, dsname = None, ensembleVarName = None, ensembleDepthVarName = 'depth'):
         '''Gets ensemble tables from the LiPD graph
 
         Parameters
         ----------
```

### Comparing `pylipd-1.3.1/pylipd/lipd_series.py` & `pylipd-1.3.2/pylipd/lipd_series.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/lipd_to_rdf.py` & `pylipd-1.3.2/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/multi_processing.py` & `pylipd-1.3.2/pylipd/multi_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from tqdm import tqdm
 from pylipd.globals.queries import QUERY_ALL_VARIABLES_GRAPH
 from pylipd.lipd_to_rdf import LipdToRDF
 import multiprocessing as mp
 import copy
 
-def convert_to_rdf(lipdfile, rdffile):
+def convert_to_rdf(files):
+    (lipdfile, rdffile) = files
     converter = LipdToRDF()    
     """Worker that converts one lipdfile to an rdffile"""
     try:
         converter.convert(lipdfile)
         converter.serialize(rdffile)
     except Exception as e:
         print(f"ERROR: Could not convert LiPD file {lipdfile} to RDF")            
         raise e
 
 
 def multi_convert_to_rdf(filemap, parallel=True):
     if parallel:
         """Create a pool to convert all lipdfiles to rdffiles"""
-        pool = mp.Pool(mp.cpu_count())
         args = [(lipdfile, rdffile) for lipdfile, rdffile in filemap.items()]
-        pool.starmap(convert_to_rdf, args, chunksize=1)
+        pool = mp.Pool(mp.cpu_count())
+        for file in tqdm(pool.imap_unordered(convert_to_rdf, args, chunksize=1), total=len(args)):
+            pass
         pool.close()
     else:
         for lipdfile, rdffile in filemap.items():
             convert_to_rdf(lipdfile, rdffile)
 
 
 def convert_lipd_to_graph(lipdfile):
```

### Comparing `pylipd-1.3.1/pylipd/rdf_graph.py` & `pylipd-1.3.2/pylipd/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/rdf_to_lipd.py` & `pylipd-1.3.2/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/series/regexes.py` & `pylipd-1.3.2/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/test.py` & `pylipd-1.3.2/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd/usage.py` & `pylipd-1.3.2/pylipd/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 print(lipd.get_all_dataset_names())
 
 #lipdfiles = [local_lipd_dir + "/" + dsname + ".lpd" for dsname in dsnames]
 #print(lipdfiles)
 
 #lipd.load(lipdfiles)
 lipd.load_from_dir("examples/data")
+
+lipd.load_from_dir("/Users/varun/Downloads/example_sisal_lipds")
 print(lipd.get_all_dataset_names())
 
 lat = -77.08
 lon = 38.91
 radius = 50
 
 (result, result_df) = lipd.query("""
@@ -129,15 +131,15 @@
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
         print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 '''
 
 print("Popping ...")
-poplipd = lipd.pop(lipd.get_all_dataset_names())
+poplipd = lipd.pop(lipd.get_all_dataset_names()[0])
 print(lipd.get_all_dataset_names())
 print(poplipd.get_all_dataset_names())
 
 print("Creating separate lipd file for popped")
 dsname = poplipd.get_all_dataset_names()[0]
 lipdfile = f"{dsname}.lpd"
 poplipd.create_lipd(dsname, lipdfile)
```

### Comparing `pylipd-1.3.1/pylipd/usage_parallel.py` & `pylipd-1.3.2/pylipd/usage_parallel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 if __name__ == "__main__":
     from pylipd.lipd import LiPD
 
     local_lipd_dir = "/Users/varun/git/LiPD/PyLiPD/data/lpd.latest"
 
     L = LiPD()
+
+    # Convert LiPD files to RDF    
+    L.convert_lipd_dir_to_rdf(
+        local_lipd_dir,
+        local_lipd_dir+".nq", 
+        parallel=True)
+    
+    '''
     L.load_from_dir(local_lipd_dir, parallel=True, cutoff=1000)
     
     print(f"Total number of datasets: {len(L.get_all_dataset_names())}")
 
     print("Filtering by archive type and bounding box")
     
     Lfiltered = L.filter_by_archive_type("marine").filter_by_geo_bbox(-50, -50, 50, 50)
@@ -22,9 +30,10 @@
     S = Lfiltered.to_lipd_series(parallel=True)
 
     print("Filtering LiPD Series with variable name starting with 'd18O'")
     S = S.filter_by_name("d18O")
     
     print("Printing all valid variables")
     print(S.get_all_variables()['varname'])
+    '''
 
     exit()
```

### Comparing `pylipd-1.3.1/pylipd/utils.py` & `pylipd-1.3.2/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.2/pylipd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.1/pylipd.egg-info/SOURCES.txt` & `pylipd-1.3.2/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.1/setup.cfg` & `pylipd-1.3.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.3.1
+version = 1.3.2
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.3.1/setup.py` & `pylipd-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.3.1'
+version = '1.3.2'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

