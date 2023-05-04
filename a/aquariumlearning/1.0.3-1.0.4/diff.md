# Comparing `tmp/aquariumlearning-1.0.3.tar.gz` & `tmp/aquariumlearning-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquariumlearning-1.0.3.tar", last modified: Wed Apr 19 20:02:08 2023, max compression
+gzip compressed data, was "dist/aquariumlearning-1.0.4.tar", last modified: Thu May  4 19:40:12 2023, max compression
```

## Comparing `aquariumlearning-1.0.3.tar` & `aquariumlearning-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/README.md
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning/
--rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/__init__.py
--rw-r--r--   0 robinyang   (501) staff       (20)    27866 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/base_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/class_map.py
--rw-r--r--   0 robinyang   (501) staff       (20)    82398 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/collection_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/coordinate_frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/dataset_client.py
--rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-03-27 18:45:55.000000 aquariumlearning-1.0.3/aquariumlearning/datasets.py
--rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-03-27 18:45:55.000000 aquariumlearning-1.0.3/aquariumlearning/datasharing.py
--rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/embedding_distance_sampling.py
--rw-r--r--   0 robinyang   (501) staff       (20)    36142 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/frames.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17446 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/inferences.py
--rw-r--r--   0 robinyang   (501) staff       (20)    18378 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/metrics_manager.py
--rw-r--r--   0 robinyang   (501) staff       (20)    17181 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/aquariumlearning/modified_labels.py
--rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/sampling_agent.py
--rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/segments.py
--rw-r--r--   0 robinyang   (501) staff       (20)    19457 2023-04-10 17:47:19.000000 aquariumlearning-1.0.3/aquariumlearning/sensor_data.py
--rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.3/aquariumlearning/turbo.py
--rw-r--r--   0 robinyang   (501) staff       (20)    18392 2023-04-12 17:37:02.000000 aquariumlearning-1.0.3/aquariumlearning/util.py
--rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.3/aquariumlearning/viridis.py
--rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-03-15 18:23:45.000000 aquariumlearning-1.0.3/aquariumlearning/work_queues.py
-drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/
--rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/PKG-INFO
--rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/SOURCES.txt
--rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/dependency_links.txt
--rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/requires.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/aquariumlearning.egg-info/top_level.txt
--rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-04-19 20:02:08.000000 aquariumlearning-1.0.3/setup.cfg
--rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-04-19 20:00:57.000000 aquariumlearning-1.0.3/setup.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      125 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/README.md
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning/
+-rw-r--r--   0 robinyang   (501) staff       (20)     5264 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/__init__.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    27894 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/base_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19772 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/class_map.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    82456 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    37335 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/collection_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    13675 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/coordinate_frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4221 2023-04-20 18:28:38.000000 aquariumlearning-1.0.4/aquariumlearning/dataset_client.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    45024 2023-03-27 18:45:55.000000 aquariumlearning-1.0.4/aquariumlearning/datasets.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     4405 2023-03-27 18:45:55.000000 aquariumlearning-1.0.4/aquariumlearning/datasharing.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     5319 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/embedding_distance_sampling.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    36142 2023-05-04 17:33:24.000000 aquariumlearning-1.0.4/aquariumlearning/frames.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17446 2023-04-24 23:38:39.000000 aquariumlearning-1.0.4/aquariumlearning/inferences.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    21566 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    23775 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/metrics_manager.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    17181 2023-04-24 23:38:39.000000 aquariumlearning-1.0.4/aquariumlearning/modified_labels.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     1768 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/sampling_agent.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    28949 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/segments.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    19457 2023-04-10 17:47:19.000000 aquariumlearning-1.0.4/aquariumlearning/sensor_data.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     8622 2023-02-08 03:39:31.000000 aquariumlearning-1.0.4/aquariumlearning/turbo.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    18412 2023-05-04 19:32:27.000000 aquariumlearning-1.0.4/aquariumlearning/util.py
+-rw-r--r--   0 robinyang   (501) staff       (20)     9477 2023-02-08 03:39:31.000000 aquariumlearning-1.0.4/aquariumlearning/viridis.py
+-rw-r--r--   0 robinyang   (501) staff       (20)    10213 2023-03-15 18:23:45.000000 aquariumlearning-1.0.4/aquariumlearning/work_queues.py
+drwxr-xr-x   0 robinyang   (501) staff       (20)        0 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/
+-rw-r--r--   0 robinyang   (501) staff       (20)      642 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/PKG-INFO
+-rw-r--r--   0 robinyang   (501) staff       (20)      919 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)        1 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)      349 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/requires.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       17 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/aquariumlearning.egg-info/top_level.txt
+-rw-r--r--   0 robinyang   (501) staff       (20)       38 2023-05-04 19:40:12.000000 aquariumlearning-1.0.4/setup.cfg
+-rw-r--r--   0 robinyang   (501) staff       (20)     1373 2023-05-04 19:32:56.000000 aquariumlearning-1.0.4/setup.py
```

### Comparing `aquariumlearning-1.0.3/PKG-INFO` & `aquariumlearning-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.3
+Version: 1.0.4
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning/__init__.py` & `aquariumlearning-1.0.4/aquariumlearning/__init__.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/base_labels.py` & `aquariumlearning-1.0.4/aquariumlearning/base_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
     def to_dict(self) -> Dict[str, Any]:
         label_dict = {
             "uuid": self.id,
             "label_type": self.label_type,
             "label": self.classification,
             "class_id": self.classification_id,
-            "label_coordinate_frame": self.sensor_id,
+            "label_coordinate_frame": self.sensor_id or self.coordinate_frame_id,
             "attributes": self.attributes,
             "reuse_latest_embedding": self.reuse_latest_embedding,
             "change": self.update_type,
         }
 
         if self.update_type == "MODIFY":
             # only return the fields that are populated
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning/class_map.py` & `aquariumlearning-1.0.4/aquariumlearning/class_map.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/client.py` & `aquariumlearning-1.0.4/aquariumlearning/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,15 +561,15 @@
             project_name, dataset_name
         )
         r = requests_retry.delete(url, headers=self._get_creds_headers())
 
         raise_resp_exception_error(r)
 
     def dataset_exists(self, project_name: str, dataset_name: str) -> bool:
