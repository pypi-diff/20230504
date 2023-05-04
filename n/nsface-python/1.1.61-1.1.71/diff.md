# Comparing `tmp/nsface_python-1.1.61-py3-none-any.whl.zip` & `tmp/nsface_python-1.1.71-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 202854 bytes, number of entries: 94
+Zip file size: 204885 bytes, number of entries: 95
 -rw-r--r--  2.0 unx      191 b- defN 23-Jan-26 22:19 nsface/__init__.py
 -rw-r--r--  2.0 unx     4395 b- defN 23-Jan-26 22:19 nsface/bbox_anchor.py
 -rw-r--r--  2.0 unx    13954 b- defN 23-Jan-26 22:19 nsface/eval_widerface.py
 -rw-r--r--  2.0 unx    14998 b- defN 23-Jan-26 22:19 nsface/get_config.py
 -rw-r--r--  2.0 unx     6322 b- defN 23-Jan-26 22:19 nsface/get_widerface_txt.py
 -rw-r--r--  2.0 unx     2389 b- defN 23-Jan-26 22:19 nsface/onnx2trt.py
 -rw-r--r--  2.0 unx       72 b- defN 23-Jan-26 22:19 nsface/print_info.py
@@ -41,56 +41,57 @@
 -rw-r--r--  2.0 unx       87 b- defN 23-Jan-26 22:19 nsface/eval/verification/eval_util/__init__.py
 -rw-r--r--  2.0 unx    18457 b- defN 23-Jan-26 22:19 nsface/eval/verification/eval_util/verification.py
 -rw-r--r--  2.0 unx    17798 b- defN 23-Jan-26 22:19 nsface/eval/verification/eval_util/verification_g.py
 -rw-r--r--  2.0 unx    16539 b- defN 23-Jan-26 22:19 nsface/eval/verification/eval_util/verification_m.py
 -rw-r--r--  2.0 unx       67 b- defN 23-Jan-26 22:19 nsface/face/__init__.py
 -rw-r--r--  2.0 unx     6642 b- defN 23-Jan-27 01:05 nsface/face/blur.py
 -rw-r--r--  2.0 unx      400 b- defN 23-Jan-26 22:19 nsface/face/common.py
--rw-r--r--  2.0 unx    14039 b- defN 23-Apr-12 06:42 nsface/face/get_result.py
+-rw-r--r--  2.0 unx    14772 b- defN 23-May-04 00:29 nsface/face/get_result.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Jan-26 22:19 nsface/model_zoo/__init__.py
--rw-r--r--  2.0 unx     4119 b- defN 23-Apr-12 06:03 nsface/model_zoo/get_models.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-May-04 00:35 nsface/model_zoo/get_models.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/__init__.py
 -rw-r--r--  2.0 unx    15538 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/groupface.py
 -rw-r--r--  2.0 unx     7801 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/iresnet.py
 -rw-r--r--  2.0 unx     4895 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/mobilefacenet.py
 -rw-r--r--  2.0 unx     4598 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/net.py
 -rw-r--r--  2.0 unx     2493 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/race_linear.py
 -rw-r--r--  2.0 unx     5530 b- defN 23-Jan-26 22:19 nsface/model_zoo/backbones/retinaface.py
--rw-r--r--  2.0 unx       91 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_attribute/__init__.py
--rw-r--r--  2.0 unx     2287 b- defN 23-Apr-24 06:38 nsface/model_zoo/model_attribute/arcface_GenderAge.py
--rw-r--r--  2.0 unx     2060 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_attribute/arcface_Race.py
+-rw-r--r--  2.0 unx      201 b- defN 23-May-04 00:10 nsface/model_zoo/model_attribute/__init__.py
+-rw-r--r--  2.0 unx     2723 b- defN 23-May-03 07:15 nsface/model_zoo/model_attribute/arcface_GenderAge.py
+-rw-r--r--  2.0 unx     2327 b- defN 23-May-03 07:15 nsface/model_zoo/model_attribute/arcface_Race.py
+-rw-r--r--  2.0 unx     3361 b- defN 23-May-04 00:38 nsface/model_zoo/model_attribute/expression.py
+-rw-r--r--  2.0 unx     3618 b- defN 23-May-04 00:17 nsface/model_zoo/model_attribute/liveness.py
+-rw-r--r--  2.0 unx     3011 b- defN 23-Mar-20 03:25 nsface/model_zoo/model_attribute/mask_detector.py
 -rw-r--r--  2.0 unx      207 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_common/__init__.py
 -rw-r--r--  2.0 unx     2719 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_common/load_onnx.py
 -rw-r--r--  2.0 unx     3354 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_common/load_openvino.py
 -rw-r--r--  2.0 unx     3603 b- defN 23-Apr-13 06:23 nsface/model_zoo/model_common/load_tensorRT.py
 -rw-r--r--  2.0 unx     6037 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_common/load_tensorRT_multiple.py
 -rw-r--r--  2.0 unx     7325 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_common/load_torch.py
--rw-r--r--  2.0 unx      251 b- defN 23-Apr-12 05:49 nsface/model_zoo/model_detection/__init__.py
+-rw-r--r--  2.0 unx      180 b- defN 23-May-04 00:10 nsface/model_zoo/model_detection/__init__.py
 -rw-r--r--  2.0 unx     8151 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/blazeface.py
 -rw-r--r--  2.0 unx     7872 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/blazeface640.py
 -rw-r--r--  2.0 unx     1126 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/dlib_detector.py
