# Comparing `tmp/napatrackmater-3.5.2.tar.gz` & `tmp/napatrackmater-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-psodessx/napatrackmater-3.5.2.tar", last modified: Thu May  4 19:34:18 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-nlxg5vas/napatrackmater-3.5.3.tar", last modified: Thu May  4 19:43:09 2023, max compression
```

## Comparing `napatrackmater-3.5.2.tar` & `napatrackmater-3.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:34:18.915952 napatrackmater-3.5.2/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.2/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-04 19:34:18.909953 napatrackmater-3.5.2/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.2/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:34:18.707689 napatrackmater-3.5.2/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.5.2/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.5.2/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   111572 2023-05-04 19:32:51.000000 napatrackmater-3.5.2/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.2/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.2/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13523 2023-05-04 16:47:51.000000 napatrackmater-3.5.2/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.2/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.2/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.5.2/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-04 19:31:17.000000 napatrackmater-3.5.2/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:34:18.878953 napatrackmater-3.5.2/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-04 19:34:18.000000 napatrackmater-3.5.2/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-04 19:34:18.916956 napatrackmater-3.5.2/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.5.2/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:43:09.490558 napatrackmater-3.5.3/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.5.3/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-04 19:43:09.486408 napatrackmater-3.5.3/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.5.3/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:43:09.282219 napatrackmater-3.5.3/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.5.3/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.5.3/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   111740 2023-05-04 19:41:19.000000 napatrackmater-3.5.3/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.5.3/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.5.3/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13523 2023-05-04 16:47:51.000000 napatrackmater-3.5.3/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.5.3/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.5.3/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.5.3/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-04 19:41:52.000000 napatrackmater-3.5.3/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-04 19:43:09.450505 napatrackmater-3.5.3/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-04 19:43:08.000000 napatrackmater-3.5.3/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-04 19:43:09.492570 napatrackmater-3.5.3/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.5.3/setup.py
```

### Comparing `napatrackmater-3.5.2/LICENSE` & `napatrackmater-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/PKG-INFO` & `napatrackmater-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.2
+Version: 3.5.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.2/README.md` & `napatrackmater-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.5.3/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.5.3/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/Trackmate.py` & `napatrackmater-3.5.3/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -4504,2471 +4504,2481 @@
 00011970: 7266 6163 655f 6172 6561 5b69 5d0d 0a20  rface_area[i].. 
 00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000119a0: 2020 2064 6973 742c 2069 6e64 6578 203d     dist, index =
 000119b0: 2074 7265 652e 7175 6572 7928 6365 6e74   tree.query(cent
 000119c0: 726f 6964 290d 0a20 2020 2020 2020 2020  roid)..         
 000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 2020 2020 2020 2020 2063 6c6f 7365             close
-000119f0: 7374 5f63 656e 7472 6f69 6420 3d20 7370  st_centroid = sp
-00011a00: 6f74 5f63 656e 7472 6f69 6473 5b69 6e64  ot_centroids[ind
-00011a10: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
-00011a40: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
-00011a50: 696e 7428 7469 6d65 5f6b 6579 292c 636c  int(time_key),cl
-00011a60: 6f73 6573 745f 6365 6e74 726f 6964 5b30  osest_centroid[0
-00011a70: 5d2c 2063 6c6f 7365 7374 5f63 656e 7472  ], closest_centr
-00011a80: 6f69 645b 315d 2c20 636c 6f73 6573 745f  oid[1], closest_
-00011a90: 6365 6e74 726f 6964 5b32 5d29 0d0a 2020  centroid[2])..  
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2020 636c 6f73 6573 745f 6365 6c6c 5f69    closest_cell_i
-00011ad0: 6420 3d20 7365 6c66 2e75 6e69 7175 655f  d = self.unique_
-00011ae0: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
-00011af0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00011b00: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 2020 2020 2020 6d61 736b 5f76 6563          mask_vec
-00011b30: 746f 7220 3d20 5b20 666c 6f61 7428 7365  tor = [ float(se
-00011b40: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011b50: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011b60: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
-00011b70: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00011b80: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
-00011b90: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00011ba0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00011bb0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011bc0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-00011bd0: 726f 6964 5f79 5f6b 6579 5d29 2c20 666c  roid_y_key]), fl
-00011be0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00011bf0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00011c00: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00011c10: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00011c20: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
-00011c30: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c50: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
-00011c60: 5f6d 6173 6b20 3d20 616e 6775 6c61 725f  _mask = angular_
-00011c70: 6368 616e 6765 2863 656c 6c5f 6178 6973  change(cell_axis
-00011c80: 2c20 6d61 736b 5f76 6563 746f 7229 0d0a  , mask_vector)..
+000119e0: 2020 2020 2020 2020 2020 2069 6620 6469             if di
+000119f0: 7374 203c 2071 7561 6c69 7479 3a0d 0a20  st < quality:.. 
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 2020 2020 2020 2020 2020 2063 6c6f 7365             close
+00011a30: 7374 5f63 656e 7472 6f69 6420 3d20 7370  st_centroid = sp
+00011a40: 6f74 5f63 656e 7472 6f69 6473 5b69 6e64  ot_centroids[ind
+00011a50: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
+00011a90: 726f 6964 203d 2028 696e 7428 7469 6d65  roid = (int(time
+00011aa0: 5f6b 6579 292c 636c 6f73 6573 745f 6365  _key),closest_ce
+00011ab0: 6e74 726f 6964 5b30 5d2c 2063 6c6f 7365  ntroid[0], close
+00011ac0: 7374 5f63 656e 7472 6f69 645b 315d 2c20  st_centroid[1], 
+00011ad0: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
+00011ae0: 5b32 5d29 0d0a 2020 2020 2020 2020 2020  [2])..          
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b10: 2020 636c 6f73 6573 745f 6365 6c6c 5f69    closest_cell_i
+00011b20: 6420 3d20 7365 6c66 2e75 6e69 7175 655f  d = self.unique_
+00011b30: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
+00011b40: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+00011b50: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 6d61 736b 5f76 6563 746f 7220 3d20 5b20  mask_vector = [ 
+00011b90: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00011ba0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011bb0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011bc0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+00011bd0: 6b63 656e 7472 6f69 645f 785f 6b65 795d  kcentroid_x_key]
+00011be0: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
+00011bf0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00011c00: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00011c10: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
+00011c20: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+00011c30: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
+00011c40: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00011c50: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00011c60: 6573 745f 6365 6c6c 5f69 6429 5d5b 7365  est_cell_id)][se
+00011c70: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00011c80: 7a5f 6b65 795d 2920 5d0d 0a20 2020 2020  z_key]) ]..     
 00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cd0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00011ce0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00011cf0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00011d00: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00011d10: 7465 287b 7365 6c66 2e63 656c 6c61 7869  te({self.cellaxi
-00011d20: 735f 6d61 736b 5f6b 6579 203a 2063 656c  s_mask_key : cel
-00011d30: 6c5f 6178 6973 5f6d 6173 6b7d 290d 0a20  l_axis_mask}).. 
-00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d60: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00011d70: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011d80: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00011d90: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00011da0: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
-00011db0: 6579 203a 2063 6c75 7374 6572 5f63 6c61  ey : cluster_cla
-00011dc0: 7373 7d29 0d0a 2020 2020 2020 2020 2020  ss})..          
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00011df0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00011e00: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00011e10: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00011e20: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
-00011e30: 7363 6f72 655f 6b65 7920 3a20 636c 7573  score_key : clus
-00011e40: 7465 725f 7363 6f72 657d 290d 0a20 2020  ter_score})..   
+00011cb0: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+00011cc0: 5f6d 6173 6b20 3d20 616e 6775 6c61 725f  _mask = angular_
+00011cd0: 6368 616e 6765 2863 656c 6c5f 6178 6973  change(cell_axis
+00011ce0: 2c20 6d61 736b 5f76 6563 746f 7229 0d0a  , mask_vector)..
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011d50: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011d60: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011d70: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00011d80: 7465 287b 7365 6c66 2e63 656c 6c61 7869  te({self.cellaxi
+00011d90: 735f 6d61 736b 5f6b 6579 203a 2063 656c  s_mask_key : cel
+00011da0: 6c5f 6178 6973 5f6d 6173 6b7d 290d 0a20  l_axis_mask}).. 
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011de0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011df0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00011e00: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+00011e10: 6174 6528 7b73 656c 662e 636c 7573 7465  ate({self.cluste
+00011e20: 7263 6c61 7373 5f6b 6579 203a 2063 6c75  rclass_key : clu
+00011e30: 7374 6572 5f63 6c61 7373 7d29 0d0a 2020  ster_class})..  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00011e80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00011e90: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011ea0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00011eb0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00011ec0: 705f 6669 7273 746b 6579 203a 2065 6363  p_firstkey : ecc
-00011ed0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00011ee0: 6972 7374 797a 5b30 5d7d 290d 0a20 2020  irstyz[0]})..   
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f10: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00011f20: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00011f30: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00011f40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00011f50: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00011f60: 705f 7365 636f 6e64 6b65 7920 3a20 6563  p_secondkey : ec
-00011f70: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00011f80: 6669 7273 7479 7a5b 315d 7d29 0d0a 2020  firstyz[1]})..  
+00011e60: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011e70: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011e80: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00011e90: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00011ea0: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
+00011eb0: 7363 6f72 655f 6b65 7920 3a20 636c 7573  score_key : clus
+00011ec0: 7465 725f 7363 6f72 657d 290d 0a20 2020  ter_score})..   
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ef0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00011f00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00011f10: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00011f20: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00011f30: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
+00011f40: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
+00011f50: 6579 203a 2065 6363 656e 7472 6963 6974  ey : eccentricit
+00011f60: 795f 636f 6d70 5f66 6972 7374 797a 5b30  y_comp_firstyz[0
+00011f70: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00011fc0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00011fd0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00011fe0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00011ff0: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-00012000: 7920 3a20 7375 7266 6163 655f 6172 6561  y : surface_area
-00012010: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00011fa0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00011fb0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00011fc0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00011fd0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00011fe0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00011ff0: 705f 7365 636f 6e64 6b65 7920 3a20 6563  p_secondkey : ec
+00012000: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012010: 6669 7273 7479 7a5b 315d 7d29 0d0a 2020  firstyz[1]})..  
 00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012030: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012040: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012050: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012060: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00012070: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
