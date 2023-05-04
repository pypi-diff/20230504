# Comparing `tmp/material_zui-0.0.3.tar.gz` & `tmp/material_zui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.0.3.tar", last modified: Mon May  1 14:12:41 2023, max compression
+gzip compressed data, was "material_zui-0.0.4.tar", last modified: Thu May  4 07:38:15 2023, max compression
```

## Comparing `material_zui-0.0.3.tar` & `material_zui-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,47 @@
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.934539 material_zui-0.0.3/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 14:12:41.934539 material_zui-0.0.3/PKG-INFO
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/image/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      121 2023-04-30 11:48:20.000000 material_zui-0.0.3/image/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1604 2023-04-30 11:48:06.000000 material_zui-0.0.3/image/convert.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-04-28 09:55:18.000000 material_zui-0.0.3/image/data.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1392 2023-04-30 12:03:19.000000 material_zui-0.0.3/image/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      801 2023-04-29 15:11:22.000000 material_zui-0.0.3/image/remove_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      278 2023-04-29 15:11:37.000000 material_zui-0.0.3/image/transparent_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      249 2023-04-28 09:24:02.000000 material_zui-0.0.3/image/type.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     3842 2023-04-30 11:48:06.000000 material_zui-0.0.3/image/upscale.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/log/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-04-30 11:48:06.000000 material_zui-0.0.3/log/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      858 2023-04-28 04:39:06.000000 material_zui-0.0.3/log/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/material_zui.egg-info/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/PKG-INFO
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      557 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/SOURCES.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/dependency_links.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/requires.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       51 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/top_level.txt
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/replicate/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       43 2023-04-30 11:47:27.000000 material_zui-0.0.3/replicate/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1884 2023-04-30 14:10:18.000000 material_zui-0.0.3/replicate/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-01 14:12:41.934539 material_zui-0.0.3/setup.cfg
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      864 2023-05-01 14:11:46.000000 material_zui-0.0.3/setup.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/telegram_bot/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 15:00:34.000000 material_zui-0.0.3/telegram_bot/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-30 15:00:34.000000 material_zui-0.0.3/telegram_bot/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/text/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:27.000000 material_zui-0.0.3/text/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:27.000000 material_zui-0.0.3/text/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/tmp/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 11:48:06.000000 material_zui-0.0.3/tmp/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-28 03:39:00.000000 material_zui-0.0.3/tmp/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.934539 material_zui-0.0.3/validate/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:23.000000 material_zui-0.0.3/validate/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:23.000000 material_zui-0.0.3/validate/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.903938 material_zui-0.0.4/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      710 2023-05-04 07:38:15.903938 material_zui-0.0.4/PKG-INFO
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.891938 material_zui-0.0.4/crawl/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-02 13:44:44.000000 material_zui-0.0.4/crawl/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-02 13:44:44.000000 material_zui-0.0.4/crawl/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/image/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      162 2023-05-03 05:30:05.000000 material_zui-0.0.4/image/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1445 2023-05-03 14:42:30.000000 material_zui-0.0.4/image/combine.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1904 2023-05-03 05:27:27.000000 material_zui-0.0.4/image/convert.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-04-28 09:55:18.000000 material_zui-0.0.4/image/data.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1755 2023-05-03 05:42:32.000000 material_zui-0.0.4/image/index.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      801 2023-04-29 15:11:22.000000 material_zui-0.0.4/image/remove_background.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      278 2023-04-29 15:11:37.000000 material_zui-0.0.4/image/transparent_background.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      249 2023-04-28 09:24:02.000000 material_zui-0.0.4/image/type.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     4458 2023-05-03 14:24:10.000000 material_zui-0.0.4/image/upscale.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/language_model/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       48 2023-05-02 05:21:47.000000 material_zui-0.0.4/language_model/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      987 2023-05-02 05:36:54.000000 material_zui-0.0.4/language_model/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.895938 material_zui-0.0.4/log/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-04-30 11:48:06.000000 material_zui-0.0.4/log/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      858 2023-04-28 04:39:06.000000 material_zui-0.0.4/log/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/material_zui.egg-info/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      710 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/PKG-INFO
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      691 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/requires.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-05-04 07:38:15.000000 material_zui-0.0.4/material_zui.egg-info/top_level.txt
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/regex/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       39 2023-05-02 05:15:13.000000 material_zui-0.0.4/regex/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     5344 2023-05-02 05:18:47.000000 material_zui-0.0.4/regex/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/replicate/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       43 2023-04-30 11:47:27.000000 material_zui-0.0.4/replicate/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     2481 2023-05-01 15:33:18.000000 material_zui-0.0.4/replicate/index.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-04 07:38:15.903938 material_zui-0.0.4/setup.cfg
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      864 2023-05-04 07:36:57.000000 material_zui-0.0.4/setup.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/telegram_bot/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       46 2023-05-02 13:44:38.000000 material_zui-0.0.4/telegram_bot/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      129 2023-05-02 14:08:52.000000 material_zui-0.0.4/telegram_bot/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/time/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-02 14:46:45.000000 material_zui-0.0.4/time/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      692 2023-05-02 15:04:19.000000 material_zui-0.0.4/time/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.899938 material_zui-0.0.4/tmp/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 11:48:06.000000 material_zui-0.0.4/tmp/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-28 03:39:00.000000 material_zui-0.0.4/tmp/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-04 07:38:15.903938 material_zui-0.0.4/validate/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:23.000000 material_zui-0.0.4/validate/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:23.000000 material_zui-0.0.4/validate/index.py
```

### Comparing `material_zui-0.0.3/image/index.py` & `material_zui-0.0.4/image/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import os
+
+import cv2
+from cv2 import Mat
 from material_zui.image.data import IMG_EXT
 import requests
 
 # def get_image_sizes(directory_path: str) -> list[dict[{'name': str, 'width': int, 'height': int}]]:
 #     images = get_image(directory_path)
 #     images_name = get_image_name(directory_path)
 #     return [{'name': images_name[index], 'width':image.width, 'height':image.height}
