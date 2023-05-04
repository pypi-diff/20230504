# Comparing `tmp/maxeqx-dc-webhook.py-1.0.3.tar.gz` & `tmp/maxeqx-dc-webhook.py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxeqx-dc-webhook.py-1.0.3.tar", last modified: Thu May  4 18:59:37 2023, max compression
+gzip compressed data, was "maxeqx-dc-webhook.py-1.0.4.tar", last modified: Thu May  4 19:00:31 2023, max compression
```

## Comparing `maxeqx-dc-webhook.py-1.0.3.tar` & `maxeqx-dc-webhook.py-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:59:37.453424 maxeqx-dc-webhook.py-1.0.3/
--rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      655 2023-05-04 18:59:37.440730 maxeqx-dc-webhook.py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 18:59:37.436962 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-04 18:59:36.000000 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-04 18:59:37.000000 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 18:59:36.000000 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 18:59:36.000000 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 18:59:37.000000 maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 18:59:37.438901 maxeqx-dc-webhook.py-1.0.3/maxwebhook/
--rw-rw-rw-   0        0        0      498 2023-05-04 17:43:05.000000 maxeqx-dc-webhook.py-1.0.3/maxwebhook/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 18:59:37.453921 maxeqx-dc-webhook.py-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-05-04 18:59:20.000000 maxeqx-dc-webhook.py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 19:00:31.694408 maxeqx-dc-webhook.py-1.0.4/
+-rw-rw-rw-   0        0        0     1051 2023-05-04 14:40:55.000000 maxeqx-dc-webhook.py-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 14:44:57.000000 maxeqx-dc-webhook.py-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      655 2023-05-04 19:00:31.692542 maxeqx-dc-webhook.py-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-04 18:20:45.000000 maxeqx-dc-webhook.py-1.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 19:00:31.687626 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-04 19:00:31.000000 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-04 19:00:31.000000 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 19:00:31.000000 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 19:00:31.000000 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 19:00:31.000000 maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 19:00:31.689624 maxeqx-dc-webhook.py-1.0.4/maxwebhook/
+-rw-rw-rw-   0        0        0      860 2023-05-04 19:00:06.000000 maxeqx-dc-webhook.py-1.0.4/maxwebhook/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 19:00:31.695397 maxeqx-dc-webhook.py-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-05-04 19:00:21.000000 maxeqx-dc-webhook.py-1.0.4/setup.py
```

### Comparing `maxeqx-dc-webhook.py-1.0.3/LICENSE.txt` & `maxeqx-dc-webhook.py-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.3/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is simple webhook sender in discord. (Version 1.0.3 adding embed)
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.3/README.txt` & `maxeqx-dc-webhook.py-1.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `maxeqx-dc-webhook.py-1.0.3/maxeqx_dc_webhook.py.egg-info/PKG-INFO` & `maxeqx-dc-webhook.py-1.0.4/maxeqx_dc_webhook.py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxeqx-dc-webhook.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is simple webhook sender in discord. (Version 1.0.3 adding embed)
 Home-page: 
 Author: maxeqx
 Author-email: maxeqxmail@gmail.com
 License: MIT
 Keywords: discord webhook sender
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `maxeqx-dc-webhook.py-1.0.3/setup.py` & `maxeqx-dc-webhook.py-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='maxeqx-dc-webhook.py',
-  version='1.0.3',
+  version='1.0.4',
   description='This is simple webhook sender in discord. (Version 1.0.3 adding embed)',
   long_description="Long description and usage is on my github: https://github.com/makseksowny/maxeqx-dc-webhook.",
   url='',  
   author='maxeqx',
   author_email='maxeqxmail@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