--rw-r--r--  2.0 unx     3351 b- defN 23-Apr-12 06:38 nsface/model_zoo/model_detection/liveness.py
--rw-r--r--  2.0 unx     3011 b- defN 23-Mar-20 03:25 nsface/model_zoo/model_detection/mask_detector.py
 -rw-r--r--  2.0 unx     8137 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/retinaface_insightface.py
 -rw-r--r--  2.0 unx     9723 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/retinaface_torch.py
 -rw-r--r--  2.0 unx    11771 b- defN 23-Mar-16 07:00 nsface/model_zoo/model_detection/scrfd.py
 -rw-r--r--  2.0 unx     8636 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_detection/scrfd_pre.py
 -rw-r--r--  2.0 unx       29 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_landmark/__init__.py
 -rw-r--r--  2.0 unx     2564 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_landmark/det2d106.py
 -rw-r--r--  2.0 unx    12050 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_landmark/pipnet.py
--rw-r--r--  2.0 unx     5471 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_landmark/tddfa.py
+-rw-r--r--  2.0 unx     5700 b- defN 23-May-03 07:41 nsface/model_zoo/model_landmark/tddfa.py
 -rw-r--r--  2.0 unx       35 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_recognition/__init__.py
 -rw-r--r--  2.0 unx     4325 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_recognition/arcface.py
 -rw-r--r--  2.0 unx     4434 b- defN 23-Jan-26 22:19 nsface/model_zoo/model_recognition/arcface_modify.py
 -rw-r--r--  2.0 unx      173 b- defN 23-Jan-26 22:19 nsface/utils/__init__.py
--rw-r--r--  2.0 unx      522 b- defN 23-Jan-26 22:19 nsface/utils/util_attribute.py
--rw-r--r--  2.0 unx     6735 b- defN 23-Apr-12 06:44 nsface/utils/util_common.py
--rw-r--r--  2.0 unx    25077 b- defN 23-Apr-12 05:50 nsface/utils/util_detection.py
--rw-r--r--  2.0 unx    16094 b- defN 23-Mar-13 02:22 nsface/utils/util_landmark.py
+-rw-r--r--  2.0 unx     2162 b- defN 23-May-04 00:17 nsface/utils/util_attribute.py
+-rw-r--r--  2.0 unx     6831 b- defN 23-May-03 06:24 nsface/utils/util_common.py
+-rw-r--r--  2.0 unx    23450 b- defN 23-May-04 00:17 nsface/utils/util_detection.py
+-rw-r--r--  2.0 unx    16178 b- defN 23-May-03 07:01 nsface/utils/util_landmark.py
 -rw-r--r--  2.0 unx      759 b- defN 23-Jan-26 22:19 nsface/utils/util_recognition.py
 -rw-r--r--  2.0 unx     3003 b- defN 23-Jan-26 22:19 nsface/utils/util_warp.py
--rw-r--r--  2.0 unx      531 b- defN 23-Apr-24 06:40 nsface_python-1.1.61.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 06:40 nsface_python-1.1.61.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-24 06:40 nsface_python-1.1.61.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-24 06:40 nsface_python-1.1.61.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8913 b- defN 23-Apr-24 06:40 nsface_python-1.1.61.dist-info/RECORD
-94 files, 655099 bytes uncompressed, 188390 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx      531 b- defN 23-May-04 00:38 nsface_python-1.1.71.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 00:38 nsface_python-1.1.71.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-May-04 00:38 nsface_python-1.1.71.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-04 00:38 nsface_python-1.1.71.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9018 b- defN 23-May-04 00:38 nsface_python-1.1.71.dist-info/RECORD
+95 files, 661158 bytes uncompressed, 190253 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -171,14 +171,23 @@
 
 Filename: nsface/model_zoo/model_attribute/arcface_GenderAge.py
 Comment: 
 
 Filename: nsface/model_zoo/model_attribute/arcface_Race.py
 Comment: 
 
+Filename: nsface/model_zoo/model_attribute/expression.py
+Comment: 
+
+Filename: nsface/model_zoo/model_attribute/liveness.py
+Comment: 
+
+Filename: nsface/model_zoo/model_attribute/mask_detector.py
+Comment: 
+
 Filename: nsface/model_zoo/model_common/__init__.py
 Comment: 
 
 Filename: nsface/model_zoo/model_common/load_onnx.py
 Comment: 
 
 Filename: nsface/model_zoo/model_common/load_openvino.py
@@ -201,20 +210,14 @@
 
 Filename: nsface/model_zoo/model_detection/blazeface640.py
 Comment: 
 
 Filename: nsface/model_zoo/model_detection/dlib_detector.py
 Comment: 
 
-Filename: nsface/model_zoo/model_detection/liveness.py
-Comment: 
-
-Filename: nsface/model_zoo/model_detection/mask_detector.py
-Comment: 
-
 Filename: nsface/model_zoo/model_detection/retinaface_insightface.py
 Comment: 
 
 Filename: nsface/model_zoo/model_detection/retinaface_torch.py
 Comment: 
 
 Filename: nsface/model_zoo/model_detection/scrfd.py
@@ -261,23 +264,23 @@
 
 Filename: nsface/utils/util_recognition.py
 Comment: 
 
 Filename: nsface/utils/util_warp.py
 Comment: 
 
-Filename: nsface_python-1.1.61.dist-info/METADATA
+Filename: nsface_python-1.1.71.dist-info/METADATA
 Comment: 
 
-Filename: nsface_python-1.1.61.dist-info/WHEEL
+Filename: nsface_python-1.1.71.dist-info/WHEEL
 Comment: 
 
-Filename: nsface_python-1.1.61.dist-info/entry_points.txt
+Filename: nsface_python-1.1.71.dist-info/entry_points.txt
 Comment: 
 
-Filename: nsface_python-1.1.61.dist-info/top_level.txt
+Filename: nsface_python-1.1.71.dist-info/top_level.txt
 Comment: 
 
-Filename: nsface_python-1.1.61.dist-info/RECORD
+Filename: nsface_python-1.1.71.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nsface/face/get_result.py

