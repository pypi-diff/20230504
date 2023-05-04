# Comparing `tmp/CVAugmentor-1.0.8.tar.gz` & `tmp/CVAugmentor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.8.tar", last modified: Mon May  1 07:18:20 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.9.tar", last modified: Mon May  1 07:31:43 2023, max compression
```

## Comparing `CVAugmentor-1.0.8.tar` & `CVAugmentor-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.839698 CVAugmentor-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.797703 CVAugmentor-1.0.8/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-05-01 07:17:55.000000 CVAugmentor-1.0.8/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.821698 CVAugmentor-1.0.8/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.8/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.830706 CVAugmentor-1.0.8/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.8/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26921 2023-05-01 06:45:51.000000 CVAugmentor-1.0.8/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.8/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.8/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.836698 CVAugmentor-1.0.8/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.8/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.8/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.8/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     7033 2023-05-01 07:17:52.000000 CVAugmentor-1.0.8/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:18:20.819697 CVAugmentor-1.0.8/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-01 07:18:20.000000 CVAugmentor-1.0.8/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-01 07:18:20.000000 CVAugmentor-1.0.8/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 07:18:20.000000 CVAugmentor-1.0.8/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-01 07:18:20.000000 CVAugmentor-1.0.8/CVAugmentor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 07:18:20.000000 CVAugmentor-1.0.8/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.8/LICENCE
--rw-rw-rw-   0        0        0     3318 2023-05-01 07:18:20.838698 CVAugmentor-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2763 2023-05-01 07:07:19.000000 CVAugmentor-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 07:18:20.839698 CVAugmentor-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-05-01 07:18:00.000000 CVAugmentor-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.288228 CVAugmentor-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.245230 CVAugmentor-1.0.9/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-05-01 07:29:10.000000 CVAugmentor-1.0.9/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.269231 CVAugmentor-1.0.9/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.9/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.278235 CVAugmentor-1.0.9/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.9/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26921 2023-05-01 06:45:51.000000 CVAugmentor-1.0.9/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.9/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.9/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.285232 CVAugmentor-1.0.9/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.9/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.9/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.9/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     7281 2023-05-01 07:30:51.000000 CVAugmentor-1.0.9/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:31:43.267233 CVAugmentor-1.0.9/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-01 07:31:43.000000 CVAugmentor-1.0.9/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-01 07:31:43.000000 CVAugmentor-1.0.9/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:31:43.000000 CVAugmentor-1.0.9/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-01 07:31:43.000000 CVAugmentor-1.0.9/CVAugmentor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 07:31:43.000000 CVAugmentor-1.0.9/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.9/LICENCE
+-rw-rw-rw-   0        0        0     3318 2023-05-01 07:31:43.287229 CVAugmentor-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2763 2023-05-01 07:07:19.000000 CVAugmentor-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:31:43.288228 CVAugmentor-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-05-01 07:29:13.000000 CVAugmentor-1.0.9/setup.py
```

### Comparing `CVAugmentor-1.0.8/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.9/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.9/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.9/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.9/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.9/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.9/CVAugmentor/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,22 @@
                         This means that the data will be saved only after all augmentations were applied.
 
         augmentations : dict
             Dict of augmentations to be applied to the data. 
             The keys are the names of the augmentations and the values are the augmentations themselves.
 
         verbose : bool, optional
+            If True, prints the overall progress of the augmentation process. The default is False.
+
+        aug_verbose : bool, optional
             If True, prints the progress of the augmentation process. The default is False.
 
+        warn_verbose : bool, optional
+            If True, prints the warnings. The default is False.
+
         
         Returns
         -------
         None.
         
         """
 
@@ -130,15 +136,15 @@
         else:
             raise ValueError(f"Invalid target type: {target}")
         
         # Augmentation
         if process_type == "batch":
             
             # Looping through the input files
-            for input_file in tqdm(self.sorted_alphanumeric(os.listdir(input_path)), desc='Overall Progress', unit=' Videos', leave=False, dynamic_ncols=True, diable=not verbose):
+            for input_file in tqdm(self.sorted_alphanumeric(os.listdir(input_path)), desc='Overall Progress', unit=' Videos', leave=False, dynamic_ncols=True, disable=not verbose):
                 
                 # Checking if the input file is valid
                 if not self.is_target_type(input_file, target):
 
                     if warn_verbose:
                         print(f"Skipping invalid input file: {input_file}")
```

### Comparing `CVAugmentor-1.0.8/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.9/CVAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.8/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.9/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/LICENCE` & `CVAugmentor-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/PKG-INFO` & `CVAugmentor-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.8/README.md` & `CVAugmentor-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.8/setup.py` & `CVAugmentor-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.8',
+        version='1.0.9',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

