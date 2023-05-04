# Comparing `tmp/unstructured_inference-0.4.2.tar.gz` & `tmp/unstructured_inference-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.4.2.tar", last modified: Fri Apr 21 04:10:10 2023, max compression
+gzip compressed data, was "unstructured_inference-0.4.3.tar", last modified: Thu May  4 20:32:37 2023, max compression
```

## Comparing `unstructured_inference-0.4.2.tar` & `unstructured_inference-0.4.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.078570 unstructured_inference-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.082570 unstructured_inference-0.4.2/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.086570 unstructured_inference-0.4.2/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/yolox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.082570 unstructured_inference-0.4.2/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-21 04:10:10.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.355679 unstructured_inference-0.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.355679 unstructured_inference-0.4.3/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.359679 unstructured_inference-0.4.3/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.359679 unstructured_inference-0.4.3/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.4.2/PKG-INFO` & `unstructured_inference-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.2/README.md` & `unstructured_inference-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/setup.py` & `unstructured_inference-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/api.py` & `unstructured_inference-0.4.3/unstructured_inference/api.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/inference/elements.py` & `unstructured_inference-0.4.3/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/inference/layout.py` & `unstructured_inference-0.4.3/unstructured_inference/inference/layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from __future__ import annotations
 import os
 import tempfile
 from typing import List, Optional, Tuple, Union, BinaryIO
 
 import numpy as np
-import pdfplumber
 import pdf2image
+from pdfminer import psparser
 from PIL import Image
 
 from unstructured_inference.inference.elements import (
     TextRegion,
     EmbeddedTextRegion,
     ImageTextRegion,
 )
 from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.logger import logger
 from unstructured_inference.models.base import get_model
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
+from unstructured_inference.patches.pdfminer import parse_keyword
+
+# NOTE(alan): Patching this to fix a bug in pdfminer.six. Submitted this PR into pdfminer.six to fix
+# the bug: https://github.com/pdfminer/pdfminer.six/pull/885
+psparser.PSBaseParser._parse_keyword = parse_keyword  # type: ignore
+
+import pdfplumber  # noqa
 
 VALID_OCR_STRATEGIES = (
     "auto",  # Use OCR when it looks like other methods have failed
     "force",  # Always use OCR
     "never",  # Never use OCR
 )
```

### Comparing `unstructured_inference-0.4.2/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.4.3/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/base.py` & `unstructured_inference-0.4.3/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.4.3/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/donut.py` & `unstructured_inference-0.4.3/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.4.3/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/tables.py` & `unstructured_inference-0.4.3/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.4.3/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.4.3/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/models/yolox.py` & `unstructured_inference-0.4.3/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/utils.py` & `unstructured_inference-0.4.3/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference/visualize.py` & `unstructured_inference-0.4.3/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.2/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.4.3/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.2/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.4.3/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