-        """Check if a dataset exists.
+        """Check if a dataset exists. This includes datasets that have been archived.
 
         Args:
             project_name (str): project_name
             dataset_name (str): dataset_name
 
         Returns:
             bool: Whether the dataset already exists.
@@ -885,15 +885,15 @@
         project_name: str,
         dataset_name: str,
         upload_prefix: str,
         upload_suffix: str,
         file_names: List[str],
         delete_after_upload: bool = True,
         bucket: str = "aquarium-dev",
-        file_metadata: List[Dict[str, str]] = None,
+        file_metadata: Optional[List[Dict[str, str]]] = None,
     ) -> List[str]:
         # Get upload / download URLs
         get_upload_path = (
             self.api_endpoint
             + "/projects/{}/datasets/{}/get_upload_url".format(
                 project_name, dataset_name
             )
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning/collection_client.py` & `aquariumlearning-1.0.4/aquariumlearning/collection_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/coordinate_frames.py` & `aquariumlearning-1.0.4/aquariumlearning/coordinate_frames.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/dataset_client.py` & `aquariumlearning-1.0.4/aquariumlearning/dataset_client.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/datasets.py` & `aquariumlearning-1.0.4/aquariumlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/datasharing.py` & `aquariumlearning-1.0.4/aquariumlearning/datasharing.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/embedding_distance_sampling.py` & `aquariumlearning-1.0.4/aquariumlearning/embedding_distance_sampling.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/frames.py` & `aquariumlearning-1.0.4/aquariumlearning/frames.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/inferences.py` & `aquariumlearning-1.0.4/aquariumlearning/inferences.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/labels.py` & `aquariumlearning-1.0.4/aquariumlearning/labels.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Dict, List, Optional, Union, Tuple, cast
+from typing import Any, Dict, List, Optional, Union
+from typing_extensions import TypedDict
 
 from .dataset_client import DatasetClient
 from .base_labels import (
     Coordinate2D,
     _BaseCrop,
-    _BaseSingleCrop,
     _BaseCropSet,
     _Bbox2D,
     _Classification2D,
     _Classification3D,
     _Cuboid3D,
     _Keypoint2D,
     _LineSegment2D,
@@ -468,46 +468,134 @@
     Classification2DLabel,
     Classification3DLabel,
     Cuboid3DLabel,
     TextTokenLabel,
 ]
 
 
+class _CommonLabelKwargs(TypedDict):
+    id: str
+    classification: str
+    sensor_id: str
+    user_attrs: Dict[str, Any]
+
+
 def _get_single_label_from_json(label_json: Dict[str, Any]) -> Label:
-    iscrowd = label_json["attributes"].pop("iscrowd", None)
     label_type = label_json["label_type"]
-    # instantiate base sensor directly & cast to the right class
-    base_label = _BaseSingleCrop(
+
+    iscrowd = label_json["attributes"].pop("iscrowd", None)
+    user_attrs = {
+        key: value
+        for key, value in label_json["attributes"].items()
+        if key.startswith("user__")
+    }
+    base_label_kwargs = _CommonLabelKwargs(
         id=label_json["uuid"],
-        update_type="ADD",
-        label_type=label_json["label_type"],
         classification=label_json["label"],
         sensor_id=label_json["label_coordinate_frame"],
-        iscrowd=iscrowd,
-        attributes=label_json["attributes"],
+        user_attrs=user_attrs,
     )
 
     if label_type == "BBOX_2D":
-        return cast(Bbox2DLabel, base_label)
+        top = label_json["attributes"]["top"]
+        left = label_json["attributes"]["left"]
+        width = label_json["attributes"]["width"]
+        height = label_json["attributes"]["height"]
+        return Bbox2DLabel(
+            **base_label_kwargs,
+            iscrowd=iscrowd,
+            top=top,
+            left=left,
+            width=width,
+            height=height,
+        )
     elif label_type == "LINE_SEGMENT_2D":
-        return cast(LineSegment2DLabel, base_label)
+        x1 = label_json["attributes"]["x1"]
+        y1 = label_json["attributes"]["y1"]
+        x2 = label_json["attributes"]["x2"]
+        y2 = label_json["attributes"]["y2"]
+        return LineSegment2DLabel(
+            **base_label_kwargs, iscrowd=iscrowd, x1=x1, y1=y1, x2=x2, y2=y2
+        )
     elif label_type == "KEYPOINTS_2D":
-        return cast(Keypoint2DLabel, base_label)
+        keypoints = label_json["attributes"]["keypoints"]
+        top = label_json["attributes"].get("top")
+        left = label_json["attributes"].get("left")
+        width = label_json["attributes"].get("width")
+        height = label_json["attributes"].get("height")
+        polygons = label_json["attributes"].get("polygons")
+        center = label_json["attributes"].get("center")
+        return Keypoint2DLabel(
+            **base_label_kwargs,
+            iscrowd=iscrowd,
+            keypoints=keypoints,
+            top=top,
+            left=left,
+            width=width,
+            height=height,
+            polygons=polygons,
+            center=center,
+        )
     elif label_type == "POLYGON_LIST_2D":
-        return cast(PolygonList2DLabel, base_label)
+        polygons = label_json["attributes"]["polygons"]
+        center = label_json["attributes"].get("center")
+        return PolygonList2DLabel(
+            **base_label_kwargs, iscrowd=iscrowd, polygons=polygons, center=center
+        )
     elif label_type == "SEMANTIC_LABEL_URL_2D":
-        return cast(Semseg2DLabel, base_label)
+        mask_url = label_json["attributes"]["url"]
+        resize_mode = label_json["attributes"].get("resize_mode")
+        return Semseg2DLabel(
+            id=label_json["uuid"],
+            mask_url=mask_url,
+            resize_mode=resize_mode,
+            sensor_id=label_json["label_coordinate_frame"],
+        )
     elif label_type == "CLASSIFICATION_2D":
-        return cast(Classification2DLabel, base_label)
+        secondary_labels = {
+            key: value
+            for key, value in label_json["attributes"].items()
+            if not key.startswith("user__") and not key.startswith("derived__")
+        }
+        return Classification2DLabel(
+            **base_label_kwargs, secondary_labels=secondary_labels
+        )
     elif label_type == "CLASSIFICATION_3D":
-        return cast(Classification3DLabel, base_label)
+        return Classification3DLabel(**base_label_kwargs)
     elif label_type == "CUBOID_3D":
-        return cast(Cuboid3DLabel, base_label)
+        pos_x = label_json["attributes"]["pos_x"]
+        pos_y = label_json["attributes"]["pos_y"]
+        pos_z = label_json["attributes"]["pos_z"]
+        position = [pos_x, pos_y, pos_z]
+        dim_x = label_json["attributes"]["dim_x"]
+        dim_y = label_json["attributes"]["dim_y"]
+        dim_z = label_json["attributes"]["dim_z"]
+        dimensions = [dim_x, dim_y, dim_z]
+        rot_x = label_json["attributes"]["rot_x"]
+        rot_y = label_json["attributes"]["rot_y"]
+        rot_z = label_json["attributes"]["rot_z"]
+        rot_w = label_json["attributes"]["rot_w"]
+        rotation = [rot_x, rot_y, rot_z, rot_w]
+
+        return Cuboid3DLabel(
+            id=label_json["uuid"],
+            classification=label_json["label"],
+            coordinate_frame_id=label_json["label_coordinate_frame"],
+            position=position,
+            dimensions=dimensions,
+            rotation=rotation,
+            user_attrs=user_attrs,
+        )
     elif label_type == "TEXT_TOKEN":
-        return cast(TextTokenLabel, base_label)
+        index = label_json["attributes"]["index"]
+        token = label_json["attributes"]["token"]
+        visible = label_json["attributes"]["visible"]
+        return TextTokenLabel(
+            **base_label_kwargs, index=index, token=token, visible=visible
+        )
     else:
         raise Exception(f"Cannot reinstantiate a label of type {label_type}")
 
 
 def _get_instance_seg_label_from_jsons(
     mask_json: Dict[str, Any],
     instances: List[Dict[str, Any]],
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning/metrics_manager.py` & `aquariumlearning-1.0.4/aquariumlearning/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/modified_labels.py` & `aquariumlearning-1.0.4/aquariumlearning/modified_labels.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/sampling_agent.py` & `aquariumlearning-1.0.4/aquariumlearning/sampling_agent.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/segments.py` & `aquariumlearning-1.0.4/aquariumlearning/segments.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/sensor_data.py` & `aquariumlearning-1.0.4/aquariumlearning/sensor_data.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/turbo.py` & `aquariumlearning-1.0.4/aquariumlearning/turbo.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/util.py` & `aquariumlearning-1.0.4/aquariumlearning/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     get_upload_path: str,
     headers: Dict[str, Any],
     upload_prefix: str,
     upload_suffix: str,
     bucket: str = "aquarium-dev",
     delete_after_upload: bool = True,
     file_metadata: Optional[List[Dict[str, str]]] = None,
-    client_version: str = None,
+    client_version: Optional[str] = None,
 ) -> List[str]:
     """This uploads a set of files with a reader, and then deletes it.
 
     Args:
         file_names (str): The local file_names (files to be uploaded)
         get_upload_path (str): The URL that generates upload URLs
         headers (Dict[str, Any]): Headers for the get_upload_path request
@@ -503,15 +503,15 @@
     id: int
     classification: Optional[str]
     attributes: Optional[Dict[str, Any]]
 
     def __init__(
         self,
         id: int,
-        classification: str = None,
+        classification: Optional[str] = None,
         attributes: Optional[Dict[str, Any]] = None,
     ):
         self.id = id
         self.classification = classification
         self.attributes = attributes
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning/viridis.py` & `aquariumlearning-1.0.4/aquariumlearning/viridis.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning/work_queues.py` & `aquariumlearning-1.0.4/aquariumlearning/work_queues.py`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/aquariumlearning.egg-info/PKG-INFO` & `aquariumlearning-1.0.4/aquariumlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquariumlearning
-Version: 1.0.3
+Version: 1.0.4
 Summary: Aquarium Learning Python Client
 Home-page: https://www.aquariumlearning.com
 Author: Quinn Johnson
 Author-email: quinn@aquarium-learn.com
 License: UNKNOWN
 Description: # Aquarium Learning Python Client Library
```

### Comparing `aquariumlearning-1.0.3/aquariumlearning.egg-info/SOURCES.txt` & `aquariumlearning-1.0.4/aquariumlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquariumlearning-1.0.3/setup.py` & `aquariumlearning-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aquariumlearning",  # Replace with your own username
-    version="1.0.3",
+    version="1.0.4",
     author="Quinn Johnson",
     author_email="quinn@aquarium-learn.com",
     description="Aquarium Learning Python Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aquariumlearning.com",
     packages=setuptools.find_packages(
```

