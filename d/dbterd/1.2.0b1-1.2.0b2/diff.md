# Comparing `tmp/dbterd-1.2.0b1.tar.gz` & `tmp/dbterd-1.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.2.0b1.tar", max compression
+gzip compressed data, was "dbterd-1.2.0b2.tar", max compression
```

## Comparing `dbterd-1.2.0b1.tar` & `dbterd-1.2.0b2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      203 2023-05-02 17:48:15.565293 dbterd-1.2.0b1/LICENSE
--rw-r--r--   0        0        0     4473 2023-05-02 17:48:15.565293 dbterd-1.2.0b1/README.md
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     4896 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     3157 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/filter.py
--rw-r--r--   0        0        0      571 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     2505 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     2561 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/base.py
--rw-r--r--   0        0        0      560 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     1729 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1597 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      222 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/main.py
--rw-r--r--   0        0        0     1928 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-05-02 17:48:15.569294 dbterd-1.2.0b1/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4494 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-05-02 17:48:15.573294 dbterd-1.2.0b1/dbterd/main.py
--rw-r--r--   0        0        0     2097 2023-05-02 17:48:32.197444 dbterd-1.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 dbterd-1.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0      203 2023-05-04 06:25:22.667425 dbterd-1.2.0b2/LICENSE
+-rw-r--r--   0        0        0     2937 2023-05-04 06:25:22.667425 dbterd-1.2.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4801 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      571 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     3724 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2575 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     1729 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1597 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/cli/params.py
+-rw-r--r--   0        0        0      114 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/constants.py
+-rw-r--r--   0        0        0      284 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/main.py
+-rw-r--r--   0        0        0     2097 2023-05-04 06:25:36.563597 dbterd-1.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 dbterd-1.2.0b2/PKG-INFO
```

### Comparing `dbterd-1.2.0b1/dbterd/adapters/algos/base.py` & `dbterd-1.2.0b2/dbterd/adapters/algos/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,36 +91,34 @@
 
     if catalog_node:
         for column, metadata in catalog_node.columns.items():
             table.columns.append(
                 Column(
                     name=str(column).lower(),
                     data_type=str(metadata.type).lower(),
-                    description=metadata.comment or "",  # TODO escape quote
+                    description=metadata.comment or "",
                 )
             )
 
     for column_name, column_metadata in manifest_node.columns.items():
         column_name = column_name.strip('"')
         find_columns = [
             c for c in table.columns if c.name.lower() == column_name.lower()
         ]
         if not find_columns:
             table.columns.append(
                 Column(
                     name=column_name.lower(),
                     data_type=str(column_metadata.data_type or "unknown").lower(),
-                    description=column_metadata.description or "",  # TODO escape quote
+                    description=column_metadata.description or "",
                 )
             )
         else:
             find_columns[0].description = (
-                find_columns[0].description
-                or column_metadata.description
-                or ""  # TODO escape quote
+                find_columns[0].description or column_metadata.description or ""
             )
 
     if not table.columns:
         table.columns.append(Column())
 
     return table
```

### Comparing `dbterd-1.2.0b1/dbterd/adapters/algos/filter.py` & `dbterd-1.2.0b2/dbterd/adapters/algos/filter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/adapters/algos/meta.py` & `dbterd-1.2.0b2/dbterd/adapters/algos/meta.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.2.0b2/dbterd/adapters/algos/test_relationship.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dbterd.adapters.algos import base
 from dbterd.adapters.algos.filter import is_selected_table
 from dbterd.adapters.algos.meta import Ref
+from dbterd.constants import DEFAULT_ALGO_RULE, TEST_META_IGNORE_IN_ERD
 
 
 def parse(manifest, catalog, **kwargs):
     """Get all information (tables, relationships) needed for building diagram
 
     Args:
         manifest (dict): Manifest json
@@ -25,15 +26,15 @@
             select_rules=(kwargs.get("select") or []),
             resource_types=kwargs.get("resource_type", []),
             exclude_rules=kwargs.get("exclude", []),
         )
     ]
 
     # Parse Ref
-    relationships = get_relationships(manifest=manifest)
+    relationships = get_relationships(manifest=manifest, **kwargs)
     table_names = [x.name for x in tables]
     relationships = [
         x
         for x in relationships
         if x.table_map[0] in table_names and x.table_map[1] in table_names
     ]
 
@@ -41,41 +42,66 @@
     tables = base.enrich_tables_from_relationships(
         tables=tables, relationships=relationships
     )
 
     return (tables, relationships)
 
 
-def get_relationships(manifest):
+def get_relationships(manifest, **kwargs):
     """Extract relationships from dbt artifacts based on test relationship
 
     Args:
         manifest (dict): Manifest json