```diff
@@ -357,20 +357,21 @@
             r.max_flag=False
     return ret
 '''
 
 
 def get_landmark(model_name,model,img,faces,**kwargs):
     
+    eye_dist = kwargs.get('eye_dist',False)
     if model_name=='3ddfa':
         #param_lst, roi_box_lst = model.get_results(img,faces)
         param_lst=[]
         roi_box_lst=[]
         for face in faces:
-            param,roi_box,_ = model.get(img,face)
+            param,roi_box,_ = model.get(img,face,eye_dist=eye_dist)
             param_lst.append(param)
             roi_box_lst.append(roi_box)
             
         return faces, param_lst, roi_box_lst
 
     elif model_name=='2d106det':
         land_all=[]
@@ -384,43 +385,61 @@
         for face in faces:
             input_size = kwargs.get("input_size",256)
             scale_mul = kwargs.get("scale_mul",1.1)
             _ = model.get(img,face,input_size=input_size,scale_mul=scale_mul)
 
         return faces
 
-def get_ageGender(model_name,model,img,faces,to_bgr=False):
+def get_ageGender(model_name,model,img,faces,to_bgr=False,mask_off=False,eye_min=0):
         
     if model_name=='arcface_cmt':
         for face in faces:
-            model.get(img,face,to_bgr)
+            model.get(img,face,to_bgr,mask_off=mask_off,eye_min=eye_min)
             
     return faces
 
-def get_Race(model_name,model,img,faces,to_bgr=False):
+def get_Race(model_name,model,img,faces,to_bgr=False,mask_off=False,eye_min=0):
         
     if model_name=='arcface_race':
         for face in faces:
-            model.get(img,face,to_bgr)
+            model.get(img,face,to_bgr,mask_off=mask_off,eye_min=eye_min)
             
     return faces
 
 def get_features(model_name, model, img, faces,to_bgr=False):
 
     if model_name=='arcface':
         for face in faces:
             model.get(img,face,to_bgr)
 
     return faces
 
+def get_features_mask(model_name, model, model_mask, img, faces,to_bgr=False):
+
+    if model_name=='arcface':
+        for face in faces:
+            if np.argmax(face.mask_sf)==1: # mask
+                model_mask.get(img,face,to_bgr)
+            else:
+                model.get(img,face,to_bgr)
+
+    return faces
+
 def get_mask(model,faces,**kwargs):
 
     for face in faces:
         model.mask_check(face) # face.mask_sf
 
     return faces
 
-def get_liveness(model,faces,img,**kwargs):
+def get_liveness(model,faces,img,mask_off=False,eye_min=0,**kwargs):
+    for face in faces:
+        model.liveness_check(img,face,mask_off=mask_off,eye_min=eye_min)
+
+    return faces
+
+def get_expression(model,faces,mask_off=False,eye_min=0,**kwargs):
+
     for face in faces:
-        model.liveness_check(img,face)
+        model.get(face) # face.expression (expression result string)
 
     return faces
```

## nsface/model_zoo/get_models.py

```diff
@@ -1,10 +1,10 @@
-from .model_detection import scrfd, dlib_detector, retinaface_torch, retinaface_insightface, blazeface, blazeface640, mask_detector, liveness
+from .model_detection import scrfd, dlib_detector, retinaface_torch, retinaface_insightface, blazeface, blazeface640
 from .model_landmark import tddfa, pipnet,det2d106
-from .model_attribute import arcface_GenderAge, arcface_Race
+from .model_attribute import arcface_GenderAge, arcface_Race, mask_detector, liveness, expression
 from .model_recognition import arcface_modify as arcface
 
 
 def get_detection_model(name,path,**kwargs):
     model=None
     if type(path)==list:
         model_format = "openvino"
@@ -136,7 +136,24 @@
 
     if model is None:
         print("{} is None".format(name))
         return None
     else:
         print("liveness model {} loaded".format(model_format))
         return model
+
+def get_expression_model(path,**kwargs):
+    model=None
+    if type(path)==list:
+        model_format = "openvino"
+    else:
+        model_format = path.split(".")[-1]
+
+    model = expression.Expression_DAN(model_format,path,**kwargs)
+
+    if model is None:
+        print("{} is None".format(name))
+        return None
+    else:
+        print("expression model {} loaded".format(model_format))
+        return model
+
```

## nsface/model_zoo/model_attribute/__init__.py

```diff
@@ -1,2 +1,5 @@
 from .arcface_GenderAge import Arcface_GenderAge_cmt
-from .arcface_Race import Arcface_Race
+from .arcface_Race import Arcface_Race
+from .mask_detector import MaskDetector
+from .liveness import Liveness
+from .expression import Expression_DAN
```

## nsface/model_zoo/model_attribute/arcface_GenderAge.py

```diff
@@ -26,15 +26,27 @@
             self.net = load_onnx.Onnx_session(self.model_path,input_mean=0.0, input_std=1.0,onnx_device=kwargs.get("onnx_device",'cuda'))
         elif self.model_type=='trt':
             self.net = load_tensorRT.TrtModel(self.model_path)
             self.shape = self.net.engine.get_binding_shape(0)
         elif self.model_type=='openvino':
             self.net = load_openvino.Openvino(self.model_path,device=kwargs.get("device",'CPU'))
 
-    def get(self,img,face,to_bgr):
+    def get(self,img,face,to_bgr,mask_off=False,eye_min=0):
+        if mask_off and np.argmax(face['mask_sf'])==1:
+            face.gender=[]
+            face.age=[]
+            face.gender_sf=[]
+            return face.gender, face.age, face.gender_sf
+        if eye_min>0 and 'eye_dist' in face.keys() and face.eye_dist<eye_min:
+            face.gender=[]
+            face.age=[]
+            face.gender_sf=[]
+            return face.gender, face.age, face.gender_sf
+
+
         if not 'aimg' in face.keys():
             aimg = face_align(img,LMARK_REF_ARC,face.land5,self.out_size)
             face.aimg = aimg
         aimg = face.aimg
         #if self.model_type in ['trt','openvino']:
         #    aimg = read_torchImage(aimg,self.out_size,to_bgr=to_bgr).numpy()
         #elif self.model_type in ['pt','pth']:
```

