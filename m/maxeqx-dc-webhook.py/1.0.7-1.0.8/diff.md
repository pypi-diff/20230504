# Comparing `tmp/maxeqx-dc-webhook.py-1.0.7.tar.gz` & `tmp/maxeqx-dc-webhook.py-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-webhook.py-1.0.7.tar", last modified: Thu May  4 19:47:09 2023, max compression
+gzip compressed data, was "maxeqx-dc-webhook.py-1.0.8.tar", last modified: Thu May  4 20:12:39 2023, max compression
```

## Comparing `maxeqx-dc-webhook.py-1.0.7.tar` & `maxeqx-dc-webhook.py-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 19:47:09.453264 maxeqx-dc-webhook.py-1.0.7/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2023-05-04 19:47:09.453264 maxeqx-dc-webhook.py-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 19:47:09.453264 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/
--rw-rw-rw-   0        0        0      626 2023-05-04 19:47:09.000000 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-04 19:47:09.000000 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 19:47:09.000000 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 19:47:09.000000 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 19:47:09.000000 maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 19:47:09.453264 maxeqx-dc-webhook.py-1.0.7/maxwebhook/
--rw-rw-rw-   0        0        0      812 2023-05-04 19:45:26.000000 maxeqx-dc-webhook.py-1.0.7/maxwebhook/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 19:47:09.453264 maxeqx-dc-webhook.py-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-05-04 19:46:56.000000 maxeqx-dc-webhook.py-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.273499 maxeqx-dc-webhook.py-1.0.8/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2023-05-04 20:12:39.268501 maxeqx-dc-webhook.py-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.263999 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 20:12:39.000000 maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 20:12:39.265499 maxeqx-dc-webhook.py-1.0.8/maxwebhook/
+-rw-rw-rw-   0        0        0     1732 2023-05-04 20:10:21.000000 maxeqx-dc-webhook.py-1.0.8/maxwebhook/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:12:39.273999 maxeqx-dc-webhook.py-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-05-04 19:59:09.000000 maxeqx-dc-webhook.py-1.0.8/setup.py
```

### Comparing `maxeqx-dc-webhook.py-1.0.7/LICENSE.txt` & `maxeqx-dc-webhook.py-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.7/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.7
+Version: 1.0.8
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.7/README.txt` & `maxeqx-dc-webhook.py-1.0.8/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.7/maxeqx_dc_webhook.py.egg-info/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.8/maxeqx_dc_webhook.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.7
+Version: 1.0.8
 Summary: This is simple webhook sender in discord.
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.7/maxwebhook/__init__.py` & `maxeqx-dc-webhook.py-1.0.8/maxwebhook/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,24 +6,46 @@
         self.username : str = None
         self.avatar_url : str = None
         self.message : str = None
         self.embedtitle : str = None
         self.embeddescription : str = None
     def send(self):     
         url = self.url
-        embed = {
-        "description": self.embeddescription,
-        "title": self.embedtitle
-        }
-        data = {
-            "content" : self.message,
-            "username" : self.username,
-            "avatar_url" : self.avatar_url,
-            "embeds": [embed]
-            }
 
         headers = {
         "Content-Type": "application/json"
         }
 
-        result = requests.post(url, json=data, headers=headers)
-        result.raise_for_status()
+        if self.embeddescription or self.embedtitle != None:
+            embed = {
+            "description": self.embeddescription,
+            "title": self.embedtitle
+            }
+            data = {
+            "username" : self.username,
+            "avatar_url" : self.avatar_url,
+            "embeds": [embed]
+            }
+            result = requests.post(url, json=data, headers=headers)
+            result.raise_for_status()
+        elif self.embeddescription and self.embedtitle and self.message != None:
+            embed = {
+            "description": self.embeddescription,
+            "title": self.embedtitle,
+            "content": self.message
+            }
+            data = {
+            "username" : self.username,
+            "avatar_url" : self.avatar_url,
+            "embeds": [embed]
+            }
+            result = requests.post(url, json=data, headers=headers)
+            result.raise_for_status()
+        else:
+            if self.message != None:
+                data = {
+                    "username" : self.username,
+                    "avatar_url" : self.avatar_url,
+                    "content" : self.message
+                }
+                result = requests.post(url, json=data, headers=headers)
+                result.raise_for_status
```

### Comparing `maxeqx-dc-webhook.py-1.0.7/setup.py` & `maxeqx-dc-webhook.py-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-webhook.py',
-  version='1.0.7',
+  version='1.0.8',
   description='This is simple webhook sender in discord.',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

