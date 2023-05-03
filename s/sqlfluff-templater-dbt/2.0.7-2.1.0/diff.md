# Comparing `tmp/sqlfluff-templater-dbt-2.0.7.tar.gz` & `tmp/sqlfluff-templater-dbt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-p7agkjh1/sqlfluff-templater-dbt-2.0.7.tar", last modified: Thu Apr 20 21:06:10 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-5j982rty/sqlfluff-templater-dbt-2.1.0.tar", last modified: Wed May  3 23:19:59 2023, max compression
```

## Comparing `sqlfluff-templater-dbt-2.0.7.tar` & `sqlfluff-templater-dbt-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 21:05:50.000000 sqlfluff-templater-dbt-2.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 21:05:50.000000 sqlfluff-templater-dbt-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 21:05:50.000000 sqlfluff-templater-dbt-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 21:05:50.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-20 21:05:50.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 21:06:10.000000 sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-05-03 23:19:45.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 23:19:59.000000 sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-2.0.7/LICENSE.md` & `sqlfluff-templater-dbt-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.0.7/PKG-INFO` & `sqlfluff-templater-dbt-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.0.7
+Version: 2.1.0
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-templater-dbt-2.0.7/setup.cfg` & `sqlfluff-templater-dbt-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 2.0.7
+version = 2.1.0
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -61,15 +61,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	sqlfluff==2.0.7
+	sqlfluff==2.1.0
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt/templater.py` & `sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt/templater.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import os.path
 import logging
 from typing import List, Optional, Iterator, Tuple, Any, Dict, Deque
 
 from dataclasses import dataclass
 
 from dbt.version import get_installed_version
-from dbt.config import read_user_config
 from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
 from dbt.adapters.factory import register_adapter, get_adapter
 from dbt.compilation import Compiler as DbtCompiler
 
 try:
     from dbt.exceptions import (
         CompilationException as DbtCompilationException,
@@ -61,16 +60,17 @@
 class DbtConfigArgs:
     """Arguments to load dbt runtime config."""
 
     project_dir: Optional[str] = None
     profiles_dir: Optional[str] = None
     profile: Optional[str] = None
     target: Optional[str] = None
+    threads: int = 1
     single_threaded: bool = False
-    vars: str = ""
+    vars: Optional[Dict] = None
 
 
 class DbtTemplater(JinjaTemplater):
     """A templater using dbt."""
 
     name = "dbt"
     sequential_fail_limit = 3
@@ -93,37 +93,32 @@
     def dbt_version(self):  # pragma: no cover
         """Gets the dbt version."""
         return DBT_VERSION_STRING
 
     @cached_property
     def dbt_config(self):
         """Loads the dbt config."""
-        # Here, we read flags.PROFILE_DIR directly, prior to calling
-        # set_from_args(). Apparently, set_from_args() sets PROFILES_DIR
-        # to a lowercase version of the value, and the profile wouldn't be
-        # found if the directory name contained uppercase letters. This fix
-        # was suggested and described here:
-        # https://github.com/sqlfluff/sqlfluff/issues/2253#issuecomment-1018722979
-        user_config = read_user_config(flags.PROFILES_DIR)
         flags.set_from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
                 vars=self._get_cli_vars(),
+                threads=1,
             ),
-            user_config,
+            None,
         )
         self.dbt_config = DbtRuntimeConfig.from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
                 target=self._get_target(),
                 vars=self._get_cli_vars(),
+                threads=1,
             )
         )
         register_adapter(self.dbt_config)
         return self.dbt_config
 
     @cached_property
     def dbt_compiler(self):
@@ -239,20 +234,20 @@
 
     def _get_target(self):
         """Get a dbt target name from the configuration."""
         return self.sqlfluff_config.get_section(
             (self.templater_selector, self.name, "target")
         )
 
-    def _get_cli_vars(self) -> str:
+    def _get_cli_vars(self) -> dict:
         cli_vars = self.sqlfluff_config.get_section(
             (self.templater_selector, self.name, "context")
         )
 
-        return str(cli_vars) if cli_vars else "{}"
+        return cli_vars if cli_vars else {}
 
     def sequence_files(
         self, fnames: List[str], config=None, formatter=None
     ) -> Iterator[str]:
         """Reorder fnames to process dependent files first.
 
         This avoids errors when an ephemeral model is processed before use.
@@ -370,15 +365,15 @@
                 ]
             else:
                 raise  # pragma: no cover
         except DbtFailedToConnectException as e:
             return None, [
                 SQLTemplaterError(
                     "dbt tried to connect to the database and failed: you could use "
-                    "'execute' to skip the database calls. See"
+                    "'execute' to skip the database calls. See "
                     "https://docs.getdbt.com/reference/dbt-jinja-functions/execute/ "
                     f"Error: {e.msg}",
                     fatal=True,
                 )
             ]
         # If a SQLFluff error is raised, just pass it through
         except SQLTemplaterError as e:  # pragma: no cover
```

### Comparing `sqlfluff-templater-dbt-2.0.7/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff-templater-dbt-2.1.0/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.0.7
+Version: 2.1.0
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

