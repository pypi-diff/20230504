# Comparing `tmp/JsonPreprocessor-0.2.2.tar.gz` & `tmp/JsonPreprocessor-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.2.2.tar", last modified: Thu Apr 27 09:39:19 2023, max compression
+gzip compressed data, was "JsonPreprocessor-0.2.3.tar", last modified: Thu May  4 14:30:17 2023, max compression
```

## Comparing `JsonPreprocessor-0.2.2.tar` & `JsonPreprocessor-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:19.141926 JsonPreprocessor-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:19.141926 JsonPreprocessor-0.2.2/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)    27824 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   304189 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:19.141926 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-27 09:39:19.000000 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:39:19.000000 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:39:19.000000 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 09:39:19.000000 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:39:19.000000 JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-27 09:39:19.141926 JsonPreprocessor-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:39:19.141926 JsonPreprocessor-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-27 09:36:47.000000 JsonPreprocessor-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   274550 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:30:17.405166 JsonPreprocessor-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/setup.py
```

### Comparing `JsonPreprocessor-0.2.2/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.2.3/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -275,18 +275,29 @@
 
                 # length of lImportedFiles should equal to recursive_level
                 self.lImportedFiles = self.lImportedFiles[:self.recursive_level]
                 if abs_path_file in self.lImportedFiles:
                     raise Exception(f"Cyclic imported json file '{abs_path_file}'!")
                 
                 oJsonImport = self.jsonLoad(abs_path_file, masterFile=False)
+                tmpOutdict = copy.deepcopy(out_dict)
+                for k1, v1 in tmpOutdict.items():
+                    for k2, v2 in oJsonImport.items():
+                        if k2 == k1:
+                            del out_dict[k1]
+                del tmpOutdict
                 out_dict.update(oJsonImport)
 
                 self.recursive_level = self.recursive_level - 1     # descrease recursive level
             else:
+                tmpOutdict = copy.deepcopy(out_dict)
+                for k1, v1 in tmpOutdict.items():
+                    if k1 == key:
+                        del out_dict[k1]
+                del tmpOutdict
                 out_dict[key] = value
         return out_dict
 
     def __load_and_removeComments(self, jsonFile : str) -> str:
         """
       Loads a given json file and filters all C/C++ style comments.
 
@@ -467,14 +478,23 @@
                 del oJson[keyNested]
                 if '[' in k:
                     sExec = k + " = \"" + v + "\"" if isinstance(v, str) else k + " = " + str(v)
                     try:
                         exec(sExec, globals())
                     except:
                         raise Exception(f"Could not set variable '{k}' with value '{v}'!")
+                    
+                    if isinstance(v, str):
+                        sExec = "oJson['" + k.split('[', 1)[0] + "'][" + k.split('[', 1)[1] + " = \"" + v + "\""
+                    else:
+                        sExec = "oJson['" + k.split('[', 1)[0] + "'][" + k.split('[', 1)[1] + " = " + str(v)
+                    try:
+                        exec(sExec, globals())
+                    except:
+                        pass
                 else:
                     oJson[k] = v
                
             else:
                 if bNested:
                     oJson[k] = v
```

### Comparing `JsonPreprocessor-0.2.2/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.2.3/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.2/JsonPreprocessor/version.py` & `JsonPreprocessor-0.2.3/JsonPreprocessor/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.2.2"
-VERSION_DATE = "27.04.2023"
+VERSION      = "0.2.3"
+VERSION_DATE = "04.05.2023"
```

### Comparing `JsonPreprocessor-0.2.2/JsonPreprocessor.egg-info/PKG-INFO` & `JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.2.2/LICENSE` & `JsonPreprocessor-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.2/PKG-INFO` & `JsonPreprocessor-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.2.2/README.rst` & `JsonPreprocessor-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.2/setup.py` & `JsonPreprocessor-0.2.3/setup.py`

 * *Files identical despite different names*