## nsface/model_zoo/model_attribute/arcface_Race.py

```diff
@@ -25,15 +25,22 @@
         elif self.model_type=='onnx':
             self.net = load_onnx.Onnx_session(self.model_path,input_mean=0.0, input_std=1.0,onnx_device=kwargs.get("onnx_device",'cuda'))
         elif self.model_type=='trt':
             self.net = load_tensorRT.TrtModel(self.model_path)
         elif self.model_type=='openvino':
             self.net = load_openvino.Openvino(self.model_path,device=kwargs.get("device",'CPU'))
 
-    def get(self,img,face,to_bgr):
+    def get(self,img,face,to_bgr,mask_off=False,eye_min=0):
+        if mask_off and np.argmax(face['mask_sf'])==1:
+            face.race=[]
+            return face.race
+        if eye_min>0 and 'eye_dist' in face.keys() and face.eye_dist<eye_min:
+            face.race=[]
+            return face.race
+
         if not 'aimg' in face.keys():
             aimg = face_align(img,LMARK_REF_ARC,face.land5,self.out_size)
             face.aimg = aimg
         else:
             aimg = face.aimg
 
         if self.model_type=='onnx':
```

## nsface/model_zoo/model_detection/__init__.py

```diff
@@ -1,7 +1,5 @@
 from .retinaface_torch import RetinaFace
 from .retinaface_insightface import RetinaFace
 from .dlib_detector import Dlib
 from .scrfd import SCRFD_CV
-from .blazeface import BlazeFace
-from .mask_detector import MaskDetector
-from .liveness import Liveness
+from .blazeface import BlazeFace
```

## nsface/model_zoo/model_landmark/tddfa.py

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import cv2
 import onnxruntime
 
-from ...utils.util_landmark import parse_roi_box_from_bbox, crop_img, recon_ver, calc_pose
+from ...utils.util_landmark import parse_roi_box_from_bbox, crop_img, recon_ver, calc_pose, get_distance_point
 from ...data.constant import PARAM_STD, PARAM_MEAN, U_BASE, W_SHP_BASE, W_EXP_BASE, STD_SIZE
 
 from ..model_common import load_tensorRT, load_onnx, load_openvino,load_torch
 
 
 class TDDFA3D_V2:
     def __init__(self,model_type,model_path,**kwargs):
@@ -16,26 +16,28 @@
         self.param_mean = PARAM_MEAN
         self.u_base = U_BASE
         self.w_exp_base = W_EXP_BASE
         self.w_shp_base = W_SHP_BASE
         self.dense = False
         self.model_path = model_path
         self.model_type = model_type
+        self.left_eye_idx = [43,44,43,47]
+        self.right_eye_idx = [41,40,38,40]
 
         if self.model_type in ['pt','pth']:
             self.net = load_torch.TorchModel(self.model_path)
         elif self.model_type=='onnx':
             self.net = load_onnx.Onnx_session(self.model_path,input_mean=0.0, input_std=1.0,output_sort=True,onnx_device=kwargs.get("onnx_device",'cuda'))
         elif self.model_type=='trt':
             self.net = load_tensorRT.TrtModel(self.model_path,not_norm=True)
             self.shape = self.net.engine.get_binding_shape(0)
         elif self.model_type=='openvino':
             self.net = load_openvino.Openvino(self.model_path,not_norm=True,device=kwargs.get("device",'CPU'))
 
-    def get(self,img,face):
+    def get(self,img,face,eye_dist=False):
         box = face.bbox
         roi_box = parse_roi_box_from_bbox(box)
 
         img = crop_img(img, roi_box)
         img = cv2.resize(img, dsize=(self.std_size,self.std_size), interpolation=cv2.INTER_LINEAR)
         img = (img - 127.5) / 128.
         # (112,112,3) normalized image
@@ -56,31 +58,36 @@
             y_pred = ver[1][i]
             
             preds_pre.append([x_pred,y_pred])
 
         preds_pre = np.array(preds_pre).astype(np.float32)
         
         land5=[]
-        eye_left = (ver[0][37]+(ver[0][38]-ver[0][37])/2 , ver[1][41]-(ver[1][41]-ver[1][37])/2)
-        eye_right = (ver[0][43]+(ver[0][44]-ver[0][43])/2, ver[1][47]-(ver[1][47]-ver[1][43])/2)
+        eye_left = (ver[0][41]+(ver[0][40]-ver[0][41])/2 , ver[1][38]+(ver[1][40]-ver[1][38])/2)
+        eye_right = (ver[0][43]+(ver[0][44]-ver[0][43])/2, ver[1][43]+(ver[1][47]-ver[1][43])/2)
         nose = (ver[0][30], ver[1][30])
         mouth_left = (ver[0][48]+(ver[0][60]-ver[0][48])/2 , ver[1][60]-(ver[1][48]-ver[1][60])/2)
         mouth_right = (ver[0][64]+(ver[0][54]-ver[0][64])/2 , ver[1][64]-(ver[1][54]-ver[1][64])/2)
         land5.append(eye_left)
         land5.append(eye_right)
         land5.append(nose)
         land5.append(mouth_left)
         land5.append(mouth_right)
         land5 = np.array(land5).astype(np.float32)
         
         face.land = preds_pre
         face.land5 = land5
         face.pose = pose
-        
+
+        if eye_dist:
+            face.eye_dist=get_distance_point(eye_left,eye_right)
+            
         return param, roi_box,face.land5
