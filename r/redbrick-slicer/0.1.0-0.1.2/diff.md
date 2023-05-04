# Comparing `tmp/redbrick-slicer-0.1.0.tar.gz` & `tmp/redbrick-slicer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbrick-slicer-0.1.0.tar", last modified: Wed May 11 12:24:57 2022, max compression
+gzip compressed data, was "redbrick-slicer-0.1.2.tar", last modified: Thu May  4 10:16:11 2023, max compression
```

## Comparing `redbrick-slicer-0.1.0.tar` & `redbrick-slicer-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/common/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/export.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/labeling.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/common/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/export/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/export/public.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/labeling/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/labeling/public.py
--rw-r--r--   0 runner    (1001) docker     (121)     4060 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/repo/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/repo/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/repo/labeling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/repo/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    14967 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/redbrick_slicer/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-11 12:24:57.000000 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-05-11 12:24:57.000000 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-11 12:24:57.000000 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-05-11 12:24:57.000000 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-11 12:24:57.000000 redbrick-slicer-0.1.0/redbrick_slicer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-11 12:24:57.825655 redbrick-slicer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-05-11 12:24:50.000000 redbrick-slicer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.727998 redbrick-slicer-0.1.2/redbrick_slicer/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/common/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/export/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/labeling/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/repo/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/redbrick_slicer/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 10:16:11.000000 redbrick-slicer-0.1.2/redbrick_slicer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-04 10:16:11.731998 redbrick-slicer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-04 10:16:00.000000 redbrick-slicer-0.1.2/setup.py
```

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/__init__.py` & `redbrick-slicer-0.1.2/redbrick_slicer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """RedBrick Slicer Integration Package."""
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 
 
 def get_task(
     url: str, token: str, endpoint: str = "https://api.redbrickai.com"
 ) -> None:
     """Interact with a RedBrick task in 3D Slicer application.
```

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/common/client.py` & `redbrick-slicer-0.1.2/redbrick_slicer/common/client.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/common/context.py` & `redbrick-slicer-0.1.2/redbrick_slicer/common/context.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/common/export.py` & `redbrick-slicer-0.1.2/redbrick_slicer/common/export.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/common/labeling.py` & `redbrick-slicer-0.1.2/redbrick_slicer/common/labeling.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/export/public.py` & `redbrick-slicer-0.1.2/redbrick_slicer/export/public.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/labeling/public.py` & `redbrick-slicer-0.1.2/redbrick_slicer/labeling/public.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/project.py` & `redbrick-slicer-0.1.2/redbrick_slicer/project.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/repo/labeling.py` & `redbrick-slicer-0.1.2/redbrick_slicer/repo/labeling.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/repo/project.py` & `redbrick-slicer-0.1.2/redbrick_slicer/repo/project.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/slicer.py` & `redbrick-slicer-0.1.2/redbrick_slicer/slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,61 +79,97 @@
             "cid": str(cat_id),
             "UMLSConceptUID": "C0344335",
             "CodeValue": str(cat_id),
             "contextGroupName": "CommonTissueSegmentationTypes",
             "SNOMEDCTConceptID": str(cat_id),
         }
 
+    def _cat2catNew(self, category: Dict, cat_id: int) -> Dict:
+        self.segment_color_map[category["category"]] = [
+            int(category["color"][i : i + 2], 16) for i in (1, 3, 5)
+        ]
+        return {
+            "recommendedDisplayRGBValue": self.segment_color_map[category["category"]],
+            "CodeMeaning": category["category"],
+            "CodingSchemeDesignator": "SCT",
+            "3dSlicerLabel": category["category"],
+            "3dSlicerIntegerLabel": cat_id,
+            "cid": str(cat_id),
+            "UMLSConceptUID": "C0344335",
+            "CodeValue": str(cat_id),
+            "contextGroupName": "CommonTissueSegmentationTypes",
+            "SNOMEDCTConceptID": str(cat_id),
+        }
+
     @no_type_check
     def get_task(self) -> None:
         """Get task for labeling."""
         task, taxonomy = self.project.export.get_raw_data_single(self.task_id)
 
