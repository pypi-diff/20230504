# Comparing `tmp/jobspire_nitra-0.1.6.tar.gz` & `tmp/jobspire_nitra-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jobspire_nitra-0.1.6.tar", last modified: Wed Feb  8 11:45:28 2023, max compression
+gzip compressed data, was "jobspire_nitra-0.1.7.tar", last modified: Thu May  4 14:03:53 2023, max compression
```

## Comparing `jobspire_nitra-0.1.6.tar` & `jobspire_nitra-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelhimmelstrup   (501) staff       (20)        0 2023-02-08 11:45:28.101003 jobspire_nitra-0.1.6/
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)     1055 2023-02-07 10:09:17.000000 jobspire_nitra-0.1.6/LICENSE
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)     1352 2023-02-08 11:45:28.100696 jobspire_nitra-0.1.6/PKG-INFO
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)     1018 2023-02-08 07:21:10.000000 jobspire_nitra-0.1.6/README.rst
-drwxr-xr-x   0 samuelhimmelstrup   (501) staff       (20)        0 2023-02-08 11:45:28.098496 jobspire_nitra-0.1.6/jobspire_nitra/
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)       39 2023-02-07 10:09:17.000000 jobspire_nitra-0.1.6/jobspire_nitra/__init__.py
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)     6142 2023-02-08 11:12:18.000000 jobspire_nitra-0.1.6/jobspire_nitra/main.py
-drwxr-xr-x   0 samuelhimmelstrup   (501) staff       (20)        0 2023-02-08 11:45:28.100279 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)     1352 2023-02-08 11:45:27.000000 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/PKG-INFO
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)      266 2023-02-08 11:45:27.000000 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/SOURCES.txt
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)        1 2023-02-08 11:45:27.000000 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/dependency_links.txt
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)        9 2023-02-08 11:45:27.000000 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/requires.txt
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)       15 2023-02-08 11:45:27.000000 jobspire_nitra-0.1.6/jobspire_nitra.egg-info/top_level.txt
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)       38 2023-02-08 11:45:28.101100 jobspire_nitra-0.1.6/setup.cfg
--rw-r--r--   0 samuelhimmelstrup   (501) staff       (20)      763 2023-02-08 11:43:54.000000 jobspire_nitra-0.1.6/setup.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/
+-rw-r--r--   0 niko      (1000) niko      (1000)     1055 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.7/LICENSE
+-rw-r--r--   0 niko      (1000) niko      (1000)     1344 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/PKG-INFO
+-rw-r--r--   0 niko      (1000) niko      (1000)     1047 2023-05-04 13:59:23.000000 jobspire_nitra-0.1.7/README.rst
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.911815 jobspire_nitra-0.1.7/jobspire_nitra/
+-rw-r--r--   0 niko      (1000) niko      (1000)       39 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.7/jobspire_nitra/__init__.py
+-rw-r--r--   0 niko      (1000) niko      (1000)     6273 2023-05-04 13:59:06.000000 jobspire_nitra-0.1.7/jobspire_nitra/main.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.912815 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/
+-rw-r--r--   0 niko      (1000) niko      (1000)     1344 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/PKG-INFO
+-rw-r--r--   0 niko      (1000) niko      (1000)      266 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/SOURCES.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)        1 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/dependency_links.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)        9 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/requires.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)       15 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/top_level.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)       38 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/setup.cfg
+-rw-r--r--   0 niko      (1000) niko      (1000)      763 2023-05-04 14:00:01.000000 jobspire_nitra-0.1.7/setup.py
```

### Comparing `jobspire_nitra-0.1.6/LICENSE` & `jobspire_nitra-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jobspire_nitra-0.1.6/PKG-INFO` & `jobspire_nitra-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: jobspire_nitra
-Version: 0.1.6
+Version: 0.1.7
 Summary: Nitra
 Home-page: https://github.com/HBS-Economics/nitra.git
 Author: JobSpire team
 Author-email: <info@jobspire.com>
-License: UNKNOWN
 Keywords: python,nitra package
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==============================================
 JobSpire truth table remote control python lib
 ==============================================
@@ -37,21 +35,20 @@
   nitra.delete_job_postings_by_source_id(source_ids: List[str])
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
+  nitra.get_contract_types()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
 
 To build:
 ``python3 -m build``
 
 To release:
 ``./release.sh``
-
-
```

### Comparing `jobspire_nitra-0.1.6/README.rst` & `jobspire_nitra-0.1.7/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   nitra.delete_job_postings_by_source_id(source_ids: List[str])
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
+  nitra.get_contract_types()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
```

### Comparing `jobspire_nitra-0.1.6/jobspire_nitra/main.py` & `jobspire_nitra-0.1.7/jobspire_nitra/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,20 @@
 
     def get_statistics(self) -> Response:
         return self.req(
             '/statistics',
             'GET'
         )
 
+    def get_contract_types(self) -> Response:
+        return self.req(
+            '/contract_types',
+            'GET'
+        )
+
     def add_company_esco_matches(
         self,
         company_esco_matches: List[dict]
     ) -> Response:
 
         body = {'esco_matches': company_esco_matches}
```

### Comparing `jobspire_nitra-0.1.6/jobspire_nitra.egg-info/PKG-INFO` & `jobspire_nitra-0.1.7/jobspire_nitra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: jobspire-nitra
-Version: 0.1.6
+Version: 0.1.7
 Summary: Nitra
 Home-page: https://github.com/HBS-Economics/nitra.git
 Author: JobSpire team
 Author-email: <info@jobspire.com>
-License: UNKNOWN
 Keywords: python,nitra package
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==============================================
 JobSpire truth table remote control python lib
 ==============================================
@@ -37,21 +35,20 @@
   nitra.delete_job_postings_by_source_id(source_ids: List[str])
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
+  nitra.get_contract_types()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
 
 To build:
 ``python3 -m build``
 
 To release:
 ``./release.sh``
-
-
```

### Comparing `jobspire_nitra-0.1.6/setup.py` & `jobspire_nitra-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Nitra'
 
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 # Setting up
```

