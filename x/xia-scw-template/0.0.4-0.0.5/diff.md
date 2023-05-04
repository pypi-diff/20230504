# Comparing `tmp/xia_scw_template-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_template-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 100773 bytes, number of entries: 10
--rw-r--r--  2.0 unx      107 b- defN 23-May-01 05:15 xia_scw_template/__init__.py
--rw-r--r--  2.0 unx   236032 b- defN 23-May-01 06:22 xia_scw_template/template.cp39-win_amd64.pyd
+Zip file size: 101421 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      107 b- defN 23-May-04 04:49 xia_scw_template/__init__.py
+-rw-r--r--  2.0 unx   237568 b- defN 23-May-04 04:52 xia_scw_template/template.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx      414 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/main.tf
 -rw-rw-rw-  2.0 unx      124 b- defN 23-May-01 05:15 xia_scw_template/templates/ScwTemplate/output.tf
 -rw-rw-rw-  2.0 unx      136 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      698 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      933 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/RECORD
-10 files, 238712 bytes uncompressed, 99141 bytes compressed:  58.5%
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-04 04:52 xia_scw_template-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      672 b- defN 23-May-04 04:52 xia_scw_template-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-04 04:52 xia_scw_template-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-04 04:52 xia_scw_template-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      933 b- defN 23-May-04 04:52 xia_scw_template-0.0.5.dist-info/RECORD
+10 files, 240220 bytes uncompressed, 99789 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: xia_scw_template/templates/ScwTemplate/output.tf
 Comment: 
 
 Filename: xia_scw_template/templates/ScwTemplate/variables.tf
 Comment: 
 
-Filename: xia_scw_template-0.0.4.dist-info/LICENSE.txt
+Filename: xia_scw_template-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.4.dist-info/METADATA
+Filename: xia_scw_template-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_template-0.0.4.dist-info/WHEEL
+Filename: xia_scw_template-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_template-0.0.4.dist-info/top_level.txt
+Filename: xia_scw_template-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.4.dist-info/RECORD
+Filename: xia_scw_template-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_template/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_template.template import ScwTemplate
 
 
 __all__ = [
     "ScwTemplate"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_scw_template-0.0.4.dist-info/METADATA` & `xia_scw_template-0.0.5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: xia-scw-template
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine-terraform
-Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-template.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-scw-template/
 
 ====================================
 X-I-A
```

## Comparing `xia_scw_template-0.0.4.dist-info/RECORD` & `xia_scw_template-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-xia_scw_template/__init__.py,sha256=tmPmPL3cUvog_LwiX_pLoNJEVFY244P4UUJeL7eDnM4,107
-xia_scw_template/template.cp39-win_amd64.pyd,sha256=uzXLSWSzBk9kaafZ7uxPs_eTg-Jt3K98oK0pki-3lcw,236032
+xia_scw_template/__init__.py,sha256=ZsN_jBptY_mX_rofnWQrmizjgAiZ1EhZeGOWx9XSbNo,107
+xia_scw_template/template.cp39-win_amd64.pyd,sha256=XcZriY-TMVI6gu8PUvDu3UzTozXz8j8Mdg2tl9W8pZE,237568
 xia_scw_template/templates/ScwTemplate/main.tf,sha256=USKe9YPVicChcPSxUbZP_-f-kcFqLY4Ssi3zkPkHS8Q,414
 xia_scw_template/templates/ScwTemplate/output.tf,sha256=DfWBNaXPS42F-qEgemsPOWdtPMiqaUN-1ekPd_h7nyc,124
 xia_scw_template/templates/ScwTemplate/variables.tf,sha256=aR-VP5gMS05TmxMvdMAIuKoGmfNULd0cBGUqelhyCv8,136
-xia_scw_template-0.0.4.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
-xia_scw_template-0.0.4.dist-info/METADATA,sha256=M0iL1hfqariA86gmpN1ptCaGb2aspJ2oOdWI18wtTLY,698
-xia_scw_template-0.0.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_template-0.0.4.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
-xia_scw_template-0.0.4.dist-info/RECORD,,
+xia_scw_template-0.0.5.dist-info/LICENSE.txt,sha256=2HzK8y__YhkYAEzI5V38DGwiVGnADL74BLH_dyBEs7I,150
+xia_scw_template-0.0.5.dist-info/METADATA,sha256=ekBVE3ljVGIVi-dA2_rNEmReOyeyvkuefwW6m_YSsIo,672
+xia_scw_template-0.0.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_template-0.0.5.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
+xia_scw_template-0.0.5.dist-info/RECORD,,
```

