# Comparing `tmp/itsimodels-0.0.8.tar.gz` & `tmp/itsimodels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itsimodels-0.0.8.tar", last modified: Mon Dec 21 19:28:22 2020, max compression
+gzip compressed data, was "dist/itsimodels-0.0.9.tar", last modified: Tue Dec 22 23:47:18 2020, max compression
```

## Comparing `itsimodels-0.0.8.tar` & `itsimodels-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-21 19:28:22.000000 itsimodels-0.0.8/
--rw-r--r--   0 jawang     (501) staff       (20)      473 2020-12-21 19:28:22.000000 itsimodels-0.0.8/PKG-INFO
--rw-r--r--   0 jawang     (501) staff       (20)      666 2020-12-02 07:22:20.000000 itsimodels-0.0.8/README.md
-drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels/
--rw-r--r--   0 jawang     (501) staff       (20)       22 2020-12-21 19:27:32.000000 itsimodels-0.0.8/itsimodels/__init__.py
-drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels/core/
--rw-r--r--   0 jawang     (501) staff       (20)        0 2020-12-02 03:14:23.000000 itsimodels-0.0.8/itsimodels/core/__init__.py
--rw-r--r--   0 jawang     (501) staff       (20)     7231 2020-12-12 02:33:49.000000 itsimodels-0.0.8/itsimodels/core/base_models.py
--rw-r--r--   0 jawang     (501) staff       (20)      188 2020-12-12 02:50:57.000000 itsimodels-0.0.8/itsimodels/core/compat.py
--rw-r--r--   0 jawang     (501) staff       (20)     1935 2020-12-12 02:51:36.000000 itsimodels-0.0.8/itsimodels/core/field_decode.py
--rw-r--r--   0 jawang     (501) staff       (20)     7519 2020-12-12 02:52:09.000000 itsimodels-0.0.8/itsimodels/core/fields.py
--rw-r--r--   0 jawang     (501) staff       (20)     2073 2020-12-12 02:31:55.000000 itsimodels-0.0.8/itsimodels/core/migrators.py
--rw-r--r--   0 jawang     (501) staff       (20)      192 2020-12-02 04:19:57.000000 itsimodels-0.0.8/itsimodels/correlation_search.py
--rw-r--r--   0 jawang     (501) staff       (20)     3561 2020-12-12 02:30:38.000000 itsimodels-0.0.8/itsimodels/deep_dive.py
--rw-r--r--   0 jawang     (501) staff       (20)     1427 2020-12-12 02:30:17.000000 itsimodels-0.0.8/itsimodels/entity_type.py
--rw-r--r--   0 jawang     (501) staff       (20)     3304 2020-12-12 02:32:32.000000 itsimodels-0.0.8/itsimodels/glass_table.py
--rw-r--r--   0 jawang     (501) staff       (20)      382 2020-12-02 03:18:45.000000 itsimodels-0.0.8/itsimodels/glass_table_icon.py
--rw-r--r--   0 jawang     (501) staff       (20)      264 2020-12-02 03:18:51.000000 itsimodels-0.0.8/itsimodels/glass_table_image.py
--rw-r--r--   0 jawang     (501) staff       (20)     1543 2020-12-02 03:19:05.000000 itsimodels-0.0.8/itsimodels/kpi_base_search.py
--rw-r--r--   0 jawang     (501) staff       (20)      637 2020-12-02 03:20:56.000000 itsimodels-0.0.8/itsimodels/kpi_threshold_template.py
--rw-r--r--   0 jawang     (501) staff       (20)     2539 2020-12-02 03:19:19.000000 itsimodels-0.0.8/itsimodels/neap.py
--rw-r--r--   0 jawang     (501) staff       (20)     5994 2020-12-12 02:30:46.000000 itsimodels-0.0.8/itsimodels/service.py
--rw-r--r--   0 jawang     (501) staff       (20)     1242 2020-12-16 00:15:51.000000 itsimodels-0.0.8/itsimodels/service_analyzer.py
--rw-r--r--   0 jawang     (501) staff       (20)      549 2020-12-02 05:44:43.000000 itsimodels-0.0.8/itsimodels/service_template.py
--rw-r--r--   0 jawang     (501) staff       (20)      573 2020-12-02 05:45:18.000000 itsimodels-0.0.8/itsimodels/team.py
-drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels.egg-info/
--rw-r--r--   0 jawang     (501) staff       (20)      473 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels.egg-info/PKG-INFO
--rw-r--r--   0 jawang     (501) staff       (20)      749 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels.egg-info/SOURCES.txt
--rw-r--r--   0 jawang     (501) staff       (20)        1 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels.egg-info/dependency_links.txt
--rw-r--r--   0 jawang     (501) staff       (20)       17 2020-12-21 19:28:22.000000 itsimodels-0.0.8/itsimodels.egg-info/top_level.txt
--rw-r--r--   0 jawang     (501) staff       (20)       38 2020-12-21 19:28:22.000000 itsimodels-0.0.8/setup.cfg
--rw-r--r--   0 jawang     (501) staff       (20)      571 2020-12-21 18:32:08.000000 itsimodels-0.0.8/setup.py
-drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-21 19:28:22.000000 itsimodels-0.0.8/tests/
--rw-r--r--   0 jawang     (501) staff       (20)        0 2020-12-02 03:14:23.000000 itsimodels-0.0.8/tests/__init__.py
--rw-r--r--   0 jawang     (501) staff       (20)     1098 2020-12-12 02:59:05.000000 itsimodels-0.0.8/tests/test_models.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-22 23:47:18.000000 itsimodels-0.0.9/
+-rw-r--r--   0 jawang     (501) staff       (20)      473 2020-12-22 23:47:18.000000 itsimodels-0.0.9/PKG-INFO
+-rw-r--r--   0 jawang     (501) staff       (20)      666 2020-12-02 07:22:20.000000 itsimodels-0.0.9/README.md
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels/
+-rw-r--r--   0 jawang     (501) staff       (20)       22 2020-12-22 23:46:39.000000 itsimodels-0.0.9/itsimodels/__init__.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels/core/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-12-02 03:14:23.000000 itsimodels-0.0.9/itsimodels/core/__init__.py
+-rw-r--r--   0 jawang     (501) staff       (20)     7231 2020-12-12 02:33:49.000000 itsimodels-0.0.9/itsimodels/core/base_models.py
+-rw-r--r--   0 jawang     (501) staff       (20)      188 2020-12-12 02:50:57.000000 itsimodels-0.0.9/itsimodels/core/compat.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1935 2020-12-12 02:51:36.000000 itsimodels-0.0.9/itsimodels/core/field_decode.py
+-rw-r--r--   0 jawang     (501) staff       (20)     7519 2020-12-12 02:52:09.000000 itsimodels-0.0.9/itsimodels/core/fields.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2073 2020-12-12 02:31:55.000000 itsimodels-0.0.9/itsimodels/core/migrators.py
+-rw-r--r--   0 jawang     (501) staff       (20)      192 2020-12-02 04:19:57.000000 itsimodels-0.0.9/itsimodels/correlation_search.py
+-rw-r--r--   0 jawang     (501) staff       (20)     3561 2020-12-12 02:30:38.000000 itsimodels-0.0.9/itsimodels/deep_dive.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1427 2020-12-12 02:30:17.000000 itsimodels-0.0.9/itsimodels/entity_type.py
+-rw-r--r--   0 jawang     (501) staff       (20)     3350 2020-12-22 23:46:08.000000 itsimodels-0.0.9/itsimodels/glass_table.py
+-rw-r--r--   0 jawang     (501) staff       (20)      382 2020-12-02 03:18:45.000000 itsimodels-0.0.9/itsimodels/glass_table_icon.py
+-rw-r--r--   0 jawang     (501) staff       (20)      264 2020-12-02 03:18:51.000000 itsimodels-0.0.9/itsimodels/glass_table_image.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1543 2020-12-02 03:19:05.000000 itsimodels-0.0.9/itsimodels/kpi_base_search.py
+-rw-r--r--   0 jawang     (501) staff       (20)      637 2020-12-02 03:20:56.000000 itsimodels-0.0.9/itsimodels/kpi_threshold_template.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2539 2020-12-02 03:19:19.000000 itsimodels-0.0.9/itsimodels/neap.py
+-rw-r--r--   0 jawang     (501) staff       (20)     5994 2020-12-12 02:30:46.000000 itsimodels-0.0.9/itsimodels/service.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1242 2020-12-16 00:15:51.000000 itsimodels-0.0.9/itsimodels/service_analyzer.py
+-rw-r--r--   0 jawang     (501) staff       (20)      549 2020-12-02 05:44:43.000000 itsimodels-0.0.9/itsimodels/service_template.py
+-rw-r--r--   0 jawang     (501) staff       (20)      573 2020-12-02 05:45:18.000000 itsimodels-0.0.9/itsimodels/team.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels.egg-info/
+-rw-r--r--   0 jawang     (501) staff       (20)      473 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels.egg-info/PKG-INFO
+-rw-r--r--   0 jawang     (501) staff       (20)      749 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels.egg-info/SOURCES.txt
+-rw-r--r--   0 jawang     (501) staff       (20)        1 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels.egg-info/dependency_links.txt
+-rw-r--r--   0 jawang     (501) staff       (20)       17 2020-12-22 23:47:18.000000 itsimodels-0.0.9/itsimodels.egg-info/top_level.txt
+-rw-r--r--   0 jawang     (501) staff       (20)       38 2020-12-22 23:47:18.000000 itsimodels-0.0.9/setup.cfg
+-rw-r--r--   0 jawang     (501) staff       (20)      571 2020-12-21 18:32:08.000000 itsimodels-0.0.9/setup.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-22 23:47:18.000000 itsimodels-0.0.9/tests/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-12-02 03:14:23.000000 itsimodels-0.0.9/tests/__init__.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1098 2020-12-12 02:59:05.000000 itsimodels-0.0.9/tests/test_models.py
```

### Comparing `itsimodels-0.0.8/README.md` & `itsimodels-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/core/base_models.py` & `itsimodels-0.0.9/itsimodels/core/base_models.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/core/field_decode.py` & `itsimodels-0.0.9/itsimodels/core/field_decode.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/core/fields.py` & `itsimodels-0.0.9/itsimodels/core/fields.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/core/migrators.py` & `itsimodels-0.0.9/itsimodels/core/migrators.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/deep_dive.py` & `itsimodels-0.0.9/itsimodels/deep_dive.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/entity_type.py` & `itsimodels-0.0.9/itsimodels/entity_type.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/glass_table.py` & `itsimodels-0.0.9/itsimodels/glass_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
 
     title = StringField(required=True)
 
     definition = TypeField(Definition)
 
     description = StringField(default='')
 
