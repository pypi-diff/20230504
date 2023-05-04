# Comparing `tmp/itkwasm_dicom_wasi-2.0.0.tar.gz` & `tmp/itkwasm_dicom_wasi-2.0.1.tar.gz`

## Comparing `itkwasm_dicom_wasi-2.0.0.tar` & `itkwasm_dicom_wasi-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/_version.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0    10287 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/structured_report_to_html.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/structured_report_to_text.py
--rwxr-xr-x   0        0        0  4530704 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
--rwxr-xr-x   0        0        0  1882868 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
--rwxr-xr-x   0        0        0  3972262 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
--rwxr-xr-x   0        0        0  3952009 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/test/test_apply_presentation_state_to_image.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/test/test_read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/test/test_structured_report_to_html.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/test/test_structured_report_to_text.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/README.md
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/_version.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_html.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_text.py
+-rwxr-xr-x   0        0        0  4530704 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
+-rwxr-xr-x   0        0        0  1882868 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
+-rwxr-xr-x   0        0        0  3972262 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
+-rwxr-xr-x   0        0        0  3952009 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_html.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_text.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/README.md
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-2.0.1/PKG-INFO
```

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated file. Do not edit.
 
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 import os
 from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
@@ -53,22 +53,22 @@
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.JsonObject),
         PipelineOutput(InterfaceTypes.Image),
     ]
 
     pipeline_inputs: List[PipelineInput] = [
-        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(image_in)),
-        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(presentation_state_file)),
+        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(PurePosixPath(image_in))),
+        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(PurePosixPath(presentation_state_file))),
     ]
 
     args: List[str] = ['--memory-io',]
     # Inputs
-    args.append(str(image_in))
-    args.append(str(presentation_state_file))
+    args.append(str(PurePosixPath(image_in)))
+    args.append(str(PurePosixPath(presentation_state_file)))
     # Outputs
     args.append('0')
     args.append('1')
     # Options
     if config_file:
         args.append('--config-file')
         args.append(str(config_file))
```

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated file. Do not edit.
 
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 import os
 from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
@@ -89,20 +89,20 @@
     pipeline = Pipeline(file_resources('itkwasm_dicom_wasi').joinpath(Path('wasm_modules') / Path('read-dicom-encapsulated-pdf.wasi.wasm')))
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.BinaryStream),
     ]
 
     pipeline_inputs: List[PipelineInput] = [
-        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(dicom_file)),
+        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(PurePosixPath(dicom_file))),
     ]
 
     args: List[str] = ['--memory-io',]
     # Inputs
-    args.append(str(dicom_file))
+    args.append(str(PurePosixPath(dicom_file)))
     # Outputs
     args.append('0')
     # Options
     if read_file_only:
         args.append('--read-file-only')
 
     if read_dataset:
```

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/structured_report_to_html.py` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated file. Do not edit.
 
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 import os
 from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
@@ -194,20 +194,20 @@
     pipeline = Pipeline(file_resources('itkwasm_dicom_wasi').joinpath(Path('wasm_modules') / Path('structured-report-to-html.wasi.wasm')))
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.TextStream),
     ]
 
     pipeline_inputs: List[PipelineInput] = [
-        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(dicom_file)),
+        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(PurePosixPath(dicom_file))),
     ]
 
     args: List[str] = ['--memory-io',]
     # Inputs
-    args.append(str(dicom_file))
+    args.append(str(PurePosixPath(dicom_file)))
     # Outputs
     args.append('0')
     # Options
     if read_file_only:
         args.append('--read-file-only')
 
     if read_dataset:
@@ -281,15 +281,15 @@
     if css_reference is not None:
         input_count_string = str(len(pipeline_inputs))
         pipeline_inputs.append(PipelineInput(InterfaceTypes.TextStream, TextStream(css_reference)))
         args.append('--css-reference')
         args.append(input_count_string)
 
     if css_file is not None:
-        input_file = str(css_file)
+        input_file = str(PurePosixPath(css_file))
         pipeline_inputs.append(PipelineInput(InterfaceTypes.TextFile, TextFile(css_file)))
         args.append('--css-file')
         args.append(input_file)
 
     if expand_inline:
         args.append('--expand-inline')
```

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/structured_report_to_text.py` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/structured_report_to_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated file. Do not edit.
 
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 import os
 from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
