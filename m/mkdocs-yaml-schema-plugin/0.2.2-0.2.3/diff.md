# Comparing `tmp/mkdocs-yaml-schema-plugin-0.2.2.tar.gz` & `tmp/mkdocs-yaml-schema-plugin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-yaml-schema-plugin-0.2.2.tar", last modified: Thu Apr 20 13:18:04 2023, max compression
+gzip compressed data, was "mkdocs-yaml-schema-plugin-0.2.3.tar", last modified: Thu May  4 12:41:23 2023, max compression
```

## Comparing `mkdocs-yaml-schema-plugin-0.2.2.tar` & `mkdocs-yaml-schema-plugin-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 13:18:04.000000 mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 13:18:04.436741 mkdocs-yaml-schema-plugin-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 13:17:58.000000 mkdocs-yaml-schema-plugin-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 12:41:23.000000 mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 12:41:23.764778 mkdocs-yaml-schema-plugin-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-04 12:41:17.000000 mkdocs-yaml-schema-plugin-0.2.3/versioneer.py
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/LICENSE.md` & `mkdocs-yaml-schema-plugin-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.2.2
+Version: 0.2.3
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/README.md` & `mkdocs-yaml-schema-plugin-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/markdown.py` & `mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     def set_config(self, config):
         self.yaml_config = []
         # CHeck why I need to fetch first object
         for f in self.safe_get_value(config, "yaml_files")[0]:
             self.yaml_config.append({
                 'tag': f['tag'],
                 'file': f['file'],
-                'regex': r"#" + re.escape(f['tag']) + r"[A-Za-z_]*#"
+                'regex': r"#" + re.escape(f['tag']) + r"[A-Za-z0-9_]*#"
             })
             print(f"Got config: File: {f['file']} Tag: {f['tag']}")
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin/plugin.py` & `mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO` & `mkdocs-yaml-schema-plugin-0.2.3/mkdocs_yaml_schema_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-yaml-schema-plugin
-Version: 0.2.2
+Version: 0.2.3
 Summary: MkDocs Plugin to parse yaml schemas.
 Home-page: https://github.com/smeds/mkdocs-yaml-schema-plugin
 Author: Patrik Smeds
 Author-email: patrik.smeds@gmail.com
 License: MIT license
 Keywords: mkdocs,plugin,yaml,schema
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/setup.py` & `mkdocs-yaml-schema-plugin-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-yaml-schema-plugin-0.2.2/versioneer.py` & `mkdocs-yaml-schema-plugin-0.2.3/versioneer.py`

 * *Files identical despite different names*

