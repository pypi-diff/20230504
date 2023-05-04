# Comparing `tmp/reviewbot-extension-3.1.1.tar.gz` & `tmp/reviewbot-extension-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviewbot-extension-3.1.1.tar", last modified: Wed Jul 27 03:05:39 2022, max compression
+gzip compressed data, was "reviewbot-extension-3.2.tar", last modified: Thu May  4 02:38:52 2023, max compression
```

## Comparing `reviewbot-extension-3.1.1.tar` & `reviewbot-extension-3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.915538 reviewbot-extension-3.1.1/
--rw-r--r--   0 chipx86    (501) staff       (20)       48 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/MANIFEST.in
--rw-r--r--   0 chipx86    (501) staff       (20)     6197 2022-07-27 03:05:39.915611 reviewbot-extension-3.1.1/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     5025 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/README.rst
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.913007 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     6197 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)      945 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       79 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/entry_points.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2022-07-27 03:05:29.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/not-zip-safe
--rw-r--r--   0 chipx86    (501) staff       (20)      179 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       13 2022-07-27 03:05:39.000000 reviewbot-extension-3.1.1/reviewbot_extension.egg-info/top_level.txt
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.914362 reviewbot-extension-3.1.1/reviewbotext/
--rw-r--r--   0 chipx86    (501) staff       (20)     1994 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2580 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/admin.py
--rw-r--r--   0 chipx86    (501) staff       (20)      501 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/admin_urls.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.914788 reviewbot-extension-3.1.1/reviewbotext/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)      118 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      144 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/evolutions/old_tool_model.py
--rw-r--r--   0 chipx86    (501) staff       (20)      237 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/evolutions/tool_working_directory_required.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4696 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/extension.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6338 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/forms.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12745 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/integration.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1988 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/models.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13201 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/resources.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.911654 reviewbot-extension-3.1.1/reviewbotext/templates/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.911540 reviewbot-extension-3.1.1/reviewbotext/templates/admin/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.911587 reviewbot-extension-3.1.1/reviewbotext/templates/admin/reviewbotext/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.914918 reviewbot-extension-3.1.1/reviewbotext/templates/admin/reviewbotext/tool/
--rw-r--r--   0 chipx86    (501) staff       (20)      786 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/templates/admin/reviewbotext/tool/change_list.html
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.915040 reviewbot-extension-3.1.1/reviewbotext/templates/reviewbot/
--rw-r--r--   0 chipx86    (501) staff       (20)      736 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/templates/reviewbot/configure.html
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:39.915385 reviewbot-extension-3.1.1/reviewbotext/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8642 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/tests/test_worker_status_view.py
--rw-r--r--   0 chipx86    (501) staff       (20)      408 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/tests/testcase.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11244 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/views.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6571 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/reviewbotext/widgets.py
--rw-r--r--   0 chipx86    (501) staff       (20)      196 2022-07-27 03:05:39.915882 reviewbot-extension-3.1.1/setup.cfg
--rwxr-xr-x   0 chipx86    (501) staff       (20)     2277 2022-07-27 03:05:28.000000 reviewbot-extension-3.1.1/setup.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.141749 reviewbot-extension-3.2/
+-rw-r--r--   0 chipx86    (501) staff       (20)       48 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/MANIFEST.in
+-rw-r--r--   0 chipx86    (501) staff       (20)     6195 2023-05-04 02:38:52.141820 reviewbot-extension-3.2/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     5025 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/README.rst
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.139268 reviewbot-extension-3.2/reviewbot_extension.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     6195 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)      945 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       79 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/entry_points.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-04 02:38:45.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/not-zip-safe
+-rw-r--r--   0 chipx86    (501) staff       (20)      179 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       13 2023-05-04 02:38:52.000000 reviewbot-extension-3.2/reviewbot_extension.egg-info/top_level.txt
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.140673 reviewbot-extension-3.2/reviewbotext/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1994 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2580 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/admin.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      501 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/admin_urls.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.141053 reviewbot-extension-3.2/reviewbotext/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)      118 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      144 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/evolutions/old_tool_model.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      237 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/evolutions/tool_working_directory_required.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4696 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/extension.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6338 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/forms.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12745 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/integration.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1988 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13201 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/resources.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.137889 reviewbot-extension-3.2/reviewbotext/templates/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.137777 reviewbot-extension-3.2/reviewbotext/templates/admin/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.137824 reviewbot-extension-3.2/reviewbotext/templates/admin/reviewbotext/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.141182 reviewbot-extension-3.2/reviewbotext/templates/admin/reviewbotext/tool/
+-rw-r--r--   0 chipx86    (501) staff       (20)      740 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/templates/admin/reviewbotext/tool/change_list.html
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.141310 reviewbot-extension-3.2/reviewbotext/templates/reviewbot/
+-rw-r--r--   0 chipx86    (501) staff       (20)      736 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/templates/reviewbot/configure.html
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:52.141638 reviewbot-extension-3.2/reviewbotext/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8642 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/tests/test_worker_status_view.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      408 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/tests/testcase.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11244 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/views.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6571 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/reviewbotext/widgets.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      196 2023-05-04 02:38:52.142073 reviewbot-extension-3.2/setup.cfg
+-rwxr-xr-x   0 chipx86    (501) staff       (20)     2277 2023-05-04 02:38:44.000000 reviewbot-extension-3.2/setup.py
```

### Comparing `reviewbot-extension-3.1.1/PKG-INFO` & `reviewbot-extension-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviewbot-extension
-Version: 3.1.1
+Version: 3.2
 Summary: Review Bot, the automated code reviewer (Review Board extension)
 Author: Beanbag, Inc.
 Author-email: support@beanbaginc.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: support@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reviewbot-extension-3.1.1/README.rst` & `reviewbot-extension-3.2/README.rst`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbot_extension.egg-info/PKG-INFO` & `reviewbot-extension-3.2/reviewbot_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviewbot-extension
-Version: 3.1.1
+Version: 3.2
 Summary: Review Bot, the automated code reviewer (Review Board extension)
 Author: Beanbag, Inc.
 Author-email: support@beanbaginc.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: support@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reviewbot-extension-3.1.1/reviewbot_extension.egg-info/SOURCES.txt` & `reviewbot-extension-3.2/reviewbot_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/__init__.py` & `reviewbot-extension-3.2/reviewbotext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 #: The version of Review Bot.
 #:
 #: This is in the format of:
 #:
 #: (Major, Minor, Micro, Patch, alpha/beta/rc/final, Release Number, Released)
 #:
-VERSION = (3, 1, 1, 0, 'final', 0, True)
+VERSION = (3, 2, 0, 0, 'final', 0, True)
 
 
 def get_version_string():
     """Return the version of Review Bot.
 
     Returns:
         unicode:
```

