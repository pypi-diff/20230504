# Comparing `tmp/capeditor-0.1.6.tar.gz` & `tmp/capeditor-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.1.6.tar", last modified: Wed May  3 14:18:10 2023, max compression
+gzip compressed data, was "capeditor-0.1.7.tar", last modified: Thu May  4 08:41:03 2023, max compression
```

## Comparing `capeditor-0.1.6.tar` & `capeditor-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.826940 capeditor-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 14:17:52.000000 capeditor-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-03 14:18:10.826940 capeditor-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-03 14:17:52.000000 capeditor-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.822940 capeditor-0.1.6/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.822940 capeditor-0.1.6/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.818940 capeditor-0.1.6/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.822940 capeditor-0.1.6/capeditor/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/static/css/header.css
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.822940 capeditor-0.1.6/capeditor/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/static/js/common.js
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/static/js/hide_attributes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.818940 capeditor-0.1.6/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.826940 capeditor-0.1.6/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/alert_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/alert_filter_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/alert_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/alert_item_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/alert_list_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/latest_alert_include.html
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/pagination_include.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.826940 capeditor-0.1.6/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/widgets/basemap_polygon.html
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templates/capeditor/widgets/polygon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.826940 capeditor-0.1.6/capeditor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/templatetags/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 14:17:52.000000 capeditor-0.1.6/capeditor/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:18:10.822940 capeditor-0.1.6/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-03 14:18:10.000000 capeditor-0.1.6/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 14:18:10.000000 capeditor-0.1.6/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:18:10.000000 capeditor-0.1.6/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 14:18:10.000000 capeditor-0.1.6/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 14:18:10.000000 capeditor-0.1.6/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:18:10.826940 capeditor-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-03 14:17:52.000000 capeditor-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 08:40:50.000000 capeditor-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-04 08:41:03.857218 capeditor-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-04 08:40:50.000000 capeditor-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.853218 capeditor-0.1.7/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/static/css/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/static/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/static/js/hide_attributes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/alert_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/alert_filter_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/alert_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/alert_item_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/alert_list_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/latest_alert_include.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/pagination_include.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/widgets/basemap_polygon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templates/capeditor/widgets/polygon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/templatetags/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 08:40:50.000000 capeditor-0.1.7/capeditor/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:41:03.857218 capeditor-0.1.7/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-04 08:41:03.000000 capeditor-0.1.7/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-04 08:41:03.000000 capeditor-0.1.7/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:41:03.000000 capeditor-0.1.7/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 08:41:03.000000 capeditor-0.1.7/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 08:41:03.000000 capeditor-0.1.7/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:41:03.857218 capeditor-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-04 08:40:50.000000 capeditor-0.1.7/setup.py
```

### Comparing `capeditor-0.1.6/PKG-INFO` & `capeditor-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.1.6/README.md` & `capeditor-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/migrations/0001_initial.py` & `capeditor-0.1.7/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/models.py` & `capeditor-0.1.7/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/renderers.py` & `capeditor-0.1.7/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/serializers.py` & `capeditor-0.1.7/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/static/css/header.css` & `capeditor-0.1.7/capeditor/static/css/header.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/static/css/style.css` & `capeditor-0.1.7/capeditor/static/css/style.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/static/js/common.js` & `capeditor-0.1.7/capeditor/static/js/common.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/static/js/hide_attributes.js` & `capeditor-0.1.7/capeditor/static/js/hide_attributes.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/alert_detail.html` & `capeditor-0.1.7/capeditor/templates/capeditor/alert_detail.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/alert_filter_include.html` & `capeditor-0.1.7/capeditor/templates/capeditor/alert_filter_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/alert_index.html` & `capeditor-0.1.7/capeditor/templates/capeditor/alert_index.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/alert_item_include.html` & `capeditor-0.1.7/capeditor/templates/capeditor/alert_item_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/alert_list_include.html` & `capeditor-0.1.7/capeditor/templates/capeditor/alert_list_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/latest_alert_include.html` & `capeditor-0.1.7/capeditor/templates/capeditor/latest_alert_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/pagination_include.html` & `capeditor-0.1.7/capeditor/templates/capeditor/pagination_include.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templates/capeditor/widgets/polygon.html` & `capeditor-0.1.7/capeditor/templates/capeditor/widgets/polygon.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/templatetags/pagination.py` & `capeditor-0.1.7/capeditor/templatetags/pagination.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/utils.py` & `capeditor-0.1.7/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/views.py` & `capeditor-0.1.7/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/wagtail_hooks.py` & `capeditor-0.1.7/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor/widgets.py` & `capeditor-0.1.7/capeditor/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/capeditor.egg-info/PKG-INFO` & `capeditor-0.1.7/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Wagtail CAP Editor can be run as standalone or integrated into website
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `capeditor-0.1.6/capeditor.egg-info/SOURCES.txt` & `capeditor-0.1.7/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.1.6/setup.py` & `capeditor-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requirements = parse_requirements(os.path.join(PROJECT_ROOT, 'requirements.txt'), session=uuid.uuid1())
 
 # e.g. ['django', 'google-api-python-client']
 requirements = [getattr(ir, 'requirement', str(getattr(ir, 'req', None))) for ir in install_requirements]
 
 setup(
     name='capeditor',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=requirements,
     include_package_data=True,
     license='MIT License',
     description='Wagtail CAP Editor can be run as standalone or integrated into website',
     long_description=README,
     long_description_content_type='text/markdown',
```