@@ -97,20 +97,20 @@
     pipeline = Pipeline(file_resources('itkwasm_dicom_wasi').joinpath(Path('wasm_modules') / Path('structured-report-to-text.wasi.wasm')))
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.TextStream),
     ]
 
     pipeline_inputs: List[PipelineInput] = [
-        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(dicom_file)),
+        PipelineInput(InterfaceTypes.BinaryFile, BinaryFile(PurePosixPath(dicom_file))),
     ]
 
     args: List[str] = ['--memory-io',]
     # Inputs
-    args.append(str(dicom_file))
+    args.append(str(PurePosixPath(dicom_file)))
     # Outputs
     args.append('0')
     # Options
     if unknown_relationship:
         args.append('--unknown-relationship')
 
     if invalid_item_value:
```

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm` & `itkwasm_dicom_wasi-2.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-2.0.0/test/test_apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-2.0.1/test/test_apply_presentation_state_to_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from pathlib import Path
+from pathlib import Path 
 import numpy as np
 import json
 
 def test_apply_presentation_state_to_dicom_image():
     from itkwasm_dicom_wasi import apply_presentation_state_to_image
 
     input_file = 'gsps-pstate-test-input-image.dcm'
-    input_file_path = Path('..', '..', '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', input_file)
+    input_file_path = Path('..', '..', 'test', 'data', 'input', input_file)
 
     p_state_file = 'gsps-pstate-test-input-pstate.dcm'
-    p_state_file_path = Path('..', '..', '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', p_state_file)
+    p_state_file_path = Path('..', '..', 'test', 'data', 'input', p_state_file)
 
     p_state_json_out, output_image = apply_presentation_state_to_image(input_file_path, p_state_file_path)
 
     assert p_state_json_out != None
     assert output_image != None
 
     assert output_image.imageType.dimension == 2
@@ -23,23 +23,23 @@
 
     assert np.array_equal(output_image.origin, [0, 0])
     assert np.array_equal(output_image.spacing, [0.683, 0.683])
     assert np.array_equal(output_image.direction, [[1, 0], [0, 1]])
     assert np.array_equal(output_image.size, [512, 512])
 
     baseline_json_file = 'gsps-pstate-baseline.json'
-    baseline_json_file_path = Path('..', '..', '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', baseline_json_file)
+    baseline_json_file_path = Path('..', '..', 'test', 'data', 'baseline', baseline_json_file)
     with open(baseline_json_file_path, 'r') as fp:
         # the slice operation removes the last EOF char from the baseline file.
         buffer = fp.read()[:-1]
     baseline_json_object = json.loads(buffer)
     assert baseline_json_object['PresentationLabel'] == p_state_json_out['PresentationLabel']
     assert baseline_json_object['PresentationSizeMode'] == p_state_json_out['PresentationSizeMode']
     assert str(baseline_json_object) == str(p_state_json_out)
 
     baseline_image = 'gsps-pstate-image-baseline.pgm'
-    baseline_image_file_path = Path('..', '..', '..', '..', 'build-emscripten','ExternalData', 'test', 'Input', baseline_image)
+    baseline_image_file_path = Path('..', '..', 'test', 'data', 'baseline', baseline_image)
     with open(baseline_image_file_path, 'rb') as fp:
         baseline_buffer = fp.read()
     # slice to get only the pixel buffer from the baseline image (pgm file)
     baseline_pixels = baseline_buffer[15:]
-    assert np.array_equal(np.frombuffer(baseline_pixels, dtype=np.uint8), output_image.data.ravel())
+    assert np.array_equal(np.frombuffer(baseline_pixels, dtype=np.uint8), output_image.data.ravel())
```

### Comparing `itkwasm_dicom_wasi-2.0.0/test/test_structured_report_to_html.py` & `itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_html.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 def test_structured_report_to_html():
     from itkwasm_dicom_wasi import structured_report_to_html
     file_name = '88.33-comprehensive-SR.dcm'
-    test_file_path = Path('..', '..' , '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', file_name)
+    test_file_path = Path('..', '..' , 'test', 'data', 'input', file_name)
 
     assert test_file_path.exists()
 
     output_text = structured_report_to_html(test_file_path)
     assert output_text.find('Comprehensive SR Document') != -1
     assert output_text.find('Breast Diagnosis 010001 (female, #BreastDx-01-0001)') != -1
     assert output_text.find('PixelMed (XSLT from di3data csv extract)') != -1