### Comparing `reviewbot-extension-3.1.1/reviewbotext/admin.py` & `reviewbot-extension-3.2/reviewbotext/admin.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/extension.py` & `reviewbot-extension-3.2/reviewbotext/extension.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/forms.py` & `reviewbot-extension-3.2/reviewbotext/forms.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/integration.py` & `reviewbot-extension-3.2/reviewbotext/integration.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/models.py` & `reviewbot-extension-3.2/reviewbotext/models.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/resources.py` & `reviewbot-extension-3.2/reviewbotext/resources.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/templates/admin/reviewbotext/tool/change_list.html` & `reviewbot-extension-3.2/reviewbotext/templates/admin/reviewbotext/tool/change_list.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% extends "admin/change_list.html" %}
-{% load admin_list admin_static admin_urls %}
 
 {% block scripts %}
 {{ block.super }}
 <script type="text/javascript">
 $(document).ready(function() {
     $("#refresh_tools").bind('click',function(e) {
         e.preventDefault();
```

### Comparing `reviewbot-extension-3.1.1/reviewbotext/templates/reviewbot/configure.html` & `reviewbot-extension-3.2/reviewbotext/templates/reviewbot/configure.html`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/tests/test_worker_status_view.py` & `reviewbot-extension-3.2/reviewbotext/tests/test_worker_status_view.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/views.py` & `reviewbot-extension-3.2/reviewbotext/views.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/reviewbotext/widgets.py` & `reviewbot-extension-3.2/reviewbotext/widgets.py`

 * *Files identical despite different names*

### Comparing `reviewbot-extension-3.1.1/setup.py` & `reviewbot-extension-3.2/setup.py`

 * *Files identical despite different names*

