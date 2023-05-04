# Comparing `tmp/itsicli-0.0.40.tar.gz` & `tmp/itsicli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itsicli-0.0.40.tar", last modified: Thu May  4 06:55:37 2023, max compression
+gzip compressed data, was "dist/itsicli-0.0.8.tar", last modified: Wed Dec  2 05:40:05 2020, max compression
```

## Comparing `itsicli-0.0.40.tar` & `itsicli-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,47 @@
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.619910 itsicli-0.0.40/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)    11357 2022-08-12 04:48:32.000000 itsicli-0.0.40/LICENSE
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     8103 2023-05-04 06:55:37.618666 itsicli-0.0.40/PKG-INFO
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     7693 2022-08-12 04:48:32.000000 itsicli-0.0.40/README.md
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.559728 itsicli-0.0.40/bin/
--rwxr-xr-x   0 dbhensdadiya   (501) staff       (20)     1351 2022-08-12 04:48:32.000000 itsicli-0.0.40/bin/itsi-content-pack
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.562848 itsicli-0.0.40/itsicli/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       23 2023-05-04 06:55:12.000000 itsicli-0.0.40/itsicli/__init__.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.578605 itsicli-0.0.40/itsicli/content_packs/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        0 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/__init__.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.588154 itsicli-0.0.40/itsicli/content_packs/backup/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        0 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/backup/__init__.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     2875 2022-12-13 11:15:46.000000 itsicli-0.0.40/itsicli/content_packs/backup/convert_backup.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)    18272 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/backup/extract_models.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      290 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/backup/field_decode.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)    11490 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/backup/remap_keys.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     2791 2022-12-13 11:15:46.000000 itsicli-0.0.40/itsicli/content_packs/backup/workspace_import.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.596026 itsicli-0.0.40/itsicli/content_packs/commands/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        0 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/commands/__init__.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1448 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/commands/base.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1893 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/commands/importbackup.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     6540 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/commands/init.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     3466 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/commands/tidyup.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     2204 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/commands/validate.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     2249 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/content_types.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     7988 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/content_packs/files.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1616 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/model_formats.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.602113 itsicli-0.0.40/itsicli/content_packs/resources/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       64 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/resources/template_README.md
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      238 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/resources/template_app.conf
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       55 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/resources/template_manifest.json
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      890 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/scaffold.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.614864 itsicli-0.0.40/itsicli/content_packs/validate/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        0 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/__init__.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      408 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/registry.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      355 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/result.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1735 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/validate_config.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      586 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/validate_icon.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1133 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/validate_metadata.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     2593 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/validate/validate_screenshots.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      549 2022-08-12 04:48:32.000000 itsicli-0.0.40/itsicli/content_packs/workspace.py
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     4930 2023-02-14 10:22:57.000000 itsicli-0.0.40/itsicli/setup_logging.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.570450 itsicli-0.0.40/itsicli.egg-info/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     8103 2023-05-04 06:55:37.000000 itsicli-0.0.40/itsicli.egg-info/PKG-INFO
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)     1489 2023-05-04 06:55:37.000000 itsicli-0.0.40/itsicli.egg-info/SOURCES.txt
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        1 2023-05-04 06:55:37.000000 itsicli-0.0.40/itsicli.egg-info/dependency_links.txt
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       41 2023-05-04 06:55:37.000000 itsicli-0.0.40/itsicli.egg-info/requires.txt
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       14 2023-05-04 06:55:37.000000 itsicli-0.0.40/itsicli.egg-info/top_level.txt
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)       38 2023-05-04 06:55:37.620367 itsicli-0.0.40/setup.cfg
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)      986 2022-12-13 09:56:01.000000 itsicli-0.0.40/setup.py
-drwxr-xr-x   0 dbhensdadiya   (501) staff       (20)        0 2023-05-04 06:55:37.616415 itsicli-0.0.40/tests/
--rw-r--r--   0 dbhensdadiya   (501) staff       (20)        0 2022-08-12 04:48:32.000000 itsicli-0.0.40/tests/__init__.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/
+-rw-r--r--   0 jawang     (501) staff       (20)     2279 2020-12-02 05:40:05.000000 itsicli-0.0.8/PKG-INFO
+-rw-r--r--   0 jawang     (501) staff       (20)     1332 2020-12-02 05:29:34.000000 itsicli-0.0.8/README.md
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/bin/
+-rwxr-xr-x   0 jawang     (501) staff       (20)     1226 2020-11-30 08:16:28.000000 itsicli-0.0.8/bin/itsi-use-case
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/
+-rw-r--r--   0 jawang     (501) staff       (20)       22 2020-12-02 05:39:28.000000 itsicli-0.0.8/itsicli/__init__.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/use_cases/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-11-30 03:22:55.000000 itsicli-0.0.8/itsicli/use_cases/__init__.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/use_cases/backup/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-11-30 03:22:55.000000 itsicli-0.0.8/itsicli/use_cases/backup/__init__.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2411 2020-11-30 03:33:05.000000 itsicli-0.0.8/itsicli/use_cases/backup/convert_backup.py
+-rw-r--r--   0 jawang     (501) staff       (20)     7414 2020-12-02 05:38:27.000000 itsicli-0.0.8/itsicli/use_cases/backup/extract_models.py
+-rw-r--r--   0 jawang     (501) staff       (20)      290 2020-12-02 05:38:48.000000 itsicli-0.0.8/itsicli/use_cases/backup/field_decode.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2961 2020-12-02 05:39:11.000000 itsicli-0.0.8/itsicli/use_cases/backup/remap_keys.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2344 2020-12-02 05:37:51.000000 itsicli-0.0.8/itsicli/use_cases/backup/workspace_import.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/use_cases/commands/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-11-30 03:22:55.000000 itsicli-0.0.8/itsicli/use_cases/commands/__init__.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1385 2020-11-30 11:02:54.000000 itsicli-0.0.8/itsicli/use_cases/commands/base.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1181 2020-11-30 11:03:10.000000 itsicli-0.0.8/itsicli/use_cases/commands/importbackup.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2375 2020-11-30 11:00:37.000000 itsicli-0.0.8/itsicli/use_cases/commands/init.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1924 2020-12-01 09:20:58.000000 itsicli-0.0.8/itsicli/use_cases/commands/validate.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2065 2020-12-02 05:37:48.000000 itsicli-0.0.8/itsicli/use_cases/content_types.py
+-rw-r--r--   0 jawang     (501) staff       (20)     4731 2020-12-02 05:37:14.000000 itsicli-0.0.8/itsicli/use_cases/files.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1616 2020-12-02 05:36:58.000000 itsicli-0.0.8/itsicli/use_cases/model_formats.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/use_cases/resources/
+-rw-r--r--   0 jawang     (501) staff       (20)       56 2020-11-30 08:10:38.000000 itsicli-0.0.8/itsicli/use_cases/resources/README.md
+-rw-r--r--   0 jawang     (501) staff       (20)       54 2020-11-30 11:00:09.000000 itsicli-0.0.8/itsicli/use_cases/resources/manifest.json
+-rw-r--r--   0 jawang     (501) staff       (20)      759 2020-11-30 08:16:34.000000 itsicli-0.0.8/itsicli/use_cases/scaffold.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli/use_cases/validate/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-11-30 03:22:55.000000 itsicli-0.0.8/itsicli/use_cases/validate/__init__.py
+-rw-r--r--   0 jawang     (501) staff       (20)      297 2020-11-30 11:08:07.000000 itsicli-0.0.8/itsicli/use_cases/validate/registry.py
+-rw-r--r--   0 jawang     (501) staff       (20)      355 2020-11-30 03:22:55.000000 itsicli-0.0.8/itsicli/use_cases/validate/result.py
+-rw-r--r--   0 jawang     (501) staff       (20)     1621 2020-11-30 11:07:43.000000 itsicli-0.0.8/itsicli/use_cases/validate/validate_config.py
+-rw-r--r--   0 jawang     (501) staff       (20)      523 2020-11-30 08:24:30.000000 itsicli-0.0.8/itsicli/use_cases/validate/validate_icon.py
+-rw-r--r--   0 jawang     (501) staff       (20)     2568 2020-11-30 09:42:07.000000 itsicli-0.0.8/itsicli/use_cases/validate/validate_screenshots.py
+-rw-r--r--   0 jawang     (501) staff       (20)      501 2020-11-30 11:01:59.000000 itsicli-0.0.8/itsicli/use_cases/workspace.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/
+-rw-r--r--   0 jawang     (501) staff       (20)     2279 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/PKG-INFO
+-rw-r--r--   0 jawang     (501) staff       (20)     1191 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/SOURCES.txt
+-rw-r--r--   0 jawang     (501) staff       (20)        1 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/dependency_links.txt
+-rw-r--r--   0 jawang     (501) staff       (20)       40 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/requires.txt
+-rw-r--r--   0 jawang     (501) staff       (20)       14 2020-12-02 05:40:05.000000 itsicli-0.0.8/itsicli.egg-info/top_level.txt
+-rw-r--r--   0 jawang     (501) staff       (20)       38 2020-12-02 05:40:05.000000 itsicli-0.0.8/setup.cfg
+-rw-r--r--   0 jawang     (501) staff       (20)      978 2020-12-02 05:29:18.000000 itsicli-0.0.8/setup.py
+drwxr-xr-x   0 jawang     (501) staff       (20)        0 2020-12-02 05:40:05.000000 itsicli-0.0.8/tests/
+-rw-r--r--   0 jawang     (501) staff       (20)        0 2020-11-30 03:22:39.000000 itsicli-0.0.8/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `itsicli-0.0.40/itsicli/content_packs/backup/convert_backup.py` & `itsicli-0.0.8/itsicli/use_cases/backup/convert_backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ${copyright}
 
 import json
 import os
 
 from collections import defaultdict
 
-from itsicli.content_packs.backup.extract_models import extractor_registry
-from itsicli.content_packs.backup.remap_keys import KeysUpdater
-from itsicli.content_packs.content_types import get_content_type_for_model_class
+from itsicli.use_cases.backup.extract_models import extractor_registry
+from itsicli.use_cases.backup.remap_keys import KeysUpdater
+from itsicli.use_cases.content_types import get_content_type_for_model_class
 
 
 BACKUP_DELIM = '___'
 
 
 def get_backup_object_type(file_path):
     if not os.path.isfile(file_path):
@@ -41,23 +41,23 @@
             data = []
 
     return data
 
 
 class BackupConverter(object):
 
-    def __init__(self, prefix='', skip_key_mapping=False):
+    def __init__(self, prefix=''):
         self.prefix = prefix
         self.remapped_keys = {}
-        self.skip_key_mapping = skip_key_mapping
 
     def to_models(self, backup_dir):
         extracted_models = self.extract_models(backup_dir)
 
         updated_models = self.update_model_keys(extracted_models)
+
         return updated_models
 
     def extract_models(self, backup_dir):
         content_models = defaultdict(list)
 
         for root, _, files in os.walk(backup_dir):
             backup_files = [os.path.join(root, file_name) for file_name in files]
@@ -69,31 +69,25 @@
                 if not record:
                     continue
 
                 model_class, extractor_class = record
 
                 raw_json = read_backup_file(backup_file)
 
-                extractor = extractor_class(model_class, self.remapped_keys, self.prefix,
-                                            self.skip_key_mapping)
+                extractor = extractor_class(model_class, self.remapped_keys, self.prefix)
                 models = extractor.extract(raw_json)
 
                 content_type = get_content_type_for_model_class(extractor.model_class)
                 content_models[content_type].extend(models)
 
             break
 
         return content_models
 
     def update_model_keys(self, extracted_models):
         keys_updater = KeysUpdater(self.remapped_keys)
 
         for content_type, models in extracted_models.items():
-            # we are replacing the ids of glass table images/icons still
-            # even with skip_key_mapping=True. Thus, we still need to
-            # do key updating for those images within glass tables.
-            if self.skip_key_mapping and not content_type == 'glass_tables':
-                continue
             for model in models:
                 keys_updater.update(model)
 
         return extracted_models
```

