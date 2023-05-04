# Comparing `tmp/vision_explanation_methods-0.0.6.tar.gz` & `tmp/vision_explanation_methods-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_explanation_methods-0.0.6.tar", last modified: Tue Apr 25 17:33:55 2023, max compression
+gzip compressed data, was "vision_explanation_methods-0.0.7.tar", last modified: Thu May  4 16:07:01 2023, max compression
```

## Comparing `vision_explanation_methods-0.0.6.tar` & `vision_explanation_methods-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/DRISE_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/drise.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 17:13:07.000000 vision_explanation_methods-0.0.6/vision_explanation_methods/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:33:55.266099 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 17:33:55.000000 vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.806374 vision_explanation_methods-0.0.7/vision_explanation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/DRISE_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/drise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.806374 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/top_level.txt
```

### Comparing `vision_explanation_methods-0.0.6/LICENSE.txt` & `vision_explanation_methods-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.6/PKG-INFO` & `vision_explanation_methods-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_explanation_methods
-Version: 0.0.6
+Version: 0.0.7
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.6/README.md` & `vision_explanation_methods-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.6/setup.py` & `vision_explanation_methods-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.6/vision_explanation_methods/DRISE_runner.py` & `vision_explanation_methods-0.0.7/vision_explanation_methods/DRISE_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,18 +186,15 @@
     saliency_scores = [saliency_scores[img_index][i]
                        for i in range(len(saliency_scores[img_index]))
                        if not torch.isnan(
                        saliency_scores[img_index][i]['detection']).any()]
 
     num_detections = len(saliency_scores)
     if num_detections == 0:
-        print("No detections found. Saving empty figure.")
-        fail = Image.new('RGB', (100, 100))
-        fail = fail.save(savename)
-        return None, None, None
+        raise ValueError("No detections found")
 
     label_list = []
     fig_list = []
     for i in range((max_figures if num_detections > max_figures
                     else num_detections)):
         fig, ax = plt.subplots(1, 1, figsize=(10, 10))
         label = int(torch.argmax(detections[img_index].class_scores[i]))
@@ -213,11 +210,16 @@
             show_colorbar=True,
             cmap=plt.cm.gist_rainbow,
             title="Detection " + str(i),
             plt_fig_axis=(fig, ax),
             use_pyplot=False
         )
 
+        stream = BytesIO()
+        plt.savefig(stream, format='jpg')
+        stream.seek(0)
+        b64_string = base64.b64encode(stream.read()).decode()
+        fig_list.append(b64_string)
         fig.savefig(savename+str(i)+IMAGE_TYPE)
         fig.clear()
-        fig_list.append(fig)
+
     return fig_list, savename, label_list
```

### Comparing `vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/common.py` & `vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/common.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.6/vision_explanation_methods/explanations/drise.py` & `vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/drise.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/PKG-INFO` & `vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-explanation-methods
-Version: 0.0.6
+Version: 0.0.7
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.6/vision_explanation_methods.egg-info/SOURCES.txt` & `vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