-        parent_cat = taxonomy.get("categories", [])
-        if len(parent_cat) == 1 and parent_cat[0]["name"] == "object":
-            for child in parent_cat[0]["children"]:
-                self.segments += RBSlicer._get_categories(child)
+        if taxonomy.get("isNew"):
+            self.segments = [
+                cat["category"]
+                for cat in taxonomy["objectTypes"]
+                if cat["labelType"] == "SEGMENTATION" and not cat.get("archived")
+            ]
+        else:
+            parent_cat = taxonomy.get("categories", [])
+            if len(parent_cat) == 1 and parent_cat[0]["name"] == "object":
+                for child in parent_cat[0]["children"]:
+                    self.segments += RBSlicer._get_categories(child)
 
         if not self.segments:
             print("Unsupported taxonomy")
             return
 
         print("Available categories:", self.segments)
 
         slicer.mrmlScene.Clear(0)
 
+        taxName = re.sub(r"[^a-zA-Z]", "", taxonomy["name"])
+
         term_json_file = os.path.join(self.project_dir, "terminologies.json")
         term_json = {
-            "SegmentationCategoryTypeContextName": taxonomy["name"],
+            "SegmentationCategoryTypeContextName": taxName,
             "@schema": "https://raw.githubusercontent.com/qiicr/dcmqi/master/doc/segment-context-schema.json#",
             "SegmentationCodes": {
                 "Category": [
                     {
                         "CodeMeaning": "Categories",
                         "CodingSchemeDesignator": "SCT",
                         "showAnatomy": True,
                         "cid": "7150",
                         "CodeValue": "85756007",
                         "contextGroupName": "SegmentationPropertyCategories",
                         "Type": [
-                            self._cat2cat(cat, idx + 1, taxonomy["colorMap"])
+                            self._cat2catNew(
+                                [
+                                    obj_type
+                                    for obj_type in taxonomy["objectTypes"]
+                                    if obj_type["labelType"] == "SEGMENTATION"
+                                    and not obj_type.get("archived")
+                                    and obj_type["category"] == cat
+                                ][0],
+                                idx + 1,
+                            )
+                            if taxonomy.get("isNew")
+                            else self._cat2cat(cat, idx + 1, taxonomy["colorMap"])
                             for idx, cat in enumerate(self.segments)
                         ],
                     }
                 ],
             },
         }
 
         with open(term_json_file, "w", encoding="utf-8") as file_:
             json.dump(term_json, file_, indent=2)
 
         termLogic = slicer.util.getModuleLogic("Terminologies")
         termLogic.LoadTerminologyFromFile(term_json_file)
 
-        taxName = re.sub(r"[^a-zA-Z]", "", taxonomy["name"])
         slicer.app.settings().setValue("Terminology/LastTerminologyContext", taxName)
         defaultCat = f"{taxName}~SCT^85756007^Categories~^^~^^~Anatomic codes - DICOM master list~^^~^^"
         slicer.app.settings().setValue(
             "Segmentations/DefaultTerminologyEntry", defaultCat
         )
 
         loop = asyncio.get_event_loop()
```

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/utils/async_utils.py` & `redbrick-slicer-0.1.2/redbrick_slicer/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/utils/files.py` & `redbrick-slicer-0.1.2/redbrick_slicer/utils/files.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer/utils/url.py` & `redbrick-slicer-0.1.2/redbrick_slicer/utils/url.py`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/redbrick_slicer.egg-info/SOURCES.txt` & `redbrick-slicer-0.1.2/redbrick_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/setup.cfg` & `redbrick-slicer-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `redbrick-slicer-0.1.0/setup.py` & `redbrick-slicer-0.1.2/setup.py`

 * *Files identical despite different names*