### Comparing `itsicli-0.0.40/itsicli/content_packs/content_types.py` & `itsicli-0.0.8/itsicli/use_cases/content_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from itsimodels.correlation_search import CorrelationSearch
 from itsimodels.deep_dive import DeepDive
 from itsimodels.entity_type import EntityType
-from itsimodels.event_management_state import EventManagementState
 from itsimodels.glass_table import GlassTable
 from itsimodels.glass_table_icon import GlassTableIcon
 from itsimodels.glass_table_image import GlassTableImage
 from itsimodels.kpi_base_search import KpiBaseSearch
 from itsimodels.kpi_threshold_template import KpiThresholdTemplate
 from itsimodels.neap import NotableEventAggregationPolicy
 from itsimodels.service import Service
@@ -14,15 +13,14 @@
 from itsimodels.team import Team
 
 
 class ContentType(object):
     CORRELATION_SEARCH = 'correlation_searches'
     DEEP_DIVE = 'deep_dives'
     ENTITY_TYPE = 'entity_types'
-    EVENT_MANAGEMENT_STATE = 'event_management_states'
     GLASS_TABLE = 'glass_tables'
     GLASS_TABLE_ICON = 'glass_table_icons'
     GLASS_TABLE_IMAGE = 'glass_table_images'
     KPI_BASE_SEARCH = 'kpi_base_searches'
     KPI_THRESHOLD_TEMPLATE = 'kpi_threshold_templates'
     NOTABLE_EVENT_AGGREGATION_POLICY = 'notable_event_aggregation_policies'
     SERVICE_ANALYZER = 'service_analyzers'