@@ -18,39 +18,39 @@
 
     output_text = structured_report_to_html(test_file_path, render_all_codes=True)
     assert output_text.find('Overall Assessment (111413, DCM)') != -1
 
 def test_read_radiation_dose_sr():
     from itkwasm_dicom_wasi import structured_report_to_html
     file_name = '88.67-radiation-dose-SR.dcm'
-    test_file_path = Path('..', '..' , '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', file_name)
+    test_file_path = Path('..', '..' , 'test', 'data', 'input', file_name)
 
     assert test_file_path.exists()
 
     output_text = structured_report_to_html(test_file_path)
     assert output_text.find('<title>X-Ray Radiation Dose SR Document</title>') != -1
     assert output_text.find('<h2>CT Accumulated Dose Data</h2>') != -1
 
 def test_read_key_object_selection_sr():
     from itkwasm_dicom_wasi import structured_report_to_html
     file_name = '88.59-KeyObjectSelection-SR.dcm'
-    test_file_path = Path('..', '..' , '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', file_name)
+    test_file_path = Path('..', '..' , 'test', 'data', 'input', file_name)
 
     assert test_file_path.exists()
 
     url_prefix = 'http://my-custom-dicom-server/dicom.cgi'
     output_text = structured_report_to_html(test_file_path,
       url_prefix=url_prefix,
       css_reference="https://css-host/dir/subdir/my-first-style.css")
     assert output_text.find(url_prefix) != -1
     assert output_text.find('http://localhost/dicom.cgi') == -1
     assert output_text.find('<link rel="stylesheet" type="text/css" href="https://css-host/dir/subdir/my-first-style.css">') != -1
 
     css_file_name = 'test-style.css'
-    test_css_file_path = Path('..', '..', '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', css_file_name)
+    test_css_file_path = Path('..', '..', 'test', 'data', 'input', css_file_name)
     output_text = structured_report_to_html(test_file_path, css_file=test_css_file_path)
 
     assert output_text.find('<style type="text/css">') != -1
     assert output_text.find('background-color: lightblue;')
     assert output_text.find('margin-left: 20px;') != -1
     assert output_text.find('</style>') != -1
     assert output_text.find('http://my-custom-dicom-server/dicom.cgi') == -1
```

### Comparing `itkwasm_dicom_wasi-2.0.0/test/test_structured_report_to_text.py` & `itkwasm_dicom_wasi-2.0.1/test/test_structured_report_to_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 def test_structured_report_to_text():
     from itkwasm_dicom_wasi import structured_report_to_text
     file_name = '88.33-comprehensive-SR.dcm'
-    test_file_path = Path('..', '..' , '..', '..', 'build-emscripten', 'ExternalData', 'test', 'Input', file_name)
+    test_file_path = Path('..', '..' , 'test', 'data', 'input', file_name)
 
     assert test_file_path.exists()
 
     output_text = structured_report_to_text(test_file_path)
     assert output_text.find('Comprehensive SR Document') != -1
     assert output_text.find('Pathology') != -1
```

### Comparing `itkwasm_dicom_wasi-2.0.0/pyproject.toml` & `itkwasm_dicom_wasi-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "itkwasm",
   "webassembly",
   "wasi",
 ]
 
 requires-python = ">=3.7"
 dependencies = [
-    "itkwasm >= 1.0.b102",
+    "itkwasm >= 1.0.b104",
     "importlib_resources",
 
 ]
 
 [tool.hatch.version]
 path = "itkwasm_dicom_wasi/_version.py"
```

### Comparing `itkwasm_dicom_wasi-2.0.0/PKG-INFO` & `itkwasm_dicom_wasi-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-wasi
-Version: 2.0.0
+Version: 2.0.1
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources
-Requires-Dist: itkwasm>=1.0.b102
+Requires-Dist: itkwasm>=1.0.b104
 Description-Content-Type: text/markdown
 
 # itkwasm-dicom-wasi
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-dicom-wasi.svg)](https://badge.fury.io/py/itkwasm-dicom-wasi)
 
 Read files and images related to DICOM file format. WASI implementation.
```

