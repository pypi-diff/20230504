# Comparing `tmp/microdata-validator-7.3.0.tar.gz` & `tmp/microdata-validator-7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata-validator-7.3.0.tar", max compression
+gzip compressed data, was "microdata-validator-7.3.1.tar", max compression
```

## Comparing `microdata-validator-7.3.0.tar` & `microdata-validator-7.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1102 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/LICENSE
--rw-r--r--   0        0        0     1707 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/README.md
--rw-r--r--   0        0        0     6573 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/__init__.py
--rw-r--r--   0        0        0     4424 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/adapter/local_storage.py
--rw-r--r--   0        0        0     5767 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/temporal_attributes.py
--rw-r--r--   0        0        0      776 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_id_types.py
--rw-r--r--   0        0        0     1609 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
--rw-r--r--   0        0        0     2091 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1525 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     2124 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1429 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1378 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232471 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1242 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1202 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1535 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1166 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/__init__.py
--rw-r--r--   0        0        0      414 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/exceptions/__init__.py
--rw-r--r--   0        0        0      872 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/model/__init__.py
--rw-r--r--   0        0        0     5781 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/model/metadata.py
--rw-r--r--   0        0        0     7854 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/steps/dataset_reader.py
--rw-r--r--   0        0        0     7837 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/steps/dataset_validator.py
--rw-r--r--   0        0        0     1663 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/steps/metadata_inliner.py
--rw-r--r--   0        0        0     1682 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/microdata_validator/steps/metadata_reader.py
--rw-r--r--   0        0        0      652 2023-03-15 09:23:29.543221 microdata-validator-7.3.0/pyproject.toml
--rw-r--r--   0        0        0     2698 2023-03-15 09:24:25.841211 microdata-validator-7.3.0/setup.py
--rw-r--r--   0        0        0     2417 2023-03-15 09:24:25.842139 microdata-validator-7.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/LICENSE
+-rw-r--r--   0        0        0     1707 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/README.md
+-rw-r--r--   0        0        0     6573 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/__init__.py
+-rw-r--r--   0        0        0     4424 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/adapter/local_storage.py
+-rw-r--r--   0        0        0     5603 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/temporal_attributes.py
+-rw-r--r--   0        0        0      776 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_id_types.py
+-rw-r--r--   0        0        0     1581 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2091 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1525 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     2124 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1202 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1535 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1166 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/exceptions/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/model/__init__.py
+-rw-r--r--   0        0        0     5781 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/model/metadata.py
+-rw-r--r--   0        0        0     7854 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/steps/dataset_reader.py
+-rw-r--r--   0        0        0     7837 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/steps/dataset_validator.py
+-rw-r--r--   0        0        0     1663 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/steps/metadata_inliner.py
+-rw-r--r--   0        0        0     1682 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/microdata_validator/steps/metadata_reader.py
+-rw-r--r--   0        0        0      652 2023-05-04 06:43:21.744052 microdata-validator-7.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2698 2023-05-04 06:44:00.025747 microdata-validator-7.3.1/setup.py
+-rw-r--r--   0        0        0     2417 2023-05-04 06:44:00.026638 microdata-validator-7.3.1/PKG-INFO
```

### Comparing `microdata-validator-7.3.0/LICENSE` & `microdata-validator-7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/README.md` & `microdata-validator-7.3.1/README.md`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/__init__.py` & `microdata-validator-7.3.1/microdata_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/adapter/local_storage.py` & `microdata-validator-7.3.1/microdata_validator/adapter/local_storage.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/temporal_attributes.py` & `microdata-validator-7.3.1/microdata_validator/components/temporal_attributes.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,31 +9,31 @@
             "description": [
                 {
                     "languageCode": "no",
                     "value": "Startdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Start date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Startdato"},
                 {"languageCode": "en", "value": "Start date"},
             ],
         },
         "STOP": {
             "description": [
                 {
                     "languageCode": "no",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stoppdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stop date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Stoppdato"},
                 {"languageCode": "en", "value": "Stop date"},
             ],
         },
@@ -43,31 +43,31 @@
             "description": [
                 {
                     "languageCode": "no",
                     "value": "Startdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Start date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Startdato"},
                 {"languageCode": "en", "value": "Start date"},
             ],
         },
         "STOP": {
             "description": [
                 {
                     "languageCode": "no",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stoppdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stop date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Stoppdato"},
                 {"languageCode": "en", "value": "Stop date"},
             ],
         },
@@ -77,31 +77,31 @@
             "description": [
                 {
                     "languageCode": "no",
                     "value": "Startdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Start date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Startdato"},
                 {"languageCode": "en", "value": "Start date"},
             ],
         },
         "STOP": {
             "description": [
                 {
                     "languageCode": "no",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stoppdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stop date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Stoppdato"},
                 {"languageCode": "en", "value": "Stop date"},
             ],
         },
@@ -111,31 +111,31 @@
             "description": [
                 {
                     "languageCode": "no",
                     "value": "Startdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Start date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Startdato"},
                 {"languageCode": "en", "value": "Start date"},
             ],
         },
         "STOP": {
             "description": [
                 {
                     "languageCode": "no",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stoppdato/måletidspunktet for hendelsen",
                 },
                 {
                     "languageCode": "en",
-                    "value": "Startdato/måletidspunktet for hendelsen",
+                    "value": "Stop date for event",
                 },
             ],
             "name": [
                 {"languageCode": "no", "value": "Stoppdato"},
                 {"languageCode": "en", "value": "Stop date"},
             ],
         },
```

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_id_types.py` & `microdata-validator-7.3.1/microdata_validator/components/unit_id_types.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'valueDomain'": "{'description': {0: {'value': 'Helsestasjonskonsultasjonbesøksid'}, 1: "*

 * *                  "{'value': 'Health center visit id'}}}"}*

```diff
@@ -46,16 +46,16 @@
         "requiresPseudonymization": false,
         "shortName": "BK_HELSESTASJONSKONSULTASJON"
     },
     "valueDomain": {
         "description": [
             {
                 "languageCode": "no",
-                "value": "Pseudonymisert helsestasjonskonsultasjonbes\u00f8ksid"
+                "value": "Helsestasjonskonsultasjonbes\u00f8ksid"
             },
             {
                 "languageCode": "en",
-                "value": "Pseudonymized healt center visit id"
+                "value": "Health center visit id"
             }
         ]
     }
 }
```

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/FAMILIE.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/FORETAK.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/HUSHOLDNING.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/JOBB.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KJORETOY.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KOMMUNE.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/KURS.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/PERSON.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/VIRKSOMHET.json` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/components/unit_type_variables/__init__.py` & `microdata-validator-7.3.1/microdata_validator/components/unit_type_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/model/__init__.py` & `microdata-validator-7.3.1/microdata_validator/model/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/model/metadata.py` & `microdata-validator-7.3.1/microdata_validator/model/metadata.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/steps/dataset_reader.py` & `microdata-validator-7.3.1/microdata_validator/steps/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/steps/dataset_validator.py` & `microdata-validator-7.3.1/microdata_validator/steps/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/steps/metadata_inliner.py` & `microdata-validator-7.3.1/microdata_validator/steps/metadata_inliner.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/microdata_validator/steps/metadata_reader.py` & `microdata-validator-7.3.1/microdata_validator/steps/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.0/pyproject.toml` & `microdata-validator-7.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-validator"
-version = "7.3.0"
+version = "7.3.1"
 description = "Python package for validating datasets in the microdata platform"
 authors = ["microdata-developers"]
 license = "Apache-2.0"
 repository = 'https://github.com/statisticsnorway/microdata-validator'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
```

### Comparing `microdata-validator-7.3.0/setup.py` & `microdata-validator-7.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'microdata-validator',
-    'version': '7.3.0',
+    'version': '7.3.1',
     'description': 'Python package for validating datasets in the microdata platform',
     'long_description': '# microdata-validator\n\nPython package for validating datasets in the microdata platform.\n\n\n### **Dataset description**\nA dataset as defined in microdata consists of one data file, and one metadata file.\n\nThe data file is a csv file seperated by semicolons. A valid example would be:\n```csv\n000000000000001;123;2020-01-01;2020-12-31;\n000000000000002;123;2020-01-01;2020-12-31;\n000000000000003;123;2020-01-01;2020-12-31;\n000000000000004;123;2020-01-01;2020-12-31;\n```\nRead more about the data format and columns in [the documentation](/docs).\n\nThe metadata files should be in json format. The requirements for the metadata is best described through the [json schema](/microdata_validator/schema/dataset_metadata_schema.json), [the examples](/docs/examples), and [the documentation](/docs).\n\n### **Basic usage**\n\nOnce you have your metadata and data files ready to go, they should be named and stored like this:\n```\nmy-input-directory/\n    MY_DATASET_NAME/\n        MY_DATASET_NAME.csv\n        MY_DATASET_NAME.json\n```\nNote that the filename only allows upper case letters A-Z, number 0-9 and underscores.\n\n\nThen use pip to install microdata-validator:\n```\npip install microdata-validator\n```\n\nImport microdata-validator in your script and validate your files:\n```py\nfrom microdata_validator import validate\n\nvalidation_errors = validate(\n    "MY_DATASET_NAME",\n    input_directory="path/to/my-input-directory"\n)\n\nif not validation_errors:\n    print("My dataset is valid")\nelse:\n    print("Dataset is invalid :(")\n    # You can print your errors like this:\n    for error in validation_errors:\n        print(error)\n```\n\n For a more in-depth explanation of usage visit [the usage documentation](/docs/USAGE.md).\n\n',
     'author': 'microdata-developers',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/statisticsnorway/microdata-validator',
```

### Comparing `microdata-validator-7.3.0/PKG-INFO` & `microdata-validator-7.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdata-validator
-Version: 7.3.0
+Version: 7.3.1
 Summary: Python package for validating datasets in the microdata platform
 Home-page: https://github.com/statisticsnorway/microdata-validator
 License: Apache-2.0
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