@@ -31,15 +29,14 @@
     TEAM = 'teams'
 
 
 ContentTypes = {
     ContentType.CORRELATION_SEARCH: CorrelationSearch,
     ContentType.DEEP_DIVE: DeepDive,
     ContentType.ENTITY_TYPE: EntityType,
-    ContentType.EVENT_MANAGEMENT_STATE: EventManagementState,
     ContentType.GLASS_TABLE: GlassTable,
     ContentType.GLASS_TABLE_ICON: GlassTableIcon,
     ContentType.GLASS_TABLE_IMAGE: GlassTableImage,
     ContentType.KPI_BASE_SEARCH: KpiBaseSearch,
     ContentType.KPI_THRESHOLD_TEMPLATE: KpiThresholdTemplate,
     ContentType.NOTABLE_EVENT_AGGREGATION_POLICY: NotableEventAggregationPolicy,
     ContentType.SERVICE: Service,
```

### Comparing `itsicli-0.0.40/itsicli/content_packs/model_formats.py` & `itsicli-0.0.8/itsicli/use_cases/model_formats.py`

 * *Files identical despite different names*

### Comparing `itsicli-0.0.40/itsicli/content_packs/scaffold.py` & `itsicli-0.0.8/itsicli/use_cases/scaffold.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ${copyright}
 
-from itsicli.setup_logging import logger
+import logging
 from pathlib import Path
 
 
 HERE = Path(__file__).resolve().parent
 
 RESOURCES = HERE.joinpath('resources')
 
@@ -13,21 +13,18 @@
 
     def __init__(self, root):
         self.root = root
 
     def create_file(self, filename):
         path = self.root.joinpath(filename)
         if path.exists():
-            logger.info('{} already exists.'.format(path))
-            return path
+            return
 
-        template_path = RESOURCES.joinpath("template_{}".format(filename))
+        template_path = RESOURCES.joinpath(filename)
         if template_path.is_dir():
-            logger.info('Creating directory at {} ...'.format(path))
+            logging.info('Creating directory at {} ...'.format(path))
             path.mkdir()
         else:
-            logger.info('Creating file at {} ...'.format(path))
+            logging.info('Creating file at {} ...'.format(path))
             contents = template_path.read_bytes()
             path.parent.mkdir(parents=True, exist_ok=True)
             path.write_bytes(contents)
-
-        return path
```

### Comparing `itsicli-0.0.40/itsicli/content_packs/validate/validate_config.py` & `itsicli-0.0.8/itsicli/use_cases/validate/validate_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import re
-from itsicli.content_packs.files import ContentPackConfig
-from itsicli.content_packs.validate.result import Level, result
-from itsicli.content_packs.workspace import root_path
+from itsicli.use_cases.files import UseCaseConfig
+from itsicli.use_cases.validate.result import Level, result
+from itsicli.use_cases.workspace import root_path
 
 
 class ValidateConfig(object):
 
-    in_progress_text = 'Checking {}'.format(ContentPackConfig.file_name)
+    in_progress_text = 'Checking {}'.format(UseCaseConfig.file_name)
 
     def run(self, *args, **kwargs):
-        config = ContentPackConfig(root_path())
+        config = UseCaseConfig(root_path())
 
         results = []
 
         if not config.exists():
             results.append(
                 result(
                     Level.ERROR, "Missing '{}' file.".format(config.path)
@@ -33,22 +32,22 @@
         if not version:
             results.append(
                 result(
                     Level.ERROR, "Add a valid 'version' setting in '{}'.".format(config.path)
                 )
             )
         else:
-            version_re = r'^(\d+\.)(\d+\.)(\*|\d+)$'
-            matched = re.match(version_re, version)
-            if not matched:
+            try:
+                int(version)
+            except ValueError:
                 results.append(
                     result(
-                        Level.ERROR, "'version' {} in '{}' does not conform to x.x.x format.".format(
-                            version, config.path)
-                    ))
+                        Level.ERROR, "Invalid single integer value for 'version' in '{}'.".format(config.path)
+                    )
+                )
 
         description = config.description
         if not description:
             results.append(
                 result(
                     Level.WARNING, "Add a valid 'description' setting in '{}'.".format(config.path)
                 )
```

### Comparing `itsicli-0.0.40/itsicli/content_packs/validate/validate_screenshots.py` & `itsicli-0.0.8/itsicli/use_cases/validate/validate_screenshots.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from itsicli.content_packs.files import CONTENT_PACK_SCREENSHOTS_DIR, ContentPackManifest
-from itsicli.content_packs.validate.result import Level, result
+from itsicli.use_cases.files import USE_CASE_SCREENSHOTS_DIR, UseCaseManifest
+from itsicli.use_cases.validate.result import Level, result
 
 
 class ValidateScreenshots(object):
 
     in_progress_text = 'Checking for screenshots'
 
     def run(self, home_path, *args, **kwargs):
         results = []
 
-        manifest = ContentPackManifest(home_path)
+        manifest = UseCaseManifest(home_path)
 
         if not manifest.path.exists():
             results.append(
                 result(
                     Level.ERROR, "Missing manifest '{}' file.".format(manifest.path)
                 )
             )
@@ -57,15 +57,15 @@
 
             if not file_name:
                 results.append(
                     result(Level.ERROR, "Add a valid '{}' property for '{}'".format(attr, name))
                 )
 
             else:
-                screenshots_dir = home_path.joinpath(*CONTENT_PACK_SCREENSHOTS_DIR)
+                screenshots_dir = home_path.joinpath(USE_CASE_SCREENSHOTS_DIR)
 
                 image_path = screenshots_dir.joinpath(file_name)
 
                 if not image_path.exists() or image_path.is_dir():
                     results.append(
                         result(Level.ERROR, "Add a valid screenshot image at '{}'".format(image_path))
                     )
```

### Comparing `itsicli-0.0.40/itsicli.egg-info/SOURCES.txt` & `itsicli-0.0.8/itsicli.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-LICENSE
 README.md
 setup.py
-bin/itsi-content-pack
+bin/itsi-use-case
 itsicli/__init__.py
-itsicli/setup_logging.py
 itsicli.egg-info/PKG-INFO
 itsicli.egg-info/SOURCES.txt
 itsicli.egg-info/dependency_links.txt
 itsicli.egg-info/requires.txt
 itsicli.egg-info/top_level.txt
-itsicli/content_packs/__init__.py
-itsicli/content_packs/content_types.py
-itsicli/content_packs/files.py
-itsicli/content_packs/model_formats.py
-itsicli/content_packs/scaffold.py
-itsicli/content_packs/workspace.py
-itsicli/content_packs/backup/__init__.py
-itsicli/content_packs/backup/convert_backup.py
-itsicli/content_packs/backup/extract_models.py
-itsicli/content_packs/backup/field_decode.py
-itsicli/content_packs/backup/remap_keys.py
-itsicli/content_packs/backup/workspace_import.py
-itsicli/content_packs/commands/__init__.py
-itsicli/content_packs/commands/base.py
-itsicli/content_packs/commands/importbackup.py
-itsicli/content_packs/commands/init.py
-itsicli/content_packs/commands/tidyup.py
-itsicli/content_packs/commands/validate.py
-itsicli/content_packs/resources/template_README.md
-itsicli/content_packs/resources/template_app.conf
-itsicli/content_packs/resources/template_manifest.json
-itsicli/content_packs/validate/__init__.py
-itsicli/content_packs/validate/registry.py
-itsicli/content_packs/validate/result.py
-itsicli/content_packs/validate/validate_config.py
-itsicli/content_packs/validate/validate_icon.py
-itsicli/content_packs/validate/validate_metadata.py
-itsicli/content_packs/validate/validate_screenshots.py
+itsicli/use_cases/__init__.py
+itsicli/use_cases/content_types.py
+itsicli/use_cases/files.py
+itsicli/use_cases/model_formats.py
+itsicli/use_cases/scaffold.py
+itsicli/use_cases/workspace.py
+itsicli/use_cases/backup/__init__.py
+itsicli/use_cases/backup/convert_backup.py
+itsicli/use_cases/backup/extract_models.py
+itsicli/use_cases/backup/field_decode.py
+itsicli/use_cases/backup/remap_keys.py
+itsicli/use_cases/backup/workspace_import.py
+itsicli/use_cases/commands/__init__.py
+itsicli/use_cases/commands/base.py
+itsicli/use_cases/commands/importbackup.py
+itsicli/use_cases/commands/init.py
+itsicli/use_cases/commands/validate.py
+itsicli/use_cases/resources/README.md
+itsicli/use_cases/resources/manifest.json
+itsicli/use_cases/validate/__init__.py
+itsicli/use_cases/validate/registry.py
+itsicli/use_cases/validate/result.py
+itsicli/use_cases/validate/validate_config.py
+itsicli/use_cases/validate/validate_icon.py
+itsicli/use_cases/validate/validate_screenshots.py
 tests/__init__.py
```

### Comparing `itsicli-0.0.40/setup.py` & `itsicli-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     name='itsicli',
     version=__version__,
     author='Splunk, Inc.',
     description='The ITSI Command Line Interface (CLI)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     scripts=[
-        'bin/itsi-content-pack'
+        'bin/itsi-use-case'
     ],
     url='https://github.com/splunk/itsi-cli',
     packages=setuptools.find_packages(),
     package_data={
-        'itsicli.content_packs': ['resources/*']
+        'itsicli.use_cases': ['resources/*']
     },
     install_requires=requirements,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
```