+        
+        
 
     def get_results(self,img_ori, faces):
         param_lst = []
         roi_box_lst = []
         
         boxes = [face.bbox for face in faces]
```

## nsface/utils/util_attribute.py

```diff
@@ -1,9 +1,10 @@
 import os
-import numpy as np   
+import numpy as np 
+import cv2  
     
     
 def get_pred(sf_gender, sf_age):#,resize):
     age_female = sf_age[:,:101]
     age_male = sf_age[:,101:]
 
     #p_female = np.reshape(sf_gender[:,0],(resize,1))*age_female
@@ -14,8 +15,61 @@
 
     p_age = p_female+p_male
 
     pred_gender = np.argmax(sf_gender)#,axis=1)
     pred_age = np.argmax(p_age)#,axis=1)
 
 
-    return pred_gender, pred_age,sf_gender
+    return pred_gender, pred_age,sf_gender
+
+# liveness
+class CropImage:
+    @staticmethod
+    def _get_new_box(src_w, src_h, bbox, scale):
+        x = bbox[0]
+        y = bbox[1]
+        box_w = bbox[2]
+        box_h = bbox[3]
+
+        scale = min((src_h-1)/box_h, min((src_w-1)/box_w, scale))
+
+        new_width = box_w * scale
+        new_height = box_h * scale
+        center_x, center_y = box_w/2+x, box_h/2+y
+
+        left_top_x = center_x-new_width/2
+        left_top_y = center_y-new_height/2
+        right_bottom_x = center_x+new_width/2
+        right_bottom_y = center_y+new_height/2
+
+        if left_top_x < 0:
+            right_bottom_x -= left_top_x
+            left_top_x = 0
+
+        if left_top_y < 0:
+            right_bottom_y -= left_top_y
+            left_top_y = 0
+
+        if right_bottom_x > src_w-1:
+            left_top_x -= right_bottom_x-src_w+1
+            right_bottom_x = src_w-1
+
+        if right_bottom_y > src_h-1:
+            left_top_y -= right_bottom_y-src_h+1
+            right_bottom_y = src_h-1
+
+        return int(left_top_x), int(left_top_y),\
+               int(right_bottom_x), int(right_bottom_y)
+
+    def crop(self, org_img, bbox, scale, out_w, out_h, crop=True):
+
+        if not crop:
+            dst_img = cv2.resize(org_img, (out_w, out_h))
+        else:
+            src_h, src_w, _ = np.shape(org_img)
+            left_top_x, left_top_y, \
+                right_bottom_x, right_bottom_y = self._get_new_box(src_w, src_h, bbox, scale)
+
+            img = org_img[left_top_y: right_bottom_y+1,
+                          left_top_x: right_bottom_x+1]
+            dst_img = cv2.resize(img, (out_w, out_h))
+        return dst_img
```

## nsface/utils/util_common.py

```diff
@@ -13,23 +13,24 @@
             face = faces[i]
             x1,y1,x2,y2 = face.bbox.astype(np.int)
             
             cv2.rectangle(dimg,(x1,y1),(x2,y2),color,size)
 
             wtxt = ''
             if ga:
-                if face.gender is not None and face.age is not None:
-                    wtxt+="{} {}".format(face.gender, face.age)
-                else:
+                if len(face.gender)<1:
                     wtxt+="{} {}".format('None','0')
-            if race:
-                if face.race is not None:
-                    wtxt+=" {}".format(face.race)
                 else:
+                    wtxt+="{} {}".format(face.gender, face.age)
+
+            if race:
+                if len(face.race)<1:
                     wtxt+=" {}".format("None")
+                else:
+                    wtxt+=" {}".format(face.race)
 
             if wtxt:
                 cv2.putText(dimg, wtxt,(x1-1, y2+25),cv2.FONT_HERSHEY_SIMPLEX,1,(0,255,0),2)
 
 
         return dimg
     
@@ -171,22 +172,25 @@
         font_scale=1
         if to_bgr:
             dimg = cv2.cvtColor(dimg,cv2.COLOR_BGR2RGB)
         
         for i in range(len(faces)):
             face = faces[i]
             
-            liveness_lb = np.argmax(face['liveness_sf'])
-            if liveness_lb==0:
-                color = real_color
-                txt = 'real'
+            if len(face['liveness_sf'])<1:
+                continue
             else:
-                color = fake_color
-                txt = 'fake'
-            
-            x1,y1,x2,y2 = face.bbox.astype(np.int)
-            cv2.rectangle(dimg,(x1,y1),(x2,y2),color,2)
+                liveness_lb = np.argmax(face['liveness_sf'])
+                if liveness_lb==0:
+                    color = real_color
+                    txt = 'real'
+                else:
+                    color = fake_color
+                    txt = 'fake'
             
-            cv2.putText(dimg,txt,(x1-1, y2+25),cv2.FONT_HERSHEY_SIMPLEX,font_scale,color,2)
+                x1,y1,x2,y2 = face.bbox.astype(np.int)
+                cv2.rectangle(dimg,(x1,y1),(x2,y2),color,2)
+                
+                cv2.putText(dimg,txt,(x1-1, y2+25),cv2.FONT_HERSHEY_SIMPLEX,font_scale,color,2)
                 
         return dimg
```

## nsface/utils/util_detection.py

```diff
@@ -625,59 +625,7 @@
                 weighted_detection[16] = total_score / len(overlapping)
 
             output_detections.append(weighted_detection)
 
         return output_detections
 
 
