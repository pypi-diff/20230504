# Comparing `tmp/dask-felleskomponenter-0.0.7.tar.gz` & `tmp/dask-felleskomponenter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jonas/src/dask-felleskomponenter/beam-components/dist/.tmp-il4mpjob/dask-felleskomponenter-0.0.7.tar", last modified: Thu May  4 09:07:01 2023, max compression
+gzip compressed data, was "dask-felleskomponenter-0.0.8.tar", last modified: Thu May  4 12:49:23 2023, max compression
```

## Comparing `dask-felleskomponenter-0.0.7.tar` & `dask-felleskomponenter-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/
--rw-r--r--   0 jonas      (602) staff       (20)     1047 2023-03-23 08:01:02.000000 dask-felleskomponenter-0.0.7/LICENSE.txt
--rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/PKG-INFO
--rw-r--r--   0 jonas      (602) staff       (20)      602 2023-03-24 09:33:29.000000 dask-felleskomponenter-0.0.7/README.md
--rw-r--r--   0 jonas      (602) staff       (20)      112 2023-03-23 09:54:58.000000 dask-felleskomponenter-0.0.7/pyproject.toml
--rw-r--r--   0 jonas      (602) staff       (20)       38 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/setup.cfg
--rw-r--r--   0 jonas      (602) staff       (20)      923 2023-05-04 08:58:42.000000 dask-felleskomponenter-0.0.7/setup.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 10:15:30.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/__init__.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/common/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 09:48:20.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/common/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)      899 2023-03-24 10:47:56.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/common/api_client.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sinks/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-05-04 09:05:42.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sinks/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)     2865 2023-04-27 11:58:08.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sinks/json.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 07:45:40.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)     1919 2023-03-24 12:30:15.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/api_source.py
--rw-r--r--   0 jonas      (602) staff       (20)      856 2023-05-04 08:58:20.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/file.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/
--rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/PKG-INFO
--rw-r--r--   0 jonas      (602) staff       (20)      683 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/SOURCES.txt
--rw-r--r--   0 jonas      (602) staff       (20)        1 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/dependency_links.txt
--rw-r--r--   0 jonas      (602) staff       (20)       29 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/top_level.txt
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-05-04 09:07:01.000000 dask-felleskomponenter-0.0.7/src/tests/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 08:14:30.000000 dask-felleskomponenter-0.0.7/src/tests/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)      267 2023-03-24 12:38:52.000000 dask-felleskomponenter-0.0.7/src/tests/test_api_client.py
--rw-r--r--   0 jonas      (602) staff       (20)      941 2023-04-04 14:13:30.000000 dask-felleskomponenter-0.0.7/src/tests/test_api_source.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.144875 dask-felleskomponenter-0.0.8/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1047 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/LICENSE.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1700 2023-05-04 12:49:23.143855 dask-felleskomponenter-0.0.8/PKG-INFO
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1100 2023-05-04 12:44:58.000000 dask-felleskomponenter-0.0.8/README.md
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      112 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/pyproject.toml
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       38 2023-05-04 12:49:23.145197 dask-felleskomponenter-0.0.8/setup.cfg
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      895 2023-05-04 12:42:14.000000 dask-felleskomponenter-0.0.8/setup.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.131232 dask-felleskomponenter-0.0.8/src/
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.134236 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/__init__.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.136295 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      899 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/api_client.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.137668 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     3247 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/json_sink.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.139375 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1919 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/api_source.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      856 2023-05-04 12:19:28.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/file_source.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.135662 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1700 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/PKG-INFO
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      695 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/SOURCES.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        1 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/dependency_links.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       29 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/top_level.txt
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.142284 dask-felleskomponenter-0.0.8/src/tests/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      267 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/test_api_client.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      941 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/test_api_source.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dask-felleskomponenter-0.0.7/LICENSE.txt` & `dask-felleskomponenter-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.7/PKG-INFO` & `dask-felleskomponenter-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,7 +24,19 @@
 - custom apache beam sinks
 
 ## Dependencies
 You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following command
 ```bash
 pip install -r requirements.txt
 ```
