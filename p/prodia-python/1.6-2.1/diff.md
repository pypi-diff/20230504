# Comparing `tmp/prodia-python-1.6.tar.gz` & `tmp/prodia-python-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodia-python-1.6.tar", last modified: Fri Apr 21 19:13:22 2023, max compression
+gzip compressed data, was "prodia-python-2.1.tar", last modified: Thu May  4 11:25:10 2023, max compression
```

## Comparing `prodia-python-1.6.tar` & `prodia-python-2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.367084 prodia-python-1.6/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-1.6/LICENSE
--rw-rw-rw-   0        0        0     1741 2023-04-21 19:13:22.366566 prodia-python-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1515 2023-04-21 19:12:58.000000 prodia-python-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.358615 prodia-python-1.6/prodia/
--rw-rw-rw-   0        0        0       35 2023-04-21 18:53:57.000000 prodia-python-1.6/prodia/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-04-21 19:12:05.000000 prodia-python-1.6/prodia/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:13:22.365075 prodia-python-1.6/prodia_python.egg-info/
--rw-rw-rw-   0        0        0     1741 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 19:13:22.000000 prodia-python-1.6/prodia_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 19:13:22.367084 prodia-python-1.6/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-04-21 19:12:54.000000 prodia-python-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.723214 prodia-python-2.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-2.1/LICENSE
+-rw-rw-rw-   0        0        0     2010 2023-05-04 11:25:10.722539 prodia-python-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1784 2023-05-04 11:03:56.000000 prodia-python-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.707355 prodia-python-2.1/prodia/
+-rw-rw-rw-   0        0        0       76 2023-05-04 10:55:14.000000 prodia-python-2.1/prodia/__init__.py
+-rw-rw-rw-   0        0        0     4782 2023-05-04 10:55:14.000000 prodia-python-2.1/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.721336 prodia-python-2.1/prodia_python.egg-info/
+-rw-rw-rw-   0        0        0     2010 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 11:25:10.723214 prodia-python-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-05-04 11:24:52.000000 prodia-python-2.1/setup.py
```

### Comparing `prodia-python-1.6/LICENSE` & `prodia-python-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodia-python-1.6/PKG-INFO` & `prodia-python-2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 1.6
+Version: 2.1
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install git+https://github.com/yoou3-cyber/prodia-python
-```
-or
-```
-pip install prodia-python==1.6
+pip install prodia-python==2.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
-### Example of usage
+### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.run(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
+### Example of img2img usage
+```python
+import prodia
+
+key = 'your-prodia-key'
+
+image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
+
+image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+
+print(image)
+```
+
 ### Additional info
 prodia.run() have arguments:
 - `key` - string Prodia API key(required)
 - `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is blank)
-- `model` - string(you can see al available models on https://docs.prodia.com/reference/generate, default is v1-5-pruned-emaonly.ckpt [81761151])
+- `negative_prompt` - string for negative tags(default is "badly drawn")
+- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
 - `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-30, default is 25
+- `steps` - integer, 1-50, default is 25
 - `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Euler)
+- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
 - `seed` - integer(default -1, it generates images with random seed)
 - `upscale` - boolean of 2x upscaling(default False)
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodia-python-1.6/README.md` & `prodia-python-2.1/prodia_python.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,59 @@
+Metadata-Version: 2.1
+Name: prodia-python
+Version: 2.1
+Summary: Prodia API Python Wrapper
+Author: yoou3-cyber
+Author-email: zenafey@eugw.ru
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install git+https://github.com/yoou3-cyber/prodia-python
-```
-or
-```
-pip install prodia-python==1.6
+pip install prodia-python==2.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
-### Example of usage
+### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.run(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
+### Example of img2img usage
+```python
+import prodia
+
+key = 'your-prodia-key'
+
+image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
+
+image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+
+print(image)
+```
+
 ### Additional info
 prodia.run() have arguments:
 - `key` - string Prodia API key(required)
 - `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is blank)
-- `model` - string(you can see al available models on https://docs.prodia.com/reference/generate, default is v1-5-pruned-emaonly.ckpt [81761151])
+- `negative_prompt` - string for negative tags(default is "badly drawn")
+- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
 - `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-30, default is 25
+- `steps` - integer, 1-50, default is 25
 - `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Euler)
+- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
 - `seed` - integer(default -1, it generates images with random seed)
 - `upscale` - boolean of 2x upscaling(default False)
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodia-python-1.6/prodia_python.egg-info/PKG-INFO` & `prodia-python-2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-Metadata-Version: 2.1
-Name: prodia-python
-Version: 1.6
-Summary: Prodia API Python Wrapper
-Author: yoou3-cyber
-Author-email: zenafey@eugw.ru
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install git+https://github.com/yoou3-cyber/prodia-python
-```
-or
-```
-pip install prodia-python==1.6
+pip install prodia-python==2.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
-### Example of usage
+### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.run(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
+### Example of img2img usage
+```python
+import prodia
+
+key = 'your-prodia-key'
+
+image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
+
+image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+
+print(image)
+```
+
 ### Additional info
 prodia.run() have arguments:
 - `key` - string Prodia API key(required)
 - `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is blank)
-- `model` - string(you can see al available models on https://docs.prodia.com/reference/generate, default is v1-5-pruned-emaonly.ckpt [81761151])
+- `negative_prompt` - string for negative tags(default is "badly drawn")
+- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
 - `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-30, default is 25
+- `steps` - integer, 1-50, default is 25
 - `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Euler)
+- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
 - `seed` - integer(default -1, it generates images with random seed)
 - `upscale` - boolean of 2x upscaling(default False)
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