-# liveness
-class CropImage:
-    @staticmethod
-    def _get_new_box(src_w, src_h, bbox, scale):
-        x = bbox[0]
-        y = bbox[1]
-        box_w = bbox[2]
-        box_h = bbox[3]
-
-        scale = min((src_h-1)/box_h, min((src_w-1)/box_w, scale))
-
-        new_width = box_w * scale
-        new_height = box_h * scale
-        center_x, center_y = box_w/2+x, box_h/2+y
-
-        left_top_x = center_x-new_width/2
-        left_top_y = center_y-new_height/2
-        right_bottom_x = center_x+new_width/2
-        right_bottom_y = center_y+new_height/2
-
-        if left_top_x < 0:
-            right_bottom_x -= left_top_x
-            left_top_x = 0
-
-        if left_top_y < 0:
-            right_bottom_y -= left_top_y
-            left_top_y = 0
-
-        if right_bottom_x > src_w-1:
-            left_top_x -= right_bottom_x-src_w+1
-            right_bottom_x = src_w-1
-
-        if right_bottom_y > src_h-1:
-            left_top_y -= right_bottom_y-src_h+1
-            right_bottom_y = src_h-1
-
-        return int(left_top_x), int(left_top_y),\
-               int(right_bottom_x), int(right_bottom_y)
-
-    def crop(self, org_img, bbox, scale, out_w, out_h, crop=True):
-
-        if not crop:
-            dst_img = cv2.resize(org_img, (out_w, out_h))
-        else:
-            src_h, src_w, _ = np.shape(org_img)
-            left_top_x, left_top_y, \
-                right_bottom_x, right_bottom_y = self._get_new_box(src_w, src_h, bbox, scale)
-
-            img = org_img[left_top_y: right_bottom_y+1,
-                          left_top_x: right_bottom_x+1]
-            dst_img = cv2.resize(img, (out_w, out_h))
-        return dst_img
```

## nsface/utils/util_landmark.py

```diff
@@ -1,13 +1,13 @@
 from math import sqrt
 import pickle
 import os
 import numpy as np
 import cv2
-from math import cos, sin, atan2, asin, sqrt
+from math import cos, sin, atan2, asin, sqrt, dist
 
 from ..data.constant import U_BASE, W_EXP_BASE, W_SHP_BASE
 
 
 def parse_roi_box_from_bbox(bbox):
     left, top, right, bottom = bbox[:4]
     old_size = (right - left + bottom - top) / 2
@@ -473,7 +473,11 @@
     land5=[]
     
     for k in dict_to_5[lms_num]:
         land5.append(pip_get_point(lands,dict_to_5[lms_num][k]))
             
             
     return land5
+
+def get_distance_point(p1,p2):
+    eye_dist = dist(p1,p2)
+    return eye_dist
```

## Comparing `nsface/model_zoo/model_detection/liveness.py` & `nsface/model_zoo/model_attribute/liveness.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os.path as osp
 import cv2
 import time
 import torch
 
 from ..model_common import load_tensorRT, load_onnx, load_openvino,load_torch,  load_tensorRT_multiple
 from ...data.image import read_torchImage,resize_image_multi
-from ...utils.util_detection import CropImage
+from ...utils.util_attribute import CropImage
 
 def softmax(x):
     f_x = np.exp(x) / np.sum(np.exp(x))
     return f_x
 
 class Liveness:
     def __init__(self, model_type,model_path,**kwargs):
@@ -58,15 +58,22 @@
             if self.load_multi:
                 self.net = load_openvino.Openvino_multi(self.model_path,transform=False,output_sort=True)
                 self.outs_len = len(self.net.output_names)
             else:
                 self.net = load_openvino.Openvino(self.model_path,not_norm=True,torch_image=True,device='CPU')
                 self.outs_len = self.net.outs_len
 