+        kwargs.algo (str): |
+            Algorithm name and optional rules.
+            Smaples:
+            - test_relationship
+            - test_relationship:(name:relationship|c_from:column_name|c_to:field)
+            - test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:pk_column_name)
 
     Returns:
         List[Ref]: List of parsed relationship
     """
+    algo_parts = (kwargs.get("algo") or "").replace(" ", "").split(":", 1)
+    rules, _ = (
+        algo_parts[1] if len(algo_parts) > 1 else DEFAULT_ALGO_RULE,
+        algo_parts[0],
+    )
+    rules = rules[1:-1]  # remove brackets
+    rules = dict(arg.split(":") for arg in rules.split("|"))
+
     refs = [
         Ref(
             name=x,
             table_map=manifest.parent_map[x],
             column_map=[
                 str(
-                    manifest.nodes[x].test_metadata.kwargs.get("field", "unknown")
+                    manifest.nodes[x].test_metadata.kwargs.get(rules.get("c_to"))
+                    or "_and_".join(
+                        manifest.nodes[x].test_metadata.kwargs.get(
+                            f'{rules.get("c_to")}s', "unknown"
+                        )
+                    )
                 ).lower(),
                 str(
-                    manifest.nodes[x].test_metadata.kwargs.get("column_name", "unknown")
+                    manifest.nodes[x].test_metadata.kwargs.get("column_name")
+                    or manifest.nodes[x].test_metadata.kwargs.get(rules.get("c_from"))
+                    or "_and_".join(
+                        manifest.nodes[x].test_metadata.kwargs.get(
+                            f'{rules.get("c_from")}s', "unknown"
+                        )
+                    )
                 ).lower(),
             ],
         )
         for x in manifest.nodes
         if (
             x.startswith("test")
-            and "relationship" in x.lower()
-            and manifest.nodes[x].meta.get("ignore_in_erd", "0") == "0"
+            and rules.get("name").lower() in x.lower()
+            and manifest.nodes[x].meta.get(TEST_META_IGNORE_IN_ERD, "0") == "0"
         )
     ]
 
     # remove duplicates
     if refs:
         distinct_list = [refs[0]]
         for ref in refs:
```

### Comparing `dbterd-1.2.0b1/dbterd/adapters/base.py` & `dbterd-1.2.0b2/dbterd/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def __run_by_strategy(self, **kwargs):
         """Read artifacts and export the diagram file following the target"""
         target = factory.load_executor(name=kwargs["target"])  # import {target}
         run_operation_dispatcher = getattr(target, "run_operation_dispatcher")
         operation_default = getattr(target, "run_operation_default")
         operation = run_operation_dispatcher.get(
-            f"{kwargs['target']}_{kwargs['algo']}",
+            f"{kwargs['target']}_{kwargs['algo'].split(':')[0]}",
             operation_default,
         )
         manifest = self.__read_manifest(
             mp=kwargs.get("manifest_path") or kwargs["artifacts_dir"],
             mv=kwargs["manifest_version"],
         )
         catalog = self.__read_catalog(
```

### Comparing `dbterd-1.2.0b1/dbterd/adapters/factory.py` & `dbterd-1.2.0b2/dbterd/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.2.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.2.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/cli/main.py` & `dbterd-1.2.0b2/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/cli/params.py` & `dbterd-1.2.0b2/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/cli_messaging.py` & `dbterd-1.2.0b2/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/dict.py` & `dbterd-1.2.0b2/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/file.py` & `dbterd-1.2.0b2/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/jsonify.py` & `dbterd-1.2.0b2/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/log.py` & `dbterd-1.2.0b2/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/dbterd/helpers/yaml.py` & `dbterd-1.2.0b2/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b1/pyproject.toml` & `dbterd-1.2.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.2.0b1"
+version = "1.2.0b2"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

