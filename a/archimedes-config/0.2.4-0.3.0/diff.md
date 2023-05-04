# Comparing `tmp/archimedes_config-0.2.4.tar.gz` & `tmp/archimedes_config-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_config-0.2.4.tar", max compression
+gzip compressed data, was "archimedes_config-0.3.0.tar", max compression
```

## Comparing `archimedes_config-0.2.4.tar` & `archimedes_config-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/__init__.py
--rw-r--r--   0        0        0     7834 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/arckeyl.py
--rw-r--r--   0        0        0    13575 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/config_manager.py
--rw-r--r--   0        0        0     2308 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/keyvault_client.py
--rw-r--r--   0        0        0     1242 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/keyvault_config_manager.py
--rw-r--r--   0        0        0     1311 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/utils/path_utils.py
--rw-r--r--   0        0        0     3898 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/utils/util.py
--rw-r--r--   0        0        0      673 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/add_secrets.py
--rw-r--r--   0        0        0      965 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/lock_secrets.py
--rw-r--r--   0        0        0     2127 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/secret_creation.py
--rw-r--r--   0        0        0      944 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/unlock_secrets.py
--rw-r--r--   0        0        0     4126 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/workflow_base.py
--rw-r--r--   0        0        0      753 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      188 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/__init__.py
+-rw-r--r--   0        0        0     8622 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/arckeyl.py
+-rw-r--r--   0        0        0    13575 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/config_manager.py
+-rw-r--r--   0        0        0     2308 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/keyvault_client.py
+-rw-r--r--   0        0        0     1242 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/keyvault_config_manager.py
+-rw-r--r--   0        0        0     1947 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/utils/path_utils.py
+-rw-r--r--   0        0        0     3898 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/utils/util.py
+-rw-r--r--   0        0        0      673 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/add_secrets.py
+-rw-r--r--   0        0        0      965 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/lock_secrets.py
+-rw-r--r--   0        0        0     2127 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/secret_creation.py
+-rw-r--r--   0        0        0      944 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/unlock_secrets.py
+-rw-r--r--   0        0        0     4126 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/archimedes_config/workflows/workflow_base.py
+-rw-r--r--   0        0        0      753 2023-05-04 13:22:12.072898 archimedes_config-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.0/PKG-INFO
```

### Comparing `archimedes_config-0.2.4/archimedes_config/arckeyl.py` & `archimedes_config-0.3.0/archimedes_config/arckeyl.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import os
 import stat
 from pathlib import Path
 
 import click
 import tomlkit
 
-from archimedes_config.utils.path_utils import clean_filename, find_repo_root
+from archimedes_config.utils.path_utils import (
+    clean_filename,
+    find_pyproject_directory,
+    find_repo_root,
+)
 from archimedes_config.utils.util import (
     RegisteredConfigDecrypted,
     check_encrypted,
     get_registered_configs,
     get_secret,
     register_config,
     register_secret,
@@ -50,15 +54,15 @@
         {COMMAND_NAME} unregister   Unregister config from pre-commit hook
     """.format(
         COMMAND_NAME=COMMAND_NAME
     )
 
 
 @cli.command("init")
-def init():
+def init():  # pylint:disable=too-many-statements
     """Initializes pre-commit"""
 
     # CREATE CONFIG REGISTRY
     if not Path(PRE_COMMIT_CHECK_PATH).exists():
         print(f"{COMMAND_NAME} config does not exist. Creating a new config...")
         config = tomlkit.document()
         config.add(
@@ -99,27 +103,40 @@
     else:
         print("Created .gitignore and added secrets to it")
         with open(gitignore_path, "a", encoding="utf8") as file:
             file.write(f"{SECRET_KEYS_FILE_NAME}\n")
 
     # CREATE PRE-COMMIT HOOK
     pre_commit_path = ROOT_PATH / ".git" / "hooks" / "pre-commit"
-    command = f"poetry run {COMMAND_NAME} check"
+    command_header = "##### ARCHIMEDES CONFIGURATION START ######\n"
+    pyproject_directory = str(find_pyproject_directory()).replace("\\", "\\\\")
+    command = f"pushd {pyproject_directory};poetry run {COMMAND_NAME} check;popd;\n"
+    command_tail = "##### ARCHIMEDES CONFIGURATION END ######\n"
     try:
         with open(pre_commit_path, "r", encoding="utf8") as file:
             lines = file.readlines()
-        if command not in lines:
-            lines.append(f"\n{command}")
+        if command_header not in lines:
+            lines.append(command_header)
+            lines.append(command)
+            lines.append(command_tail)
             print("Added encryption check to existing pre-commit webhook")
-            with open(pre_commit_path, "w", encoding="utf8") as file:
-                file.writelines(lines)
+        else:
+            pre = lines[0 : lines.index(command_header)]
+            post = lines[::-1]
+            post = post[0 : post.index(command_tail)][::-1]
+            lines = pre + ["\n", command_header, command, command_tail] + post
+            print("Updating encryption check to existing pre-commit webhook")
+        with open(pre_commit_path, "w", encoding="utf8") as file:
+            file.writelines(lines)
     except FileNotFoundError:
         print("Creating pre commit webhook")
         with open(pre_commit_path, "w", encoding="utf8") as file:
-            sample = f"#!/usr/bin/env bash\n\n{command}"
+            sample = (
+                f"#!/usr/bin/env bash\n\n{command_header}\n{command}\n{command_tail}"
+            )
             file.write(sample)
     try:
         os.chmod(
             pre_commit_path,
             os.stat(pre_commit_path).st_mode
             | stat.S_IXUSR  # user execute
             | stat.S_IXGRP  # group execute
```

### Comparing `archimedes_config-0.2.4/archimedes_config/config_manager.py` & `archimedes_config-0.3.0/archimedes_config/config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/keyvault_client.py` & `archimedes_config-0.3.0/archimedes_config/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/keyvault_config_manager.py` & `archimedes_config-0.3.0/archimedes_config/keyvault_config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/utils/util.py` & `archimedes_config-0.3.0/archimedes_config/utils/util.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/workflows/add_secrets.py` & `archimedes_config-0.3.0/archimedes_config/workflows/add_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/workflows/lock_secrets.py` & `archimedes_config-0.3.0/archimedes_config/workflows/lock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/workflows/secret_creation.py` & `archimedes_config-0.3.0/archimedes_config/workflows/secret_creation.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/workflows/unlock_secrets.py` & `archimedes_config-0.3.0/archimedes_config/workflows/unlock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/archimedes_config/workflows/workflow_base.py` & `archimedes_config-0.3.0/archimedes_config/workflows/workflow_base.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.4/pyproject.toml` & `archimedes_config-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archimedes-config"
-version = "0.2.4"
+version = "0.3.0"
 description = ""
 authors = ["BigyaPradhan <bigya.pradhan@optimeering.com>"]
 packages = [{include = "archimedes_config"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 cryptography = "^39.0.1"
```

### Comparing `archimedes_config-0.2.4/PKG-INFO` & `archimedes_config-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archimedes-config
-Version: 0.2.4
+Version: 0.3.0
 Summary: 
 Author: BigyaPradhan
 Author-email: bigya.pradhan@optimeering.com
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