-    def liveness_check(self,img,face): # RGB input original image, (x1,y1,x2,y2) bbox_ori
+    def liveness_check(self,img,face,mask_off=False,eye_min=0): # RGB input original image, (x1,y1,x2,y2) bbox_ori
+
+        if mask_off and np.argmax(face['mask_sf'])==1:
+            face.liveness_sf=[]
+            return []
+        if eye_min>0 and 'eye_dist' in face.keys() and face.eye_dist<eye_min:
+            face.liveness_sf=[]
+            return []
 
         bbox_ori = face.bbox
         bbox = [int(bbox_ori[0]), int(bbox_ori[1]), int(bbox_ori[2]-bbox_ori[0]+1), int(bbox_ori[3]-bbox_ori[1]+1)]
 
         self.param = {
             "org_img": img,
             "bbox": bbox, # x1 y1 w h
```

## Comparing `nsface/model_zoo/model_detection/mask_detector.py` & `nsface/model_zoo/model_attribute/mask_detector.py`

 * *Files identical despite different names*

## Comparing `nsface_python-1.1.61.dist-info/METADATA` & `nsface_python-1.1.71.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsface-python
-Version: 1.1.61
+Version: 1.1.71
 Summary: Test Face model
 Home-page: UNKNOWN
 Author: minsuny
 Author-email: minsun.y@nsensecorp.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

## Comparing `nsface_python-1.1.61.dist-info/RECORD` & `nsface_python-1.1.71.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -40,55 +40,56 @@
 nsface/eval/verification/eval_util/__init__.py,sha256=WXj3WvIkCAjyzqDOS_EtE_PFMCYBiD6o-LUcynXWcpk,87
 nsface/eval/verification/eval_util/verification.py,sha256=ep7Z4owtsTCaI_2wgWYmNBsToFX0g3HaChULKUfGhZg,18457
 nsface/eval/verification/eval_util/verification_g.py,sha256=ThnQeZst5QHFYY7Lteou5TD8ANh07Y2hcARXc8h09jU,17798
 nsface/eval/verification/eval_util/verification_m.py,sha256=U4yCmVATlgwQFOsT0tUQLVwN3EmuZJaYSVmhE2iWL1s,16539
 nsface/face/__init__.py,sha256=F0MyXtPxuvIU1Wed0fBs2q_nj9bOpmeQ2iz8DldTHqo,67
 nsface/face/blur.py,sha256=4zdD4-nddC9-7jBEq66cMcKsXncVGBCS1YUjKcZbXN0,6642
 nsface/face/common.py,sha256=7nHL58GsOc38LAvP0jkkmPoVOumi9X3fy193XcoruWE,400
-nsface/face/get_result.py,sha256=gX_fqHF4LULjw508eEkwnkod4JFizxuZe9g6d7aZRM8,14039
+nsface/face/get_result.py,sha256=At62Avp1xp2q7wyWBWKy1WCdxfakB19upFugWU0aahc,14772
 nsface/model_zoo/__init__.py,sha256=pLN1-cq3qgyVjjR_PTmxLM3n9oZ6DDkY-CEfXfQQp0Y,204
-nsface/model_zoo/get_models.py,sha256=JP7oCzlSJ0k8YeuScO2xU42tPdE-LEK3ZKnb7vSq_PY,4119
+nsface/model_zoo/get_models.py,sha256=74L45E7gz0osdcpU8mEQrSNqd036ycZYtxxb6hGsxZo,4548
 nsface/model_zoo/backbones/__init__.py,sha256=KwoCIapMDGsnPcVIPqSDFGqa1EkU6fPm5qdHG2JtxLY,148
 nsface/model_zoo/backbones/groupface.py,sha256=oQxVdYypif3FPDPZmGdr3-Kd0ofnBcm7ibevcLUJ6Zk,15538
 nsface/model_zoo/backbones/iresnet.py,sha256=p28qCBXJ8xYZZRcmnWkkI_QWW5Mj_WPAaxPKMrb0cOc,7801
 nsface/model_zoo/backbones/mobilefacenet.py,sha256=2WJlphfILNWAJWCcjS8cTVNZGHtCgYEtyrfIlRp0Tvg,4895
 nsface/model_zoo/backbones/net.py,sha256=27iFwNe9AoZcOPbJ8GoDsMWGIBqCT3l8V86HykZqiW8,4598
 nsface/model_zoo/backbones/race_linear.py,sha256=cm0GOWyv5YIqdK379OTCnZJCKnLzqQm5OOsHfIbTpsI,2493
 nsface/model_zoo/backbones/retinaface.py,sha256=Vpqn1lq6CY6dtjxHUAWwhorJyk2lDMPHfeoR0ME1-VU,5530
-nsface/model_zoo/model_attribute/__init__.py,sha256=BEIhJcTgm7uWOtZAFckZsUcpadbfmi4hX0DgidabmFY,91
-nsface/model_zoo/model_attribute/arcface_GenderAge.py,sha256=BPjtivNoILRm0LiaL7dBQHEfNtfhsiMT6fmW8b8ogIo,2287
-nsface/model_zoo/model_attribute/arcface_Race.py,sha256=wdHZV2jvlqndAJAovAPL_Xg7Sxf48Iq4jcuRQXYUCtI,2060
+nsface/model_zoo/model_attribute/__init__.py,sha256=cwdJwGatrHa5nCTBeH1itNe_MHzqTWl1_BUqn-qonmI,201
+nsface/model_zoo/model_attribute/arcface_GenderAge.py,sha256=3I9usNpEKZszi_7rpI5c1iqWazWFn4rQCEtOBPnbEsM,2723
+nsface/model_zoo/model_attribute/arcface_Race.py,sha256=Gx4r6jpNXNFcBHD3Rd1NrDdZ4tVZnsrCe_z_JStxq4Y,2327
+nsface/model_zoo/model_attribute/expression.py,sha256=1PX1txX1D7ldkV2v64IKkJRUZTXmkdsibtzaKNSeWUE,3361
+nsface/model_zoo/model_attribute/liveness.py,sha256=LlqG91zBgX4u4N5O3oYXqIiMqu8mFtkhm8EEoRcp6Qg,3618
+nsface/model_zoo/model_attribute/mask_detector.py,sha256=tVSVLQh2NWat5tnCqKg5jGzS4Gz7ImDXN-JAMVA5tnI,3011
 nsface/model_zoo/model_common/__init__.py,sha256=WMoExjueiq31TszCdG1VLiZt16xONmyjoyruv_LHO1E,207
 nsface/model_zoo/model_common/load_onnx.py,sha256=KOI8NFi-Zt2h0vAREhqeN4dNpJRSDDTObkGnycRLIYc,2719
 nsface/model_zoo/model_common/load_openvino.py,sha256=JIFcMYiZm_scwtN3Kf5YyWAqUqBjmO1GWY6etsb0cCU,3354
 nsface/model_zoo/model_common/load_tensorRT.py,sha256=reCKfIFDpRpBu0bB6qEi27Kj8I9zrQLifwTZYGwXuNw,3603
 nsface/model_zoo/model_common/load_tensorRT_multiple.py,sha256=g3cR1UlyYqZtfDK_bGaZCwkJJWxCUcaeNI2FRccosBg,6037
 nsface/model_zoo/model_common/load_torch.py,sha256=WLjMu-CeHGf54Z5Q8xA4BrfL0mbLasJ41PizjMlt79Y,7325
-nsface/model_zoo/model_detection/__init__.py,sha256=t2OTqK4FQJKfh4UeYwYobxi_nP4EWyXIRdDuTeemEIE,251
+nsface/model_zoo/model_detection/__init__.py,sha256=8c4ZXFQ7XcFPiuzwOgDP6mO5yyAD38Kv5pUQ4LioUkg,180
 nsface/model_zoo/model_detection/blazeface.py,sha256=5tgQc1sDLNThfcv_p1tO3fdwQPk_DsOmnmBkiN4cI3w,8151
 nsface/model_zoo/model_detection/blazeface640.py,sha256=ApSqIACW1ZJ9IxP1cndGhg8wjdGZdT6fmWhPh3QQjho,7872
 nsface/model_zoo/model_detection/dlib_detector.py,sha256=4zy7giSH3HUIfCVe7UwaMgQb2XhJX2a1mv5WUR_GbDA,1126
-nsface/model_zoo/model_detection/liveness.py,sha256=4EoCdyL4afPu09blcLpZRT1bidKZtD-UMju2kG1MfOY,3351
-nsface/model_zoo/model_detection/mask_detector.py,sha256=tVSVLQh2NWat5tnCqKg5jGzS4Gz7ImDXN-JAMVA5tnI,3011
 nsface/model_zoo/model_detection/retinaface_insightface.py,sha256=75opyP6Fk2fcqRsgdjpDyVGH-8LSneazT3P6s2EL_pQ,8137
 nsface/model_zoo/model_detection/retinaface_torch.py,sha256=eEPlsneKyvqlMruJ6VVY_HSoDUHuipA7HwiAdnebXGI,9723
 nsface/model_zoo/model_detection/scrfd.py,sha256=Se0V6omXdA9wlIhHYHEMjZiovd8yhHCA1-zANTSjo9s,11771
 nsface/model_zoo/model_detection/scrfd_pre.py,sha256=TlmybqMFunC9h7u8rAO3-Xtcs_dwRZk9XulLY9VwRNE,8636
 nsface/model_zoo/model_landmark/__init__.py,sha256=6IhuM-t9NhZR94x2S7EOjsp-l6dnUUYz0qDEWpDHivs,29
 nsface/model_zoo/model_landmark/det2d106.py,sha256=TmiSh25kx5dZ4j5bKQ4T3l4FnF3VR1iLWxKYbuGaBcM,2564
 nsface/model_zoo/model_landmark/pipnet.py,sha256=YmUUbZpkAlEWdWy73pfN9aBCA80ydZr_TpUj5mTanks,12050
-nsface/model_zoo/model_landmark/tddfa.py,sha256=EXt-nT3AGRSBzx4A_W560solDFw4uDctBkzHvPtdCnA,5471
+nsface/model_zoo/model_landmark/tddfa.py,sha256=Xx8MrhVo0n_damaLnIgTkOPkxeiTPBSA6jVHqaWzsKo,5700
 nsface/model_zoo/model_recognition/__init__.py,sha256=eVI_ENcGFvgR5C9TCQKVsPkp0YDWBgp2R12-XR8XBXo,35
 nsface/model_zoo/model_recognition/arcface.py,sha256=MMRS5X_BKzU3yfH03QrHxcp2U4QVDLS1btiHWdB0rII,4325
 nsface/model_zoo/model_recognition/arcface_modify.py,sha256=7qiV6p5Q83Ky1VrYE_l6rizzBBd04DatBTTjkBv4O-w,4434
 nsface/utils/__init__.py,sha256=nCWNMSBAxrgdDra5eQ-ar3_wiJjWiJEmYJ1oNgqaGio,173
-nsface/utils/util_attribute.py,sha256=Fzfsuz4LYmkvrrJT0L9X3A2jiboaC5FIFX9uchmP0VY,522
-nsface/utils/util_common.py,sha256=Q27T6XQ64Kiqc7afsFOjDSsHLK6HWlzvQUwpsQeJnQA,6735
-nsface/utils/util_detection.py,sha256=oqAuKHx8L2-zQWHgRu348doUz2xk8nMo6dncpM15nDk,25077
-nsface/utils/util_landmark.py,sha256=qniOm3QVXsrWuJa2v2Xk_AdKMTb2FOoZy1pdrk7mums,16094
+nsface/utils/util_attribute.py,sha256=mCJO3FdOnCJ-fm6-1yWTC49clH5YA4FJjsLQeOd3dvA,2162
+nsface/utils/util_common.py,sha256=vsPecmvf_AIHH3fXkJOVwmuGbPzZLhaVF2HsLeBE0L8,6831
+nsface/utils/util_detection.py,sha256=Rshw-Hu1nok0TfeLCSR8Gdt7VsVSu-Uo_npN12vGoaM,23450
+nsface/utils/util_landmark.py,sha256=6EEYa21MmkEuuIAoS11RFdWdqmuIkw23cqyKcxjkBbM,16178
 nsface/utils/util_recognition.py,sha256=OYoiGTlE1Tp5VowcOHyCxb-QXnTcVfGTPsNklQ-teeU,759
 nsface/utils/util_warp.py,sha256=V0_QZ4LhG_nBH37UNq3UpbYoM28vGcvk2RagGo_9QTA,3003
-nsface_python-1.1.61.dist-info/METADATA,sha256=szXcj-AxsWqswEMcVZ64Nnce0xMnPQC2ujSs8x1NOBQ,531
-nsface_python-1.1.61.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nsface_python-1.1.61.dist-info/entry_points.txt,sha256=DbtzII_7RVEDraozv5k76t6JDOjZZm-ruRZs4N3nF6s,61
-nsface_python-1.1.61.dist-info/top_level.txt,sha256=Mn7kn43NX5shzD8I7wvIzyeGYMEJ9z08sfyIPRzHVfQ,7
-nsface_python-1.1.61.dist-info/RECORD,,
+nsface_python-1.1.71.dist-info/METADATA,sha256=JSceaXZPZyMiuTdCOey6dYUvp7YrKSWEH0FMCRotZL8,531
+nsface_python-1.1.71.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nsface_python-1.1.71.dist-info/entry_points.txt,sha256=DbtzII_7RVEDraozv5k76t6JDOjZZm-ruRZs4N3nF6s,61
+nsface_python-1.1.71.dist-info/top_level.txt,sha256=Mn7kn43NX5shzD8I7wvIzyeGYMEJ9z08sfyIPRzHVfQ,7
+nsface_python-1.1.71.dist-info/RECORD,,
```

