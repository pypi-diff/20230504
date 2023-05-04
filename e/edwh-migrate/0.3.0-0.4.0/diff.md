# Comparing `tmp/edwh_migrate-0.3.0.tar.gz` & `tmp/edwh_migrate-0.4.0.tar.gz`

## Comparing `edwh_migrate-0.3.0.tar` & `edwh_migrate-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources.xml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/migrate.iml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0    13833 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/workspace.xml
--rw-r--r--   0        0        0    47176 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    17991 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/test_basics.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/README.md
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 edwh_migrate-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/.gitignore
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/dataSources.xml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/migrate.iml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/workspace.xml
+-rw-r--r--   0        0        0    47176 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    19142 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/README.md
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 edwh_migrate-0.4.0/PKG-INFO
```

### Comparing `edwh_migrate-0.3.0/CHANGELOG.md` & `edwh_migrate-0.4.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.0 (2023-05-04)
+### Feature
+* Support for argv[1] as a path to a python file, or to the folder where `migrations.py` is stored. ([`7d0aba6`](https://github.com/educationwarehouse/migrate/commit/7d0aba641907ca4100a10a3fba67e3286ab8f5c6))
+
 ## v0.3.0 (2023-05-04)
 ### Feature
 * Failed tests will sometimes be written to db; better support for sqlite; better unpacker code, better docs, more translation into english ([`7701670`](https://github.com/educationwarehouse/migrate/commit/7701670b8e4adc234a2ae8abeac8780adda65330))
 
 ### Documentation
 * **env:** Environment variables documented ([`71950c2`](https://github.com/educationwarehouse/migrate/commit/71950c20d6dbed59892192b7344dafd109131e9f))
```

### Comparing `edwh_migrate-0.3.0/migrations.py` & `edwh_migrate-0.4.0/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/requirements.txt` & `edwh_migrate-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/.idea/dataSources.local.xml` & `edwh_migrate-0.4.0/.idea/dataSources.local.xml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/.idea/dataSources.xml` & `edwh_migrate-0.4.0/.idea/dataSources.xml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/.idea/jupyter-settings.xml` & `edwh_migrate-0.4.0/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/.idea/workspace.xml` & `edwh_migrate-0.4.0/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `edwh_migrate-0.3.0/.idea/workspace.xml` & `edwh_migrate-0.4.0/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="b9dfa005-973e-426b-a995-bfbb447e401a" name="Changes" comment="docs(env): environment variables documented"/>
+    <list default="true" id="b9dfa005-973e-426b-a995-bfbb447e401a" name="Changes" comment="docs(env): environment variables documented">
+      <change beforePath="$PROJECT_DIR$/src/edwh_migrate/migrate.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh_migrate/migrate.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -51,15 +53,15 @@
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/tests/sqlite_empty"/>
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.pytest for tests.test_basics">
+  <component name="RunManager" selected="Shell Script.Just build">
     <configuration name="Build and publish" type="ShConfigurationType">
       <option name="SCRIPT_TEXT" value="semantic-release publish; hatch build -c ; hatch publish"/>
       <option name="INDEPENDENT_SCRIPT_PATH" value="true"/>
       <option name="SCRIPT_PATH" value=""/>
       <option name="SCRIPT_OPTIONS" value=""/>
       <option name="INDEPENDENT_SCRIPT_WORKING_DIRECTORY" value="true"/>
       <option name="SCRIPT_WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
@@ -177,14 +179,15 @@
       <workItem from="1682856198533" duration="26000"/>
       <workItem from="1682944643103" duration="137000"/>
       <workItem from="1682944788597" duration="373000"/>
       <workItem from="1682945171245" duration="33000"/>
       <workItem from="1682945213264" duration="599000"/>
       <workItem from="1682951723167" duration="1538000"/>
       <workItem from="1683054220384" duration="7000"/>
+      <workItem from="1683191307970" duration="2286000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: initial release
 
 Cleaned a lot of previously used code.">
       <created>1682194309892</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
```

### Comparing `edwh_migrate-0.3.0/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml` & `edwh_migrate-0.4.0/.idea/dataSources/21da014d-6e3f-42ea-8c44-aedba5c52d26.xml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/src/edwh_migrate/__init__.py` & `edwh_migrate-0.4.0/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/src/edwh_migrate/migrate.py` & `edwh_migrate-0.4.0/src/edwh_migrate/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    - public."user"
    - public.item
    forget and fail...
 
 """
 import contextlib
 import datetime
+import importlib
 import os
 import pathlib
 import sqlite3
 import sys
 import time
 import typing
 import urllib
@@ -442,21 +443,41 @@
         $export MIGRATE_URI='sqlite://test.db'
         
         ''')
         exit(0)
 
     with contextlib.suppress(MigrateLockExists):
         with schema_versioned_lock_file():
-            if Path('migrations.py').exists():
+            arg = None
+            if sys.argv[1:]:
+                # use the first argument as a reference to the migrations file
+                # or the folder where the migrations file is stored
+                arg = pathlib.Path(sys.argv[1])
+                if arg.exists() and arg.is_file():
+                    print(f"importing migrations from {arg}")
+                    sys.path.insert(0, str(arg.parent))
+                    # importing the migrations.py file will register the functions
+                    importlib.import_module(arg.stem)
+                elif arg.exists() and arg.is_dir():
+                    print(f"importing migrations from {arg}/migrations.py")
+                    sys.path.insert(0, str(arg))
+                    # importing the migrations.py file will register the functions
+                    importlib.import_module('migrations')
+                else:
+                    print(f"ERROR: no migrations found at {arg}", file=sys.stderr)
+                    exit(1)
+            elif Path('migrations.py').exists():
                 print("migrations.py exists, importing @migration decorated functions.")
                 sys.path.insert(0, os.getcwd())
                 # importing the migrations.py file will register the functions
                 import migrations
                 print(f'{len(registered_functions)} migrations discovered')
-
+            else:
+                print(f"ERROR: no migrations found at {os.getcwd()}", file=sys.stderr)
+                exit(1)
             print("starting migrate hook")
             if activate_migrations():
                 print("migration completed successfully, marking success.")
             else:
                 raise MigrationFailed('Not every migration succeeded.')
 
 # ------------------------------------------------------------------------------------------------
```

### Comparing `edwh_migrate-0.3.0/tests/test_basics.py` & `edwh_migrate-0.4.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.4.0/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.4.0/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/.gitignore` & `edwh_migrate-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/LICENSE.txt` & `edwh_migrate-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/README.md` & `edwh_migrate-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/pyproject.toml` & `edwh_migrate-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.3.0/PKG-INFO` & `edwh_migrate-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.3.0
+Version: 0.4.0
 Summary: Helps migrating database schema changes using pydal. 
 Project-URL: Documentation, https://github.com/unknown/-#readme
 Project-URL: Issues, https://github.com/unknown/-/issues
 Project-URL: Source, https://github.com/unknown/-
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