-00012080: 6579 203a 2071 7561 6c69 7479 7d29 0d0a  ey : quality})..
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000120c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000120d0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-000120e0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000120f0: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
-00012100: 7175 616c 6974 7920 2a20 6d61 7468 2e70  quality * math.p
-00012110: 6f77 2873 656c 662e 7a63 616c 6962 7261  ow(self.zcalibra
-00012120: 7469 6f6e 202a 2073 656c 662e 7863 616c  tion * self.xcal
-00012130: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
-00012140: 7963 616c 6962 7261 7469 6f6e 2c20 312e  ycalibration, 1.
-00012150: 302f 332e 3029 207d 290d 0a0d 0a0d 0a20  0/3.0) })...... 
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012180: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121a0: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
-000121b0: 662e 726f 6f74 5f73 706f 7473 2e69 7465  f.root_spots.ite
-000121c0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-000121f0: 6f74 5f73 706f 7473 5b6b 5d20 3d20 7365  ot_spots[k] = se
-00012200: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012210: 726f 7065 7274 6965 735b 6b5d 2020 2020  roperties[k]    
-00012220: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00012230: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00012240: 205f 636f 6d70 7574 655f 7068 656e 6f74   _compute_phenot
-00012250: 7970 6573 2873 656c 6629 3a0d 0a0d 0a20  ypes(self):.... 
-00012260: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-00012270: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
-00012280: 655f 7472 6163 6b73 2e69 7465 6d73 2829  e_tracks.items()
-00012290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000122a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000122b0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-000122c0: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
-000122d0: 2020 2074 7261 636b 6c65 745f 7072 6f70     tracklet_prop
-000122e0: 6572 7469 6573 203d 2073 656c 662e 756e  erties = self.un
-000122f0: 6971 7565 5f74 7261 636b 5f70 726f 7065  ique_track_prope
-00012300: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
-00012310: 2020 2020 2020 2020 2020 7472 6163 6b73            tracks
-00012320: 203d 2073 656c 662e 756e 6971 7565 5f74   = self.unique_t
-00012330: 7261 636b 735b 6b5d 0d0a 2020 2020 2020  racks[k]..      
-00012340: 2020 2020 2020 2020 2020 5a20 3d20 7472            Z = tr
-00012350: 6163 6b73 5b3a 2c32 5d0d 0a20 2020 2020  acks[:,2]..     
-00012360: 2020 2020 2020 2020 2020 2059 203d 2074             Y = t
-00012370: 7261 636b 735b 3a2c 335d 0d0a 2020 2020  racks[:,3]..    
-00012380: 2020 2020 2020 2020 2020 2020 5820 3d20              X = 
-00012390: 7472 6163 6b73 5b3a 2c34 5d0d 0a20 2020  tracks[:,4]..   
-000123a0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-000123b0: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-000123c0: 7065 7274 6965 735b 3a2c 305d 0d0a 2020  perties[:,0]..  
-000123d0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-000123e0: 6971 7565 5f69 6473 203d 2074 7261 636b  ique_ids = track
-000123f0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012400: 2c31 5d0d 0a20 2020 2020 2020 2020 2020  ,1]..           
-00012410: 2020 2020 2075 6e69 7175 655f 6964 735f       unique_ids_
-00012420: 7365 7420 3d20 7365 7428 756e 6971 7565  set = set(unique
-00012430: 5f69 6473 290d 0a20 2020 2020 2020 2020  _ids)..         
-00012440: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-00012450: 6e5f 6964 7320 3d20 7472 6163 6b6c 6574  n_ids = tracklet
-00012460: 5f70 726f 7065 7274 6965 735b 3a2c 325d  _properties[:,2]
-00012470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012480: 2020 7261 6469 7573 203d 2074 7261 636b    radius = track
-00012490: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-000124a0: 2c33 5d0d 0a20 2020 2020 2020 2020 2020  ,3]..           
-000124b0: 2020 2020 2076 6f6c 756d 6520 3d20 7472       volume = tr
-000124c0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-000124d0: 735b 3a2c 345d 0d0a 2020 2020 2020 2020  s[:,4]..        
-000124e0: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-000124f0: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-00012500: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012510: 7274 6965 735b 3a2c 355d 0d0a 2020 2020  rties[:,5]..    
-00012520: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
-00012530: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00012540: 636f 6e64 203d 2074 7261 636b 6c65 745f  cond = tracklet_
-00012550: 7072 6f70 6572 7469 6573 5b3a 2c36 5d0d  properties[:,6].
-00012560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012570: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
-00012580: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012590: 6965 735b 3a2c 375d 0d0a 2020 2020 2020  ies[:,7]..      
-000125a0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-000125b0: 725f 636c 6173 7320 3d20 7472 6163 6b6c  r_class = trackl
-000125c0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000125d0: 385d 0d0a 2020 2020 2020 2020 2020 2020  8]..            
-000125e0: 2020 2020 636c 7573 7465 725f 636c 6173      cluster_clas
-000125f0: 735f 7363 6f72 6520 3d20 7472 6163 6b6c  s_score = trackl
-00012600: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012610: 395d 0d0a 2020 2020 2020 2020 2020 2020  9]..            
-00012620: 2020 2020 696e 7465 6e73 6974 7920 3d20      intensity = 
-00012630: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012640: 6965 735b 3a2c 3130 5d0d 0a20 2020 2020  ies[:,10]..     
-00012650: 2020 2020 2020 2020 2020 2073 7065 6564             speed
-00012660: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00012670: 6572 7469 6573 5b3a 2c31 315d 0d0a 2020  erties[:,11]..  
-00012680: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00012690: 7469 6f6e 5f61 6e67 6c65 203d 2074 7261  tion_angle = tra
-000126a0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000126b0: 5b3a 2c31 325d 0d0a 2020 2020 2020 2020  [:,12]..        
-000126c0: 2020 2020 2020 2020 6163 6365 6c65 7261          accelera
-000126d0: 7469 6f6e 203d 2074 7261 636b 6c65 745f  tion = tracklet_
-000126e0: 7072 6f70 6572 7469 6573 5b3a 2c31 335d  properties[:,13]
-000126f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012700: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-00012710: 6d61 736b 203d 2074 7261 636b 6c65 745f  mask = tracklet_
-00012720: 7072 6f70 6572 7469 6573 5b3a 2c31 345d  properties[:,14]
-00012730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012740: 2020 7261 6469 616c 5f61 6e67 6c65 203d    radial_angle =
-00012750: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012760: 7469 6573 5b3a 2c31 355d 0d0a 2020 2020  ties[:,15]..    
-00012770: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00012780: 5f61 7869 735f 6d61 736b 203d 2074 7261  _axis_mask = tra
-00012790: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000127a0: 5b3a 2c31 365d 0d0a 0d0a 0d0a 2020 2020  [:,16]......    
-000127b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000127c0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-000127d0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-000127e0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
-000127f0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00012800: 2020 2075 6e69 7175 655f 636c 7573 7465     unique_cluste
-00012810: 725f 7072 6f70 6572 7469 6573 5f74 7261  r_properties_tra
-00012820: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
-00012830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012840: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
-00012850: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00012860: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00012870: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012880: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00012890: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-000128a0: 3d20 7b7d 0d0a 0d0a 2020 2020 2020 2020  = {}....        
-000128b0: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
-000128c0: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
-000128d0: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000128f0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-00012900: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00012910: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
-00012920: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012930: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00012940: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00012950: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00012960: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00012970: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-00012980: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00012990: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-000129a0: 2020 2020 6578 7061 6e64 6564 5f74 696d      expanded_tim
-000129b0: 6520 3d20 6e70 2e7a 6572 6f73 2873 656c  e = np.zeros(sel
-000129c0: 662e 7465 6e64 202d 2073 656c 662e 7473  f.tend - self.ts
-000129d0: 7461 7274 202b 2031 290d 0a20 2020 2020  tart + 1)..     
-000129e0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-000129f0: 5f73 616d 706c 6520 3d20 6578 7061 6e64  _sample = expand
-00012a00: 6564 5f74 696d 652e 7368 6170 655b 305d  ed_time.shape[0]
-00012a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012a20: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00012a30: 286c 656e 2865 7870 616e 6465 645f 7469  (len(expanded_ti
-00012a40: 6d65 2929 3a0d 0a20 2020 2020 2020 2020  me)):..         
-00012a50: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00012a60: 7061 6e64 6564 5f74 696d 655b 695d 203d  panded_time[i] =
-00012a70: 2069 200d 0a20 2020 2020 2020 2020 2020   i ..           
-00012a80: 2020 2020 2066 6f72 2063 7572 7265 6e74       for current
-00012a90: 5f75 6e69 7175 655f 6964 2069 6e20 756e  _unique_id in un
-00012aa0: 6971 7565 5f69 6473 5f73 6574 3a0d 0a20  ique_ids_set:.. 
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00012ad0: 2020 2020 2020 2065 7870 616e 6465 645f         expanded_
-00012ae0: 696e 7465 6e73 6974 7920 3d20 6e70 2e7a  intensity = np.z
-00012af0: 6572 6f73 2873 656c 662e 7465 6e64 202d  eros(self.tend -
-00012b00: 2073 656c 662e 7473 7461 7274 202b 2031   self.tstart + 1
-00012b10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012b20: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00012b30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 6375 7272 656e 745f 7469 6d65 203d 205b  current_time = [
-00012b60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012b70: 2020 2020 2020 6375 7272 656e 745f 7a20        current_z 
-00012b80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012b90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012ba0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00012bb0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012bc0: 656e 745f 7820 3d20 5b5d 0d0a 2020 2020  ent_x = []..    
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012be0: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
-00012bf0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012c00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012c10: 745f 636c 7573 7465 725f 636c 6173 7320  t_cluster_class 
-00012c20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012c30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012c40: 5f63 6c75 7374 6572 5f63 6c61 7373 5f73  _cluster_class_s
-00012c50: 636f 7265 203d 205b 5d0d 0a20 2020 2020  core = []..     
-00012c60: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012c70: 7272 656e 745f 7261 6469 7573 203d 205b  rrent_radius = [
-00012c80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012c90: 2020 2020 2020 6375 7272 656e 745f 766f        current_vo
-00012ca0: 6c75 6d65 203d 205b 5d0d 0a20 2020 2020  lume = []..     
-00012cb0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012cc0: 7272 656e 745f 7370 6565 6420 3d20 5b5d  rrent_speed = []
-00012cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012ce0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
-00012cf0: 696f 6e5f 616e 676c 6520 3d20 5b5d 0d0a  ion_angle = []..
-00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d10: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
-00012d20: 6572 6174 696f 6e20 3d20 5b5d 0d0a 2020  eration = []..  
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2063 7572 7265 6e74 5f64 6973 7461 6e63   current_distanc
-00012d50: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
-00012d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012d70: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00012d80: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00012d90: 6972 7374 203d 205b 5d0d 0a20 2020 2020  irst = []..     
-00012da0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012db0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00012dc0: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
-00012dd0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012de0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012df0: 7375 7266 6163 655f 6172 6561 203d 205b  surface_area = [
-00012e00: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00012e10: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012e20: 7261 6469 616c 5f61 6e67 6c65 203d 205b  radial_angle = [
-00012e30: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012e40: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
-00012e50: 6c6c 5f61 7869 735f 6d61 736b 203d 205b  ll_axis_mask = [
-00012e60: 5d20 0d0a 2020 2020 2020 2020 2020 2020  ] ..            
-00012e70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012e80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012e90: 6a20 696e 2072 616e 6765 2874 696d 652e  j in range(time.
-00012ea0: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00012050: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00012060: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00012070: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00012080: 7465 287b 7365 6c66 2e73 7572 6661 6365  te({self.surface
+00012090: 5f61 7265 615f 6b65 7920 3a20 7375 7266  _area_key : surf
+000120a0: 6163 655f 6172 6561 7d29 0d0a 2020 2020  ace_area})..    
+000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000120e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000120f0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012100: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00012110: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
+00012120: 6579 203a 2071 7561 6c69 7479 7d29 0d0a  ey : quality})..
+00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012160: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00012170: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00012180: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00012190: 6461 7465 287b 7365 6c66 2e72 6164 6975  date({self.radiu
+000121a0: 735f 6b65 7920 3a20 7175 616c 6974 7920  s_key : quality 
+000121b0: 2a20 6d61 7468 2e70 6f77 2873 656c 662e  * math.pow(self.
+000121c0: 7a63 616c 6962 7261 7469 6f6e 202a 2073  zcalibration * s
+000121d0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+000121e0: 202a 2073 656c 662e 7963 616c 6962 7261   * self.ycalibra
+000121f0: 7469 6f6e 2c20 312e 302f 332e 3029 207d  tion, 1.0/3.0) }
+00012200: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012240: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00012250: 2920 696e 2073 656c 662e 726f 6f74 5f73  ) in self.root_s
+00012260: 706f 7473 2e69 7465 6d73 2829 3a0d 0a20  pots.items():.. 
+00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012290: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
+000122a0: 5b6b 5d20 3d20 7365 6c66 2e75 6e69 7175  [k] = self.uniqu
+000122b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000122c0: 735b 6b5d 2020 2020 2020 2020 200d 0a20  s[k]         .. 
+000122d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000122e0: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
+000122f0: 655f 7068 656e 6f74 7970 6573 2873 656c  e_phenotypes(sel
+00012300: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
+00012310: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00012320: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00012330: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00012340: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012350: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00012360: 636b 5f69 6420 3d20 6b0d 0a20 2020 2020  ck_id = k..     
+00012370: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00012380: 6c65 745f 7072 6f70 6572 7469 6573 203d  let_properties =
+00012390: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+000123a0: 636b 5f70 726f 7065 7274 6965 735b 6b5d  ck_properties[k]
+000123b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000123c0: 2020 7472 6163 6b73 203d 2073 656c 662e    tracks = self.
+000123d0: 756e 6971 7565 5f74 7261 636b 735b 6b5d  unique_tracks[k]
+000123e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000123f0: 2020 5a20 3d20 7472 6163 6b73 5b3a 2c32    Z = tracks[:,2
+00012400: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012410: 2020 2059 203d 2074 7261 636b 735b 3a2c     Y = tracks[:,
+00012420: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+00012430: 2020 2020 5820 3d20 7472 6163 6b73 5b3a      X = tracks[:
+00012440: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
+00012450: 2020 2020 2074 696d 6520 3d20 7472 6163       time = trac
+00012460: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012470: 3a2c 305d 0d0a 2020 2020 2020 2020 2020  :,0]..          
+00012480: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+00012490: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000124a0: 6572 7469 6573 5b3a 2c31 5d0d 0a20 2020  erties[:,1]..   
+000124b0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+000124c0: 7175 655f 6964 735f 7365 7420 3d20 7365  que_ids_set = se
+000124d0: 7428 756e 6971 7565 5f69 6473 290d 0a20  t(unique_ids).. 
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000124f0: 656e 6572 6174 696f 6e5f 6964 7320 3d20  eneration_ids = 
+00012500: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00012510: 6965 735b 3a2c 325d 0d0a 2020 2020 2020  ies[:,2]..      
+00012520: 2020 2020 2020 2020 2020 7261 6469 7573            radius
+00012530: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012540: 6572 7469 6573 5b3a 2c33 5d0d 0a20 2020  erties[:,3]..   
+00012550: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00012560: 756d 6520 3d20 7472 6163 6b6c 6574 5f70  ume = tracklet_p
+00012570: 726f 7065 7274 6965 735b 3a2c 345d 0d0a  roperties[:,4]..
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000125a0: 705f 6669 7273 7420 3d20 7472 6163 6b6c  p_first = trackl
+000125b0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000125c0: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+000125d0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+000125e0: 5f63 6f6d 705f 7365 636f 6e64 203d 2074  _comp_second = t
+000125f0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012600: 6573 5b3a 2c36 5d0d 0a20 2020 2020 2020  es[:,6]..       
+00012610: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00012620: 5f61 7265 6120 3d20 7472 6163 6b6c 6574  _area = tracklet
+00012630: 5f70 726f 7065 7274 6965 735b 3a2c 375d  _properties[:,7]
+00012640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012650: 2020 636c 7573 7465 725f 636c 6173 7320    cluster_class 
+00012660: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012670: 7274 6965 735b 3a2c 385d 0d0a 2020 2020  rties[:,8]..    
+00012680: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00012690: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
+000126a0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+000126b0: 7274 6965 735b 3a2c 395d 0d0a 2020 2020  rties[:,9]..    
+000126c0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+000126d0: 6e73 6974 7920 3d20 7472 6163 6b6c 6574  nsity = tracklet
+000126e0: 5f70 726f 7065 7274 6965 735b 3a2c 3130  _properties[:,10
+000126f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012700: 2020 2073 7065 6564 203d 2074 7261 636b     speed = track
+00012710: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00012720: 2c31 315d 0d0a 2020 2020 2020 2020 2020  ,11]..          
+00012730: 2020 2020 2020 6d6f 7469 6f6e 5f61 6e67        motion_ang
+00012740: 6c65 203d 2074 7261 636b 6c65 745f 7072  le = tracklet_pr
+00012750: 6f70 6572 7469 6573 5b3a 2c31 325d 0d0a  operties[:,12]..
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 6163 6365 6c65 7261 7469 6f6e 203d 2074  acceleration = t
+00012780: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012790: 6573 5b3a 2c31 335d 0d0a 2020 2020 2020  es[:,13]..      
+000127a0: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+000127b0: 6365 5f63 656c 6c5f 6d61 736b 203d 2074  ce_cell_mask = t
+000127c0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000127d0: 6573 5b3a 2c31 345d 0d0a 2020 2020 2020  es[:,14]..      
+000127e0: 2020 2020 2020 2020 2020 7261 6469 616c            radial
+000127f0: 5f61 6e67 6c65 203d 2074 7261 636b 6c65  _angle = trackle
+00012800: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
+00012810: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+00012820: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+00012830: 736b 203d 2074 7261 636b 6c65 745f 7072  sk = tracklet_pr
+00012840: 6f70 6572 7469 6573 5b3a 2c31 365d 0d0a  operties[:,16]..
+00012850: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00012860: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012870: 2020 2020 2020 756e 6971 7565 5f66 6674        unique_fft
+00012880: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00012890: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
+000128a0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+000128b0: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+000128c0: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
+000128d0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000128e0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000128f0: 6666 745f 7072 6f70 6572 7469 6573 5b74  fft_properties[t
+00012900: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
+00012910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012920: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00012930: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
+00012940: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 0d0a  ack_id] = {}....
+00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012960: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00012970: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00012980: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00012990: 2020 2020 2020 2075 6e69 7175 655f 6479         unique_dy
+000129a0: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+000129b0: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129d0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+000129e0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
+000129f0: 636b 5f69 645d 203d 207b 7d0d 0a20 2020  ck_id] = {}..   
+00012a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012a10: 662e 756e 6971 7565 5f64 796e 616d 6963  f.unique_dynamic
+00012a20: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+00012a30: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
+00012a40: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+00012a50: 6e64 6564 5f74 696d 6520 3d20 6e70 2e7a  nded_time = np.z
+00012a60: 6572 6f73 2873 656c 662e 7465 6e64 202d  eros(self.tend -
+00012a70: 2073 656c 662e 7473 7461 7274 202b 2031   self.tstart + 1
+00012a80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012a90: 2020 2070 6f69 6e74 5f73 616d 706c 6520     point_sample 
+00012aa0: 3d20 6578 7061 6e64 6564 5f74 696d 652e  = expanded_time.
+00012ab0: 7368 6170 655b 305d 0d0a 2020 2020 2020  shape[0]..      
+00012ac0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00012ad0: 696e 2072 616e 6765 286c 656e 2865 7870  in range(len(exp
+00012ae0: 616e 6465 645f 7469 6d65 2929 3a0d 0a20  anded_time)):.. 
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 2020 2020 2020 6578 7061 6e64 6564 5f74        expanded_t
+00012b10: 696d 655b 695d 203d 2069 200d 0a20 2020  ime[i] = i ..   
+00012b20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012b30: 2063 7572 7265 6e74 5f75 6e69 7175 655f   current_unique_
+00012b40: 6964 2069 6e20 756e 6971 7565 5f69 6473  id in unique_ids
+00012b50: 5f73 6574 3a0d 0a20 2020 2020 2020 2020  _set:..         
+00012b60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00012b80: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
+00012b90: 7920 3d20 6e70 2e7a 6572 6f73 2873 656c  y = np.zeros(sel
+00012ba0: 662e 7465 6e64 202d 2073 656c 662e 7473  f.tend - self.ts
+00012bb0: 7461 7274 202b 2031 290d 0a20 2020 2020  tart + 1)..     
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012be0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012bf0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012c00: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
+00012c10: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012c20: 7272 656e 745f 7a20 3d20 5b5d 0d0a 2020  rrent_z = []..  
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 2063 7572 7265 6e74 5f79 203d 205b 5d0d   current_y = [].
+00012c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c60: 2020 2020 6375 7272 656e 745f 7820 3d20      current_x = 
+00012c70: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012c80: 2020 2020 2020 2063 7572 7265 6e74 5f69         current_i
+00012c90: 6e74 656e 7369 7479 203d 205b 5d0d 0a20  ntensity = [].. 
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
+00012cc0: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ce0: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
+00012cf0: 5f63 6c61 7373 5f73 636f 7265 203d 205b  _class_score = [
+00012d00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012d10: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
+00012d20: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+00012d30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012d40: 7272 656e 745f 766f 6c75 6d65 203d 205b  rrent_volume = [
+00012d50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012d60: 2020 2020 2020 6375 7272 656e 745f 7370        current_sp
+00012d70: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
+00012d80: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012d90: 7265 6e74 5f6d 6f74 696f 6e5f 616e 676c  rent_motion_angl
+00012da0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00012db0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012dc0: 6e74 5f61 6363 656c 6572 6174 696f 6e20  nt_acceleration 
+00012dd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012de0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012df0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00012e00: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
+00012e10: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012e20: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00012e30: 795f 636f 6d70 5f66 6972 7374 203d 205b  y_comp_first = [
+00012e40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012e50: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
+00012e60: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012e70: 7365 636f 6e64 203d 205b 5d0d 0a20 2020  second = []..   
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
+00012ea0: 6172 6561 203d 205b 5d0d 0a0d 0a20 2020  area = []....   
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-00012ed0: 5f75 6e69 7175 655f 6964 203d 3d20 756e  _unique_id == un
-00012ee0: 6971 7565 5f69 6473 5b6a 5d3a 0d0a 2020  ique_ids[j]:..  
-00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012f10: 7572 7265 6e74 5f74 696d 652e 6170 7065  urrent_time.appe
-00012f20: 6e64 2874 696d 655b 6a5d 290d 0a20 2020  nd(time[j])..   
-00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f40: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00012f50: 7272 656e 745f 7a2e 6170 7065 6e64 285a  rrent_z.append(Z
-00012f60: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 2020 2020 2020 2063 7572 7265 6e74 5f79         current_y
-00012f90: 2e61 7070 656e 6428 595b 6a5d 290d 0a20  .append(Y[j]).. 
+00012ec0: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
+00012ed0: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012ef0: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
+00012f00: 6d61 736b 203d 205b 5d20 0d0a 2020 2020  mask = [] ..    
+00012f10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00012f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f30: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00012f40: 6765 2874 696d 652e 7368 6170 655b 305d  ge(time.shape[0]
+00012f50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012f60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012f70: 2063 7572 7265 6e74 5f75 6e69 7175 655f   current_unique_
+00012f80: 6964 203d 3d20 756e 6971 7565 5f69 6473  id == unique_ids
+00012f90: 5b6a 5d3a 0d0a 2020 2020 2020 2020 2020  [j]:..          
 00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 6375 7272 656e 745f 782e 6170 7065 6e64  current_x.append
-00012fd0: 2858 5b6a 5d29 0d0a 2020 2020 2020 2020  (X[j])..        
+00012fb0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00012fc0: 696d 652e 6170 7065 6e64 2874 696d 655b  ime.append(time[
+00012fd0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
 00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ff0: 2020 2020 2020 2020 2065 7870 616e 6465           expande
-00013000: 645f 696e 7465 6e73 6974 795b 696e 7428  d_intensity[int(
-00013010: 7469 6d65 5b6a 5d29 5d20 3d20 696e 7465  time[j])] = inte
-00013020: 6e73 6974 795b 6a5d 0d0a 2020 2020 2020  nsity[j]..      
-00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013050: 6e74 5f69 6e74 656e 7369 7479 2e61 7070  nt_intensity.app
-00013060: 656e 6428 696e 7465 6e73 6974 795b 6a5d  end(intensity[j]
-00013070: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012ff0: 2020 2020 2020 6375 7272 656e 745f 7a2e        current_z.
+00013000: 6170 7065 6e64 285a 5b6a 5d29 0d0a 2020  append(Z[j])..  
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013030: 7572 7265 6e74 5f79 2e61 7070 656e 6428  urrent_y.append(
+00013040: 595b 6a5d 290d 0a20 2020 2020 2020 2020  Y[j])..         
+00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013060: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013070: 782e 6170 7065 6e64 2858 5b6a 5d29 0d0a  x.append(X[j])..
 00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013090: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
-000130a0: 7465 725f 636c 6173 732e 6170 7065 6e64  ter_class.append
-000130b0: 2863 6c75 7374 6572 5f63 6c61 7373 5b6a  (cluster_class[j
-000130c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130e0: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
-000130f0: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
-00013100: 2e61 7070 656e 6428 636c 7573 7465 725f  .append(cluster_
-00013110: 636c 6173 735f 7363 6f72 655b 6a5d 290d  class_score[j]).
-00013120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013140: 2020 6375 7272 656e 745f 7261 6469 7573    current_radius
-00013150: 2e61 7070 656e 6428 7261 6469 7573 5b6a  .append(radius[j
-00013160: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130a0: 2065 7870 616e 6465 645f 696e 7465 6e73   expanded_intens
+000130b0: 6974 795b 696e 7428 7469 6d65 5b6a 5d29  ity[int(time[j])
+000130c0: 5d20 3d20 696e 7465 6e73 6974 795b 6a5d  ] = intensity[j]
+000130d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130f0: 2020 2063 7572 7265 6e74 5f69 6e74 656e     current_inten
+00013100: 7369 7479 2e61 7070 656e 6428 696e 7465  sity.append(inte
+00013110: 6e73 6974 795b 6a5d 290d 0a20 2020 2020  nsity[j])..     
+00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013130: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013140: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
+00013150: 732e 6170 7065 6e64 2863 6c75 7374 6572  s.append(cluster
+00013160: 5f63 6c61 7373 5b6a 5d29 0d0a 2020 2020  _class[j])..    
 00013170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013180: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
-00013190: 756d 652e 6170 7065 6e64 2876 6f6c 756d  ume.append(volum
-000131a0: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000131d0: 7370 6565 642e 6170 7065 6e64 2873 7065  speed.append(spe
-000131e0: 6564 5b6a 5d29 0d0a 2020 2020 2020 2020  ed[j])..        
-000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013210: 5f6d 6f74 696f 6e5f 616e 676c 652e 6170  _motion_angle.ap
-00013220: 7065 6e64 286d 6f74 696f 6e5f 616e 676c  pend(motion_angl
-00013230: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-00013240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013250: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013260: 6163 6365 6c65 7261 7469 6f6e 2e61 7070  acceleration.app
-00013270: 656e 6428 6163 6365 6c65 7261 7469 6f6e  end(acceleration
-00013280: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013180: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013190: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+000131a0: 7373 5f73 636f 7265 2e61 7070 656e 6428  ss_score.append(
+000131b0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+000131c0: 6f72 655b 6a5d 290d 0a20 2020 2020 2020  ore[j])..       
+000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000131f0: 745f 7261 6469 7573 2e61 7070 656e 6428  t_radius.append(
+00013200: 7261 6469 7573 5b6a 5d29 0d0a 2020 2020  radius[j])..    
+00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013220: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013230: 7265 6e74 5f76 6f6c 756d 652e 6170 7065  rent_volume.appe
+00013240: 6e64 2876 6f6c 756d 655b 6a5d 290d 0a20  nd(volume[j]).. 
+00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013270: 6375 7272 656e 745f 7370 6565 642e 6170  current_speed.ap
+00013280: 7065 6e64 2873 7065 6564 5b6a 5d29 0d0a  pend(speed[j])..
 00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2020 2020 2020 2063 7572 7265 6e74 5f64         current_d
-000132b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000132c0: 6b2e 6170 7065 6e64 2864 6973 7461 6e63  k.append(distanc
-000132d0: 655f 6365 6c6c 5f6d 6173 6b5b 6a5d 290d  e_cell_mask[j]).
-000132e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
+000132c0: 616e 676c 652e 6170 7065 6e64 286d 6f74  angle.append(mot
+000132d0: 696f 6e5f 616e 676c 655b 6a5d 290d 0a20  ion_angle[j]).. 
+000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00013310: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013320: 742e 6170 7065 6e64 2865 6363 656e 7472  t.append(eccentr
-00013330: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013340: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-00013370: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00013380: 5f73 6563 6f6e 642e 6170 7065 6e64 2865  _second.append(e
-00013390: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000133a0: 5f73 6563 6f6e 645b 6a5d 290d 0a20 2020  _second[j])..   
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000133d0: 7272 656e 745f 7375 7266 6163 655f 6172  rrent_surface_ar
-000133e0: 6561 2e61 7070 656e 6428 7375 7266 6163  ea.append(surfac
-000133f0: 655f 6172 6561 5b6a 5d29 0d0a 2020 2020  e_area[j])..    
-00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013410: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013420: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
-00013430: 652e 6170 7065 6e64 2872 6164 6961 6c5f  e.append(radial_
-00013440: 616e 676c 655b 6a5d 290d 0a20 2020 2020  angle[j])..     
-00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013460: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013470: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
-00013480: 736b 2e61 7070 656e 6428 6365 6c6c 5f61  sk.append(cell_a
-00013490: 7869 735f 6d61 736b 5b6a 5d29 0d0a 2020  xis_mask[j])..  
-000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134b0: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
-000134c0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-000134d0: 6e74 5f74 696d 6529 0d0a 2020 2020 2020  nt_time)..      
-000134e0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000134f0: 7265 6e74 5f69 6e74 656e 7369 7479 203d  rent_intensity =
-00013500: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00013510: 656e 745f 696e 7465 6e73 6974 7929 0d0a  ent_intensity)..
-00013520: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00013530: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00013540: 6c75 7374 6572 5f63 6c61 7373 203d 206e  luster_class = n
-00013550: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00013560: 745f 636c 7573 7465 725f 636c 6173 7329  t_cluster_class)
-00013570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013580: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
-00013590: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
-000135a0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-000135b0: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
-000135c0: 6173 735f 7363 6f72 6529 2020 200d 0a0d  ass_score)   ...
-000135d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000135e0: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-000135f0: 7573 203d 206e 702e 6173 6172 7261 7928  us = np.asarray(
-00013600: 6375 7272 656e 745f 7261 6469 7573 290d  current_radius).
-00013610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013620: 2020 2020 6375 7272 656e 745f 766f 6c75      current_volu
-00013630: 6d65 203d 206e 702e 6173 6172 7261 7928  me = np.asarray(
-00013640: 6375 7272 656e 745f 766f 6c75 6d65 290d  current_volume).
-00013650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013660: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00013670: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00013680: 7273 7420 3d20 6e70 2e61 7361 7272 6179  rst = np.asarray
-00013690: 2863 7572 7265 6e74 5f65 6363 656e 7472  (current_eccentr
-000136a0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-000136b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000136c0: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-000136d0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000136e0: 7365 636f 6e64 203d 206e 702e 6173 6172  second = np.asar
-000136f0: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
-00013700: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013710: 636f 6e64 290d 0a20 2020 2020 2020 2020  cond)..         
-00013720: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013730: 745f 7375 7266 6163 655f 6172 6561 203d  t_surface_area =
-00013740: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00013750: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00013760: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00013770: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013780: 7370 6565 6420 3d20 6e70 2e61 7361 7272  speed = np.asarr
-00013790: 6179 2863 7572 7265 6e74 5f73 7065 6564  ay(current_speed
-000137a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000137b0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-000137c0: 7469 6f6e 5f61 6e67 6c65 203d 206e 702e  tion_angle = np.
-000137d0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-000137e0: 6d6f 7469 6f6e 5f61 6e67 6c65 290d 0a20  motion_angle).. 
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
-00013810: 7261 7469 6f6e 203d 206e 702e 6173 6172  ration = np.asar
-00013820: 7261 7928 6375 7272 656e 745f 6163 6365  ray(current_acce
-00013830: 6c65 7261 7469 6f6e 290d 0a20 2020 2020  leration)..     
-00013840: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013850: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
-00013860: 656c 6c5f 6d61 736b 203d 206e 702e 6173  ell_mask = np.as
-00013870: 6172 7261 7928 6375 7272 656e 745f 6469  array(current_di
-00013880: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00013890: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000138a0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
-000138b0: 6469 616c 5f61 6e67 6c65 203d 206e 702e  dial_angle = np.
-000138c0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-000138d0: 7261 6469 616c 5f61 6e67 6c65 290d 0a20  radial_angle).. 
-000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
-00013900: 7869 735f 6d61 736b 203d 206e 702e 6173  xis_mask = np.as
-00013910: 6172 7261 7928 6375 7272 656e 745f 6365  array(current_ce
-00013920: 6c6c 5f61 7869 735f 6d61 736b 290d 0a0d  ll_axis_mask)...
-00013930: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00013940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013950: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013970: 6966 2070 6f69 6e74 5f73 616d 706c 6520  if point_sample 
-00013980: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 2020 2020 7866 5f73 616d 706c 6520        xf_sample 
-000139b0: 3d20 6666 7466 7265 7128 706f 696e 745f  = fftfreq(point_
-000139c0: 7361 6d70 6c65 2c20 7365 6c66 2e74 6361  sample, self.tca
-000139d0: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-000139e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139f0: 2020 2020 2020 2020 2020 2020 6666 7473              ffts
-00013a00: 7472 6970 5f73 616d 706c 6520 3d20 6666  trip_sample = ff
-00013a10: 7428 6578 7061 6e64 6564 5f69 6e74 656e  t(expanded_inten
-00013a20: 7369 7479 290d 0a20 2020 2020 2020 2020  sity)..         
+00013300: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00013310: 7469 6f6e 2e61 7070 656e 6428 6163 6365  tion.append(acce
+00013320: 6c65 7261 7469 6f6e 5b6a 5d29 0d0a 2020  leration[j])..  
+00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013340: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013350: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
+00013360: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00013370: 2864 6973 7461 6e63 655f 6365 6c6c 5f6d  (distance_cell_m
+00013380: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
+00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000133b0: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+000133c0: 6f6d 705f 6669 7273 742e 6170 7065 6e64  omp_first.append
+000133d0: 2865 6363 656e 7472 6963 6974 795f 636f  (eccentricity_co
+000133e0: 6d70 5f66 6972 7374 5b6a 5d29 0d0a 2020  mp_first[j])..  
+000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013400: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013410: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013420: 6974 795f 636f 6d70 5f73 6563 6f6e 642e  ity_comp_second.
+00013430: 6170 7065 6e64 2865 6363 656e 7472 6963  append(eccentric
+00013440: 6974 795f 636f 6d70 5f73 6563 6f6e 645b  ity_comp_second[
+00013450: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 2020 2020 2020 6375 7272 656e 745f 7375        current_su
+00013480: 7266 6163 655f 6172 6561 2e61 7070 656e  rface_area.appen
+00013490: 6428 7375 7266 6163 655f 6172 6561 5b6a  d(surface_area[j
+000134a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134c0: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
+000134d0: 6961 6c5f 616e 676c 652e 6170 7065 6e64  ial_angle.append
+000134e0: 2872 6164 6961 6c5f 616e 676c 655b 6a5d  (radial_angle[j]
+000134f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
+00013520: 5f61 7869 735f 6d61 736b 2e61 7070 656e  _axis_mask.appen
+00013530: 6428 6365 6c6c 5f61 7869 735f 6d61 736b  d(cell_axis_mask
+00013540: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013550: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013560: 5f74 696d 6520 3d20 6e70 2e61 7361 7272  _time = np.asarr
+00013570: 6179 2863 7572 7265 6e74 5f74 696d 6529  ay(current_time)
+00013580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013590: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
+000135a0: 656e 7369 7479 203d 206e 702e 6173 6172  ensity = np.asar
+000135b0: 7261 7928 6375 7272 656e 745f 696e 7465  ray(current_inte
+000135c0: 6e73 6974 7929 0d0a 0d0a 0d0a 2020 2020  nsity)......    
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135e0: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+000135f0: 6c61 7373 203d 206e 702e 6173 6172 7261  lass = np.asarra
+00013600: 7928 6375 7272 656e 745f 636c 7573 7465  y(current_cluste
+00013610: 725f 636c 6173 7329 0d0a 2020 2020 2020  r_class)..      
+00013620: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013630: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00013640: 7373 5f73 636f 7265 203d 206e 702e 6173  ss_score = np.as
+00013650: 6172 7261 7928 6375 7272 656e 745f 636c  array(current_cl
+00013660: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+00013670: 6529 2020 200d 0a0d 0a20 2020 2020 2020  e)   ....       
+00013680: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013690: 656e 745f 7261 6469 7573 203d 206e 702e  ent_radius = np.
+000136a0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+000136b0: 7261 6469 7573 290d 0a20 2020 2020 2020  radius)..       
+000136c0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000136d0: 656e 745f 766f 6c75 6d65 203d 206e 702e  ent_volume = np.
+000136e0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+000136f0: 766f 6c75 6d65 290d 0a20 2020 2020 2020  volume)..       
+00013700: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013710: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013720: 5f63 6f6d 705f 6669 7273 7420 3d20 6e70  _comp_first = np
+00013730: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013740: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00013750: 6d70 5f66 6972 7374 290d 0a20 2020 2020  mp_first)..     
+00013760: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013770: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013780: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00013790: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000137a0: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+000137b0: 5f63 6f6d 705f 7365 636f 6e64 290d 0a20  _comp_second).. 
+000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137d0: 2020 6375 7272 656e 745f 7375 7266 6163    current_surfac
+000137e0: 655f 6172 6561 203d 206e 702e 6173 6172  e_area = np.asar
+000137f0: 7261 7928 6375 7272 656e 745f 7375 7266  ray(current_surf
+00013800: 6163 655f 6172 6561 290d 0a0d 0a20 2020  ace_area)....   
+00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013820: 6375 7272 656e 745f 7370 6565 6420 3d20  current_speed = 
+00013830: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013840: 6e74 5f73 7065 6564 290d 0a20 2020 2020  nt_speed)..     
+00013850: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013860: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
+00013870: 6c65 203d 206e 702e 6173 6172 7261 7928  le = np.asarray(
+00013880: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+00013890: 6e67 6c65 290d 0a20 2020 2020 2020 2020  ngle)..         
+000138a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000138b0: 745f 6163 6365 6c65 7261 7469 6f6e 203d  t_acceleration =
+000138c0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000138d0: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
+000138e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000138f0: 2020 2020 2020 6375 7272 656e 745f 6469        current_di
+00013900: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013910: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00013920: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
+00013930: 656c 6c5f 6d61 736b 290d 0a20 2020 2020  ell_mask)..     
+00013940: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013950: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
+00013960: 6c65 203d 206e 702e 6173 6172 7261 7928  le = np.asarray(
+00013970: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
+00013980: 6e67 6c65 290d 0a20 2020 2020 2020 2020  ngle)..         
+00013990: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000139a0: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
+000139b0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+000139c0: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
+000139d0: 6d61 736b 290d 0a0d 0a0d 0a20 2020 2020  mask)......     
+000139e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00013a10: 2020 2020 2020 2020 6966 2070 6f69 6e74          if point
+00013a20: 5f73 616d 706c 6520 3e20 303a 0d0a 2020  _sample > 0:..  
 00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a40: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
-00013a50: 7361 6d70 6c65 203d 206e 702e 6162 7328  sample = np.abs(
-00013a60: 6666 7473 7472 6970 5f73 616d 706c 6529  fftstrip_sample)
-00013a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a90: 2020 7866 5f73 616d 706c 6520 3d20 7866    xf_sample = xf
-00013aa0: 5f73 616d 706c 655b 3020 3a20 6c65 6e28  _sample[0 : len(
-00013ab0: 7866 5f73 616d 706c 6529 202f 2f20 325d  xf_sample) // 2]
-00013ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013a40: 2020 2020 2020 2020 2020 2020 2020 7866                xf
+00013a50: 5f73 616d 706c 6520 3d20 6666 7466 7265  _sample = fftfre
+00013a60: 7128 706f 696e 745f 7361 6d70 6c65 2c20  q(point_sample, 
+00013a70: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00013a80: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013aa0: 2020 2020 6666 7473 7472 6970 5f73 616d      fftstrip_sam
+00013ab0: 706c 6520 3d20 6666 7428 6578 7061 6e64  ple = fft(expand
+00013ac0: 6564 5f69 6e74 656e 7369 7479 290d 0a20  ed_intensity).. 
 00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ae0: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
-00013af0: 6520 3d20 6666 7474 6f74 616c 5f73 616d  e = ffttotal_sam
-00013b00: 706c 655b 3020 3a20 6c65 6e28 6666 7474  ple[0 : len(fftt
-00013b10: 6f74 616c 5f73 616d 706c 6529 202f 2f20  otal_sample) // 
-00013b20: 325d 0d0a 0d0a 2020 2020 2020 2020 2020  2]....          
-00013b30: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00013b40: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
-00013b50: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00013b60: 756e 6971 7565 5f69 645d 203d 2065 7870  unique_id] = exp
-00013b70: 616e 6465 645f 7469 6d65 2c20 6578 7061  anded_time, expa
-00013b80: 6e64 6564 5f69 6e74 656e 7369 7479 2c20  nded_intensity, 
-00013b90: 7866 5f73 616d 706c 652c 2066 6674 746f  xf_sample, fftto
-00013ba0: 7461 6c5f 7361 6d70 6c65 0d0a 2020 2020  tal_sample..    
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00013bc0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-00013bd0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00013be0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00013bf0: 5f69 645d 203d 2020 6375 7272 656e 745f  _id] =  current_
-00013c00: 7469 6d65 2c20 6375 7272 656e 745f 636c  time, current_cl
-00013c10: 7573 7465 725f 636c 6173 732c 2063 7572  uster_class, cur
-00013c20: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00013c30: 7373 5f73 636f 7265 0d0a 2020 2020 2020  ss_score..      
-00013c40: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00013c50: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00013c60: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00013c70: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00013c80: 203d 2063 7572 7265 6e74 5f74 696d 652c   = current_time,
-00013c90: 2063 7572 7265 6e74 5f7a 2c20 6375 7272   current_z, curr
-00013ca0: 656e 745f 792c 2063 7572 7265 6e74 5f78  ent_y, current_x
-00013cb0: 2c20 6375 7272 656e 745f 7261 6469 7573  , current_radius
-00013cc0: 2c20 6375 7272 656e 745f 766f 6c75 6d65  , current_volume
-00013cd0: 2c20 6375 7272 656e 745f 6563 6365 6e74  , current_eccent
-00013ce0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013cf0: 742c 2063 7572 7265 6e74 5f65 6363 656e  t, current_eccen
-00013d00: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013d10: 6f6e 642c 2063 7572 7265 6e74 5f73 7572  ond, current_sur
-00013d20: 6661 6365 5f61 7265 612c 2063 7572 7265  face_area, curre
-00013d30: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00013d40: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
-00013d50: 725f 636c 6173 735f 7363 6f72 650d 0a20  r_class_score.. 
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d70: 2020 756e 6971 7565 5f64 796e 616d 6963    unique_dynamic
-00013d80: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013d90: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013da0: 7175 655f 6964 5d20 3d20 6375 7272 656e  que_id] = curren
-00013db0: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
-00013dc0: 7370 6565 642c 2063 7572 7265 6e74 5f6d  speed, current_m
-00013dd0: 6f74 696f 6e5f 616e 676c 652c 2063 7572  otion_angle, cur
-00013de0: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
-00013df0: 6e2c 2063 7572 7265 6e74 5f64 6973 7461  n, current_dista
-00013e00: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 2063  nce_cell_mask, c
-00013e10: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00013e20: 676c 652c 2063 7572 7265 6e74 5f63 656c  gle, current_cel
-00013e30: 6c5f 6178 6973 5f6d 6173 6b0d 0a20 2020  l_axis_mask..   
-00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e50: 7365 6c66 2e75 6e69 7175 655f 6666 745f  self.unique_fft_
-00013e60: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-00013e70: 5f69 645d 2e75 7064 6174 6528 7b63 7572  _id].update({cur
-00013e80: 7265 6e74 5f75 6e69 7175 655f 6964 3a75  rent_unique_id:u
-00013e90: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-00013ea0: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00013eb0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00013ec0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00013ed0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013ee0: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00013ef0: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
-00013f00: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
-00013f10: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
-00013f20: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
-00013f30: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-00013f40: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
-00013f50: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00013f60: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00013f70: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00013f80: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
-00013f90: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
-00013fa0: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
-00013fb0: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00013fc0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013fd0: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 2020 2073 656c 662e 756e 6971 7565 5f64     self.unique_d
-00014000: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
-00014010: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-00014020: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-00014030: 7565 5f69 643a 756e 6971 7565 5f64 796e  ue_id:unique_dyn
-00014040: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
-00014050: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00014060: 5f75 6e69 7175 655f 6964 5d7d 290d 0a0d  _unique_id]})...
-00014070: 0a20 2020 2064 6566 205f 7365 636f 6e64  .    def _second
-00014080: 5f63 6861 6e6e 656c 5f73 706f 7473 2873  _channel_spots(s
-00014090: 656c 662c 2066 7261 6d65 2c20 7a2c 2079  elf, frame, z, y
-000140a0: 2c20 782c 2063 656c 6c5f 6964 2c20 7472  , x, cell_id, tr
-000140b0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-000140c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000140d0: 2020 2074 7265 652c 2063 656e 7472 6f69     tree, centroi
-000140e0: 6473 2c20 6c61 6265 6c73 2c20 766f 6c75  ds, labels, volu
-000140f0: 6d65 2c20 696e 7465 6e73 6974 795f 6d65  me, intensity_me
-00014100: 616e 2c20 696e 7465 6e73 6974 795f 746f  an, intensity_to
-00014110: 7461 6c2c 2062 6f75 6e64 696e 675f 626f  tal, bounding_bo
-00014120: 7865 7320 3d20 7365 6c66 2e5f 7469 6d65  xes = self._time
-00014130: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
-00014140: 6167 655b 7374 7228 696e 7428 666c 6f61  age[str(int(floa
-00014150: 7428 6672 616d 6529 2929 5d0d 0a20 2020  t(frame)))]..   
-00014160: 2020 2020 2020 2020 2070 6978 656c 7465           pixelte
-00014170: 7374 6c6f 6361 7469 6f6e 203d 2028 7a2c  stlocation = (z,
-00014180: 792c 7829 0d0a 2020 2020 2020 2020 2020  y,x)..          
-00014190: 2020 6469 7374 2c20 696e 6465 7820 3d20    dist, index = 
-000141a0: 7472 6565 2e71 7565 7279 2870 6978 656c  tree.query(pixel
-000141b0: 7465 7374 6c6f 6361 7469 6f6e 290d 0a0d  testlocation)...
-000141c0: 0a0d 0a20 2020 2020 2020 2020 2020 2062  ...            b
-000141d0: 626f 7820 3d20 626f 756e 6469 6e67 5f62  box = bounding_b
-000141e0: 6f78 6573 5b69 6e64 6578 5d0d 0a20 2020  oxes[index]..   
-000141f0: 2020 2020 2020 2020 2073 697a 657a 203d           sizez =
-00014200: 2061 6273 2862 626f 785b 305d 202d 2062   abs(bbox[0] - b
-00014210: 626f 785b 335d 290d 0a20 2020 2020 2020  box[3])..       
-00014220: 2020 2020 2073 697a 6579 203d 2061 6273       sizey = abs
-00014230: 2862 626f 785b 315d 202d 2062 626f 785b  (bbox[1] - bbox[
-00014240: 345d 290d 0a20 2020 2020 2020 2020 2020  4])..           
-00014250: 2073 697a 6578 203d 2061 6273 2862 626f   sizex = abs(bbo
-00014260: 785b 325d 202d 2062 626f 785b 355d 2920  x[2] - bbox[5]) 
-00014270: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-00014280: 746f 5f76 6f6c 756d 6520 3d20 7369 7a65  to_volume = size
-00014290: 7820 2a20 7369 7a65 7920 2a20 7369 7a65  x * sizey * size
-000142a0: 7a0d 0a20 2020 2020 2020 2020 2020 2076  z..            v
-000142b0: 6574 6f5f 7261 6469 7573 203d 206d 6174  eto_radius = mat
-000142c0: 682e 706f 7728 3320 2a20 7665 746f 5f76  h.pow(3 * veto_v
-000142d0: 6f6c 756d 6520 2f20 2834 202a 206d 6174  olume / (4 * mat
-000142e0: 682e 7069 292c 2031 2e30 202f 2033 2e30  h.pi), 1.0 / 3.0
-000142f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00014300: 206c 6f63 6174 696f 6e20 3d20 2863 656e   location = (cen
-00014310: 7472 6f69 6473 5b69 6e64 6578 5d5b 305d  troids[index][0]
-00014320: 202a 2073 656c 662e 7a63 616c 6962 7261   * self.zcalibra
-00014330: 7469 6f6e 2c20 6365 6e74 726f 6964 735b  tion, centroids[
-00014340: 696e 6465 785d 5b31 5d2a 7365 6c66 2e79  index][1]*self.y
-00014350: 6361 6c69 6272 6174 696f 6e2c 2063 656e  calibration, cen
-00014360: 7472 6f69 6473 5b69 6e64 6578 5d5b 325d  troids[index][2]
-00014370: 2a73 656c 662e 7863 616c 6962 7261 7469  *self.xcalibrati
-00014380: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-00014390: 2051 5541 4c49 5459 203d 2076 6f6c 756d   QUALITY = volum
-000143a0: 655b 696e 6465 785d 0d0a 2020 2020 2020  e[index]..      
-000143b0: 2020 2020 2020 5241 4449 5553 203d 206d        RADIUS = m
-000143c0: 6174 682e 706f 7728 5155 414c 4954 5920  ath.pow(QUALITY 
-000143d0: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-000143e0: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
-000143f0: 6272 6174 696f 6e20 2a20 7365 6c66 2e7a  bration * self.z
-00014400: 6361 6c69 6272 6174 696f 6e2c 2031 2e30  calibration, 1.0
-00014410: 2f33 2e30 2920 0d0a 0d0a 2020 2020 2020  /3.0) ....      
-00014420: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
-00014430: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
-00014440: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
-00014450: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
-00014460: 2866 7261 6d65 2c20 6c6f 6361 7469 6f6e  (frame, location
-00014470: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00014480: 6620 6469 7374 203c 3d20 3220 2a20 7665  f dist <= 2 * ve
-00014490: 746f 5f72 6164 6975 733a 0d0a 2020 2020  to_radius:..    
-000144a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000144b0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-000144c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000144d0: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
-000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144f0: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
-00014500: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
-00014510: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
-00014520: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014530: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
-00014540: 3a20 696e 7428 6672 616d 6529 2c0d 0a20  : int(frame),.. 
-00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014560: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
-00014570: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
-00014580: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014590: 305d 2a20 7365 6c66 2e7a 6361 6c69 6272  0]* self.zcalibr
-000145a0: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-000145d0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
-000145e0: 6473 5b69 6e64 6578 5d5b 315d 2a20 7365  ds[index][1]* se
-000145f0: 6c66 2e79 6361 6c69 6272 6174 696f 6e29  lf.ycalibration)
-00014600: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014620: 7870 6f73 6964 5f6b 6579 203a 2066 6c6f  xposid_key : flo
-00014630: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00014640: 6578 5d5b 325d 2a20 7365 6c66 2e78 6361  ex][2]* self.xca
-00014650: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014670: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
-00014680: 645f 6b65 793a 2069 6e74 2874 7261 636b  d_key: int(track
-00014690: 5f69 6429 2c0d 0a20 2020 2020 2020 2020  _id),..         
-000146a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000146b0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-000146c0: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
-000146d0: 2869 6e74 656e 7369 7479 5f74 6f74 616c  (intensity_total
-000146e0: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
-000146f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014700: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-00014710: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00014720: 6c6f 6174 2869 6e74 656e 7369 7479 5f6d  loat(intensity_m
-00014730: 6561 6e5b 696e 6465 785d 2929 2c0d 0a0d  ean[index])),...
-00014740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014750: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00014760: 6469 7573 5f6b 6579 203a 2028 666c 6f61  dius_key : (floa
-00014770: 7428 5241 4449 5553 2929 2c0d 0a20 2020  t(RADIUS)),..   
-00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014790: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
-000147a0: 795f 6b65 7920 3a20 2866 6c6f 6174 2851  y_key : (float(Q
-000147b0: 5541 4c49 5459 2929 2c0d 0a20 2020 2020  UALITY)),..     
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2020 2073 656c 662e 6469 7374 616e 6365     self.distance
-000147e0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 3a20  _cell_mask_key: 
-000147f0: 666c 6f61 7428 6469 7374 616e 6365 5f63  float(distance_c
-00014800: 656c 6c5f 6d61 736b 292c 0d0a 2020 2020  ell_mask),..    
-00014810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014820: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-00014830: 7472 6f69 645f 7a5f 6b65 793a 2066 6c6f  troid_z_key: flo
-00014840: 6174 286d 6173 6b63 656e 7472 6f69 645b  at(maskcentroid[
-00014850: 305d 292c 0d0a 2020 2020 2020 2020 2020  0]),..          
-00014860: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014870: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-00014880: 795f 6b65 793a 2066 6c6f 6174 286d 6173  y_key: float(mas
-00014890: 6b63 656e 7472 6f69 645b 315d 292c 0d0a  kcentroid[1]),..
-000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148b0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-000148c0: 6b63 656e 7472 6f69 645f 785f 6b65 793a  kcentroid_x_key:
-000148d0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-000148e0: 6f69 645b 325d 2920 0d0a 0d0a 2020 2020  oid[2]) ....    
-000148f0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00014900: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00014910: 6365 6c6c 5f69 6420 696e 2073 656c 662e  cell_id in self.
-00014920: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00014930: 7570 2e6b 6579 7328 293a 0d0a 2020 2020  up.keys():..    
-00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014960: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-00014970: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-00014980: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00014990: 645d 203d 2073 656c 662e 756e 6971 7565  d] = self.unique
-000149a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000149b0: 5b63 656c 6c5f 6964 5d0d 0a0d 0a20 2020  [cell_id]....   
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-000149e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000149f0: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00014a00: 6461 7465 287b 7365 6c66 2e74 6f74 616c  date({self.total
-00014a10: 5f69 6e74 656e 7369 7479 5f6b 6579 3a20  _intensity_key: 
-00014a20: 4e6f 6e65 7d29 0d0a 2020 2020 2020 2020  None})..        
-00014a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014a40: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-00014a50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014a60: 6365 6c6c 5f69 645d 2e75 7064 6174 6528  cell_id].update(
-00014a70: 7b73 656c 662e 6d65 616e 5f69 6e74 656e  {self.mean_inten
-00014a80: 7369 7479 5f6b 6579 3a20 4e6f 6e65 7d29  sity_key: None})
-00014a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014aa0: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-00014ab0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-00014ac0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00014ad0: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00014ae0: 7261 6469 7573 5f6b 6579 3a20 4e6f 6e65  radius_key: None
-00014af0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00014b00: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00014b10: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00014b20: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00014b30: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-00014b40: 662e 7175 616c 6974 795f 6b65 793a 204e  f.quality_key: N
-00014b50: 6f6e 657d 290d 0a0d 0a0d 0a20 2020 2020  one})......     
-00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00014b80: 2020 6465 6620 5f64 6963 745f 7570 6461    def _dict_upda
-00014b90: 7465 2873 656c 662c 2075 6e69 7175 655f  te(self, unique_
-00014ba0: 7472 6163 6b6c 6574 5f69 6473 3a20 4c69  tracklet_ids: Li
-00014bb0: 7374 2c20 2063 656c 6c5f 6964 3a20 696e  st,  cell_id: in
-00014bc0: 742c 2074 7261 636b 5f69 643a 2069 6e74  t, track_id: int
-00014bd0: 2c20 736f 7572 6365 5f69 643a 2069 6e74  , source_id: int
-00014be0: 2c20 7461 7267 6574 5f69 643a 2069 6e74  , target_id: int
-00014bf0: 293a 0d0a 0d0a 200d 0a20 2020 2020 2020  ):.... ..       
-00014c00: 2067 656e 6572 6174 696f 6e5f 6964 203d   generation_id =
-00014c10: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00014c20: 5f64 6963 745b 6365 6c6c 5f69 645d 0d0a  _dict[cell_id]..
-00014c30: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00014c40: 5f69 6420 3d20 7365 6c66 2e74 7261 636b  _id = self.track
-00014c50: 6c65 745f 6469 6374 5b63 656c 6c5f 6964  let_dict[cell_id
-00014c60: 5d0d 0a0d 0a20 2020 2020 2020 2075 6e69  ]....        uni
-00014c70: 7175 655f 6964 203d 2073 7472 2874 7261  que_id = str(tra
-00014c80: 636b 5f69 6429 202b 2073 7472 2873 656c  ck_id) + str(sel
-00014c90: 662e 6d61 785f 7472 6163 6b5f 6964 2920  f.max_track_id) 
-00014ca0: 2b20 7374 7228 6765 6e65 7261 7469 6f6e  + str(generation
-00014cb0: 5f69 6429 202b 2073 7472 2874 7261 636b  _id) + str(track
-00014cc0: 6c65 745f 6964 290d 0a20 2020 2020 2020  let_id)..       
-00014cd0: 200d 0a20 2020 2020 2020 2076 6563 5f6d   ..        vec_m
-00014ce0: 6173 6b20 3d20 5b66 6c6f 6174 2873 656c  ask = [float(sel
-00014cf0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014d00: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014d10: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-00014d20: 6365 6e74 726f 6964 5f78 5f6b 6579 5d29  centroid_x_key])
-00014d30: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
-00014d40: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014d50: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014d60: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
-00014d70: 6f69 645f 795f 6b65 795d 292c 2066 6c6f  oid_y_key]), flo
-00014d80: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014d90: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014da0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014db0: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-00014dc0: 5f6b 6579 5d29 205d 0d0a 0d0a 2020 2020  _key]) ]....    
-00014dd0: 2020 2020 7665 635f 6365 6c6c 203d 205b      vec_cell = [
-00014de0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00014df0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014e00: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00014e10: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00014e20: 2920 2c20 0d0a 2020 2020 2020 2020 2020  ) , ..          
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
-00014e50: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014e60: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014e70: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00014e80: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
-00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ea0: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
-00014eb0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014ec0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014ed0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
-00014ee0: 6579 5d29 5d0d 0a0d 0a20 2020 2020 2020  ey])]....       
-00014ef0: 2061 6e67 6c65 203d 2061 6e67 756c 6172   angle = angular
-00014f00: 5f63 6861 6e67 6528 7665 635f 6d61 736b  _change(vec_mask
-00014f10: 2c20 7665 635f 6365 6c6c 290d 0a0d 0a20  , vec_cell).... 
-00014f20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014f30: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014f40: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014f50: 2e75 7064 6174 6528 7b73 656c 662e 7261  .update({self.ra
-00014f60: 6469 616c 5f61 6e67 6c65 5f6b 6579 203a  dial_angle_key :
-00014f70: 2061 6e67 6c65 7d29 2020 2020 2020 2020   angle})        
-00014f80: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00014f90: 2020 2020 2020 2020 756e 6971 7565 5f74          unique_t
-00014fa0: 7261 636b 6c65 745f 6964 732e 6170 7065  racklet_ids.appe
-00014fb0: 6e64 2873 7472 2875 6e69 7175 655f 6964  nd(str(unique_id
-00014fc0: 2929 0d0a 2020 2020 2020 2020 7365 6c66  ))..        self
-00014fd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014fe0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014ff0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015000: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00015010: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-00015020: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015030: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015040: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015050: 7570 6461 7465 287b 7365 6c66 2e63 6c75  update({self.clu
-00015060: 7374 6572 7363 6f72 655f 6b65 7920 3a20  sterscore_key : 
-00015070: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
-00015080: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015090: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000150a0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000150b0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-000150c0: 203a 2073 7472 2875 6e69 7175 655f 6964   : str(unique_id
-000150d0: 297d 290d 0a20 2020 2020 2020 2073 656c  )})..        sel
-000150e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000150f0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015100: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015110: 656c 662e 7472 6163 6b6c 6574 6964 5f6b  elf.trackletid_k
-00015120: 6579 203a 2073 7472 2874 7261 636b 6c65  ey : str(trackle
-00015130: 745f 6964 297d 2920 0d0a 2020 2020 2020  t_id)}) ..      
-00015140: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015150: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015160: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015170: 7465 287b 7365 6c66 2e67 656e 6572 6174  te({self.generat
-00015180: 696f 6e69 645f 6b65 7920 3a20 7374 7228  ionid_key : str(
-00015190: 6765 6e65 7261 7469 6f6e 5f69 6429 7d29  generation_id)})
-000151a0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-000151b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000151c0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000151d0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000151e0: 662e 7472 6163 6b69 645f 6b65 7920 3a20  f.trackid_key : 
-000151f0: 7374 7228 7472 6163 6b5f 6964 297d 290d  str(track_id)}).
-00015200: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00015210: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015220: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015230: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015240: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00015250: 203a 2030 2e30 7d29 0d0a 2020 2020 2020   : 0.0})..      
-00015260: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015270: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015280: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015290: 7465 287b 7365 6c66 2e73 7065 6564 5f6b  te({self.speed_k
-000152a0: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
-000152b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000152c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000152d0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000152e0: 6461 7465 287b 7365 6c66 2e61 6363 656c  date({self.accel
-000152f0: 6572 6174 696f 6e5f 6b65 7920 3a20 302e  eration_key : 0.
-00015300: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
-00015310: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015320: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015330: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015340: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00015350: 5f63 6f6d 705f 6669 7273 746b 6579 203a  _comp_firstkey :
-00015360: 204e 6f6e 657d 290d 0a20 2020 2020 2020   None})..       
-00015370: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015380: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015390: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000153a0: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
-000153b0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000153c0: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-000153d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000153e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000153f0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015400: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
-00015410: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
-00015420: 4e6f 6e65 7d29 0d0a 2020 2020 2020 2020  None})..        
-00015430: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015440: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015450: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015460: 287b 7365 6c66 2e63 656c 6c61 7869 735f  ({self.cellaxis_
-00015470: 6d61 736b 5f6b 6579 203a 204e 6f6e 657d  mask_key : None}
-00015480: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-00015490: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
-000154a0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000154b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000154c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000154d0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000154e0: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
-000154f0: 6569 645f 6b65 7920 3a20 696e 7428 736f  eid_key : int(so
-00015500: 7572 6365 5f69 6429 7d29 0d0a 2020 2020  urce_id)})..    
-00015510: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
-00015520: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-00015530: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015540: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015550: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015560: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
-00015570: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015580: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015590: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-000155a0: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-000155d0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000155e0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-000155f0: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00015600: 7369 645f 6b65 795d 2920 2d20 666c 6f61  sid_key]) - floa
-00015610: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015620: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015630: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
-00015640: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
-00015650: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00015660: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015670: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015680: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015690: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-000156a0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-000156b0: 202d 2020 666c 6f61 7428 7365 6c66 2e75   -  float(self.u
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013af0: 6674 746f 7461 6c5f 7361 6d70 6c65 203d  fttotal_sample =
+00013b00: 206e 702e 6162 7328 6666 7473 7472 6970   np.abs(fftstrip
+00013b10: 5f73 616d 706c 6529 0d0a 2020 2020 2020  _sample)..      
+00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b30: 2020 2020 2020 2020 2020 7866 5f73 616d            xf_sam
+00013b40: 706c 6520 3d20 7866 5f73 616d 706c 655b  ple = xf_sample[
+00013b50: 3020 3a20 6c65 6e28 7866 5f73 616d 706c  0 : len(xf_sampl
+00013b60: 6529 202f 2f20 325d 0d0a 2020 2020 2020  e) // 2]..      
+00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b80: 2020 2020 2020 2020 2020 6666 7474 6f74            ffttot
+00013b90: 616c 5f73 616d 706c 6520 3d20 6666 7474  al_sample = fftt
+00013ba0: 6f74 616c 5f73 616d 706c 655b 3020 3a20  otal_sample[0 : 
+00013bb0: 6c65 6e28 6666 7474 6f74 616c 5f73 616d  len(ffttotal_sam
+00013bc0: 706c 6529 202f 2f20 325d 0d0a 0d0a 2020  ple) // 2]....  
+00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013be0: 2075 6e69 7175 655f 6666 745f 7072 6f70   unique_fft_prop
+00013bf0: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013c00: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013c10: 645d 203d 2065 7870 616e 6465 645f 7469  d] = expanded_ti
+00013c20: 6d65 2c20 6578 7061 6e64 6564 5f69 6e74  me, expanded_int
+00013c30: 656e 7369 7479 2c20 7866 5f73 616d 706c  ensity, xf_sampl
+00013c40: 652c 2066 6674 746f 7461 6c5f 7361 6d70  e, ffttotal_samp
+00013c50: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
+00013c60: 2020 2020 2020 2075 6e69 7175 655f 636c         unique_cl
+00013c70: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013c80: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00013c90: 745f 756e 6971 7565 5f69 645d 203d 2020  t_unique_id] =  
+00013ca0: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
+00013cb0: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00013cc0: 6173 732c 2063 7572 7265 6e74 5f63 6c75  ass, current_clu
+00013cd0: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
+00013ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013cf0: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
+00013d00: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+00013d10: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00013d20: 6971 7565 5f69 645d 203d 2063 7572 7265  ique_id] = curre
+00013d30: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
+00013d40: 5f7a 2c20 6375 7272 656e 745f 792c 2063  _z, current_y, c
+00013d50: 7572 7265 6e74 5f78 2c20 6375 7272 656e  urrent_x, curren
+00013d60: 745f 7261 6469 7573 2c20 6375 7272 656e  t_radius, curren
+00013d70: 745f 766f 6c75 6d65 2c20 6375 7272 656e  t_volume, curren
+00013d80: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00013d90: 6f6d 705f 6669 7273 742c 2063 7572 7265  omp_first, curre
+00013da0: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00013db0: 636f 6d70 5f73 6563 6f6e 642c 2063 7572  comp_second, cur
+00013dc0: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013dd0: 612c 2063 7572 7265 6e74 5f63 6c75 7374  a, current_clust
+00013de0: 6572 5f63 6c61 7373 2c20 6375 7272 656e  er_class, curren
+00013df0: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013e00: 7363 6f72 650d 0a20 2020 2020 2020 2020  score..         
+00013e10: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013e20: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+00013e30: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00013e40: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+00013e50: 3d20 6375 7272 656e 745f 7469 6d65 2c20  = current_time, 
+00013e60: 6375 7272 656e 745f 7370 6565 642c 2063  current_speed, c
+00013e70: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
+00013e80: 676c 652c 2063 7572 7265 6e74 5f61 6363  gle, current_acc
+00013e90: 656c 6572 6174 696f 6e2c 2063 7572 7265  eleration, curre
+00013ea0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+00013eb0: 5f6d 6173 6b2c 2063 7572 7265 6e74 5f72  _mask, current_r
+00013ec0: 6164 6961 6c5f 616e 676c 652c 2063 7572  adial_angle, cur
+00013ed0: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+00013ee0: 6173 6b0d 0a20 2020 2020 2020 2020 2020  ask..           
+00013ef0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00013f00: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+00013f10: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+00013f20: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+00013f30: 7175 655f 6964 3a75 6e69 7175 655f 6666  que_id:unique_ff
+00013f40: 745f 7072 6f70 6572 7469 6573 5f74 7261  t_properties_tra
+00013f50: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00013f60: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013f80: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00013f90: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
+00013fa0: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+00013fb0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013fc0: 643a 756e 6971 7565 5f63 6c75 7374 6572  d:unique_cluster
+00013fd0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013fe0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013ff0: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+00014020: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
+00014030: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+00014040: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00014050: 3a75 6e69 7175 655f 7368 6170 655f 7072  :unique_shape_pr
+00014060: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00014070: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00014080: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
+00014090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000140a0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
+000140b0: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+000140c0: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
+000140d0: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
+000140e0: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+000140f0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00014100: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+00014110: 6964 5d7d 290d 0a0d 0a20 2020 2064 6566  id]})....    def
+00014120: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
+00014130: 5f73 706f 7473 2873 656c 662c 2066 7261  _spots(self, fra
+00014140: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
+00014150: 6c5f 6964 2c20 7472 6163 6b5f 6964 293a  l_id, track_id):
+00014160: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+00014170: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
+00014180: 2063 656e 7472 6f69 6473 2c20 6c61 6265   centroids, labe
+00014190: 6c73 2c20 766f 6c75 6d65 2c20 696e 7465  ls, volume, inte
+000141a0: 6e73 6974 795f 6d65 616e 2c20 696e 7465  nsity_mean, inte
+000141b0: 6e73 6974 795f 746f 7461 6c2c 2062 6f75  nsity_total, bou
+000141c0: 6e64 696e 675f 626f 7865 7320 3d20 7365  nding_boxes = se
+000141d0: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
+000141e0: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
+000141f0: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
+00014200: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
+00014210: 2070 6978 656c 7465 7374 6c6f 6361 7469   pixeltestlocati
+00014220: 6f6e 203d 2028 7a2c 792c 7829 0d0a 2020  on = (z,y,x)..  
+00014230: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
+00014240: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+00014250: 7279 2870 6978 656c 7465 7374 6c6f 6361  ry(pixeltestloca
+00014260: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
+00014270: 2020 2020 2020 2062 626f 7820 3d20 626f         bbox = bo
+00014280: 756e 6469 6e67 5f62 6f78 6573 5b69 6e64  unding_boxes[ind
+00014290: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+000142a0: 2073 697a 657a 203d 2061 6273 2862 626f   sizez = abs(bbo
+000142b0: 785b 305d 202d 2062 626f 785b 335d 290d  x[0] - bbox[3]).
+000142c0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+000142d0: 6579 203d 2061 6273 2862 626f 785b 315d  ey = abs(bbox[1]
+000142e0: 202d 2062 626f 785b 345d 290d 0a20 2020   - bbox[4])..   
+000142f0: 2020 2020 2020 2020 2073 697a 6578 203d           sizex =
+00014300: 2061 6273 2862 626f 785b 325d 202d 2062   abs(bbox[2] - b
+00014310: 626f 785b 355d 2920 0d0a 2020 2020 2020  box[5]) ..      
+00014320: 2020 2020 2020 7665 746f 5f76 6f6c 756d        veto_volum
+00014330: 6520 3d20 7369 7a65 7820 2a20 7369 7a65  e = sizex * size
+00014340: 7920 2a20 7369 7a65 7a0d 0a20 2020 2020  y * sizez..     
+00014350: 2020 2020 2020 2076 6574 6f5f 7261 6469         veto_radi
+00014360: 7573 203d 206d 6174 682e 706f 7728 3320  us = math.pow(3 
+00014370: 2a20 7665 746f 5f76 6f6c 756d 6520 2f20  * veto_volume / 
+00014380: 2834 202a 206d 6174 682e 7069 292c 2031  (4 * math.pi), 1
+00014390: 2e30 202f 2033 2e30 290d 0a0d 0a20 2020  .0 / 3.0)....   
+000143a0: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+000143b0: 6e20 3d20 2863 656e 7472 6f69 6473 5b69  n = (centroids[i
+000143c0: 6e64 6578 5d5b 305d 202a 2073 656c 662e  ndex][0] * self.
+000143d0: 7a63 616c 6962 7261 7469 6f6e 2c20 6365  zcalibration, ce
+000143e0: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
+000143f0: 5d2a 7365 6c66 2e79 6361 6c69 6272 6174  ]*self.ycalibrat
+00014400: 696f 6e2c 2063 656e 7472 6f69 6473 5b69  ion, centroids[i
+00014410: 6e64 6578 5d5b 325d 2a73 656c 662e 7863  ndex][2]*self.xc
+00014420: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+00014430: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
+00014440: 203d 2076 6f6c 756d 655b 696e 6465 785d   = volume[index]
+00014450: 0d0a 2020 2020 2020 2020 2020 2020 5241  ..            RA
+00014460: 4449 5553 203d 206d 6174 682e 706f 7728  DIUS = math.pow(
+00014470: 5155 414c 4954 5920 2a20 7365 6c66 2e78  QUALITY * self.x
+00014480: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
+00014490: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
+000144a0: 2a20 7365 6c66 2e7a 6361 6c69 6272 6174  * self.zcalibrat
+000144b0: 696f 6e2c 2031 2e30 2f33 2e30 2920 0d0a  ion, 1.0/3.0) ..
+000144c0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+000144d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000144e0: 2c20 6d61 736b 6365 6e74 726f 6964 203d  , maskcentroid =
+000144f0: 2073 656c 662e 5f67 6574 5f62 6f75 6e64   self._get_bound
+00014500: 6172 795f 6469 7374 2866 7261 6d65 2c20  ary_dist(frame, 
+00014510: 6c6f 6361 7469 6f6e 290d 0a20 2020 2020  location)..     
+00014520: 2020 2020 2020 2069 6620 6469 7374 203c         if dist <
+00014530: 3d20 3220 2a20 7665 746f 5f72 6164 6975  = 2 * veto_radiu
+00014540: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00014550: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00014560: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00014570: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00014580: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00014590: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000145a0: 6c66 2e63 656c 6c69 645f 6b65 793a 2069  lf.cellid_key: i
+000145b0: 6e74 2863 656c 6c5f 6964 292c 200d 0a20  nt(cell_id), .. 
+000145c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145d0: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+000145e0: 6569 645f 6b65 7920 3a20 696e 7428 6672  eid_key : int(fr
+000145f0: 616d 6529 2c0d 0a20 2020 2020 2020 2020  ame),..         
+00014600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014610: 656c 662e 7a70 6f73 6964 5f6b 6579 203a  elf.zposid_key :
+00014620: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
+00014630: 5b69 6e64 6578 5d5b 305d 2a20 7365 6c66  [index][0]* self
+00014640: 2e7a 6361 6c69 6272 6174 696f 6e29 2c0d  .zcalibration),.
+00014650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014660: 2020 2020 2020 2020 2073 656c 662e 7970           self.yp
+00014670: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
+00014680: 2863 656e 7472 6f69 6473 5b69 6e64 6578  (centroids[index
+00014690: 5d5b 315d 2a20 7365 6c66 2e79 6361 6c69  ][1]* self.ycali
+000146a0: 6272 6174 696f 6e29 2c0d 0a20 2020 2020  bration),..     
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+000146d0: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
+000146e0: 6f69 6473 5b69 6e64 6578 5d5b 325d 2a20  oids[index][2]* 
+000146f0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00014700: 6e29 2c0d 0a20 2020 2020 2020 2020 2020  n),..           
+00014710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014720: 662e 7472 6163 6b69 645f 6b65 793a 2069  f.trackid_key: i
+00014730: 6e74 2874 7261 636b 5f69 6429 2c0d 0a20  nt(track_id),.. 
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00014760: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
+00014770: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
+00014780: 7479 5f74 6f74 616c 5b69 6e64 6578 5d29  ty_total[index])
+00014790: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000147a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000147b0: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+000147c0: 6b65 7920 3a20 2866 6c6f 6174 2869 6e74  key : (float(int
+000147d0: 656e 7369 7479 5f6d 6561 6e5b 696e 6465  ensity_mean[inde
+000147e0: 785d 2929 2c0d 0a0d 0a20 2020 2020 2020  x])),....       
+000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014800: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
+00014810: 203a 2028 666c 6f61 7428 5241 4449 5553   : (float(RADIUS
+00014820: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+00014830: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014840: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+00014850: 2866 6c6f 6174 2851 5541 4c49 5459 2929  (float(QUALITY))
+00014860: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014880: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00014890: 736b 5f6b 6579 3a20 666c 6f61 7428 6469  sk_key: float(di
+000148a0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000148b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000148c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000148d0: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
+000148e0: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+000148f0: 656e 7472 6f69 645b 305d 292c 0d0a 2020  entroid[0]),..  
+00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014910: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
+00014920: 656e 7472 6f69 645f 795f 6b65 793a 2066  entroid_y_key: f
+00014930: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
+00014940: 645b 315d 292c 0d0a 2020 2020 2020 2020  d[1]),..        
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00014970: 645f 785f 6b65 793a 2066 6c6f 6174 286d  d_x_key: float(m
+00014980: 6173 6b63 656e 7472 6f69 645b 325d 2920  askcentroid[2]) 
+00014990: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000149a0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
+000149b0: 2020 2065 6c69 6620 6365 6c6c 5f69 6420     elif cell_id 
+000149c0: 696e 2073 656c 662e 6564 6765 5f73 6f75  in self.edge_sou
+000149d0: 7263 655f 6c6f 6f6b 7570 2e6b 6579 7328  rce_lookup.keys(
+000149e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000149f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00014a00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014a10: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00014a20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014a30: 735b 6365 6c6c 5f69 645d 203d 2073 656c  s[cell_id] = sel
+00014a40: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014a50: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00014a60: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00014a70: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00014a80: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00014a90: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00014aa0: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
+00014ab0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+00014ac0: 7479 5f6b 6579 3a20 4e6f 6e65 7d29 0d0a  ty_key: None})..
+00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ae0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00014af0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00014b00: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00014b10: 2e75 7064 6174 6528 7b73 656c 662e 6d65  .update({self.me
+00014b20: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+00014b30: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
+00014b40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014b50: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00014b60: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014b70: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
+00014b80: 6528 7b73 656c 662e 7261 6469 7573 5f6b  e({self.radius_k
+00014b90: 6579 3a20 4e6f 6e65 7d29 0d0a 2020 2020  ey: None})..    
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+00014bc0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014bd0: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
+00014be0: 6174 6528 7b73 656c 662e 7175 616c 6974  ate({self.qualit
+00014bf0: 795f 6b65 793a 204e 6f6e 657d 290d 0a0d  y_key: None})...
+00014c00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00014c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c20: 2020 2020 0d0a 2020 2020 6465 6620 5f64      ..    def _d
+00014c30: 6963 745f 7570 6461 7465 2873 656c 662c  ict_update(self,
+00014c40: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
+00014c50: 5f69 6473 3a20 4c69 7374 2c20 2063 656c  _ids: List,  cel
+00014c60: 6c5f 6964 3a20 696e 742c 2074 7261 636b  l_id: int, track
+00014c70: 5f69 643a 2069 6e74 2c20 736f 7572 6365  _id: int, source
+00014c80: 5f69 643a 2069 6e74 2c20 7461 7267 6574  _id: int, target
+00014c90: 5f69 643a 2069 6e74 293a 0d0a 0d0a 200d  _id: int):.... .
+00014ca0: 0a20 2020 2020 2020 2067 656e 6572 6174  .        generat
+00014cb0: 696f 6e5f 6964 203d 2073 656c 662e 6765  ion_id = self.ge
+00014cc0: 6e65 7261 7469 6f6e 5f64 6963 745b 6365  neration_dict[ce
+00014cd0: 6c6c 5f69 645d 0d0a 2020 2020 2020 2020  ll_id]..        
+00014ce0: 7472 6163 6b6c 6574 5f69 6420 3d20 7365  tracklet_id = se
+00014cf0: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00014d00: 5b63 656c 6c5f 6964 5d0d 0a0d 0a20 2020  [cell_id]....   
+00014d10: 2020 2020 2075 6e69 7175 655f 6964 203d       unique_id =
+00014d20: 2073 7472 2874 7261 636b 5f69 6429 202b   str(track_id) +
+00014d30: 2073 7472 2873 656c 662e 6d61 785f 7472   str(self.max_tr
+00014d40: 6163 6b5f 6964 2920 2b20 7374 7228 6765  ack_id) + str(ge
+00014d50: 6e65 7261 7469 6f6e 5f69 6429 202b 2073  neration_id) + s
+00014d60: 7472 2874 7261 636b 6c65 745f 6964 290d  tr(tracklet_id).
+00014d70: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00014d80: 2020 2076 6563 5f6d 6173 6b20 3d20 5b66     vec_mask = [f
+00014d90: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014da0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014db0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014dc0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00014dd0: 5f78 5f6b 6579 5d29 2c20 666c 6f61 7428  _x_key]), float(
+00014de0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014df0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014e00: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00014e10: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
+00014e20: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00014e30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014e40: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014e50: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+00014e60: 6e74 726f 6964 5f7a 5f6b 6579 5d29 205d  ntroid_z_key]) ]
+00014e70: 0d0a 0d0a 2020 2020 2020 2020 7665 635f  ....        vec_
+00014e80: 6365 6c6c 203d 205b 666c 6f61 7428 7365  cell = [float(se
+00014e90: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014ea0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014eb0: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
+00014ec0: 7369 645f 6b65 795d 2920 2c20 0d0a 2020  sid_key]) , ..  
+00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ee0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00014ef0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014f00: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014f10: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00014f20: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00014f50: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014f60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014f70: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014f80: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a0d  zposid_key])]...
+00014f90: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+00014fa0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+00014fb0: 7665 635f 6d61 736b 2c20 7665 635f 6365  vec_mask, vec_ce
+00014fc0: 6c6c 290d 0a0d 0a20 2020 2020 2020 2073  ll)....        s
+00014fd0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014fe0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014ff0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015000: 7b73 656c 662e 7261 6469 616c 5f61 6e67  {self.radial_ang
+00015010: 6c65 5f6b 6579 203a 2061 6e67 6c65 7d29  le_key : angle})
+00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015030: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00015040: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+00015050: 6964 732e 6170 7065 6e64 2873 7472 2875  ids.append(str(u
+00015060: 6e69 7175 655f 6964 2929 0d0a 2020 2020  nique_id))..    
+00015070: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015080: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015090: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000150a0: 6461 7465 287b 7365 6c66 2e63 6c75 7374  date({self.clust
+000150b0: 6572 636c 6173 735f 6b65 7920 3a20 4e6f  erclass_key : No
+000150c0: 6e65 7d29 0d0a 2020 2020 2020 2020 7365  ne})..        se
+000150d0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000150e0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000150f0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015100: 7365 6c66 2e63 6c75 7374 6572 7363 6f72  self.clusterscor
+00015110: 655f 6b65 7920 3a20 307d 290d 0a20 2020  e_key : 0})..   
+00015120: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015130: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015140: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015150: 7064 6174 6528 7b73 656c 662e 756e 6971  pdate({self.uniq
+00015160: 7565 6964 5f6b 6579 203a 2073 7472 2875  ueid_key : str(u
+00015170: 6e69 7175 655f 6964 297d 290d 0a20 2020  nique_id)})..   
+00015180: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015190: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000151a0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000151b0: 7064 6174 6528 7b73 656c 662e 7472 6163  pdate({self.trac
+000151c0: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+000151d0: 2874 7261 636b 6c65 745f 6964 297d 2920  (tracklet_id)}) 
+000151e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000151f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015200: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015210: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015220: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+00015230: 7920 3a20 7374 7228 6765 6e65 7261 7469  y : str(generati
+00015240: 6f6e 5f69 6429 7d29 200d 0a20 2020 2020  on_id)}) ..     
+00015250: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015260: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015270: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015280: 6174 6528 7b73 656c 662e 7472 6163 6b69  ate({self.tracki
+00015290: 645f 6b65 7920 3a20 7374 7228 7472 6163  d_key : str(trac
+000152a0: 6b5f 6964 297d 290d 0a20 2020 2020 2020  k_id)})..       
+000152b0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000152c0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000152d0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+000152e0: 6528 7b73 656c 662e 6d6f 7469 6f6e 5f61  e({self.motion_a
+000152f0: 6e67 6c65 5f6b 6579 203a 2030 2e30 7d29  ngle_key : 0.0})
+00015300: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00015310: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015320: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015330: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015340: 2e73 7065 6564 5f6b 6579 203a 2030 2e30  .speed_key : 0.0
+00015350: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015360: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015370: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015380: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015390: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+000153a0: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
+000153b0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000153c0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000153d0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000153e0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+000153f0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00015400: 7273 746b 6579 203a 204e 6f6e 657d 290d  rstkey : None}).
+00015410: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015420: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015430: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015440: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015450: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00015460: 705f 7365 636f 6e64 6b65 7920 3a20 4e6f  p_secondkey : No
+00015470: 6e65 7d29 0d0a 2020 2020 2020 2020 7365  ne})..        se
+00015480: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015490: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000154a0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000154b0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+000154c0: 615f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  a_key : None})..
+000154d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000154e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000154f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015500: 5d2e 7570 6461 7465 287b 7365 6c66 2e63  ].update({self.c
+00015510: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+00015520: 203a 204e 6f6e 657d 290d 0a0d 0a20 2020   : None})....   
+00015530: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
+00015540: 6420 6973 206e 6f74 204e 6f6e 653a 0d0a  d is not None:..
+00015550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015560: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015570: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015580: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015590: 6c66 2e62 6566 6f72 6569 645f 6b65 7920  lf.beforeid_key 
+000155a0: 3a20 696e 7428 736f 7572 6365 5f69 6429  : int(source_id)
+000155b0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000155c0: 7665 635f 3120 3d20 5b66 6c6f 6174 2873  vec_1 = [float(s
+000155d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000155e0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000155f0: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
+00015600: 6f73 6964 5f6b 6579 5d29 202d 2066 6c6f  osid_key]) - flo
+00015610: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015620: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015630: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+00015640: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00015650: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00015660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015670: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015680: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015690: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+000156a0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+000156b0: 2920 2d20 666c 6f61 7428 7365 6c66 2e75  ) - float(self.u
 000156c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
 000156d0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-000156e0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-000156f0: 645f 6b65 795d 295d 0d0a 2020 2020 2020  d_key])]..      
