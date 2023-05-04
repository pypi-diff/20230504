# Comparing `tmp/itkwasm_dicom_emscripten-2.0.0.tar.gz` & `tmp/itkwasm_dicom_emscripten-2.0.1.tar.gz`

## Comparing `itkwasm_dicom_emscripten-2.0.0.tar` & `itkwasm_dicom_emscripten-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/_version.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/js_package.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/__init__.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/fixtures.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/test_apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/test_itkwasm_dicom.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/test_read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/test_structured_report_to_html_async.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/test/test_structured_report_to_text_async.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/README.md
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/_version.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/js_package.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_text_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/fixtures.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_itkwasm_dicom.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_html_async.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/README.md
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.1/PKG-INFO
```

### Comparing `itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.1/itkwasm_dicom_emscripten/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/test/test_apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.1/test/test_apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/test/test_itkwasm_dicom.py` & `itkwasm_dicom_emscripten-2.0.1/test/test_itkwasm_dicom.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/test/test_read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.1/test/test_read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/test/test_structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/test/test_structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.1/test/test_structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/pyproject.toml` & `itkwasm_dicom_emscripten-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.0/PKG-INFO` & `itkwasm_dicom_emscripten-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-emscripten
-Version: 2.0.0
+Version: 2.0.1
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

