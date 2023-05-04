# Comparing `tmp/katalytic-images-0.2.2.tar.gz` & `tmp/katalytic-images-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.2.2.tar", last modified: Mon May  1 12:36:43 2023, max compression
+gzip compressed data, was "katalytic-images-0.3.0.tar", last modified: Thu May  4 17:58:36 2023, max compression
```

## Comparing `katalytic-images-0.2.2.tar` & `katalytic-images-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-05-01 07:17:35.782858 katalytic-images-0.2.2/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 12:19:15.021593 katalytic-images-0.2.2/.gitignore
--rw-r--r--   0        0        0     3324 2023-05-01 07:17:35.782858 katalytic-images-0.2.2/.gitlab-ci.yml
--rw-r--r--   0        0        0     1571 2023-05-01 12:36:40.486378 katalytic-images-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-05-01 07:17:35.782858 katalytic-images-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2130 2023-05-01 07:17:35.782858 katalytic-images-0.2.2/README.md
--rw-r--r--   0        0        0     1503 2023-05-01 12:36:40.486378 katalytic-images-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6786 2023-05-01 12:35:02.246362 katalytic-images-0.2.2/src/katalytic/images.py
--rw-r--r--   0        0        0    11945 2023-05-01 12:19:15.021593 katalytic-images-0.2.2/tests/test_images.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 katalytic-images-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.3.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3324 2023-04-30 14:15:39.110597 katalytic-images-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1912 2023-05-04 17:58:14.314350 katalytic-images-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.3.0/README.md
+-rw-r--r--   0        0        0     1551 2023-05-04 17:58:14.298350 katalytic-images-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7582 2023-05-02 05:00:49.687540 katalytic-images-0.3.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    13039 2023-05-01 19:23:22.988107 katalytic-images-0.3.0/tests/test_images.py
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 katalytic-images-0.3.0/PKG-INFO
```

### Comparing `katalytic-images-0.2.2/.gitignore` & `katalytic-images-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.2/.gitlab-ci.yml` & `katalytic-images-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.2/CHANGELOG.md` & `katalytic-images-0.3.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.3.0 (2023-05-04)
+### feat
+- [[`d824d98`](https://gitlab.com/katalytic/katalytic-images/commit/d824d989ce58efd8ffe644e2527d02952a230a92)] **draw:** add more shape types
+- [[`62be07d`](https://gitlab.com/katalytic/katalytic-images/commit/62be07dfbc5aca96d490732eaa421d6083c5d663)] **draw:** implement 'mask' and 'polylines' shape types
+
+
 ## 0.2.2 (2023-05-01)
 ### fix
 - [[`acf64bf`](https://gitlab.com/katalytic/katalytic-images/commit/acf64bf7dd6a9cac64d83403bc4eb33a2eec9119)] **draw:** KeyError: "background"
 
 
 ## 0.2.1 (2023-05-01)
 ### fix
```

### Comparing `katalytic-images-0.2.2/LICENSE.txt` & `katalytic-images-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.2/README.md` & `katalytic-images-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.2/pyproject.toml` & `katalytic-images-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.2.2"
+version = "0.3.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -24,25 +24,27 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
+    "katalytic-checks>=0.1.1",
     "katalytic-files>=0.3.0",
     "katalytic-pkg>=0.2.0",
     "numpy>=1.14",
-    "opencv-python>=4.0.0,<4.7",
+    "opencv-python>=4.0.0",
     "pillow>=8.4.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
+    "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-images.git"
 repository = "https://gitlab.com/katalytic/katalytic-images.git"
```

### Comparing `katalytic-images-0.2.2/src/katalytic/images.py` & `katalytic-images-0.3.0/src/katalytic/images.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,14 +83,26 @@
         if shape['type'] == 'text':
             # extract background info only after the call to
             # _insert_defaults() and _rename_kwargs()
             # Otherwise you might miscalculate the bg size and position
             bg = _get_text_bg(shape)
             if bg:
                 draw_inplace(image, bg)
+        elif shape['type'] in ('mask', 'polylines'):
+            pts = shape['pts']
+            if is_iterable(pts):
+                if not is_iterable(pts[0][0]):
+                    pts = [pts]
+
+            if not isinstance(pts, np.ndarray):
+                pts = np.array(pts, dtype=np.int32)
+            elif pts.dtype != np.int32:
+                pts = pts.astype(np.int32)
+
+            shape['pts'] = pts
 
         del shape['type']
         draw_shape(image, **shape)
 
 
 def _get_text_bg(text):
     bg = text.pop('background', None)
@@ -142,44 +154,53 @@
         'font': 'fontFace',
         'font_scale': 'fontScale',
         'line_type': 'lineType',
         'draw_above_origin': 'bottomLeftOrigin',
         'p1': 'pt1',
         'p2': 'pt2',
         'origin': 'org',
+        'is_closed': 'isClosed',
     }
 
     return {conversion.get(k, k): v for k, v in shape.items()}
 
 
 def _pick_draw_function(shape_type):
     fn = {
+        'arrowed_line': cv2.arrowedLine,
         'circle': cv2.circle,
+        'contours': cv2.drawContours,
+        'convex_polygon': cv2.fillConvexPoly,
+        'ellipse': cv2.ellipse,
+        'ellipse_polygon': cv2.ellipse2Poly,
         'line': cv2.line,
+        'marker': cv2.drawMarker,
+        'mask': cv2.fillPoly,
+        'polylines': cv2.polylines,
         'rectangle': cv2.rectangle,
         'text': cv2.putText,
     }
 
     if shape_type not in fn:
         raise ValueError(f'Unknown shape: {shape_type!r}')
     else:
         return fn[shape_type]
 
 
 def _insert_defaults(shape):
     defaults = {
         'circle': {'thickness': -1},
-        'line': {},
+        'line': {'thickness': 3},
         'rectangle': {'thickness': -1},
         'text': {
             'font': cv2.FONT_HERSHEY_SIMPLEX,
             'font_scale': 1.25,
             'thickness': 3,
         },
-        'polygon': {},
+        'polylines': {'is_closed': True, 'thickness': 3},
     }
 
     return {**defaults.get(shape['type'], {}), **shape}
 
 
 @mark('load::png')
 @mark('load::jpg')
```

### Comparing `katalytic-images-0.2.2/tests/test_images.py` & `katalytic-images-0.3.0/tests/test_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,14 +209,31 @@
         }
 
         processed = draw(original, shape)
         assert not are_arrays_equal(original, processed)
         assert (processed == text_color).any()
         assert (processed == bg_color).any()
 
+    @pytest.mark.parametrize('shape', [
+        {'type': 'mask', 'pts': [(100,100), (250,250), (250,100), (150,200)]},
+        {'type': 'mask', 'pts': [[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))]},
+        {'type': 'mask', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]])},
+        {'type': 'mask', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8)},
+        {'type': 'polylines', 'pts': [(100,100), (250,250), (250,100), (150,200)]},
+        {'type': 'polylines', 'pts': [[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))]},
+        {'type': 'polylines', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]])},
+        {'type': 'polylines', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8)},
+    ])
+    def test_masks_and_polylines(self, shape):
+        shape['color'] = (0, 255, 0)
+
+        original = 255 * np.ones((1000, 1000, 3), dtype=np.uint8)
+        processed = draw(original, shape)
+        assert not are_arrays_equal(original, processed)
+
 
 class Test_are_arrays_equal:
     @pytest.mark.parametrize('img_1, img_2', [
         (_create_RGB(), _create_RGB()),
         (_create_RGB(np.float32), _create_RGB(np.uint8)),
         (_create_RGB(np.float32), _create_RGB(np.uint8)),
         (np.array([[0,1], [2,3]]), np.array([[0,1], [2,3]])),
```

### Comparing `katalytic-images-0.2.2/PKG-INFO` & `katalytic-images-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.2.2
+Version: 0.3.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,21 +14,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Requires-Dist: katalytic-checks>=0.1.1
 Requires-Dist: katalytic-files>=0.3.0
 Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: numpy>=1.14
-Requires-Dist: opencv-python>=4.0.0,<4.7
+Requires-Dist: opencv-python>=4.0.0
 Requires-Dist: pillow>=8.4.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-images.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-images.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
```

