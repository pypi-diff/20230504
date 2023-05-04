# Comparing `tmp/maxeqx-dc-webhook.py-1.0.5.tar.gz` & `tmp/maxeqx-dc-webhook.py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-webhook.py-1.0.5.tar", last modified: Thu May  4 19:36:04 2023, max compression
+gzip compressed data, was "maxeqx-dc-webhook.py-1.0.6.tar", last modified: Thu May  4 19:39:28 2023, max compression
```

## Comparing `maxeqx-dc-webhook.py-1.0.5.tar` & `maxeqx-dc-webhook.py-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 19:36:04.813960 maxeqx-dc-webhook.py-1.0.5/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2023-05-04 19:36:04.810427 maxeqx-dc-webhook.py-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 19:36:04.805924 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/
--rw-rw-rw-   0        0        0      626 2023-05-04 19:36:04.000000 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-04 19:36:04.000000 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 19:36:04.000000 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 19:36:04.000000 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 19:36:04.000000 maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 19:36:04.806687 maxeqx-dc-webhook.py-1.0.5/maxwebhook/
--rw-rw-rw-   0        0        0     1102 2023-05-04 19:30:07.000000 maxeqx-dc-webhook.py-1.0.5/maxwebhook/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 19:36:04.815346 maxeqx-dc-webhook.py-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-05-04 19:30:16.000000 maxeqx-dc-webhook.py-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:39:28.462308 maxeqx-dc-webhook.py-1.0.6/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2023-05-04 19:39:28.459324 maxeqx-dc-webhook.py-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 19:39:28.452746 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-05-04 19:39:28.000000 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-04 19:39:28.000000 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 19:39:28.000000 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 19:39:28.000000 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 19:39:28.000000 maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 19:39:28.454753 maxeqx-dc-webhook.py-1.0.6/maxwebhook/
+-rw-rw-rw-   0        0        0      705 2023-05-04 19:39:22.000000 maxeqx-dc-webhook.py-1.0.6/maxwebhook/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 19:39:28.462950 maxeqx-dc-webhook.py-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-05-04 19:38:17.000000 maxeqx-dc-webhook.py-1.0.6/setup.py
```

### Comparing `maxeqx-dc-webhook.py-1.0.5/LICENSE.txt` & `maxeqx-dc-webhook.py-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.5/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.5/README.txt` & `maxeqx-dc-webhook.py-1.0.6/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.5/maxeqx_dc_webhook.py.egg-info/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.6/maxeqx_dc_webhook.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.5/maxwebhook/__init__.py` & `maxeqx-dc-webhook.py-1.0.6/maxwebhook/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,23 +11,13 @@
     def send(self):     
         url = self.url
         data = {
             "content" : self.message,
             "username" : self.username,
             "avatar_url" : self.avatar_url
             }
-        datae = {
-            "username" : self.username,
-            "avatar_url" : self.avatar_url
-            }
-        datae["embed"] = [{
+        data["embed"] = [{
             "description" : self.embeddescription,
             "title" : self.embedtitle
         }]
-        if self.embeddescription or self.embedtitle != None:
-            result = requests.post(url, json = datae, headers={"Content-Type": "application/json"})
-
-            result.raise_for_status()
-        else:
-            result = requests.post(url, json = data, headers={"Content-Type": "application/json"})
-
-            result.raise_for_status()
+        result = requests.post(url, json = data)
+        result.raise_for_status()
```

### Comparing `maxeqx-dc-webhook.py-1.0.5/setup.py` & `maxeqx-dc-webhook.py-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-webhook.py',
-  version='1.0.5',
+  version='1.0.6',
   description='This is simple webhook sender in discord.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

