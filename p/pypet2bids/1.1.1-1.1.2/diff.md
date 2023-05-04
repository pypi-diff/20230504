# Comparing `tmp/pypet2bids-1.1.1.tar.gz` & `tmp/pypet2bids-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypet2bids-1.1.1.tar", max compression
+gzip compressed data, was "pypet2bids-1.1.2.tar", max compression
```

## Comparing `pypet2bids-1.1.1.tar` & `pypet2bids-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      428 2022-11-30 20:30:12.412732 pypet2bids-1.1.1/pypet2bids/Pipfile
--rw-r--r--   0        0        0     9755 2022-11-30 20:30:12.413053 pypet2bids-1.1.1/pypet2bids/README.md
--rw-r--r--   0        0        0        0 2022-11-30 20:30:12.413084 pypet2bids-1.1.1/pypet2bids/__init__.py
--rw-r--r--   0        0        0    37643 2022-11-30 20:30:12.413624 pypet2bids-1.1.1/pypet2bids/convert_pmod_to_blood.py
--rw-r--r--   0        0        0    62353 2023-02-21 16:26:31.650653 pypet2bids-1.1.1/pypet2bids/dcm2niix4pet.py
--rwxr-xr-x   0        0        0    18241 2022-11-30 20:30:12.414789 pypet2bids-1.1.1/pypet2bids/dicom_convert.py
--rw-r--r--   0        0        0    14006 2023-01-20 20:54:10.147427 pypet2bids-1.1.1/pypet2bids/ecat.py
--rw-r--r--   0        0        0    10704 2023-01-20 20:54:10.147812 pypet2bids-1.1.1/pypet2bids/ecat2nii.py
--rw-r--r--   0        0        0     9516 2022-11-30 20:30:12.415581 pypet2bids-1.1.1/pypet2bids/ecat_cli.py
--rw-r--r--   0        0        0   162568 2022-11-30 20:30:12.416153 pypet2bids-1.1.1/pypet2bids/ecat_headers.json
--rw-r--r--   0        0        0     4996 2022-11-30 20:30:12.416272 pypet2bids-1.1.1/pypet2bids/golden_ecat.py
--rw-r--r--   0        0        0    33773 2023-02-22 18:22:21.292332 pypet2bids-1.1.1/pypet2bids/helper_functions.py
--rw-r--r--   0        0        0     6763 2023-03-21 19:42:40.042472 pypet2bids-1.1.1/pypet2bids/is_pet.py
--rw-r--r--   0        0        0     1386 2023-03-21 19:42:51.290148 pypet2bids-1.1.1/pypet2bids/metadata/PET_Radionuclide.mkd
--rw-r--r--   0        0        0     1710 2023-03-21 19:42:51.291715 pypet2bids-1.1.1/pypet2bids/metadata/PET_metadata.json
--rw-r--r--   0        0        0     3377 2023-03-21 19:42:51.290548 pypet2bids-1.1.1/pypet2bids/metadata/PET_reconstruction_methods.json
--rw-r--r--   0        0        0      384 2023-03-21 19:42:51.289753 pypet2bids-1.1.1/pypet2bids/metadata/blood_metadata.json
--rw-r--r--   0        0        0     1182 2023-03-21 19:42:51.291425 pypet2bids-1.1.1/pypet2bids/metadata/definitions.json
--rw-r--r--   0        0        0     2667 2023-03-21 19:42:51.289160 pypet2bids-1.1.1/pypet2bids/metadata/dicom2bids.json
--rw-r--r--   0        0        0     3915 2022-11-30 20:30:12.417192 pypet2bids-1.1.1/pypet2bids/metadata_spreadsheet_example_reader.py
--rw-r--r--   0        0        0     8569 2022-12-27 23:28:49.169202 pypet2bids-1.1.1/pypet2bids/multiple_spreadsheets.py
--rw-r--r--   0        0        0     1541 2023-03-21 19:42:51.294184 pypet2bids-1.1.1/pypet2bids/pyproject.toml
--rw-r--r--   0        0        0    17315 2022-11-30 20:30:12.417834 pypet2bids-1.1.1/pypet2bids/read_ecat.py
--rw-r--r--   0        0        0     3298 2022-11-30 20:30:12.418133 pypet2bids-1.1.1/pypet2bids/sidecar.py
--rw-r--r--   0        0        0     8484 2022-11-30 20:30:12.418396 pypet2bids-1.1.1/pypet2bids/single_spreadsheet.py
--rw-r--r--   0        0        0       95 2022-11-30 20:30:12.418472 pypet2bids-1.1.1/pypet2bids/template.env
--rw-r--r--   0        0        0    12798 2022-11-30 20:30:12.418809 pypet2bids-1.1.1/pypet2bids/write_ecat.py
--rw-r--r--   0        0        0     1541 2023-03-21 19:42:40.042669 pypet2bids-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 pypet2bids-1.1.1/setup.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 pypet2bids-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      428 2022-11-30 20:30:12.412732 pypet2bids-1.1.2/pypet2bids/Pipfile
+-rw-r--r--   0        0        0     9755 2022-11-30 20:30:12.413053 pypet2bids-1.1.2/pypet2bids/README.md
+-rw-r--r--   0        0        0        0 2022-11-30 20:30:12.413084 pypet2bids-1.1.2/pypet2bids/__init__.py
+-rw-r--r--   0        0        0    37643 2022-11-30 20:30:12.413624 pypet2bids-1.1.2/pypet2bids/convert_pmod_to_blood.py
+-rw-r--r--   0        0        0    62353 2023-05-04 17:10:47.656853 pypet2bids-1.1.2/pypet2bids/dcm2niix4pet.py
+-rwxr-xr-x   0        0        0    18241 2022-11-30 20:30:12.414789 pypet2bids-1.1.2/pypet2bids/dicom_convert.py
+-rw-r--r--   0        0        0    14006 2023-01-20 20:54:10.147427 pypet2bids-1.1.2/pypet2bids/ecat.py
+-rw-r--r--   0        0        0    10704 2023-01-20 20:54:10.147812 pypet2bids-1.1.2/pypet2bids/ecat2nii.py
+-rw-r--r--   0        0        0     9516 2022-11-30 20:30:12.415581 pypet2bids-1.1.2/pypet2bids/ecat_cli.py
+-rw-r--r--   0        0        0   162568 2022-11-30 20:30:12.416153 pypet2bids-1.1.2/pypet2bids/ecat_headers.json
+-rw-r--r--   0        0        0     4996 2022-11-30 20:30:12.416272 pypet2bids-1.1.2/pypet2bids/golden_ecat.py
+-rw-r--r--   0        0        0    33773 2023-02-22 18:22:21.292332 pypet2bids-1.1.2/pypet2bids/helper_functions.py
+-rw-r--r--   0        0        0     6763 2023-03-21 20:12:05.711580 pypet2bids-1.1.2/pypet2bids/is_pet.py
+-rw-r--r--   0        0        0     1386 2023-05-04 17:35:51.289125 pypet2bids-1.1.2/pypet2bids/metadata/PET_Radionuclide.mkd
+-rw-r--r--   0        0        0     1710 2023-05-04 17:35:51.290897 pypet2bids-1.1.2/pypet2bids/metadata/PET_metadata.json
+-rw-r--r--   0        0        0     3377 2023-05-04 17:35:51.289555 pypet2bids-1.1.2/pypet2bids/metadata/PET_reconstruction_methods.json
+-rw-r--r--   0        0        0      384 2023-05-04 17:35:51.288683 pypet2bids-1.1.2/pypet2bids/metadata/blood_metadata.json
+-rw-r--r--   0        0        0     1182 2023-05-04 17:35:51.290656 pypet2bids-1.1.2/pypet2bids/metadata/definitions.json
+-rw-r--r--   0        0        0     2667 2023-05-04 17:35:51.288365 pypet2bids-1.1.2/pypet2bids/metadata/dicom2bids.json
+-rw-r--r--   0        0        0     3915 2022-11-30 20:30:12.417192 pypet2bids-1.1.2/pypet2bids/metadata_spreadsheet_example_reader.py
+-rw-r--r--   0        0        0     8569 2022-12-27 23:28:49.169202 pypet2bids-1.1.2/pypet2bids/multiple_spreadsheets.py
+-rw-r--r--   0        0        0     1542 2023-05-04 17:35:51.294584 pypet2bids-1.1.2/pypet2bids/pyproject.toml
+-rw-r--r--   0        0        0    17315 2022-11-30 20:30:12.417834 pypet2bids-1.1.2/pypet2bids/read_ecat.py
+-rw-r--r--   0        0        0     3298 2022-11-30 20:30:12.418133 pypet2bids-1.1.2/pypet2bids/sidecar.py
+-rw-r--r--   0        0        0     8484 2022-11-30 20:30:12.418396 pypet2bids-1.1.2/pypet2bids/single_spreadsheet.py
+-rw-r--r--   0        0        0       95 2022-11-30 20:30:12.418472 pypet2bids-1.1.2/pypet2bids/template.env
+-rw-r--r--   0        0        0    12798 2022-11-30 20:30:12.418809 pypet2bids-1.1.2/pypet2bids/write_ecat.py
+-rw-r--r--   0        0        0     1542 2023-05-04 17:19:08.656037 pypet2bids-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 pypet2bids-1.1.2/setup.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 pypet2bids-1.1.2/PKG-INFO
```

### Comparing `pypet2bids-1.1.1/pypet2bids/README.md` & `pypet2bids-1.1.2/pypet2bids/README.md`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/convert_pmod_to_blood.py` & `pypet2bids-1.1.2/pypet2bids/convert_pmod_to_blood.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/dcm2niix4pet.py` & `pypet2bids-1.1.2/pypet2bids/dcm2niix4pet.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/dicom_convert.py` & `pypet2bids-1.1.2/pypet2bids/dicom_convert.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/ecat.py` & `pypet2bids-1.1.2/pypet2bids/ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/ecat2nii.py` & `pypet2bids-1.1.2/pypet2bids/ecat2nii.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/ecat_cli.py` & `pypet2bids-1.1.2/pypet2bids/ecat_cli.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/ecat_headers.json` & `pypet2bids-1.1.2/pypet2bids/ecat_headers.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/golden_ecat.py` & `pypet2bids-1.1.2/pypet2bids/golden_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/helper_functions.py` & `pypet2bids-1.1.2/pypet2bids/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/is_pet.py` & `pypet2bids-1.1.2/pypet2bids/is_pet.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata/PET_Radionuclide.mkd` & `pypet2bids-1.1.2/pypet2bids/metadata/PET_Radionuclide.mkd`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata/PET_metadata.json` & `pypet2bids-1.1.2/pypet2bids/metadata/PET_metadata.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata/PET_reconstruction_methods.json` & `pypet2bids-1.1.2/pypet2bids/metadata/PET_reconstruction_methods.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata/definitions.json` & `pypet2bids-1.1.2/pypet2bids/metadata/definitions.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata/dicom2bids.json` & `pypet2bids-1.1.2/pypet2bids/metadata/dicom2bids.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/metadata_spreadsheet_example_reader.py` & `pypet2bids-1.1.2/pypet2bids/metadata_spreadsheet_example_reader.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/multiple_spreadsheets.py` & `pypet2bids-1.1.2/pypet2bids/multiple_spreadsheets.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/pyproject.toml` & `pypet2bids-1.1.2/pypet2bids/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypet2bids"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python implementation of an ECAT to BIDS converter."
 authors = ["anthony galassi <28850131+bendhouseart@users.noreply.github.com>"]
 license = "MIT"
 include = [
     'pypet2bids/metadata/blood_metadata.json',
     'pypet2bids/metadata/definitions.json',
     'pypet2bids/metadata/dicom2bids.json',
@@ -12,15 +12,15 @@
     'pypet2bids/metadata/PET_Radionuclide.mkd',
     'pypet2bids/metadata/PET_reconstruction_methods.json',
     'pypet2bids/pyproject.toml',
     ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.11.1"
-nibabel = "^3.2.1"
+nibabel = ">=3.2.1"
 numpy = "^1.21.3"
 pyparsing = "^3.0.4"
 python-dateutil = "^2.8.2"
 python-dotenv = "^0.19.1"
 scipy = "^1.7.1"
 six = "^1.16.0"
 pytest = "^6.2.5"
```

### Comparing `pypet2bids-1.1.1/pypet2bids/read_ecat.py` & `pypet2bids-1.1.2/pypet2bids/read_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/sidecar.py` & `pypet2bids-1.1.2/pypet2bids/sidecar.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/single_spreadsheet.py` & `pypet2bids-1.1.2/pypet2bids/single_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pypet2bids/write_ecat.py` & `pypet2bids-1.1.2/pypet2bids/write_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.1/pyproject.toml` & `pypet2bids-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypet2bids"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python implementation of an ECAT to BIDS converter."
 authors = ["anthony galassi <28850131+bendhouseart@users.noreply.github.com>"]
 license = "MIT"
 include = [
     'pypet2bids/metadata/blood_metadata.json',
     'pypet2bids/metadata/definitions.json',
     'pypet2bids/metadata/dicom2bids.json',
@@ -12,15 +12,15 @@
     'pypet2bids/metadata/PET_Radionuclide.mkd',
     'pypet2bids/metadata/PET_reconstruction_methods.json',
     'pypet2bids/pyproject.toml',
     ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.11.1"
-nibabel = "^3.2.1"
+nibabel = ">=3.2.1"
 numpy = "^1.21.3"
 pyparsing = "^3.0.4"
 python-dateutil = "^2.8.2"
 python-dotenv = "^0.19.1"
 scipy = "^1.7.1"
 six = "^1.16.0"
 pytest = "^6.2.5"
```

### Comparing `pypet2bids-1.1.1/setup.py` & `pypet2bids-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 'metadata/dicom2bids.json',
                 'metadata/dicom2bids.json',
                 'metadata/dicom2bids.json']}
 
 install_requires = \
 ['joblib>=1.2.0,<2.0.0',
  'json-maj>=0.0.7,<0.0.8',
- 'nibabel>=3.2.1,<4.0.0',
+ 'nibabel>=3.2.1',
  'numpy>=1.21.3,<2.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pandas>=1.4.4,<2.0.0',
  'pydicom>=2.2.2,<3.0.0',
  'pyparsing>=3.0.4,<4.0.0',
  'pytest>=6.2.5,<7.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
@@ -69,15 +69,15 @@
                      'ecatpet2bids = pypet2bids.ecat_cli:main',
                      'ispet = pypet2bids.is_pet:main',
                      'pet2bids-spreadsheet-template = '
                      'pypet2bids.helper_functions:write_out_module']}
 
 setup_kwargs = {
     'name': 'pypet2bids',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'A python implementation of an ECAT to BIDS converter.',
     'long_description': 'None',
     'author': 'anthony galassi',
     'author_email': '28850131+bendhouseart@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pypet2bids-1.1.1/PKG-INFO` & `pypet2bids-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pypet2bids
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python implementation of an ECAT to BIDS converter.
 License: MIT
 Author: anthony galassi
 Author-email: 28850131+bendhouseart@users.noreply.github.com
 Requires-Python: >=3.8,<=3.11.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: json-maj (>=0.0.7,<0.0.8)
-Requires-Dist: nibabel (>=3.2.1,<4.0.0)
+Requires-Dist: nibabel (>=3.2.1)
 Requires-Dist: numpy (>=1.21.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pydicom (>=2.2.2,<3.0.0)
 Requires-Dist: pyparsing (>=3.0.4,<4.0.0)
 Requires-Dist: pytest (>=6.2.5,<7.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