-00015700: 2020 2020 2020 7370 6565 6420 3d20 6e70        speed = np
-00015710: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
-00015720: 5f31 2c20 7665 635f 3129 292f 7365 6c66  _1, vec_1))/self
-00015730: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
-00015740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015750: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015760: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015770: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015780: 662e 7370 6565 645f 6b65 7920 3a20 7370  f.speed_key : sp
-00015790: 6565 647d 290d 0a0d 0a20 2020 2020 2020  eed})....       
-000157a0: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
-000157b0: 6520 3d20 616e 6775 6c61 725f 6368 616e  e = angular_chan
-000157c0: 6765 2876 6563 5f6d 6173 6b2c 2076 6563  ge(vec_mask, vec
-000157d0: 5f31 290d 0a0d 0a20 2020 2020 2020 2020  _1)....         
-000157e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000157f0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015800: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015810: 6174 6528 7b73 656c 662e 6d6f 7469 6f6e  ate({self.motion
-00015820: 5f61 6e67 6c65 5f6b 6579 203a 206d 6f74  _angle_key : mot
-00015830: 696f 6e5f 616e 676c 657d 2920 0d0a 0d0a  ion_angle}) ....
-00015840: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00015850: 6f75 7263 655f 6964 2069 6e20 7365 6c66  ource_id in self
-00015860: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
-00015870: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00015880: 2020 2020 2020 2020 2020 7072 655f 736f            pre_so
-00015890: 7572 6365 5f69 6420 3d20 7365 6c66 2e65  urce_id = self.e
-000158a0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-000158b0: 705b 736f 7572 6365 5f69 645d 0d0a 2020  p[source_id]..  
-000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000158e0: 2020 2020 2020 2020 7665 635f 3220 3d20          vec_2 = 
-000158f0: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-00015900: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015910: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015920: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015930: 5d29 202d 2032 202a 2066 6c6f 6174 2873  ]) - 2 * float(s
-00015940: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015950: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
-00015960: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00015970: 7870 6f73 6964 5f6b 6579 5d29 202b 2066  xposid_key]) + f
-00015980: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015990: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000159a0: 5b69 6e74 2870 7265 5f73 6f75 7263 655f  [int(pre_source_
-000159b0: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-000159c0: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
-000159f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015a00: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015a10: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00015a20: 645f 6b65 795d 2920 2d20 3220 2a20 666c  d_key]) - 2 * fl
-00015a30: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00015a40: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015a50: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00015a60: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00015a70: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
-00015a80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015a90: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
-00015aa0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
-00015ab0: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ad0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00015ae0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015af0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015b00: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015b10: 7a70 6f73 6964 5f6b 6579 5d29 202d 2020  zposid_key]) -  
-00015b20: 3220 2a20 666c 6f61 7428 7365 6c66 2e75  2 * float(self.u
-00015b30: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015b40: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-00015b50: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00015b60: 645f 6b65 795d 2920 2b20 666c 6f61 7428  d_key]) + float(
-00015b70: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015b80: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015b90: 7072 655f 736f 7572 6365 5f69 6429 5d5b  pre_source_id)][
-00015ba0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-00015bb0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00015bc0: 2020 2020 2020 2020 6163 6320 3d20 6e70          acc = np
-00015bd0: 2e73 7172 7428 6e70 2e64 6f74 2876 6563  .sqrt(np.dot(vec
-00015be0: 5f32 2c20 7665 635f 3229 292f 7365 6c66  _2, vec_2))/self
-00015bf0: 2e74 6361 6c69 6272 6174 696f 6e0d 0a20  .tcalibration.. 
-00015c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015c20: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00015c30: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015c40: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015c50: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015c60: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00015c70: 203a 2061 6363 7d29 0d0a 2020 2020 2020   : acc})..      
-00015c80: 2020 656c 6966 2073 6f75 7263 655f 6964    elif source_id
-00015c90: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00015ca0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015cb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015cc0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015cd0: 2e75 7064 6174 6528 7b73 656c 662e 6265  .update({self.be
-00015ce0: 666f 7265 6964 5f6b 6579 203a 204e 6f6e  foreid_key : Non
-00015cf0: 657d 2920 0d0a 2020 2020 2020 2020 2020  e}) ..          
-00015d00: 2020 0d0a 0d0a 2020 2020 2020 2020 6966    ....        if
-00015d10: 2074 6172 6765 745f 6964 2069 7320 6e6f   target_id is no
-00015d20: 7420 4e6f 6e65 3a20 2020 2020 2020 0d0a  t None:       ..
-00015d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015d40: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015d50: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015d60: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015d70: 6c66 2e61 6674 6572 6964 5f6b 6579 203a  lf.afterid_key :
-00015d80: 2069 6e74 2874 6172 6765 745f 6964 297d   int(target_id)}
-00015d90: 2920 0d0a 2020 2020 2020 2020 656c 6966  ) ..        elif
-00015da0: 2074 6172 6765 745f 6964 2069 7320 4e6f   target_id is No
-00015db0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00015dc0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015dd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015de0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015df0: 6528 7b73 656c 662e 6166 7465 7269 645f  e({self.afterid_
-00015e00: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-00015e10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00015e20: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
-00015e30: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
-00015e40: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
-00015e50: 6429 2020 2020 0d0a 0d0a 0d0a 2020 2020  d)    ......    
-00015e60: 6465 6620 5f74 656d 706f 7261 6c5f 706c  def _temporal_pl
-00015e70: 6f74 735f 7472 6163 6b6d 6174 6528 7365  ots_trackmate(se
-00015e80: 6c66 293a 0d0a 2020 2020 0d0a 2020 2020  lf):..    ..    
-00015e90: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00015ea0: 2020 2020 2020 2020 7365 6c66 2e41 7474          self.Att
-00015eb0: 7220 3d20 7b7d 0d0a 2020 2020 2020 2020  r = {}..        
-00015ec0: 2020 2020 2020 2020 7374 6172 7474 696d          starttim
-00015ed0: 6520 3d20 696e 7428 6d69 6e28 7365 6c66  e = int(min(self
-00015ee0: 2e41 6c6c 5661 6c75 6573 5b73 656c 662e  .AllValues[self.
-00015ef0: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
-00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f10: 656e 6474 696d 6520 3d20 696e 7428 6d61  endtime = int(ma
-00015f20: 7828 7365 6c66 2e41 6c6c 5661 6c75 6573  x(self.AllValues
-00015f30: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
-00015f40: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
-00015f50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015f60: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00015f70: 6d65 203d 205b 5d0d 0a20 2020 2020 2020  me = []..       
-00015f80: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015f90: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015fa0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015fb0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015fc0: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
-00015fd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00015fe0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015ff0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-00016000: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016010: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016020: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-00016030: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016040: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016050: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
-00016060: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016070: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016080: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
-00016090: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000160a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000160b0: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
-000160c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000160d0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000160e0: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-000160f0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016100: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016110: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
-00016120: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016130: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00016140: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
-00016150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016160: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00016170: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00016180: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016190: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
-000161a0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-000161b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000161c0: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
-000161d0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000161e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000161f0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016200: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-00016210: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00016220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016230: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00016240: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00016250: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00016260: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016270: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00016280: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00016290: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000162a0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000162b0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000162c0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-000162d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000162e0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000162f0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-00016300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016310: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016320: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
-00016330: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016340: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016350: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-00016360: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016370: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016380: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00016390: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-000163a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000163b0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-000163c0: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
-000163d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000163e0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-000163f0: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
-00016400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016410: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00016420: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-00016430: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016440: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00016450: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00016460: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016470: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016480: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00016490: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-000164a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000164b0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000164c0: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
-000164d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000164e0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
-000164f0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-00016500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016510: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016520: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016530: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016540: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016550: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00016560: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016570: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00016580: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016590: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000165a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000165b0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-000165c0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000165d0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000165e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000165f0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016600: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00016610: 6c5f 6d65 616e 5f64 6973 705f 7a20 3d20  l_mean_disp_z = 
-00016620: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016630: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016640: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-00016650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016660: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00016670: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016690: 616c 6c5f 7661 725f 6469 7370 5f79 203d  all_var_disp_y =
-000166a0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000166b0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000166c0: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
-000166d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000166e0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-000166f0: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
-00016700: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016710: 6c66 2e61 6c6c 5f6d 6561 6e5f 7261 6469  lf.all_mean_radi
-00016720: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016730: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00016740: 6c5f 7661 725f 7261 6469 7573 203d 205b  l_var_radius = [
-00016750: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016760: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00016770: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
-00016780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016790: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
-000167a0: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-000167b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000167c0: 6c6c 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ll_mean_acc = []
-000167d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000167e0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f61    self.all_var_a
-000167f0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-00016800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016810: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
-00016820: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00016830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016840: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00016850: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016860: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00016870: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016880: 6c6c 5f6d 6561 6e5f 6469 7374 616e 6365  ll_mean_distance
-00016890: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-000168a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168b0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-000168c0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000168d0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000168e0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000168f0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00016900: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016910: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016920: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
-00016930: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
-00016940: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016950: 656c 662e 616c 6c5f 636c 7573 7465 725f  elf.all_cluster_
-00016960: 636c 6173 7320 3d20 5b5d 0d0a 0d0a 2020  class = []....  
-00016970: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016980: 6c5f 7370 6f74 735f 7472 6163 6b73 203d  l_spots_tracks =
-00016990: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-000169a0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-000169b0: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
-000169c0: 6f74 5f70 726f 7065 7274 6965 732e 6974  ot_properties.it
-000169d0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-000169e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 2020 2020 616c 6c5f 7370 6f74 7320        all_spots 
-00016a10: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00016a20: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-00016a30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016a50: 7472 6163 6b69 645f 6b65 7920 696e 2061  trackid_key in a
-00016a60: 6c6c 5f73 706f 7473 3a0d 0a20 2020 2020  ll_spots:..     
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
-00016a90: 7261 636b 735b 6b5d 203d 2061 6c6c 5f73  racks[k] = all_s
-00016aa0: 706f 7473 0d0a 2020 2020 2020 2020 2020  pots..          
-00016ab0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00016ac0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00016ad0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-00016ae0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
-00016af0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-00016b00: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-00016b10: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
-00016b20: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
-00016b30: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-00016b40: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
-00016b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016b70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00016b80: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
-00016b90: 2873 7461 7274 7469 6d65 2c20 656e 6474  (starttime, endt
-00016ba0: 696d 6529 2c20 746f 7461 6c3d 656e 6474  ime), total=endt
-00016bb0: 696d 6520 2d20 7374 6172 7474 696d 6529  ime - starttime)
-00016bc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016bd0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-00016c00: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-00016c10: 7428 7365 6c66 2e5f 636f 6d70 7574 655f  t(self._compute_
-00016c20: 7465 6d70 6f72 616c 2c20 692c 2061 6c6c  temporal, i, all
-00016c30: 5f73 706f 7473 5f74 7261 636b 7329 290d  _spots_tracks)).
-00016c40: 0a20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00016c50: 2020 2020 2020 2020 5b72 2e72 6573 756c          [r.resul
-00016c60: 7428 2920 666f 7220 7220 696e 2063 6f6e  t() for r in con
-00016c70: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00016c80: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-00016c90: 7572 6573 295d 0d0a 0d0a 0d0a 2020 2020  ures)]......    
-00016ca0: 6465 6620 5f63 6f6d 7075 7465 5f74 656d  def _compute_tem
-00016cb0: 706f 7261 6c28 7365 6c66 2c20 692c 2061  poral(self, i, a
-00016cc0: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
-00016cd0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00016ce0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016cf0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016d00: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00016d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d20: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
-00016d30: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016d40: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016d50: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d70: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-00016d80: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016d90: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016da0: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2020 206d 6974 6f74 6963 5f61 6363 203d     mitotic_acc =
-00016dd0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016de0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016df0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016e00: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016e10: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016e20: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00016e30: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016e40: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016e50: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00016e60: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-00016e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e80: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016e90: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00016ec0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016ee0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00016ef0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00016f00: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00016f10: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
-00016f20: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016f30: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016f40: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
-00016f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f60: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016f70: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016f80: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016f90: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00016fa0: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016fb0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016fc0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016fd0: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
-00016fe0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00016ff0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00017000: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00017010: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00017020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017030: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017040: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017050: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+000156e0: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
+000156f0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
+00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015710: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00015720: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015730: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015740: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
+00015750: 6964 5f6b 6579 5d29 202d 2020 666c 6f61  id_key]) -  floa
+00015760: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015770: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015780: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+00015790: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
+000157a0: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+000157b0: 6565 6420 3d20 6e70 2e73 7172 7428 6e70  eed = np.sqrt(np
+000157c0: 2e64 6f74 2876 6563 5f31 2c20 7665 635f  .dot(vec_1, vec_
+000157d0: 3129 292f 7365 6c66 2e74 6361 6c69 6272  1))/self.tcalibr
+000157e0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000157f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015800: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015810: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015820: 6174 6528 7b73 656c 662e 7370 6565 645f  ate({self.speed_
+00015830: 6b65 7920 3a20 7370 6565 647d 290d 0a0d  key : speed})...
+00015840: 0a20 2020 2020 2020 2020 2020 206d 6f74  .            mot
+00015850: 696f 6e5f 616e 676c 6520 3d20 616e 6775  ion_angle = angu
+00015860: 6c61 725f 6368 616e 6765 2876 6563 5f6d  lar_change(vec_m
+00015870: 6173 6b2c 2076 6563 5f31 290d 0a0d 0a20  ask, vec_1).... 
+00015880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015890: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000158a0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000158b0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000158c0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+000158d0: 6579 203a 206d 6f74 696f 6e5f 616e 676c  ey : motion_angl
+000158e0: 657d 2920 0d0a 0d0a 2020 2020 2020 2020  e}) ....        
+000158f0: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
+00015900: 2069 6e20 7365 6c66 2e65 6467 655f 736f   in self.edge_so
+00015910: 7572 6365 5f6c 6f6f 6b75 703a 0d0a 2020  urce_lookup:..  
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 2020 7072 655f 736f 7572 6365 5f69 6420    pre_source_id 
+00015940: 3d20 7365 6c66 2e65 6467 655f 736f 7572  = self.edge_sour
+00015950: 6365 5f6c 6f6f 6b75 705b 736f 7572 6365  ce_lookup[source
+00015960: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
+00015970: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00015980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015990: 7665 635f 3220 3d20 5b66 6c6f 6174 2873  vec_2 = [float(s
+000159a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000159b0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000159c0: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
+000159d0: 6f73 6964 5f6b 6579 5d29 202d 2032 202a  osid_key]) - 2 *
+000159e0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+000159f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015a00: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00015a10: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00015a20: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+00015a30: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015a40: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+00015a50: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+00015a60: 662e 7870 6f73 6964 5f6b 6579 5d29 2c20  f.xposid_key]), 
+00015a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015a80: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00015a90: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00015aa0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015ab0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00015ac0: 6c66 2e79 706f 7369 645f 6b65 795d 2920  lf.yposid_key]) 
+00015ad0: 2d20 3220 2a20 666c 6f61 7428 7365 6c66  - 2 * float(self
+00015ae0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015af0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00015b00: 6365 5f69 6429 5d5b 7365 6c66 2e79 706f  ce_id)][self.ypo
+00015b10: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+00015b20: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015b30: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015b40: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00015b50: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00015b60: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+00015b90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015ba0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015bb0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00015bc0: 6579 5d29 202d 2020 3220 2a20 666c 6f61  ey]) -  2 * floa
+00015bd0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015be0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015bf0: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+00015c00: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
+00015c10: 2b20 666c 6f61 7428 7365 6c66 2e75 6e69  + float(self.uni
+00015c20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015c30: 6965 735b 696e 7428 7072 655f 736f 7572  ies[int(pre_sour
+00015c40: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
+00015c50: 7369 645f 6b65 795d 295d 0d0a 2020 2020  sid_key])]..    
+00015c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c70: 6163 6320 3d20 6e70 2e73 7172 7428 6e70  acc = np.sqrt(np
+00015c80: 2e64 6f74 2876 6563 5f32 2c20 7665 635f  .dot(vec_2, vec_
+00015c90: 3229 292f 7365 6c66 2e74 6361 6c69 6272  2))/self.tcalibr
+00015ca0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00015cb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cd0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00015ce0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015cf0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00015d00: 6528 7b73 656c 662e 6163 6365 6c65 7261  e({self.accelera
+00015d10: 7469 6f6e 5f6b 6579 203a 2061 6363 7d29  tion_key : acc})
+00015d20: 0d0a 2020 2020 2020 2020 656c 6966 2073  ..        elif s
+00015d30: 6f75 7263 655f 6964 2069 7320 4e6f 6e65  ource_id is None
+00015d40: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00015d50: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015d60: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015d70: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015d80: 7b73 656c 662e 6265 666f 7265 6964 5f6b  {self.beforeid_k
+00015d90: 6579 203a 204e 6f6e 657d 2920 0d0a 2020  ey : None}) ..  
+00015da0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00015db0: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
+00015dc0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a20  id is not None: 
+00015dd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00015de0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015df0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015e00: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015e10: 6461 7465 287b 7365 6c66 2e61 6674 6572  date({self.after
+00015e20: 6964 5f6b 6579 203a 2069 6e74 2874 6172  id_key : int(tar
+00015e30: 6765 745f 6964 297d 2920 0d0a 2020 2020  get_id)}) ..    
+00015e40: 2020 2020 656c 6966 2074 6172 6765 745f      elif target_
+00015e50: 6964 2069 7320 4e6f 6e65 3a0d 0a20 2020  id is None:..   
+00015e60: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015e70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015e80: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015e90: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015ea0: 6166 7465 7269 645f 6b65 7920 3a20 4e6f  afterid_key : No
+00015eb0: 6e65 7d29 0d0a 2020 2020 2020 2020 2020  ne})..          
+00015ec0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00015ed0: 2e5f 7365 636f 6e64 5f63 6861 6e6e 656c  ._second_channel
+00015ee0: 5f75 7064 6174 6528 6365 6c6c 5f69 642c  _update(cell_id,
+00015ef0: 2074 7261 636b 5f69 6429 2020 2020 0d0a   track_id)    ..
+00015f00: 0d0a 0d0a 2020 2020 6465 6620 5f74 656d  ....    def _tem
+00015f10: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
+00015f20: 6b6d 6174 6528 7365 6c66 293a 0d0a 2020  kmate(self):..  
+00015f30: 2020 0d0a 2020 2020 0d0a 2020 2020 0d0a    ..    ..    ..
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 7365 6c66 2e41 7474 7220 3d20 7b7d 0d0a  self.Attr = {}..
+00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f70: 7374 6172 7474 696d 6520 3d20 696e 7428  starttime = int(
+00015f80: 6d69 6e28 7365 6c66 2e41 6c6c 5661 6c75  min(self.AllValu
+00015f90: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+00015fa0: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
+00015fb0: 2020 2020 2020 2020 656e 6474 696d 6520          endtime 
+00015fc0: 3d20 696e 7428 6d61 7828 7365 6c66 2e41  = int(max(self.A
+00015fd0: 6c6c 5661 6c75 6573 5b73 656c 662e 6672  llValues[self.fr
+00015fe0: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00016000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016010: 2073 656c 662e 7469 6d65 203d 205b 5d0d   self.time = [].
+00016020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016030: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00016040: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
+00016050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016060: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00016070: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
+00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016090: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+000160a0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
+000160b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000160c0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+000160d0: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+000160e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000160f0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00016100: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00016110: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016120: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00016130: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
+00016140: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016150: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00016160: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00016170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016180: 662e 6d69 746f 7469 635f 7661 725f 7261  f.mitotic_var_ra
+00016190: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+000161a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000161b0: 662e 6d69 746f 7469 635f 6d65 616e 5f73  f.mitotic_mean_s
+000161c0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+000161d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000161e0: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
+000161f0: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
+00016200: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016210: 6974 6f74 6963 5f6d 6561 6e5f 6163 6320  itotic_mean_acc 
+00016220: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016230: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016240: 6963 5f76 6172 5f61 6363 203d 205b 5d0d  ic_var_acc = [].
+00016250: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016260: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00016270: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00016280: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00016290: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000162a0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+000162b0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000162c0: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
+000162d0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000162e0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
+000162f0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00016300: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016310: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016320: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00016330: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00016340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016350: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016360: 635f 6d65 616e 5f64 6973 705f 7a20 3d20  c_mean_disp_z = 
+00016370: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016380: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016390: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
+000163a0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000163b0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000163c0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+000163d0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+000163e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000163f0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00016400: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+00016410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016420: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016430: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
+00016440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016450: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016460: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
+00016470: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016480: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00016490: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+000164a0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+000164b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000164c0: 6e5f 6d69 746f 7469 635f 7661 725f 7261  n_mitotic_var_ra
+000164d0: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+000164e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000164f0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016500: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
+00016510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016520: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016530: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
+00016540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016550: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016560: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
+00016570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016580: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016590: 6963 5f76 6172 5f61 6363 203d 205b 5d0d  ic_var_acc = [].
+000165a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000165b0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000165c0: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
+000165d0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000165e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000165f0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016600: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
+00016610: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00016620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016630: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016640: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00016650: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00016660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016670: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016680: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00016690: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+000166a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000166b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+000166c0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+000166d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000166e0: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a20  .all_var_disp_z 
+000166f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016700: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00016710: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
+00016720: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016730: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00016740: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+00016750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016760: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00016770: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00016780: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016790: 6c6c 5f76 6172 5f64 6973 705f 7820 3d20  ll_var_disp_x = 
+000167a0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+000167b0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+000167c0: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
+000167d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000167e0: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
+000167f0: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+00016800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016810: 662e 616c 6c5f 6d65 616e 5f73 7065 6564  f.all_mean_speed
+00016820: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016830: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016840: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
+00016850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016860: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00016870: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00016880: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016890: 6c6c 5f76 6172 5f61 6363 203d 205b 5d0d  ll_var_acc = [].
+000168a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000168b0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+000168c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000168d0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+000168e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000168f0: 6c6c 5f76 6172 5f64 6972 6563 7469 6f6e  ll_var_direction
+00016900: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00016910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016920: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00016930: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00016940: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
+00016950: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00016960: 6c5f 7661 725f 6469 7374 616e 6365 5f63  l_var_distance_c
+00016970: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00016980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016990: 2073 656c 662e 6d69 746f 7469 635f 636c   self.mitotic_cl
+000169a0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+000169b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000169c0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000169d0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+000169e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000169f0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016a00: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
+00016a10: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016a20: 2020 2020 2020 616c 6c5f 7370 6f74 735f        all_spots_
+00016a30: 7472 6163 6b73 203d 207b 7d0d 0a20 2020  tracks = {}..   
+00016a40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00016a50: 2028 6b2c 7629 2069 6e20 7365 6c66 2e75   (k,v) in self.u
+00016a60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00016a70: 7274 6965 732e 6974 656d 7328 293a 0d0a  rties.items():..
+00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016ab0: 6c5f 7370 6f74 7320 3d20 7365 6c66 2e75  l_spots = self.u
+00016ac0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00016ad0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
+00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016af0: 6966 2073 656c 662e 7472 6163 6b69 645f  if self.trackid_
+00016b00: 6b65 7920 696e 2061 6c6c 5f73 706f 7473  key in all_spots
+00016b10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016b20: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00016b30: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016b40: 203d 2061 6c6c 5f73 706f 7473 0d0a 2020   = all_spots..  
+00016b50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016b60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016b70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016b80: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
+00016b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ba0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
+00016bb0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
+00016bc0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
+00016bd0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
+00016be0: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
+00016bf0: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
+00016c00: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c20: 2020 2020 2066 6f72 2069 2069 6e20 7471       for i in tq
+00016c30: 646d 2872 616e 6765 2873 7461 7274 7469  dm(range(startti
+00016c40: 6d65 2c20 656e 6474 696d 6529 2c20 746f  me, endtime), to
+00016c50: 7461 6c3d 656e 6474 696d 6520 2d20 7374  tal=endtime - st
+00016c60: 6172 7474 696d 6529 3a0d 0a20 2020 2020  arttime):..     
+00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016c90: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+00016ca0: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+00016cb0: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+00016cc0: 636f 6d70 7574 655f 7465 6d70 6f72 616c  compute_temporal
+00016cd0: 2c20 692c 2061 6c6c 5f73 706f 7473 5f74  , i, all_spots_t
+00016ce0: 7261 636b 7329 290d 0a20 0d0a 2020 2020  racks)).. ..    
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d00: 5b72 2e72 6573 756c 7428 2920 666f 7220  [r.result() for 
+00016d10: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+00016d20: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+00016d30: 6574 6564 2866 7574 7572 6573 295d 0d0a  eted(futures)]..
+00016d40: 0d0a 0d0a 2020 2020 6465 6620 5f63 6f6d  ....    def _com
+00016d50: 7075 7465 5f74 656d 706f 7261 6c28 7365  pute_temporal(se
+00016d60: 6c66 2c20 692c 2061 6c6c 5f73 706f 7473  lf, i, all_spots
+00016d70: 5f74 7261 636b 7329 3a20 2020 2020 2020  _tracks):       
+00016d80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016d90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016da0: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
+00016db0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016dc0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016dd0: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 206d 6974 6f74 6963 5f64 6973 705f 7820   mitotic_disp_x 
+00016e00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016e10: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016e20: 635f 7261 6469 7573 203d 205b 5d0d 0a20  c_radius = [].. 
+00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e40: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
+00016e50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016e60: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016e70: 6963 5f61 6363 203d 205b 5d0d 0a20 2020  ic_acc = []..   
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 206d 6974 6f74 6963 5f64 6972 6563 7469   mitotic_directi
+00016ea0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+00016eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ec0: 2020 2020 2020 6d69 746f 7469 635f 636c        mitotic_cl
+00016ed0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+00016ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ef0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016f00: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016f10: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016f20: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016f30: 5f6d 6974 6f74 6963 5f64 6973 705f 7a20  _mitotic_disp_z 
+00016f40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016f50: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016f60: 746f 7469 635f 6469 7370 5f79 203d 205b  totic_disp_y = [
+00016f70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016f80: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016f90: 6963 5f64 6973 705f 7820 3d20 5b5d 0d0a  ic_disp_x = []..
+00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fb0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016fc0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fe0: 206e 6f6e 5f6d 6974 6f74 6963 5f73 7065   non_mitotic_spe
+00016ff0: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
+00017000: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00017010: 5f6d 6974 6f74 6963 5f61 6363 203d 205b  _mitotic_acc = [
+00017020: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017030: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00017040: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00017050: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
 00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 616c 6c5f 6469 7370 5f79 203d 205b 5d0d  all_disp_y = [].
-00017080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017090: 2020 2020 2061 6c6c 5f64 6973 705f 7820       all_disp_x 
-000170a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000170b0: 2020 2020 2020 2020 2020 616c 6c5f 7261            all_ra
-000170c0: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-000170d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000170e0: 6c6c 5f73 7065 6564 203d 205b 5d0d 0a20  ll_speed = [].. 
-000170f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017100: 2020 2061 6c6c 5f61 6363 203d 205b 5d0d     all_acc = [].
-00017110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017120: 2020 2020 2061 6c6c 5f64 6972 6563 7469       all_directi
-00017130: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00017140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017150: 2020 2020 2020 616c 6c5f 636c 7573 7465        all_cluste
-00017160: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017180: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
-00017190: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-000171a0: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
-000171b0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-000171c0: 6b2c 7629 2069 6e20 616c 6c5f 7370 6f74  k,v) in all_spot
-000171d0: 735f 7472 6163 6b73 2e69 7465 6d73 2829  s_tracks.items()
-000171e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000171f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00017200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017210: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00017220: 7265 6e74 5f74 696d 6520 3d20 616c 6c5f  rent_time = all_
-00017230: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017240: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00017250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017260: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017270: 6974 6f74 6963 203d 2061 6c6c 5f73 706f  itotic = all_spo
-00017280: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017290: 662e 6469 7669 6469 6e67 5f6b 6579 5d0d  f.dividing_key].
-000172a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172d0: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-000172e0: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
-000172f0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+00017070: 6e6f 6e5f 6d69 746f 7469 635f 636c 7573  non_mitotic_clus
+00017080: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170a0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+000170b0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000170c0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
+000170d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170f0: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
+00017100: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017110: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00017120: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00017130: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017140: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017160: 2020 616c 6c5f 7261 6469 7573 203d 205b    all_radius = [
+00017170: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017180: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
+00017190: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000171a0: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
+000171b0: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+000171c0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000171d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000171e0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+000171f0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017200: 6c5f 636c 7573 7465 725f 636c 6173 7320  l_cluster_class 
+00017210: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017220: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017230: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00017240: 203d 205b 5d0d 0a0d 0a0d 0a0d 0a0d 0a20   = [].......... 
+00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017260: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00017270: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017280: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172c0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
+000172d0: 6520 3d20 616c 6c5f 7370 6f74 735f 7472  e = all_spots_tr
+000172e0: 6163 6b73 5b6b 5d5b 7365 6c66 2e66 7261  acks[k][self.fra
+000172f0: 6d65 6964 5f6b 6579 5d0d 0a20 2020 2020  meid_key]..     
 00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2020 6966 206d 6974 6f74          if mitot
-00017320: 6963 3a0d 0a20 2020 2020 2020 2020 2020  ic:..           
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017350: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00017360: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017370: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00017380: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017310: 2020 2020 2020 206d 6974 6f74 6963 203d         mitotic =
+00017320: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00017330: 735b 6b5d 5b73 656c 662e 6469 7669 6469  s[k][self.dividi
+00017340: 6e67 5f6b 6579 5d0d 0a20 2020 2020 2020  ng_key]..       
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017360: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017380: 2020 6966 2069 203d 3d20 696e 7428 6375    if i == int(cu
+00017390: 7272 656e 745f 7469 6d65 293a 0d0a 2020  rrent_time):..  
 000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173b0: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
-000173c0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000173d0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000173e0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017410: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017420: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
-00017430: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017440: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00017450: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017470: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00017480: 7469 635f 7261 6469 7573 2e61 7070 656e  tic_radius.appen
-00017490: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000174a0: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-000174b0: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 206d 6974 6f74 6963 5f73 7065 6564 2e61   mitotic_speed.a
-000174f0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017500: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-00017510: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 2020 2020 6d69 746f 7469 635f 6163 632e      mitotic_acc.
-00017550: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017560: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017570: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00017580: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175a0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000175b0: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-000175c0: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
-000175d0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000175e0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
-000175f0: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017620: 2020 206d 6974 6f74 6963 5f64 6973 7461     mitotic_dista
-00017630: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00017640: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017650: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00017660: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00017670: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176a0: 6966 2073 656c 662e 636c 7573 7465 7263  if self.clusterc
-000176b0: 6c61 7373 5f6b 6579 2069 6e20 616c 6c5f  lass_key in all_
-000176c0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d2e  spots_tracks[k].
-000176d0: 6b65 7973 2829 203a 0d0a 2020 2020 2020  keys() :..      
-000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017710: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-00017720: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017730: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e63  tracks[k][self.c
-00017740: 6c75 7374 6572 636c 6173 735f 6b65 795d  lusterclass_key]
-00017750: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00017780: 6d69 746f 7469 633a 0d0a 2020 2020 2020  mitotic:..      
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 6966 206d 6974 6f74 6963 3a0d 0a20 2020  if mitotic:..   
+000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00017400: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
+00017410: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017420: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00017430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017460: 635f 6469 7370 5f79 2e61 7070 656e 6428  c_disp_y.append(
+00017470: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017480: 5b6b 5d5b 7365 6c66 2e79 706f 7369 645f  [k][self.yposid_
+00017490: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000174c0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
+000174d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000174e0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+000174f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017520: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
+00017530: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
+00017540: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017550: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
+00017560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017590: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+000175a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000175b0: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+000175c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175e0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000175f0: 7469 635f 6163 632e 6170 7065 6e64 2861  tic_acc.append(a
+00017600: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017610: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
+00017620: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 2020 2020 6d69 746f 7469 635f 6469 7265      mitotic_dire
+00017660: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00017670: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017680: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+00017690: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+000176a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176c0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000176d0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000176e0: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
+000176f0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017700: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+00017710: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017740: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00017750: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00017760: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
+00017770: 6163 6b73 5b6b 5d2e 6b65 7973 2829 203a  acks[k].keys() :
+00017780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177b0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-000177c0: 7370 5f7a 2e61 7070 656e 6428 616c 6c5f  sp_z.append(all_
-000177d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000177e0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-000177f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000177b0: 206d 6974 6f74 6963 5f63 6c75 7374 6572   mitotic_cluster
+000177c0: 5f63 6c61 7373 2e61 7070 656e 6428 616c  _class.append(al
+000177d0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000177e0: 5d5b 7365 6c66 2e63 6c75 7374 6572 636c  ][self.clustercl
+000177f0: 6173 735f 6b65 795d 290d 0a0d 0a0d 0a20  ass_key])...... 
 00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017820: 6974 6f74 6963 5f64 6973 705f 792e 6170  itotic_disp_y.ap
-00017830: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017840: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
-00017850: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017880: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017890: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
-000178a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000178b0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-000178c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178e0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-000178f0: 5f6d 6974 6f74 6963 5f72 6164 6975 732e  _mitotic_radius.
-00017900: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017910: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017920: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017950: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017960: 635f 7370 6565 642e 6170 7065 6e64 2861  c_speed.append(a
-00017970: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017980: 6b5d 5b73 656c 662e 7370 6565 645f 6b65  k][self.speed_ke
-00017990: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-000179c0: 5f6d 6974 6f74 6963 5f61 6363 2e61 7070  _mitotic_acc.app
-000179d0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000179e0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-000179f0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-00017a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017a30: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00017a40: 5f63 6861 6e67 652e 6170 7065 6e64 2861  _change.append(a
-00017a50: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017a60: 6b5d 5b73 656c 662e 6d6f 7469 6f6e 5f61  k][self.motion_a
-00017a70: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017aa0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017ab0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017ac0: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
-00017ad0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017ae0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-00017af0: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
-00017b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b20: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
-00017b30: 7374 6572 636c 6173 735f 6b65 7920 696e  sterclass_key in
-00017b40: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00017b50: 735b 6b5d 2e6b 6579 7328 2920 3a0d 0a20  s[k].keys() :.. 
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b80: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017b90: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
-00017ba0: 725f 636c 6173 732e 6170 7065 6e64 2861  r_class.append(a
-00017bb0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017bc0: 6b5d 5b73 656c 662e 636c 7573 7465 7263  k][self.clusterc
-00017bd0: 6c61 7373 5f6b 6579 5d29 0d0a 0d0a 2020  lass_key])....  
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c00: 616c 6c5f 6469 7370 5f7a 2e61 7070 656e  all_disp_z.appen
-00017c10: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00017c20: 6b73 5b6b 5d5b 7365 6c66 2e7a 706f 7369  ks[k][self.zposi
-00017c30: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c50: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017c60: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
-00017c70: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017c80: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00017c90: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cb0: 2020 2020 2020 616c 6c5f 6469 7370 5f78        all_disp_x
-00017cc0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017cd0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017ce0: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
+00017830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017850: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017860: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+00017870: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017880: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+00017890: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178c0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000178d0: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
+000178e0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000178f0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00017900: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017920: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017930: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
+00017940: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017950: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
+00017960: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017990: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000179a0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+000179b0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+000179c0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+000179d0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179f0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017a00: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
+00017a10: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017a20: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017a30: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a60: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00017a70: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00017a80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017a90: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00017aa0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ad0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
+00017ae0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00017af0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017b00: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017b10: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
+00017b20: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b40: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017b50: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00017b60: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00017b70: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017b80: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00017b90: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00017ba0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017bd0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00017be0: 735f 6b65 7920 696e 2061 6c6c 5f73 706f  s_key in all_spo
+00017bf0: 7473 5f74 7261 636b 735b 6b5d 2e6b 6579  ts_tracks[k].key
+00017c00: 7328 2920 3a0d 0a20 2020 2020 2020 2020  s() :..         
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c30: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017c40: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00017c50: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017c60: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017c70: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00017c80: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ca0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00017cb0: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
+00017cc0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017cd0: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+00017ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d10: 2061 6c6c 5f72 6164 6975 732e 6170 7065   all_radius.appe
-00017d20: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017d30: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-00017d40: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d60: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017d70: 7370 6565 642e 6170 7065 6e64 2861 6c6c  speed.append(all
-00017d80: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017d90: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
-00017da0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dc0: 2020 2020 2061 6c6c 5f61 6363 2e61 7070       all_acc.app
-00017dd0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017de0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-00017df0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-00017e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e20: 2020 2061 6c6c 5f64 6972 6563 7469 6f6e     all_direction
-00017e30: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00017e40: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017e50: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-00017e60: 5f61 6e67 6c65 5f6b 6579 5d29 2020 200d  _angle_key])   .
-00017e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 2061 6c6c 5f64 6973 7461 6e63 655f     all_distance_
-00017ea0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00017eb0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017ec0: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017ed0: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00017ee0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-00017f10: 7573 7465 7263 6c61 7373 5f6b 6579 2069  usterclass_key i
-00017f20: 6e20 616c 6c5f 7370 6f74 735f 7472 6163  n all_spots_trac
-00017f30: 6b73 5b6b 5d2e 6b65 7973 2829 203a 0d0a  ks[k].keys() :..
-00017f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017f70: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
-00017f80: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017f90: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017fa0: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
-00017fb0: 795d 2920 2020 200d 0a20 2020 2020 2020  y])    ..       
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-00017ff0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00018000: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
-00018010: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
-00018020: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
-00018030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018040: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00018050: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00018060: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
-00018070: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018080: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00018090: 6963 5f64 6973 705f 7820 3d20 6e70 2e61  ic_disp_x = np.a
-000180a0: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-000180b0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180d0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000180e0: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
-000180f0: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
-00018100: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
-00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018120: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00018130: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00018140: 6469 6666 286e 6f6e 5f6d 6974 6f74 6963  diff(non_mitotic
-00018150: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00018160: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00018170: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00018180: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
-00018190: 6666 286e 6f6e 5f6d 6974 6f74 6963 5f64  ff(non_mitotic_d
-000181a0: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
-000181b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000181c0: 6c6c 5f64 6973 705f 7a20 3d20 6e70 2e61  ll_disp_z = np.a
-000181d0: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
-000181e0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-000181f0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00018200: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-00018210: 286e 702e 6469 6666 2861 6c6c 5f64 6973  (np.diff(all_dis
-00018220: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018230: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00018240: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-00018250: 702e 6469 6666 2861 6c6c 5f64 6973 705f  p.diff(all_disp_
-00018260: 7829 290d 0a0d 0a0d 0a20 2020 2020 2020  x))......       
-00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000182a0: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-000182b0: 2e61 7070 656e 6428 6920 2a20 7365 6c66  .append(i * self
-000182c0: 2e74 6361 6c69 6272 6174 696f 6e29 0d0a  .tcalibration)..
-000182d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000182e0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000182f0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-00018300: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
-00018310: 6179 286d 6974 6f74 6963 5f63 6c75 7374  ay(mitotic_clust
-00018320: 6572 5f63 6c61 7373 2929 0d0a 2020 2020  er_class))..    
-00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018340: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018350: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-00018360: 7070 656e 6428 6e70 2e61 7361 7272 6179  ppend(np.asarray
-00018370: 286e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  (non_mitotic_clu
-00018380: 7374 6572 5f63 6c61 7373 2929 0d0a 2020  ster_class))..  
-00018390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183a0: 2020 7365 6c66 2e61 6c6c 5f63 6c75 7374    self.all_clust
-000183b0: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
-000183c0: 6e70 2e61 7361 7272 6179 2861 6c6c 5f63  np.asarray(all_c
-000183d0: 6c75 7374 6572 5f63 6c61 7373 2929 0d0a  luster_class))..
-000183e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000183f0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018400: 6963 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ic_mean_disp_z.a
-00018410: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018420: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018440: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018450: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
-00018460: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00018470: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-000184a0: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
-000184b0: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-000184c0: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
-000184d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184e0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-000184f0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00018500: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00018510: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00018520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018530: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018540: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00018550: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00018560: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
-00018570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018580: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00018590: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
-000185a0: 6428 6d69 746f 7469 635f 6469 7370 5f78  d(mitotic_disp_x
-000185b0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000185c0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000185d0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-000185e0: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
-000185f0: 6e28 6d69 746f 7469 635f 7261 6469 7573  n(mitotic_radius
-00018600: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018610: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018620: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
-00018630: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00018640: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00018650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018660: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018670: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
-00018680: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018690: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
-000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186b0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-000186c0: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
-000186d0: 6e70 2e73 7464 286d 6974 6f74 6963 5f73  np.std(mitotic_s
-000186e0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-000186f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018700: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018710: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
-00018720: 616e 286d 6974 6f74 6963 5f61 6363 2929  an(mitotic_acc))
-00018730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018740: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018750: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
-00018760: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018770: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-00018780: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018790: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-000187a0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000187b0: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-000187c0: 6e28 6d69 746f 7469 635f 6469 7265 6374  n(mitotic_direct
-000187d0: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018800: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-00018810: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-00018820: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00018830: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018840: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018850: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018860: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
-00018870: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018880: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018890: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-000188a0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-000188d0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000188e0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-000188f0: 6428 6d69 746f 7469 635f 6469 7374 616e  d(mitotic_distan
-00018900: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-00018910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018920: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018930: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00018940: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
-00018950: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018960: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00018970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018980: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018990: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-000189a0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-000189b0: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
-000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189d0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000189e0: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
-000189f0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00018a00: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00018a10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018a20: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018a30: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00018a40: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
-00018a50: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018a60: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00018a70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018a80: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018a90: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
-00018aa0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018ab0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00017d00: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
+00017d10: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017d20: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00017d30: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d50: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017d60: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
+00017d70: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017d80: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
+00017d90: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017db0: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+00017dc0: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+00017dd0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017de0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+00017df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e10: 2020 2020 616c 6c5f 7370 6565 642e 6170      all_speed.ap
+00017e20: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017e30: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
+00017e40: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00017e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017e70: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00017e80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017e90: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00017ea0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ec0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017ed0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00017ee0: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
+00017ef0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017f00: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+00017f10: 6579 5d29 2020 200d 0a20 2020 2020 2020  ey])   ..       
+00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f30: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017f40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017f50: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017f60: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017f70: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00017f80: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017fb0: 2073 656c 662e 636c 7573 7465 7263 6c61   self.clustercla
+00017fc0: 7373 5f6b 6579 2069 6e20 616c 6c5f 7370  ss_key in all_sp
+00017fd0: 6f74 735f 7472 6163 6b73 5b6b 5d2e 6b65  ots_tracks[k].ke
+00017fe0: 7973 2829 203a 0d0a 2020 2020 2020 2020  ys() :..        
+00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018010: 2020 2020 2020 2061 6c6c 5f63 6c75 7374         all_clust
+00018020: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
+00018030: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00018040: 5b6b 5d5b 7365 6c66 2e63 6c75 7374 6572  [k][self.cluster
+00018050: 636c 6173 735f 6b65 795d 2920 2020 200d  class_key])    .
+00018060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018080: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00018090: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000180a0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+000180b0: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
+000180c0: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
+000180d0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+000180e0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+000180f0: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+00018100: 2e61 6273 286e 702e 6469 6666 286d 6974  .abs(np.diff(mit
+00018110: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018130: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00018140: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
+00018150: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
+00018160: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00018170: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00018180: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
+00018190: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
+000181a0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+000181b0: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+000181c0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+000181d0: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+000181e0: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
+000181f0: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
+00018200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018210: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00018220: 6963 5f64 6973 705f 7820 3d20 6e70 2e61  ic_disp_x = np.a
+00018230: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+00018240: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00018250: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018260: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00018270: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00018280: 6666 2861 6c6c 5f64 6973 705f 7a29 290d  ff(all_disp_z)).
+00018290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000182a0: 2020 2020 2061 6c6c 5f64 6973 705f 7920       all_disp_y 
+000182b0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+000182c0: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182e0: 2020 2061 6c6c 5f64 6973 705f 7820 3d20     all_disp_x = 
+000182f0: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+00018300: 6c6c 5f64 6973 705f 7829 290d 0a0d 0a0d  ll_disp_x)).....
+00018310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018330: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00018340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018350: 656c 662e 7469 6d65 2e61 7070 656e 6428  elf.time.append(
+00018360: 6920 2a20 7365 6c66 2e74 6361 6c69 6272  i * self.tcalibr
+00018370: 6174 696f 6e29 0d0a 0d0a 2020 2020 2020  ation)....      
+00018380: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018390: 6c66 2e6d 6974 6f74 6963 5f63 6c75 7374  lf.mitotic_clust
+000183a0: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
+000183b0: 6e70 2e61 7361 7272 6179 286d 6974 6f74  np.asarray(mitot
+000183c0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+000183d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000183e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000183f0: 5f6d 6974 6f74 6963 5f63 6c75 7374 6572  _mitotic_cluster
+00018400: 5f63 6c61 7373 2e61 7070 656e 6428 6e70  _class.append(np
+00018410: 2e61 7361 7272 6179 286e 6f6e 5f6d 6974  .asarray(non_mit
+00018420: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00018430: 7373 2929 0d0a 2020 2020 2020 2020 2020  ss))..          
+00018440: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018450: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
+00018460: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
+00018470: 6179 2861 6c6c 5f63 6c75 7374 6572 5f63  ay(all_cluster_c
+00018480: 6c61 7373 2929 0d0a 0d0a 2020 2020 2020  lass))....      
+00018490: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000184a0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+000184b0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+000184c0: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+000184d0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+000184e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000184f0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00018500: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+00018510: 6428 6d69 746f 7469 635f 6469 7370 5f7a  d(mitotic_disp_z
+00018520: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018530: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018540: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018550: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+00018560: 6e28 6d69 746f 7469 635f 6469 7370 5f79  n(mitotic_disp_y
+00018570: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018580: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018590: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
+000185a0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000185b0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+000185c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000185d0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000185e0: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+000185f0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00018600: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00018610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018620: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018630: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+00018640: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018650: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018670: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00018680: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
+00018690: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+000186a0: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
+000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186c0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+000186d0: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+000186e0: 702e 7374 6428 6d69 746f 7469 635f 7261  p.std(mitotic_ra
+000186f0: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
+00018700: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018710: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018720: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+00018730: 6d65 616e 286d 6974 6f74 6963 5f73 7065  mean(mitotic_spe
+00018740: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+00018750: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018760: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
+00018770: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00018780: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+00018790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000187a0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000187b0: 6963 5f6d 6561 6e5f 6163 632e 6170 7065  ic_mean_acc.appe
+000187c0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+000187d0: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
+000187e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000187f0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
+00018800: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
+00018810: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
+00018820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018830: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018840: 6963 5f6d 6561 6e5f 6469 7265 6374 696f  ic_mean_directio
+00018850: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018860: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00018870: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00018880: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
+00018890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000188a0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6972  .mitotic_var_dir
+000188b0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+000188c0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000188d0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+000188e0: 6c5f 6368 616e 6765 2929 0d0a 0d0a 2020  l_change))....  
+000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018900: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00018910: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00018920: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00018930: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+00018940: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018950: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018960: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018970: 6f74 6963 5f76 6172 5f64 6973 7461 6e63  otic_var_distanc
+00018980: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00018990: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+000189a0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
+000189b0: 6d61 736b 2929 0d0a 0d0a 2020 2020 2020  mask))....      
+000189c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000189d0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000189e0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
+000189f0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018a00: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00018a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a20: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018a30: 6f74 6963 5f76 6172 5f64 6973 705f 7a2e  otic_var_disp_z.
+00018a40: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00018a50: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00018a60: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018a70: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018a80: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00018a90: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00018aa0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018ab0: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
 00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018ae0: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
-00018af0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-00018b00: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-00018b10: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018b20: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018b30: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018b40: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-00018b50: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018b60: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b80: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018b90: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00018ba0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-00018bb0: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00018bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018bd0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018be0: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-00018bf0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-00018c00: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
-00018c10: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
-00018c20: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018c30: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
-00018c40: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-00018c50: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f73  td(non_mitotic_s
-00018c60: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+00018ad0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018ae0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+00018af0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018b00: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+00018b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018b20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018b30: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018b40: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
+00018b50: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00018b60: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
+00018b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018b80: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018b90: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00018ba0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018bb0: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+00018bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bd0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018be0: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
+00018bf0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018c00: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00018c10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018c20: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018c30: 5f6d 6974 6f74 6963 5f76 6172 5f72 6164  _mitotic_var_rad
+00018c40: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00018c50: 6428 6e6f 6e5f 6d69 746f 7469 635f 7261  d(non_mitotic_ra
+00018c60: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
 00018c70: 2020 2020 2020 2020 2020 2020 2020 7365                se
 00018c80: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018c90: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00018ca0: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-00018cb0: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018cd0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00018ce0: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-00018cf0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00018d00: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-00018d10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018d20: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018d30: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00018d40: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018d50: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018d60: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-00018d70: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
-00018d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018d90: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018da0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018db0: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
-00018dc0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018dd0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018de0: 2929 200d 0a0d 0a20 2020 2020 2020 2020  )) ....         
-00018df0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018e00: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00018e10: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018e20: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
-00018e30: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00018e40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018e50: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-00018e60: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018e70: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00018e80: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018e90: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00018ea0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
-00018eb0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-00018ec0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00018ed0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018ee0: 6c5f 6d65 616e 5f64 6973 705f 7a2e 6170  l_mean_disp_z.ap
-00018ef0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00018f00: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00018f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018f20: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-00018f30: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
-00018f40: 2861 6c6c 5f64 6973 705f 7a29 290d 0a0d  (all_disp_z))...
-00018f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f60: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018f70: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
-00018f80: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-00018f90: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018fb0: 616c 6c5f 7661 725f 6469 7370 5f79 2e61  all_var_disp_y.a
-00018fc0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018fd0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
-00018fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ff0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00019000: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-00019010: 6d65 616e 2861 6c6c 5f64 6973 705f 7829  mean(all_disp_x)
-00019020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019030: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00019040: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
-00019050: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-00019060: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-00019070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019080: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
-00019090: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
-000190a0: 2861 6c6c 5f72 6164 6975 7329 290d 0a20  (all_radius)).. 
-000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190c0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-000190d0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-000190e0: 2e73 7464 2861 6c6c 5f72 6164 6975 7329  .std(all_radius)
-000190f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019100: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00019110: 6c5f 6d65 616e 5f73 7065 6564 2e61 7070  l_mean_speed.app
-00019120: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00019130: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
-00019140: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019150: 662e 616c 6c5f 7661 725f 7370 6565 642e  f.all_var_speed.
-00019160: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00019170: 6c5f 7370 6565 6429 290d 0a0d 0a20 2020  l_speed))....   
-00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019190: 2073 656c 662e 616c 6c5f 6d65 616e 5f61   self.all_mean_a
-000191a0: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-000191b0: 6e28 616c 6c5f 6163 6329 290d 0a20 2020  n(all_acc))..   
-000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191d0: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
-000191e0: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
-000191f0: 616c 6c5f 6163 6329 290d 0a0d 0a0d 0a0d  all_acc)).......
-00019200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019210: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00019220: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00019230: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00019240: 6d65 616e 2861 6c6c 5f64 6972 6563 7469  mean(all_directi
-00019250: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00019260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019270: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00019280: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00019290: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-000192a0: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
-000192b0: 5f63 6861 6e67 6529 290d 0a0d 0a20 2020  _change))....   
-000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192d0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-000192e0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000192f0: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
-00019300: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
-00019310: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00019320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019330: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
-00019340: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00019350: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00019360: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00019370: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019390: 2020 200d 0a20 2020 2020 2020 200d 0a64     ..        ..d
-000193a0: 6566 2062 6f75 6e64 6172 795f 706f 696e  ef boundary_poin
-000193b0: 7473 286d 6173 6b2c 2078 6361 6c69 6272  ts(mask, xcalibr
-000193c0: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
-000193d0: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
-000193e0: 6e29 3a0d 0a0d 0a20 2020 206e 6469 6d20  n):....    ndim 
-000193f0: 3d20 6c65 6e28 6d61 736b 2e73 6861 7065  = len(mask.shape
-00019400: 290d 0a20 2020 2074 696d 6564 5f6d 6173  )..    timed_mas
-00019410: 6b20 3d20 7b7d 0d0a 2020 2020 6d61 736b  k = {}..    mask
-00019420: 203d 206d 6173 6b20 3e20 300d 0a20 2020   = mask > 0..   
-00019430: 206d 6173 6b20 3d20 6d61 736b 2e61 7374   mask = mask.ast
-00019440: 7970 6528 2775 696e 7438 2729 0d0a 2020  ype('uint8')..  
-00019450: 2020 2320 5958 2073 6861 7065 6420 6f62    # YX shaped ob
-00019460: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
-00019470: 6d20 3d3d 2032 3a0d 0a20 2020 2020 2020  m == 2:..       
-00019480: 200d 0a20 2020 2020 2020 2062 6f75 6e64   ..        bound
-00019490: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
-000194a0: 6172 6965 7328 6d61 736b 290d 0a20 2020  aries(mask)..   
-000194b0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-000194c0: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
-000194d0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-000194e0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
-000194f0: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00019500: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
-00019510: 3029 0d0a 2020 2020 2020 2020 7265 616c  0)..        real
-00019520: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-00019530: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-00019540: 6179 2869 6e64 6963 6573 2929 2e63 6f70  ay(indices)).cop
-00019550: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
-00019560: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00019570: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-00019580: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-00019590: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-000195a0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-000195b0: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
-000195c0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-000195d0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-000195e0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-000195f0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-00019600: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
-00019610: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
-00019620: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00019630: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-00019640: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
-00019650: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
-00019660: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
-00019670: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
-00019680: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
-00019690: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
-000196a0: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
-000196b0: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
-000196c0: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
-000196d0: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
-000196e0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-000196f0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-00019700: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
-00019710: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-00019720: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
-00019730: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
-00019740: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
-00019750: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
-00019760: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
-00019770: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00019780: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
-00019790: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
-000197a0: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
-000197b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000197c0: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-000197d0: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
-000197e0: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
-000197f0: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
-00019800: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00019810: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-00019820: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
-00019830: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00019840: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-00019850: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-00019860: 6e64 6963 6573 2929 2e63 6f70 7928 290d  ndices)).copy().
-00019870: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019880: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00019890: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
-000198a0: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
-000198b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198c0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000198d0: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
-000198e0: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
-000198f0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00019900: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00019910: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
-00019920: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019930: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
-00019940: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-00019950: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00019960: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
-00019970: 6c5f 696e 6469 6365 7329 0d0a 0d0a 2020  l_indices)....  
-00019980: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00019990: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
-000199a0: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-000199b0: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-000199c0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-000199d0: 0d0a 2020 2020 2320 545a 5958 2073 6861  ..    # TZYX sha
-000199e0: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-000199f0: 6966 206e 6469 6d20 3d3d 2034 3a0d 0a20  if ndim == 4:.. 
-00019a00: 2020 2020 2020 2070 7269 6e74 2827 4d61         print('Ma
-00019a10: 736b 7320 6d61 6465 2069 6e74 6f20 6120  sks made into a 
-00019a20: 3444 2063 796c 696e 6465 722c 2075 7027  4D cylinder, up'
-00019a30: 290d 0a20 2020 2020 2020 2062 6f75 6e64  )..        bound
-00019a40: 6172 7920 3d20 6e70 2e7a 6572 6f73 280d  ary = np.zeros(.
-00019a50: 0a20 2020 2020 2020 2020 2020 205b 6d61  .            [ma
-00019a60: 736b 2e73 6861 7065 5b30 5d2c 206d 6173  sk.shape[0], mas
-00019a70: 6b2e 7368 6170 655b 315d 2c20 6d61 736b  k.shape[1], mask
-00019a80: 2e73 6861 7065 5b32 5d2c 206d 6173 6b2e  .shape[2], mask.
-00019a90: 7368 6170 655b 335d 5d0d 0a20 2020 2020  shape[3]]..     
-00019aa0: 2020 2029 0d0a 2020 2020 2020 2020 666f     )..        fo
-00019ab0: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
-00019ac0: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
-00019ad0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00019ae0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-00019af0: 6172 795b 692c 3a5d 203d 2066 696e 645f  ary[i,:] = find_
-00019b00: 626f 756e 6461 7269 6573 286d 6173 6b5b  boundaries(mask[
-00019b10: 692c 3a5d 290d 0a20 2020 2020 2020 2020  i,:])..         
-00019b20: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-00019b30: 6420 3d20 636f 6d70 7574 655f 6365 6e74  d = compute_cent
-00019b40: 726f 6964 2862 6f75 6e64 6172 795b 692c  roid(boundary[i,
-00019b50: 3a5d 2920 0d0a 2020 2020 2020 2020 2020  :]) ..          
-00019b60: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00019b70: 6865 7265 2862 6f75 6e64 6172 795b 692c  here(boundary[i,
-00019b80: 3a5d 203e 2030 290d 0a20 2020 2020 2020  :] > 0)..       
-00019b90: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019ba0: 7320 3d20 6e70 2e74 7261 6e73 706f 7365  s = np.transpose
-00019bb0: 286e 702e 6173 6172 7261 7928 696e 6469  (np.asarray(indi
-00019bc0: 6365 7329 292e 636f 7079 2829 0d0a 0d0a  ces)).copy()....
-00019bd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019be0: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
-00019bf0: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
-00019c00: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019c10: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019c20: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-00019c30: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-00019c40: 202a 207a 6361 6c69 6272 6174 696f 6e0d   * zcalibration.
-00019c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019c60: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019c70: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
-00019c80: 6e64 6963 6573 5b6a 5d5b 315d 202a 2079  ndices[j][1] * y
-00019c90: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00019ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cb0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019cc0: 5b32 5d20 3d20 7265 616c 5f69 6e64 6963  [2] = real_indic
-00019cd0: 6573 5b6a 5d5b 325d 202a 2078 6361 6c69  es[j][2] * xcali
-00019ce0: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
-00019cf0: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-00019d00: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
-00019d10: 616c 5f69 6e64 6963 6573 290d 0a20 2020  al_indices)..   
-00019d20: 2020 2020 2020 2020 2074 696d 6564 5f6d           timed_m
-00019d30: 6173 6b5b 7374 7228 6929 5d20 3d20 5b74  ask[str(i)] = [t
-00019d40: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
-00019d50: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a20  gioncentroid].. 
-00019d60: 2020 2070 7269 6e74 2827 436f 6d70 7574     print('Comput
-00019d70: 6564 2074 6865 2062 6f75 6e64 6172 7920  ed the boundary 
-00019d80: 706f 696e 7473 2729 0d0a 0d0a 2020 2020  points')....    
-00019d90: 7265 7475 726e 2074 696d 6564 5f6d 6173  return timed_mas
-00019da0: 6b2c 2062 6f75 6e64 6172 7920 2020 2020  k, boundary     
-00019db0: 2020 200d 0a0d 0a64 6566 2063 6f6d 7075     ....def compu
-00019dc0: 7465 5f63 656e 7472 6f69 6428 6269 6e61  te_centroid(bina
-00019dd0: 7279 5f69 6d61 6765 293a 0d0a 2020 2020  ry_image):..    
-00019de0: 2320 456e 7375 7265 2062 696e 6172 7920  # Ensure binary 
-00019df0: 696d 6167 6520 6973 2061 204e 756d 5079  image is a NumPy
-00019e00: 2061 7272 6179 0d0a 2020 2020 6269 6e61   array..    bina
-00019e10: 7279 5f69 6d61 6765 203d 206e 702e 6172  ry_image = np.ar
-00019e20: 7261 7928 6269 6e61 7279 5f69 6d61 6765  ray(binary_image
-00019e30: 290d 0a0d 0a20 2020 2077 6869 7465 5f70  )....    white_p
-00019e40: 6978 656c 7320 3d20 6e70 2e77 6865 7265  ixels = np.where
-00019e50: 2862 696e 6172 795f 696d 6167 6520 3d3d  (binary_image ==
-00019e60: 2031 290d 0a20 2020 206e 756d 5f70 6978   1)..    num_pix
-00019e70: 656c 7320 3d20 6c65 6e28 7768 6974 655f  els = len(white_
-00019e80: 7069 7865 6c73 5b30 5d29 0d0a 0d0a 2020  pixels[0])....  
-00019e90: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
-00019ea0: 6365 6e74 726f 6964 206f 6620 7468 6520  centroid of the 
-00019eb0: 7768 6974 6520 7069 7865 6c73 2069 6e20  white pixels in 
-00019ec0: 7468 6520 626f 756e 6461 7279 2069 6d61  the boundary ima
-00019ed0: 6765 0d0a 2020 2020 6365 6e74 726f 6964  ge..    centroid
-00019ee0: 203d 206e 702e 7a65 726f 7328 6269 6e61   = np.zeros(bina
-00019ef0: 7279 5f69 6d61 6765 2e6e 6469 6d29 0d0a  ry_image.ndim)..
-00019f00: 2020 2020 666f 7220 6469 6d20 696e 2072      for dim in r
-00019f10: 616e 6765 2862 696e 6172 795f 696d 6167  ange(binary_imag
-00019f20: 652e 6e64 696d 293a 0d0a 2020 2020 2020  e.ndim):..      
-00019f30: 2020 6365 6e74 726f 6964 5b64 696d 5d20    centroid[dim] 
-00019f40: 3d20 7768 6974 655f 7069 7865 6c73 5b64  = white_pixels[d
-00019f50: 696d 5d2e 7375 6d28 2920 2f20 6e75 6d5f  im].sum() / num_
-00019f60: 7069 7865 6c73 0d0a 0d0a 2020 2020 7265  pixels....    re
-00019f70: 7475 726e 2063 656e 7472 6f69 640d 0a0d  turn centroid...
-00019f80: 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620 6765  ..... ....def ge
-00019f90: 745f 6373 765f 6461 7461 2863 7376 293a  t_csv_data(csv):
-00019fa0: 0d0a 0d0a 2020 2020 2020 2020 6461 7461  ....        data
-00019fb0: 7365 7420 3d20 7064 2e72 6561 645f 6373  set = pd.read_cs
-00019fc0: 7628 0d0a 2020 2020 2020 2020 2020 2020  v(..            
-00019fd0: 6373 762c 2064 656c 696d 6974 6572 3d22  csv, delimiter="
-00019fe0: 2c22 2c20 656e 636f 6469 6e67 3d22 756e  ,", encoding="un
-00019ff0: 6963 6f64 655f 6573 6361 7065 222c 206c  icode_escape", l
-0001a000: 6f77 5f6d 656d 6f72 793d 4661 6c73 650d  ow_memory=False.
-0001a010: 0a20 2020 2020 2020 2029 5b33 3a5d 0d0a  .        )[3:]..
-0001a020: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-0001a030: 696e 6465 7820 3d20 6461 7461 7365 742e  index = dataset.
-0001a040: 696e 6465 780d 0a20 2020 2020 2020 2072  index..        r
-0001a050: 6574 7572 6e20 6461 7461 7365 742c 2064  eturn dataset, d
-0001a060: 6174 6173 6574 5f69 6e64 6578 0d0a 2020  ataset_index..  
-0001a070: 2020 0d0a 6465 6620 6765 745f 7370 6f74    ..def get_spot
-0001a080: 5f64 6174 6173 6574 2873 706f 745f 6461  _dataset(spot_da
-0001a090: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
-0001a0a0: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a0b0: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
-0001a0c0: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
-0001a0d0: 6c69 6272 6174 696f 6e2c 2041 7474 7269  libration, Attri
-0001a0e0: 6275 7465 426f 786e 616d 652c 2064 6574  buteBoxname, det
-0001a0f0: 6563 7469 6f6e 6368 616e 6e65 6c29 3a0d  ectionchannel):.
-0001a100: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001a110: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001a120: 2070 6f73 6978 203d 2074 7261 636b 5f61   posix = track_a
-0001a130: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001a140: 735b 2270 6f73 6978 225d 0d0a 2020 2020  s["posix"]..    
-0001a150: 2020 2020 706f 7369 7920 3d20 7472 6163      posiy = trac
-0001a160: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a170: 6b65 7973 5b22 706f 7369 7922 5d0d 0a20  keys["posiy"].. 
-0001a180: 2020 2020 2020 2070 6f73 697a 203d 2074         posiz = t
-0001a190: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001a1a0: 6f74 5f6b 6579 735b 2270 6f73 697a 225d  ot_keys["posiz"]
-0001a1b0: 0d0a 2020 2020 2020 2020 6672 616d 6520  ..        frame 
-0001a1c0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001a1d0: 5f73 706f 745f 6b65 7973 5b22 6672 616d  _spot_keys["fram
-0001a1e0: 6522 5d0d 0a20 2020 2020 2020 200d 0a20  e"]..        .. 
-0001a1f0: 2020 2020 2020 204c 6f63 6174 696f 6e58         LocationX
-0001a200: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a210: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a220: 6f73 6978 5d2e 6173 7479 7065 2822 666c  osix].astype("fl
-0001a230: 6f61 7422 2920 2f20 7863 616c 6962 7261  oat") / xcalibra
-0001a240: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a250: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a260: 2020 2020 2020 204c 6f63 6174 696f 6e59         LocationY
-0001a270: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a280: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a290: 6f73 6979 5d2e 6173 7479 7065 2822 666c  osiy].astype("fl
-0001a2a0: 6f61 7422 2920 2f20 7963 616c 6962 7261  oat") / ycalibra
-0001a2b0: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a2c0: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a2d0: 2020 2020 2020 204c 6f63 6174 696f 6e5a         LocationZ
-0001a2e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001a2f0: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-0001a300: 6f73 697a 5d2e 6173 7479 7065 2822 666c  osiz].astype("fl
-0001a310: 6f61 7422 2920 2f20 7a63 616c 6962 7261  oat") / zcalibra
-0001a320: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-0001a330: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-0001a340: 2020 2020 2020 204c 6f63 6174 696f 6e54         LocationT
-0001a350: 203d 2028 7370 6f74 5f64 6174 6173 6574   = (spot_dataset
-0001a360: 5b66 7261 6d65 5d2e 6173 7479 7065 2822  [frame].astype("
-0001a370: 666c 6f61 7422 2929 2e61 7374 7970 6528  float")).astype(
-0001a380: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001a390: 0d0a 0d0a 2020 2020 2020 2020 6967 6e6f  ....        igno
-0001a3a0: 7265 5f76 616c 7565 7320 3d20 5b74 7261  re_values = [tra
-0001a3b0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a3c0: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
-0001a3d0: 6e73 6974 7922 5d2c 7472 6163 6b5f 616e  nsity"],track_an
-0001a3e0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a3f0: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001a400: 7922 5d5d 200d 0a20 2020 2020 2020 2066  y"]] ..        f
-0001a410: 6f72 2028 6b2c 7629 2069 6e20 7472 6163  or (k,v) in trac
-0001a420: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a430: 6b65 7973 2e69 7465 6d73 2829 3a0d 0a0d  keys.items():...
-0001a440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a450: 2069 6620 6465 7465 6374 696f 6e63 6861   if detectioncha
-0001a460: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
-0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a480: 2069 6620 6b20 3d3d 2022 6d65 616e 5f69   if k == "mean_i
-0001a490: 6e74 656e 7369 7479 5f63 6832 223a 0d0a  ntensity_ch2":..
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4b0: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0001a4c0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001a4d0: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-0001a4e0: 6e5f 696e 7465 6e73 6974 7922 5d0d 0a20  n_intensity"].. 
-0001a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a500: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-0001a510: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
-0001a520: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-0001a530: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a550: 2020 2069 6620 6b20 3d3d 2022 746f 7461     if k == "tota
-0001a560: 6c5f 696e 7465 6e73 6974 795f 6368 3222  l_intensity_ch2"
-0001a570: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a580: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0001a590: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-0001a5a0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a5b0: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
-0001a5c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001a5d0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001a5e0: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-0001a5f0: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-0001a600: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a610: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-0001a620: 2020 2020 2020 2020 2020 2069 6620 7620             if v 
-0001a630: 6e6f 7420 696e 2069 676e 6f72 655f 7661  not in ignore_va
-0001a640: 6c75 6573 3a0d 0a20 2020 2020 2020 2020  lues:..         
-0001a650: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a670: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001a680: 5b76 5d20 3d20 7370 6f74 5f64 6174 6173  [v] = spot_datas
-0001a690: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
-0001a6a0: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
-0001a6b0: 2041 6c6c 5661 6c75 6573 5b70 6f73 6978   AllValues[posix
-0001a6c0: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-0001a6d0: 6f6e 582c 3329 0d0a 2020 2020 2020 2020  onX,3)..        
-0001a6e0: 416c 6c56 616c 7565 735b 706f 7369 795d  AllValues[posiy]
-0001a6f0: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001a700: 6e59 2c33 290d 0a20 2020 2020 2020 2041  nY,3)..        A
-0001a710: 6c6c 5661 6c75 6573 5b70 6f73 697a 5d20  llValues[posiz] 
-0001a720: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-0001a730: 5a2c 3329 0d0a 2020 2020 2020 2020 416c  Z,3)..        Al
-0001a740: 6c56 616c 7565 735b 6672 616d 655d 203d  lValues[frame] =
-0001a750: 2072 6f75 6e64 284c 6f63 6174 696f 6e54   round(LocationT
-0001a760: 2c33 290d 0a20 2020 2020 2020 2041 7474  ,3)..        Att
-0001a770: 7269 6275 7465 6964 7320 3d20 5b5d 0d0a  ributeids = []..
-0001a780: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0001a790: 6569 6473 2e61 7070 656e 6428 4174 7472  eids.append(Attr
-0001a7a0: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-0001a7b0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
-0001a7c0: 6275 7465 6e61 6d65 2069 6e20 416c 6c56  butename in AllV
-0001a7d0: 616c 7565 732e 6b65 7973 2829 3a0d 0a20  alues.keys():.. 
-0001a7e0: 2020 2020 2020 2020 2020 2020 2041 7474               Att
-0001a7f0: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001a800: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
-0001a810: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001a820: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-0001a830: 2020 2020 2072 6574 7572 6e20 4174 7472       return Attr
-0001a840: 6962 7574 6569 6473 2c20 416c 6c56 616c  ibuteids, AllVal
-0001a850: 7565 7320 2020 2020 0d0a 2020 2020 0d0a  ues     ..    ..
-0001a860: 6465 6620 6765 745f 7472 6163 6b5f 6461  def get_track_da
-0001a870: 7461 7365 7428 7472 6163 6b5f 6461 7461  taset(track_data
-0001a880: 7365 742c 2074 7261 636b 5f61 6e61 6c79  set, track_analy
-0001a890: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
-0001a8a0: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001a8b0: 6163 6b5f 6b65 7973 2c20 5472 6163 6b41  ack_keys, TrackA
-0001a8c0: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a8d0: 3a0d 0a0d 0a20 2020 2020 2020 2041 6c6c  :....        All
-0001a8e0: 5472 6163 6b56 616c 7565 7320 3d20 7b7d  TrackValues = {}
-0001a8f0: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-0001a900: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
-0001a910: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
-0001a920: 7261 636b 5f69 6422 5d0d 0a20 2020 2020  rack_id"]..     
-0001a930: 2020 2054 6964 203d 2074 7261 636b 5f64     Tid = track_d
-0001a940: 6174 6173 6574 5b74 7261 636b 5f69 645d  ataset[track_id]
-0001a950: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a960: 0d0a 2020 2020 2020 200d 0a20 2020 2020  ..       ..     
-0001a970: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001a980: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001a990: 640d 0a20 2020 2020 200d 0a20 2020 2020  d..      ..     
-0001a9a0: 2020 2066 6f72 2028 6b2c 2076 2920 696e     for (k, v) in
-0001a9b0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a9c0: 7472 6163 6b5f 6b65 7973 2e69 7465 6d73  track_keys.items
-0001a9d0: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-0001a9e0: 2020 2020 2020 2078 203d 2074 7261 636b         x = track
-0001a9f0: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-0001aa00: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001aa10: 2020 2020 2020 2020 2020 2020 206d 696e               min
-0001aa20: 7661 6c20 3d20 6d69 6e28 7829 0d0a 2020  val = min(x)..  
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001aa40: 7876 616c 203d 206d 6178 2878 290d 0a0d  xval = max(x)...
-0001aa50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aa60: 2069 6620 6d69 6e76 616c 203e 2030 2061   if minval > 0 a
-0001aa70: 6e64 206d 6178 7661 6c20 3c3d 2031 3a0d  nd maxval <= 1:.
-0001aa80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001aa90: 2020 2020 2020 2078 203d 2078 202b 2031         x = x + 1
-0001aaa0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001aab0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001aac0: 6573 5b6b 5d20 3d20 726f 756e 6428 782c  es[k] = round(x,
-0001aad0: 2033 290d 0a0d 0a20 2020 2020 2020 2054   3)....        T
-0001aae0: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001aaf0: 203d 205b 5d0d 0a20 2020 2020 2020 2054   = []..        T
-0001ab00: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001ab10: 2e61 7070 656e 6428 5472 6163 6b41 7474  .append(TrackAtt
-0001ab20: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
-0001ab30: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-0001ab40: 6962 7574 656e 616d 6520 696e 2074 7261  ibutename in tra
-0001ab50: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001ab60: 6b5f 6b65 7973 2e6b 6579 7328 293a 0d0a  k_keys.keys():..
-0001ab70: 2020 2020 2020 2020 2020 2020 5472 6163              Trac
-0001ab80: 6b41 7474 7269 6275 7465 6964 732e 6170  kAttributeids.ap
-0001ab90: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
-0001aba0: 6d65 2920 2020 200d 0a20 2020 200d 0a20  me)    ..    .. 
-0001abb0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001abc0: 6163 6b41 7474 7269 6275 7465 6964 732c  ackAttributeids,
-0001abd0: 2041 6c6c 5472 6163 6b56 616c 7565 730d   AllTrackValues.
-0001abe0: 0a20 2020 200d 0a64 6566 2067 6574 5f65  .    ..def get_e
-0001abf0: 6467 6573 5f64 6174 6173 6574 2865 6467  dges_dataset(edg
-0001ac00: 6573 5f64 6174 6173 6574 2c20 6564 6765  es_dataset, edge
-0001ac10: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
-0001ac20: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001ac30: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
-0001ac40: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-0001ac50: 6b65 7973 293a 0d0a 0d0a 2020 2020 2020  keys):....      
-0001ac60: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001ac70: 203d 207b 7d0d 0a20 2020 2020 2020 2074   = {}..        t
-0001ac80: 7261 636b 5f69 6420 3d20 7472 6163 6b5f  rack_id = track_
-0001ac90: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001aca0: 7973 5b22 7472 6163 6b5f 6964 225d 0d0a  ys["track_id"]..
-0001acb0: 2020 2020 2020 2020 5469 6420 3d20 6564          Tid = ed
-0001acc0: 6765 735f 6461 7461 7365 745b 7472 6163  ges_dataset[trac
-0001acd0: 6b5f 6964 5d2e 6173 7479 7065 2822 666c  k_id].astype("fl
-0001ace0: 6f61 7422 290d 0a20 2020 2020 2020 2069  oat")..        i
-0001acf0: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-0001ad00: 6528 5469 6420 3d3d 2030 290d 0a20 2020  e(Tid == 0)..   
-0001ad10: 2020 2020 206d 6178 7472 6163 6b5f 6964       maxtrack_id
-0001ad20: 203d 206d 6178 2854 6964 290d 0a20 2020   = max(Tid)..   
-0001ad30: 2020 2020 2063 6f6e 6469 7469 6f6e 5f69       condition_i
-0001ad40: 6e64 6963 6573 203d 2065 6467 6573 5f64  ndices = edges_d
-0001ad50: 6174 6173 6574 5f69 6e64 6578 5b69 6e64  ataset_index[ind
-0001ad60: 6963 6573 5d0d 0a20 2020 2020 2020 2054  ices]..        T
-0001ad70: 6964 5b63 6f6e 6469 7469 6f6e 5f69 6e64  id[condition_ind
-0001ad80: 6963 6573 5d20 3d20 6d61 7874 7261 636b  ices] = maxtrack
-0001ad90: 5f69 6420 2b20 310d 0a20 2020 2020 2020  _id + 1..       
-0001ada0: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
-0001adb0: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
-0001adc0: 0a0d 0a20 2020 2020 2020 2066 6f72 206b  ...        for k
-0001add0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001ade0: 6973 5f65 6467 6573 5f6b 6579 732e 7661  is_edges_keys.va
-0001adf0: 6c75 6573 2829 3a0d 0a0d 0a20 2020 2020  lues():....     
-0001ae00: 2020 2020 2020 2069 6620 6b20 213d 2074         if k != t
-0001ae10: 7261 636b 5f69 643a 0d0a 2020 2020 2020  rack_id:..      
-0001ae20: 2020 2020 2020 2020 2020 7820 3d20 6564            x = ed
-0001ae30: 6765 735f 6461 7461 7365 745b 6b5d 2e61  ges_dataset[k].a
-0001ae40: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001ae50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ae60: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001ae70: 5b6b 5d20 3d20 7820 2020 0d0a 2020 2020  [k] = x   ..    
-0001ae80: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-0001ae90: 6574 7572 6e20 416c 6c45 6467 6573 5661  eturn AllEdgesVa
-0001aea0: 6c75 6573 2020 200d 0a20 2020 200d 0a20  lues   ..    .. 
-0001aeb0: 2020 2020 2020 0d0a 2020 2020 0d0a 6465        ..    ..de
-0001aec0: 6620 7363 616c 655f 7661 6c75 6528 782c  f scale_value(x,
-0001aed0: 2073 6361 6c65 203d 2032 3535 202a 2032   scale = 255 * 2
-0001aee0: 3535 293a 0d0a 0d0a 0d0a 2020 2020 2072  55):......     r
-0001aef0: 6574 7572 6e20 7820 2a20 7363 616c 6520  eturn x * scale 
-0001af00: 2020 0d0a 2020 2020 0d0a 0d0a 0d0a 6465    ..    ......de
-0001af10: 6620 7072 6f62 5f73 6967 6d6f 6964 2878  f prob_sigmoid(x
-0001af20: 293a 0d0a 2020 2020 7265 7475 726e 2031  ):..    return 1
-0001af30: 202d 206d 6174 682e 6578 7028 2d78 290d   - math.exp(-x).
-0001af40: 0a0d 0a0d 0a64 6566 2061 6e67 756c 6172  .....def angular
-0001af50: 5f63 6861 6e67 6528 7665 635f 302c 2076  _change(vec_0, v
-0001af60: 6563 5f31 293a 0d0a 2020 2020 2020 2020  ec_1):..        
-0001af70: 0d0a 2020 2020 2020 2020 7665 635f 3020  ..        vec_0 
-0001af80: 3d20 7665 635f 3020 2f20 6e70 2e6c 696e  = vec_0 / np.lin
-0001af90: 616c 672e 6e6f 726d 2876 6563 5f30 290d  alg.norm(vec_0).
-0001afa0: 0a20 2020 2020 2020 2076 6563 5f31 203d  .        vec_1 =
-0001afb0: 2076 6563 5f31 202f 206e 702e 6c69 6e61   vec_1 / np.lina
-0001afc0: 6c67 2e6e 6f72 6d28 7665 635f 3129 0d0a  lg.norm(vec_1)..
-0001afd0: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-0001afe0: 6e70 2e61 7263 636f 7328 6e70 2e63 6c69  np.arccos(np.cli
-0001aff0: 7028 6e70 2e64 6f74 2876 6563 5f30 2c20  p(np.dot(vec_0, 
-0001b000: 7665 635f 3129 2c20 2d31 2e30 2c20 312e  vec_1), -1.0, 1.
-0001b010: 3029 290d 0a20 2020 2020 2020 2061 6e67  0))..        ang
-0001b020: 6c65 203d 2061 6e67 6c65 202a 2031 3830  le = angle * 180
-0001b030: 202f 206e 702e 7069 0d0a 2020 2020 2020   / np.pi..      
-0001b040: 2020 7265 7475 726e 2061 6e67 6c65 0d0a    return angle..
-0001b050: 2020 2020 200d 0a0d 0a64 6566 2065 7661       ....def eva
-0001b060: 6c5f 626f 6f6c 2876 616c 7565 293a 0d0a  l_bool(value):..
-0001b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b080: 2020 0d0a 2020 2020 2020 2020 6966 2076    ..        if v
-0001b090: 616c 7565 2020 3d3d 2027 5472 7565 273a  alue  == 'True':
-0001b0a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001b0b0: 2020 2064 6976 5f6b 6579 203d 2054 7275     div_key = Tru
-0001b0c0: 650d 0a20 2020 2020 2020 2065 6c73 653a  e..        else:
-0001b0d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b0e0: 2020 6469 765f 6b65 7920 3d20 4661 6c73    div_key = Fals
-0001b0f0: 6520 0d0a 0d0a 2020 2020 2020 2020 7265  e ....        re
-0001b100: 7475 726e 2064 6976 5f6b 6579 2020 2020  turn div_key    
-0001b110: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0001b120: 6465 6620 6368 6563 6b5f 616e 645f 7570  def check_and_up
-0001b130: 6461 7465 5f6d 6173 6b28 6d61 736b 2c69  date_mask(mask,i
-0001b140: 6d61 6765 293a 0d0a 2020 2020 2020 200d  mage):..       .
-0001b150: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001b160: 6d61 736b 2e73 6861 7065 2920 3c20 6c65  mask.shape) < le
-0001b170: 6e28 696d 6167 652e 7368 6170 6529 3a0d  n(image.shape):.
-0001b180: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
-0001b190: 6174 655f 6d61 736b 203d 206e 702e 7a65  ate_mask = np.ze
-0001b1a0: 726f 7328 0d0a 2020 2020 2020 2020 2020  ros(..          
-0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1c0: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-0001b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1e0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001b1f0: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-0001b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b210: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001b220: 655b 315d 2c0d 0a20 2020 2020 2020 2020  e[1],..         
-0001b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b240: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001b250: 7065 5b32 5d2c 0d0a 2020 2020 2020 2020  pe[2],..        
-0001b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b270: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001b280: 6170 655b 335d 2c0d 0a20 2020 2020 2020  ape[3],..       
-0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2a0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-0001b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2c0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0001b2d0: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0001b2e0: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001b2f0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-0001b300: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0001b310: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
-0001b320: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
-0001b330: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001b340: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001b350: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
-0001b360: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
-0001b370: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001b380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b390: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
-0001b3a0: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
-0001b3b0: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
-0001b3c0: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
-0001b3d0: 2020 0d0a                                  ..
+00018c90: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+00018ca0: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
+00018cb0: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
+00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cd0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018ce0: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+00018cf0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00018d00: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+00018d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018d20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018d30: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
+00018d40: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018d50: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2929  on_mitotic_acc))
+00018d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018d70: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018d80: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+00018d90: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+00018da0: 5f6d 6974 6f74 6963 5f61 6363 2929 0d0a  _mitotic_acc))..
+00018db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018dc0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018dd0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+00018de0: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00018df0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018e00: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+00018e10: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e30: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018e40: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00018e50: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018e60: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018e70: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00018e80: 6c5f 6368 616e 6765 2929 200d 0a0d 0a20  l_change)) .... 
+00018e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ea0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018eb0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
+00018ec0: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00018ed0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00018ee0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00018ef0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018f20: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00018f30: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00018f40: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018f50: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00018f60: 5f6d 6173 6b29 290d 0a0d 0a0d 0a20 2020  _mask))......   
+00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f80: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018f90: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+00018fa0: 6d65 616e 2861 6c6c 5f64 6973 705f 7a29  mean(all_disp_z)
+00018fb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018fc0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018fd0: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
+00018fe0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+00018ff0: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
+00019000: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019010: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00019020: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
+00019030: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+00019040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019050: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00019060: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00019070: 2e73 7464 2861 6c6c 5f64 6973 705f 7929  .std(all_disp_y)
+00019080: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019090: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000190a0: 6c5f 6d65 616e 5f64 6973 705f 782e 6170  l_mean_disp_x.ap
+000190b0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+000190c0: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
+000190d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000190e0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+000190f0: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
+00019100: 2861 6c6c 5f64 6973 705f 7829 290d 0a0d  (all_disp_x))...
+00019110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019120: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00019130: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
+00019140: 286e 702e 6d65 616e 2861 6c6c 5f72 6164  (np.mean(all_rad
+00019150: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
+00019160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019170: 616c 6c5f 7661 725f 7261 6469 7573 2e61  all_var_radius.a
+00019180: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00019190: 5f72 6164 6975 7329 290d 0a0d 0a20 2020  _radius))....   
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
+000191c0: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
+000191d0: 6561 6e28 616c 6c5f 7370 6565 6429 290d  ean(all_speed)).
+000191e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000191f0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00019200: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
+00019210: 702e 7374 6428 616c 6c5f 7370 6565 6429  p.std(all_speed)
+00019220: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019230: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019240: 6c5f 6d65 616e 5f61 6363 2e61 7070 656e  l_mean_acc.appen
+00019250: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6163  d(np.mean(all_ac
+00019260: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+00019270: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019280: 6c5f 7661 725f 6163 632e 6170 7065 6e64  l_var_acc.append
+00019290: 286e 702e 7374 6428 616c 6c5f 6163 6329  (np.std(all_acc)
+000192a0: 290d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  )........       
+000192b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000192c0: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+000192d0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+000192e0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+000192f0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019300: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00019310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019320: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
+00019330: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00019340: 6428 6e70 2e73 7464 2861 6c6c 5f64 6972  d(np.std(all_dir
+00019350: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00019360: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019370: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019380: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+00019390: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+000193a0: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+000193b0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+000193c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000193d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000193e0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+000193f0: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00019400: 2e73 7464 2861 6c6c 5f64 6973 7461 6e63  .std(all_distanc
+00019410: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019430: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00019440: 2020 2020 200d 0a64 6566 2062 6f75 6e64       ..def bound
+00019450: 6172 795f 706f 696e 7473 286d 6173 6b2c  ary_points(mask,
+00019460: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
+00019470: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
+00019480: 6c69 6272 6174 696f 6e29 3a0d 0a0d 0a20  libration):.... 
+00019490: 2020 206e 6469 6d20 3d20 6c65 6e28 6d61     ndim = len(ma
+000194a0: 736b 2e73 6861 7065 290d 0a20 2020 2074  sk.shape)..    t
+000194b0: 696d 6564 5f6d 6173 6b20 3d20 7b7d 0d0a  imed_mask = {}..
+000194c0: 2020 2020 6d61 736b 203d 206d 6173 6b20      mask = mask 
+000194d0: 3e20 300d 0a20 2020 206d 6173 6b20 3d20  > 0..    mask = 
+000194e0: 6d61 736b 2e61 7374 7970 6528 2775 696e  mask.astype('uin
+000194f0: 7438 2729 0d0a 2020 2020 2320 5958 2073  t8')..    # YX s
+00019500: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+00019510: 2020 6966 206e 6469 6d20 3d3d 2032 3a0d    if ndim == 2:.
+00019520: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00019530: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
+00019540: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
+00019550: 736b 290d 0a20 2020 2020 2020 2072 6567  sk)..        reg
+00019560: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
+00019570: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
+00019580: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
+00019590: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
+000195a0: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+000195b0: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+000195c0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+000195d0: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
+000195e0: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
+000195f0: 6573 2929 2e63 6f70 7928 290d 0a0d 0a20  es)).copy().... 
+00019600: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00019610: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+00019620: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+00019630: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019640: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+00019650: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019660: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
+00019670: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00019680: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00019690: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+000196a0: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
+000196b0: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+000196c0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+000196d0: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+000196e0: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
+000196f0: 2320 5468 6973 206f 626a 6563 7420 636f  # This object co
+00019700: 6e74 6169 6e73 206c 6973 7420 6f66 2061  ntains list of a
+00019710: 6c6c 2074 6865 2070 6f69 6e74 7320 666f  ll the points fo
+00019720: 7220 616c 6c20 7468 6520 6c61 6265 6c73  r all the labels
+00019730: 2069 6e20 7468 6520 4d61 736b 2069 6d61   in the Mask ima
+00019740: 6765 2077 6974 6820 7468 6520 6c61 6265  ge with the labe
+00019750: 6c20 6964 2061 6e64 2076 6f6c 756d 6520  l id and volume 
+00019760: 6f66 2065 6163 6820 6c61 6265 6c0d 0a20  of each label.. 
+00019770: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+00019780: 6b5b 7374 7228 3029 5d20 3d20 5b74 7265  k[str(0)] = [tre
+00019790: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+000197a0: 6f6e 6365 6e74 726f 6964 5d0d 0a0d 0a20  oncentroid].... 
+000197b0: 2020 2023 2054 5958 2073 6861 7065 6420     # TYX shaped 
+000197c0: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+000197d0: 6469 6d20 3d3d 2033 3a0d 0a0d 0a0d 0a20  dim == 3:...... 
+000197e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000197f0: 7471 646d 2872 616e 6765 2830 2c20 6d61  tqdm(range(0, ma
+00019800: 736b 2e73 6861 7065 5b30 5d29 293a 0d0a  sk.shape[0])):..
+00019810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019830: 2020 626f 756e 6461 7279 203d 2066 696e    boundary = fin
+00019840: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+00019850: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+00019860: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
+00019870: 656e 7472 6f69 6420 3d20 2830 2c29 202b  entroid = (0,) +
+00019880: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00019890: 6428 626f 756e 6461 7279 2920 0d0a 2020  d(boundary) ..  
+000198a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000198b0: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+000198c0: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
+000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198e0: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
+000198f0: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
+00019900: 7361 7272 6179 2869 6e64 6963 6573 2929  sarray(indices))
+00019910: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00019920: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
+00019930: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
+00019940: 2872 6561 6c5f 696e 6469 6365 7329 293a  (real_indices)):
+00019950: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019960: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019970: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
+00019980: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00019990: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+000199a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199b0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+000199c0: 5b6a 5d5b 315d 203d 2072 6561 6c5f 696e  [j][1] = real_in
+000199d0: 6469 6365 735b 6a5d 5b31 5d20 2a20 7863  dices[j][1] * xc
+000199e0: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
+000199f0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00019a00: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00019a10: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
+00019a20: 7329 0d0a 0d0a 2020 2020 2020 2020 2020  s)....          
+00019a30: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
+00019a40: 5b73 7472 2869 295d 203d 205b 7472 6565  [str(i)] = [tree
+00019a50: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
+00019a60: 6e63 656e 7472 6f69 645d 0d0a 2020 2020  ncentroid]..    
+00019a70: 2020 2020 2020 2020 0d0a 2020 2020 2320          ..    # 
+00019a80: 545a 5958 2073 6861 7065 6420 6f62 6a65  TZYX shaped obje
+00019a90: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00019aa0: 3d3d 2034 3a0d 0a20 2020 2020 2020 2070  == 4:..        p
+00019ab0: 7269 6e74 2827 4d61 736b 7320 6d61 6465  rint('Masks made
+00019ac0: 2069 6e74 6f20 6120 3444 2063 796c 696e   into a 4D cylin
+00019ad0: 6465 722c 2075 7027 290d 0a20 2020 2020  der, up')..     
+00019ae0: 2020 2062 6f75 6e64 6172 7920 3d20 6e70     boundary = np
+00019af0: 2e7a 6572 6f73 280d 0a20 2020 2020 2020  .zeros(..       
+00019b00: 2020 2020 205b 6d61 736b 2e73 6861 7065       [mask.shape
+00019b10: 5b30 5d2c 206d 6173 6b2e 7368 6170 655b  [0], mask.shape[
+00019b20: 315d 2c20 6d61 736b 2e73 6861 7065 5b32  1], mask.shape[2
+00019b30: 5d2c 206d 6173 6b2e 7368 6170 655b 335d  ], mask.shape[3]
+00019b40: 5d0d 0a20 2020 2020 2020 2029 0d0a 2020  ]..        )..  
+00019b50: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00019b60: 616e 6765 2830 2c20 6d61 736b 2e73 6861  ange(0, mask.sha
+00019b70: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+00019b80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00019b90: 2020 2062 6f75 6e64 6172 795b 692c 3a5d     boundary[i,:]
+00019ba0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
+00019bb0: 6573 286d 6173 6b5b 692c 3a5d 290d 0a20  es(mask[i,:]).. 
+00019bc0: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+00019bd0: 6e63 656e 7472 6f69 6420 3d20 636f 6d70  ncentroid = comp
+00019be0: 7574 655f 6365 6e74 726f 6964 2862 6f75  ute_centroid(bou
+00019bf0: 6e64 6172 795b 692c 3a5d 2920 0d0a 2020  ndary[i,:]) ..  
+00019c00: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00019c10: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00019c20: 6e64 6172 795b 692c 3a5d 203e 2030 290d  ndary[i,:] > 0).
+00019c30: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00019c40: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
+00019c50: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
+00019c60: 7261 7928 696e 6469 6365 7329 292e 636f  ray(indices)).co
+00019c70: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+00019c80: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00019c90: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+00019ca0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cc0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019cd0: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+00019ce0: 6573 5b6a 5d5b 305d 202a 207a 6361 6c69  es[j][0] * zcali
+00019cf0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019d00: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019d10: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019d20: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019d30: 5d5b 315d 202a 2079 6361 6c69 6272 6174  ][1] * ycalibrat
+00019d40: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00019d50: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019d60: 6469 6365 735b 6a5d 5b32 5d20 3d20 7265  dices[j][2] = re
+00019d70: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+00019d80: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+00019d90: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00019da0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+00019db0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+00019dc0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00019dd0: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
+00019de0: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
+00019df0: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
+00019e00: 726f 6964 5d0d 0a20 2020 2070 7269 6e74  roid]..    print
+00019e10: 2827 436f 6d70 7574 6564 2074 6865 2062  ('Computed the b
+00019e20: 6f75 6e64 6172 7920 706f 696e 7473 2729  oundary points')
+00019e30: 0d0a 0d0a 2020 2020 7265 7475 726e 2074  ....    return t
+00019e40: 696d 6564 5f6d 6173 6b2c 2062 6f75 6e64  imed_mask, bound
+00019e50: 6172 7920 2020 2020 2020 200d 0a0d 0a64  ary        ....d
+00019e60: 6566 2063 6f6d 7075 7465 5f63 656e 7472  ef compute_centr
+00019e70: 6f69 6428 6269 6e61 7279 5f69 6d61 6765  oid(binary_image
+00019e80: 293a 0d0a 2020 2020 2320 456e 7375 7265  ):..    # Ensure
+00019e90: 2062 696e 6172 7920 696d 6167 6520 6973   binary image is
+00019ea0: 2061 204e 756d 5079 2061 7272 6179 0d0a   a NumPy array..
+00019eb0: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
+00019ec0: 203d 206e 702e 6172 7261 7928 6269 6e61   = np.array(bina
+00019ed0: 7279 5f69 6d61 6765 290d 0a0d 0a20 2020  ry_image)....   
+00019ee0: 2077 6869 7465 5f70 6978 656c 7320 3d20   white_pixels = 
+00019ef0: 6e70 2e77 6865 7265 2862 696e 6172 795f  np.where(binary_
+00019f00: 696d 6167 6520 3d3d 2031 290d 0a20 2020  image == 1)..   
+00019f10: 206e 756d 5f70 6978 656c 7320 3d20 6c65   num_pixels = le
+00019f20: 6e28 7768 6974 655f 7069 7865 6c73 5b30  n(white_pixels[0
+00019f30: 5d29 0d0a 0d0a 2020 2020 2320 436f 6d70  ])....    # Comp
+00019f40: 7574 6520 7468 6520 6365 6e74 726f 6964  ute the centroid
+00019f50: 206f 6620 7468 6520 7768 6974 6520 7069   of the white pi
+00019f60: 7865 6c73 2069 6e20 7468 6520 626f 756e  xels in the boun
+00019f70: 6461 7279 2069 6d61 6765 0d0a 2020 2020  dary image..    
+00019f80: 6365 6e74 726f 6964 203d 206e 702e 7a65  centroid = np.ze
+00019f90: 726f 7328 6269 6e61 7279 5f69 6d61 6765  ros(binary_image
+00019fa0: 2e6e 6469 6d29 0d0a 2020 2020 666f 7220  .ndim)..    for 
+00019fb0: 6469 6d20 696e 2072 616e 6765 2862 696e  dim in range(bin
+00019fc0: 6172 795f 696d 6167 652e 6e64 696d 293a  ary_image.ndim):
+00019fd0: 0d0a 2020 2020 2020 2020 6365 6e74 726f  ..        centro
+00019fe0: 6964 5b64 696d 5d20 3d20 7768 6974 655f  id[dim] = white_
+00019ff0: 7069 7865 6c73 5b64 696d 5d2e 7375 6d28  pixels[dim].sum(
+0001a000: 2920 2f20 6e75 6d5f 7069 7865 6c73 0d0a  ) / num_pixels..
+0001a010: 0d0a 2020 2020 7265 7475 726e 2063 656e  ..    return cen
+0001a020: 7472 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a  troid........ ..
+0001a030: 0d0a 6465 6620 6765 745f 6373 765f 6461  ..def get_csv_da
+0001a040: 7461 2863 7376 293a 0d0a 0d0a 2020 2020  ta(csv):....    
+0001a050: 2020 2020 6461 7461 7365 7420 3d20 7064      dataset = pd
+0001a060: 2e72 6561 645f 6373 7628 0d0a 2020 2020  .read_csv(..    
+0001a070: 2020 2020 2020 2020 6373 762c 2064 656c          csv, del
+0001a080: 696d 6974 6572 3d22 2c22 2c20 656e 636f  imiter=",", enco
+0001a090: 6469 6e67 3d22 756e 6963 6f64 655f 6573  ding="unicode_es
+0001a0a0: 6361 7065 222c 206c 6f77 5f6d 656d 6f72  cape", low_memor
+0001a0b0: 793d 4661 6c73 650d 0a20 2020 2020 2020  y=False..       
+0001a0c0: 2029 5b33 3a5d 0d0a 2020 2020 2020 2020   )[3:]..        
+0001a0d0: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
+0001a0e0: 6461 7461 7365 742e 696e 6465 780d 0a20  dataset.index.. 
+0001a0f0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+0001a100: 7461 7365 742c 2064 6174 6173 6574 5f69  taset, dataset_i
+0001a110: 6e64 6578 0d0a 2020 2020 0d0a 6465 6620  ndex..    ..def 
+0001a120: 6765 745f 7370 6f74 5f64 6174 6173 6574  get_spot_dataset
+0001a130: 2873 706f 745f 6461 7461 7365 742c 2074  (spot_dataset, t
+0001a140: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a150: 6f74 5f6b 6579 732c 2078 6361 6c69 6272  ot_keys, xcalibr
+0001a160: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
+0001a170: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
+0001a180: 6e2c 2041 7474 7269 6275 7465 426f 786e  n, AttributeBoxn
+0001a190: 616d 652c 2064 6574 6563 7469 6f6e 6368  ame, detectionch
+0001a1a0: 616e 6e65 6c29 3a0d 0a20 2020 2020 2020  annel):..       
+0001a1b0: 2041 6c6c 5661 6c75 6573 203d 207b 7d0d   AllValues = {}.
+0001a1c0: 0a20 2020 2020 2020 2070 6f73 6978 203d  .        posix =
+0001a1d0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a1e0: 7370 6f74 5f6b 6579 735b 2270 6f73 6978  spot_keys["posix
+0001a1f0: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
+0001a200: 7920 3d20 7472 6163 6b5f 616e 616c 7973  y = track_analys
+0001a210: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+0001a220: 7369 7922 5d0d 0a20 2020 2020 2020 2070  siy"]..        p
+0001a230: 6f73 697a 203d 2074 7261 636b 5f61 6e61  osiz = track_ana
+0001a240: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a250: 2270 6f73 697a 225d 0d0a 2020 2020 2020  "posiz"]..      
+0001a260: 2020 6672 616d 6520 3d20 7472 6163 6b5f    frame = track_
+0001a270: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a280: 7973 5b22 6672 616d 6522 5d0d 0a20 2020  ys["frame"]..   
+0001a290: 2020 2020 200d 0a20 2020 2020 2020 204c       ..        L
+0001a2a0: 6f63 6174 696f 6e58 203d 2028 0d0a 2020  ocationX = (..  
+0001a2b0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a2c0: 6174 6173 6574 5b70 6f73 6978 5d2e 6173  ataset[posix].as
+0001a2d0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a2e0: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+0001a2f0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a300: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a310: 6f63 6174 696f 6e59 203d 2028 0d0a 2020  ocationY = (..  
+0001a320: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a330: 6174 6173 6574 5b70 6f73 6979 5d2e 6173  ataset[posiy].as
+0001a340: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a350: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+0001a360: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a370: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a380: 6f63 6174 696f 6e5a 203d 2028 0d0a 2020  ocationZ = (..  
+0001a390: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a3a0: 6174 6173 6574 5b70 6f73 697a 5d2e 6173  ataset[posiz].as
+0001a3b0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a3c0: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+0001a3d0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a3e0: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a3f0: 6f63 6174 696f 6e54 203d 2028 7370 6f74  ocationT = (spot
+0001a400: 5f64 6174 6173 6574 5b66 7261 6d65 5d2e  _dataset[frame].
+0001a410: 6173 7479 7065 2822 666c 6f61 7422 2929  astype("float"))
+0001a420: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+0001a430: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0001a440: 2020 2020 6967 6e6f 7265 5f76 616c 7565      ignore_value
+0001a450: 7320 3d20 5b74 7261 636b 5f61 6e61 6c79  s = [track_analy
+0001a460: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+0001a470: 6561 6e5f 696e 7465 6e73 6974 7922 5d2c  ean_intensity"],
+0001a480: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001a490: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
+0001a4a0: 696e 7465 6e73 6974 7922 5d5d 200d 0a20  intensity"]] .. 
+0001a4b0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+0001a4c0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
+0001a4d0: 6973 5f73 706f 745f 6b65 7973 2e69 7465  is_spot_keys.ite
+0001a4e0: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
+0001a4f0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
+0001a500: 6374 696f 6e63 6861 6e6e 656c 203d 3d20  ctionchannel == 
+0001a510: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0001a520: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
+0001a530: 2022 6d65 616e 5f69 6e74 656e 7369 7479   "mean_intensity
+0001a540: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
+0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a560: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
+0001a570: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a580: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
+0001a590: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
+0001a5c0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
+0001a5d0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
+0001a5e0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
+0001a5f0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001a600: 3d3d 2022 746f 7461 6c5f 696e 7465 6e73  == "total_intens
+0001a610: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
+0001a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a630: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
+0001a640: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001a650: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
+0001a660: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
+0001a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a680: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a690: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
+0001a6a0: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001a6b0: 2266 6c6f 6174 2229 2020 2020 2020 200d  "float")       .
+0001a6c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a6d0: 2020 2069 6620 7620 6e6f 7420 696e 2069     if v not in i
+0001a6e0: 676e 6f72 655f 7661 6c75 6573 3a0d 0a20  gnore_values:.. 
+0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a700: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a710: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001a720: 6c6c 5661 6c75 6573 5b76 5d20 3d20 7370  llValues[v] = sp
+0001a730: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+0001a740: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
+0001a750: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+0001a760: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
+0001a770: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
+0001a780: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001a790: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
+0001a7a0: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
+0001a7b0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001a7c0: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
+0001a7d0: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
+0001a7e0: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a7f0: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
+0001a800: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
+0001a810: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a820: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001a830: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001a840: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
+0001a850: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+0001a860: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+0001a870: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
+0001a880: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0001a890: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001a8a0: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001a8b0: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001a8c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001a8d0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001a8e0: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
+0001a8f0: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
+0001a900: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001a910: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
+0001a920: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
+0001a930: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a940: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+0001a950: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+0001a960: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
+0001a970: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
+0001a980: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001a990: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
+0001a9a0: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
+0001a9b0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a9c0: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
+0001a9d0: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
+0001a9e0: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
+0001a9f0: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
+0001aa00: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001aa10: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
+0001aa20: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
+0001aa30: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
+0001aa40: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
+0001aa50: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
+0001aa60: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001aa70: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
+0001aa80: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001aa90: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
+0001aaa0: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001aab0: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0001aac0: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
+0001aad0: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
+0001aae0: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
+0001aaf0: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
+0001ab00: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
+0001ab10: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
+0001ab20: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
+0001ab30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001ab40: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
+0001ab50: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
+0001ab60: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
+0001ab70: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
+0001ab80: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001ab90: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
+0001aba0: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+0001abb0: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+0001abc0: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+0001abd0: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
+0001abe0: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
+0001abf0: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
+0001ac00: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
+0001ac10: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0001ac20: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+0001ac30: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001ac40: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001ac50: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
+0001ac60: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
+0001ac70: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
+0001ac80: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
+0001ac90: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
+0001aca0: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
+0001acb0: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
+0001acc0: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
+0001acd0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001ace0: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001acf0: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
+0001ad00: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
+0001ad10: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
+0001ad20: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0001ad30: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001ad40: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
+0001ad50: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
+0001ad60: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
+0001ad70: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
+0001ad80: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001ad90: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+0001ada0: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
+0001adb0: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
+0001adc0: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
+0001add0: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
+0001ade0: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
+0001adf0: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
+0001ae00: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
+0001ae10: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
+0001ae20: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
+0001ae30: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
+0001ae40: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001ae50: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
+0001ae60: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
+0001ae70: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
+0001ae80: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001ae90: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
+0001aea0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0001aeb0: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
+0001aec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001aed0: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
+0001aee0: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
+0001aef0: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
+0001af00: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
+0001af10: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
+0001af20: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
+0001af30: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
+0001af40: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
+0001af50: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
+0001af60: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
+0001af70: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
+0001af80: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
+0001af90: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
+0001afa0: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
+0001afb0: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
+0001afc0: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
+0001afd0: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
+0001afe0: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
+0001aff0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+0001b000: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
+0001b010: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001b020: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
+0001b030: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+0001b040: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
+0001b050: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
+0001b060: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001b070: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
+0001b080: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
+0001b090: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
+0001b0a0: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
+0001b0b0: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
+0001b0c0: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
+0001b0d0: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
+0001b0e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001b0f0: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
+0001b100: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
+0001b110: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
+0001b120: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001b130: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
+0001b140: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
+0001b150: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
+0001b160: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
+0001b170: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001b180: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001b190: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
+0001b1a0: 2020 2020 2020 7265 7475 726e 2064 6976        return div
+0001b1b0: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
+0001b1c0: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
+0001b1d0: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+0001b1e0: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
+0001b1f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001b200: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
+0001b210: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
+0001b220: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
+0001b230: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001b240: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
+0001b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b260: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b280: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001b290: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
+0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2b0: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001b2c0: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
+0001b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001b2f0: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
+0001b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b320: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
+0001b330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b340: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b360: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001b370: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0001b380: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
+0001b390: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
+0001b3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b3b0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+0001b3c0: 302c 2075 7064 6174 655f 6d61 736b 2e73  0, update_mask.s
+0001b3d0: 6861 7065 5b31 5d29 3a0d 0a0d 0a20 2020  hape[1]):....   
+0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3f0: 2075 7064 6174 655f 6d61 736b 5b69 2c20   update_mask[i, 
+0001b400: 6a2c 203a 2c20 3a5d 203d 206d 6173 6b5b  j, :, :] = mask[
+0001b410: 692c 203a 2c20 3a5d 0d0a 2020 2020 2020  i, :, :]..      
+0001b420: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001b430: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001b440: 6d61 736b 203d 206d 6173 6b0d 0a0d 0a20  mask = mask.... 
+0001b450: 2020 2020 2020 2072 6574 7572 6e20 7570         return up
+0001b460: 6461 7465 5f6d 6173 6b20 2020 2020 2020  date_mask       
+0001b470: 200d 0a20 2020 2020 2020 0d0a             ..       ..
```

### Comparing `napatrackmater-3.5.2/napatrackmater/Trackvector.py` & `napatrackmater-3.5.3/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/__init__.py` & `napatrackmater-3.5.3/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/clustering.py` & `napatrackmater-3.5.3/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.5.3/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/fate_mapping.py` & `napatrackmater-3.5.3/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater/pretrained.py` & `napatrackmater-3.5.3/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.5.3/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.5.2
+Version: 3.5.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.5.2/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.5.3/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.5.2/setup.py` & `napatrackmater-3.5.3/setup.py`

 * *Files identical despite different names*