+    gt_version = StringField(default='beta')
+
     latest = StringField(default='now')
 
     latest_label = StringField(default='Now')
 
     template_selected_service_id = ForeignKey('itsimodels.service.Service', alias='templateSelectedServiceId')
 
     template_swappable_service_ids = ForeignKeyList('itsimodels.service.Service', alias='templateSwappableServiceIds')
```

### Comparing `itsimodels-0.0.8/itsimodels/kpi_base_search.py` & `itsimodels-0.0.9/itsimodels/kpi_base_search.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/kpi_threshold_template.py` & `itsimodels-0.0.9/itsimodels/kpi_threshold_template.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/neap.py` & `itsimodels-0.0.9/itsimodels/neap.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/service.py` & `itsimodels-0.0.9/itsimodels/service.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/service_analyzer.py` & `itsimodels-0.0.9/itsimodels/service_analyzer.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/service_template.py` & `itsimodels-0.0.9/itsimodels/service_template.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels/team.py` & `itsimodels-0.0.9/itsimodels/team.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/itsimodels.egg-info/SOURCES.txt` & `itsimodels-0.0.9/itsimodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/setup.py` & `itsimodels-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `itsimodels-0.0.8/tests/test_models.py` & `itsimodels-0.0.9/tests/test_models.py`

 * *Files identical despite different names*