@@ -17,16 +20,25 @@
 # def get_image(directory_path: str) -> list[ZuiImage]:
 #     images_name = get_image_name(directory_path)
 #     images = [Image.open(os.path.join(directory_path, file_name))
 #               for file_name in images_name]
 #     return [{'image': image, 'name': images_name[index], 'ext': image.format or '', 'width':image.width, 'height':image.height} for index, image in enumerate(images)]
 
 
-def get_image_name(directory_path: str) -> list[str]: return list(filter(lambda file_name: file_name.endswith(
+def get_image_names(directory_path: str) -> list[str]: return list(filter(lambda file_name: file_name.endswith(
     IMG_EXT), os.listdir(directory_path)))
 
 
+def get_image_paths(directory_path: str) -> list[str]:
+    images_name = get_image_names(directory_path)
+    return [os.path.join(directory_path, image_name) for image_name in images_name]
+
+
+def get_images(directory_path: str) -> list[Mat]: return [cv2.imread(
+    image_path) for image_path in get_image_paths(directory_path)]
+
+
 def download(url: str, path: str) -> None:
     '''Download image by url to path'''
     response = requests.get(url)
     with open(path, "wb") as f:
         f.write(response.content)
```

### Comparing `material_zui-0.0.3/image/remove_background.py` & `material_zui-0.0.4/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.3/image/upscale.py` & `material_zui-0.0.4/image/upscale.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import cv2
 import os
 from PIL import Image
+from cv2 import Mat
+from multipledispatch import dispatch
 from material_zui.image.data import MAX_MP
-from material_zui.image.index import get_image_name
+from material_zui.image.index import get_image_names
 from material_zui.image.type import ZuiImage, ZuiImageRes
 from material_zui.log import printTable
 
 
 def upscale(path:  str | bytes, newPath: str, wRatio: int = 1, hRatio: int = 1, newWidth: int = 0, newHeight: int = 0, isShowImage: bool = False):
     """
     Use AI to upscale image
@@ -58,39 +60,56 @@
 #     for index, image in enumerate(images):
 #         # new_path = os.path.join(path, str(index)+'.jpg')
 #         # new_path = os.path.join(path, "{}.{}".format(index, image.format))
 #         new_path = os.path.join(path, "{}.{}".format(index, 'jpg'))
 #         print(new_path, image.getim())
 #         image.save(new_path)
 
-
-def get_ratio_to_max_mp(width: int, height: int, max_mp: int = MAX_MP) -> int:
+@dispatch(int, int, int)
+def get_ratio_to_max_mp(width: int, height: int, max_mp: int = MAX_MP) -> int:  # type: ignore
     '''
     @max_mp: max size in megapixels
     '''
     to_width, to_height = width, height
     ratio = 1
     while (to_width*to_height < max_mp):
         ratio += 1
         to_width = width * ratio
         to_height = height * ratio
     return ratio
 
 
+# @dispatch(Mat, int)
+# def get_ratio_to_max_mp(image: Mat, max_mp: int = MAX_MP) -> int:
+#     '''
+#     @max_mp: max size in megapixels
+#     '''
+#     print('image', image)
+#     height, width = image.shape[:2]
+#     return get_ratio_to_max_mp(width, height, max_mp)  # type: ignore
+
+def get_image_ratio_to_max_mp(image: Mat, max_mp: int = MAX_MP) -> int:
+    '''
+    @max_mp: max size in megapixels
+    '''
+    height, width = image.shape[:2]
+    return get_ratio_to_max_mp(width, height, max_mp)  # type: ignore
+
+
 def upscales_dir_to_max_size(directory_path:  str, new_directory_path: str = '', max_mp: int = MAX_MP) -> list[ZuiImage]:
     '''
     @max_mp: max size in megapixels
     '''
     new_directory_path = new_directory_path if new_directory_path else directory_path
-    images_name = get_image_name(directory_path)
+    images_name = get_image_names(directory_path)
     images: list[ZuiImageRes] = []
     for image_name in images_name:
         image = cv2.imread(os.path.join(directory_path, image_name))
         height, width = image.shape[:2]
-        ratio = get_ratio_to_max_mp(width, height, max_mp)
+        ratio = get_ratio_to_max_mp(width, height, max_mp)  # type: ignore
         upscale_image = cv2.resize(
             image, None, fx=ratio, fy=ratio, interpolation=cv2.INTER_CUBIC)  # type: ignore
         images.append({'name': image_name, 'width': width,
                       'height': height, 'matImage': upscale_image, 'ratio': ratio})
     return images  # type: ignore
 
 
@@ -102,8 +121,7 @@
         directory_path, new_directory_path, max_mp)
     printTable({
         'Name': [info['name'] for info in images],
         'Width': [info['width'] for info in images],
         'Height': [info['height'] for info in images],
         'Ratio': [info['ratio'] for info in images],
     })
-    print("Done.")
```

### Comparing `material_zui-0.0.3/log/index.py` & `material_zui-0.0.4/log/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.3/material_zui.egg-info/PKG-INFO` & `material_zui-0.0.4/material_zui.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.0.3
+Version: 0.0.4
 Summary: Zui Material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # Modules
 
 <ol>
+  <li>Crawl</li>
   <li>Image</li>
+  <li>Language Model</li>
+  <li>Regex</li>
   <li>Log</li>
-  <li>Replicate</li>
+  <li>Replicate: AI API</li>
   <li>Telegram Bot</li>
+  <li>Validate</li>
 </ol>
 
 # Package
 
 - https://pypi.org/project/material-zui
```

### Comparing `material_zui-0.0.3/material_zui.egg-info/SOURCES.txt` & `material_zui-0.0.4/material_zui.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 setup.py
+crawl/__init__.py
+crawl/index.py
 image/__init__.py
+image/combine.py
 image/convert.py
 image/data.py
 image/index.py
 image/remove_background.py
 image/transparent_background.py
 image/type.py
 image/upscale.py
+language_model/__init__.py
+language_model/index.py
 log/__init__.py
 log/index.py
 material_zui.egg-info/PKG-INFO
 material_zui.egg-info/SOURCES.txt
 material_zui.egg-info/dependency_links.txt
 material_zui.egg-info/requires.txt
 material_zui.egg-info/top_level.txt
+regex/__init__.py
+regex/index.py
 replicate/__init__.py
 replicate/index.py
 telegram_bot/__init__.py
 telegram_bot/index.py
-text/__init__.py
-text/index.py
+time/__init__.py
+time/index.py
 tmp/__init__.py
 tmp/index.py
 validate/__init__.py
 validate/index.py
```

### Comparing `material_zui-0.0.3/replicate/index.py` & `material_zui-0.0.4/replicate/index.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,17 +35,35 @@
 
 
 def recover_old_photo(image_path: str, with_scratch: bool = False, HR: bool = False) -> str:
     '''https://replicate.com/microsoft/bringing-old-photos-back-to-life'''
     return replicate.run(
         "microsoft/bringing-old-photos-back-to-life:c75db81db6cbd809d93cc3b7e7a088a351a3349c9fa02b6d393e35e0d51ba799",
         input={"image": open(image_path, "rb"),
-               with_scratch: with_scratch, HR: HR}
+               "with_scratch": with_scratch, "HR": HR}
     )  # type: ignore
 
 
 def fill_color(image_path: str, classes: str = "88") -> list[dict[{'image': str}]]:
     '''https://replicate.com/cjwbw/bigcolor'''
     return replicate.run(
         "cjwbw/bigcolor:9451bfbf652b21a9bccc741e5c7046540faa5586cfa3aa45abc7dbb46151a4f7",
-        input={"image": open(image_path, "rb"), classes: classes}
+        input={"image": open(image_path, "rb"), "classes": classes}
     )  # type: ignore
+
+
+def face_restore(image_path: str, task: str = "Face Restoration", broken_image: bool = False) -> list[str]:
+    '''
+    https://replicate.com/yangxy/gpen
+    @task
+    Allowed values: `Face Restoration`, `Face Colorization`, `Face Inpainting`
+    Default value: `Face Restoration`
+    '''
+    return replicate.run(
+        "yangxy/gpen:cf4e15a70049c0119884eb2906c8ae8807af8317bea98313fefd941e414d0c91",
+        input={"image": open(image_path, "rb"), "task": task,
+               "broken_image": broken_image}
+    )  # type: ignore
+
+
+def tmp(dir_input: str, dir_output: str):
+    return 1
```

### Comparing `material_zui-0.0.3/setup.py` & `material_zui-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("readme.md", "r") as fh:
     # with open("src/material_zui/readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='material_zui',
-    version='0.0.3',
+    version='0.0.4',
     # url='https://github.com/username/my_module',
     author='chauhmnguyen',
     author_email='chauhoangminhnguyen@gmail.com',
     description='Zui Material',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
```