+
+## Bulding and publishing of package
+### Steps
+- Remove old dist-folder 
+- Update version in `setup.py`, for instance `0.0.7`->`0.0.8`
+- (Run `pip install build` if you do not have this already)
+- Run `python3 -m build` (and wait some minutes...)
+- Verity that dist contains a package with the new version in the package name.
+- Run `python3 -m twine upload dist/*` to upload to pypi
+
+### To upload to PyPi test
+Replace the last command with `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/common/api_client.py` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/api_client.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sinks/json.py` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/json_sink.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import json
-
 import apache_beam as beam
 from apache_beam import coders
 from apache_beam.io.iobase import Write
-from apache_beam.transforms import PTransform   
+from apache_beam.transforms import PTransform
 from apache_beam.io.filesystem import CompressionTypes
 
+
 class JsonSink(beam.io.FileBasedSink):
     """A Dataflow sink for writing GeoJSON files."""
 
     def __init__(self,
                  file_path_prefix,
+                 crs_code,
                  file_name_suffix='',
                  num_shards=0,
                  shard_name_template=None,
                  coder=coders.StrUtf8Coder(),
                  compression_type=CompressionTypes.AUTO):
 
         super(JsonSink, self).__init__(
             file_path_prefix,
             file_name_suffix=file_name_suffix,
             num_shards=num_shards,
             shard_name_template=shard_name_template,
             coder=coder,
             mime_type='text/plain',
             compression_type=compression_type)
+
         self.last_rows = dict()
+        self.crs_code = crs_code
 
     def open(self, temp_path):
         """ Open file and initialize it w opening a list."""
         file_handle = super(JsonSink, self).open(temp_path)
-        file_handle.write(bytes('{ "type": "FeatureCollection", "features": [\n', encoding="utf-8"))
+        crs_value = f'urn:ogc:def:axis:{self.crs_code}'
+        start_of_file = f'{{"type": "FeatureCollection", "crs": "{crs_value}", "features": [\n'
+        file_handle.write(bytes(start_of_file, encoding="utf-8"))
         return file_handle
 
     def write_record(self, file_handle, value):
         """Writes a single encoded record converted to JSON and terminates the
         line w a comma."""
         if self.last_rows.get(file_handle, None) is not None:
             file_handle.write(self.coder.encode(
@@ -55,22 +60,26 @@
             # Close list and then the file
             file_handle.write(bytes('\n] }', encoding="utf-8"))
             file_handle.close()
 
 
 class WriteToGeoJSONFeatureCollection(PTransform):
     """PTransform for writing to GeoJSON files.
-    Assumes a list of features according to the GeoJSON specification, that gets put into a FeatureCollection."""
+    Assumes a list of features according to the GeoJSON specification, that gets put into a FeatureCollection.
+
+    The crs of the json-file defaults to EPSG:4326 (corresponding to WGS:84).
+    This can be overwritten by defining a crs_code on class initialization.
+    """
 
     def __init__(self,
                  file_path_prefix,
+                 crs_code='EPSG:4326',
                  file_name_suffix='',
                  num_shards=0,
                  shard_name_template=None,
                  coder=coders.StrUtf8Coder(),
                  compression_type=CompressionTypes.AUTO):
-
-        self._sink = JsonSink(file_path_prefix, file_name_suffix, num_shards,
-                               shard_name_template, coder, compression_type)
+        self._sink = JsonSink(file_path_prefix, crs_code, file_name_suffix, num_shards,
+                              shard_name_template, coder, compression_type)
 
     def expand(self, pcoll):
         return pcoll | Write(self._sink)
```

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/api_source.py` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/api_source.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter/sources/file.py` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/file_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         bucket_name, blob_name = self._file_pattern[5:].split("/", 1)
         bucket = client.get_bucket(bucket_name)
         blob = storage.Blob(blob_name, bucket)
         file_str = blob.download_as_text()
         yield file_str
 
 
-class ReadFileFromGcp(PTransform):
+class ReadFileFromGCP(PTransform):
     def __init__(self, file_pattern):
         self._file_pattern = file_pattern
 
     def expand(self, pcoll):
         return (
             pcoll
             | 'CreateInput' >> Create([None])
```

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/PKG-INFO` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,7 +24,19 @@
 - custom apache beam sinks
 
 ## Dependencies
 You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following command
 ```bash
 pip install -r requirements.txt
 ```
+
+## Bulding and publishing of package
+### Steps
+- Remove old dist-folder 
+- Update version in `setup.py`, for instance `0.0.7`->`0.0.8`
+- (Run `pip install build` if you do not have this already)
+- Run `python3 -m build` (and wait some minutes...)
+- Verity that dist contains a package with the new version in the package name.
+- Run `python3 -m twine upload dist/*` to upload to pypi
+
+### To upload to PyPi test
+Replace the last command with `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `dask-felleskomponenter-0.0.7/src/dask_felleskomponenter.egg-info/SOURCES.txt` & `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 src/dask_felleskomponenter.egg-info/PKG-INFO
 src/dask_felleskomponenter.egg-info/SOURCES.txt
 src/dask_felleskomponenter.egg-info/dependency_links.txt
 src/dask_felleskomponenter.egg-info/top_level.txt
 src/dask_felleskomponenter/common/__init__.py
 src/dask_felleskomponenter/common/api_client.py
 src/dask_felleskomponenter/sinks/__init__.py
-src/dask_felleskomponenter/sinks/json.py
+src/dask_felleskomponenter/sinks/json_sink.py
 src/dask_felleskomponenter/sources/__init__.py
 src/dask_felleskomponenter/sources/api_source.py
-src/dask_felleskomponenter/sources/file.py
+src/dask_felleskomponenter/sources/file_source.py
 src/tests/__init__.py
 src/tests/test_api_client.py
 src/tests/test_api_source.py
```

### Comparing `dask-felleskomponenter-0.0.7/src/tests/test_api_source.py` & `dask-felleskomponenter-0.0.8/src/tests/test_api_source.py`

 * *Files identical despite different names*

