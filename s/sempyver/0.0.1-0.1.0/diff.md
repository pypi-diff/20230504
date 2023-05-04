# Comparing `tmp/sempyver-0.0.1.tar.gz` & `tmp/sempyver-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sempyver-0.0.1.tar", last modified: Tue Apr  4 08:16:13 2023, max compression
+gzip compressed data, was "sempyver-0.1.0.tar", last modified: Thu May  4 06:57:13 2023, max compression
```

## Comparing `sempyver-0.0.1.tar` & `sempyver-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 08:16:02.000000 sempyver-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-04 08:16:13.244418 sempyver-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 08:16:02.000000 sempyver-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-04 08:16:02.000000 sempyver-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.240418 sempyver-0.0.1/sempyver/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/cli_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/changelog_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/changeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/modules/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver/cli_application/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/tags_for_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-04 08:16:02.000000 sempyver-0.0.1/sempyver/cli_application/utilities/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:16:13.244418 sempyver-0.0.1/sempyver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 08:16:13.000000 sempyver-0.0.1/sempyver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:16:13.244418 sempyver-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 08:16:02.000000 sempyver-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 06:57:01.000000 sempyver-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 06:57:13.929071 sempyver-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-04 06:57:01.000000 sempyver-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 06:57:01.000000 sempyver-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/cli_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver/cli_application/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/modules/changelog_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/modules/changeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/modules/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver/cli_application/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/utilities/tags_for_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/cli_application/utilities/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/helpers/cache_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/helpers/toml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-04 06:57:01.000000 sempyver-0.1.0/sempyver/helpers/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:57:13.929071 sempyver-0.1.0/sempyver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 06:57:13.000000 sempyver-0.1.0/sempyver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:57:13.929071 sempyver-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-04 06:57:01.000000 sempyver-0.1.0/setup.py
```

### Comparing `sempyver-0.0.1/LICENSE` & `sempyver-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/pyproject.toml` & `sempyver-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 pylint = "~=2.15"
 bandit = "~=1.7"
 autopep8 = "~=2.0"
 pytest = "~=7.2"
 pytest-cov = "~=2.10"
 faker = "~=17.6"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.sempyver]
+version_file_path = "sempyver/_version.py"
```

### Comparing `sempyver-0.0.1/sempyver/cli_application/cli_app.py` & `sempyver-0.1.0/sempyver/cli_application/cli_app.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/changelog_generator.py` & `sempyver-0.1.0/sempyver/cli_application/modules/changelog_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,47 +6,19 @@
 import sys
 from typing import Dict, List, Union, Tuple
 from datetime import datetime
 from pathlib import Path
 from collections import defaultdict
 from colorama import init, Fore, Style
 # Local imports
+from sempyver.helpers.update_version import update_version, update_version_file
 from sempyver.helpers.cache_generator import open_cache_file, create_cache
 from sempyver.cli_application.utilities.tags_for_change import CHANGELOG_TAG, VERSION_UPDATE
 
 
-def update_version(change: str) -> str:
-    """Update the version to write it on the changelog.
-
-    Args:
-        change (str): Type of change.
-
-    Returns:
-        str: New version
-    """
-    version = "1.0.0"
-    # Use the change list
-    position_to_change: int = VERSION_UPDATE[change]
-    version_numbers: Dict[str, str] = {
-        f"Pos. {i}": v for i, v in enumerate(version.split("."))}
-    new_version: Dict[str, str] = {}
-    _position = f"Pos. {position_to_change}"
-    already_upgrade_version: bool = False
-    for position, number_of_version in version_numbers.items():
-        if position != _position and already_upgrade_version is False:
-            new_version[position] = number_of_version
-        elif position == _position:
-            new_version[position] = f"{int(number_of_version)+1}"
-            already_upgrade_version = True
-        else:
-            new_version[position] = "0"
-    # Return the new version
-    return ".".join(version for version in new_version.values())
-
-
 def read_changesets() -> Union[
         Tuple[Dict[str, List[str]], str, List[str]],
         Tuple[None, None, None]]:
     """Read all the changesets files from the changeset folders.
 
     Returns:
         Union[List[str], List[None]]: Content found
@@ -120,14 +92,16 @@
     # Now, create a cache to avoid the unnecessary creation of repeated files
     create_cache(files)
     # Retrieve the version to assign
     if type_of_change:
         version_to_assign = update_version(type_of_change)
         content_to_write.append(
             f"## [{version_to_assign}] - {datetime.now().date()}\n\n")
+        # Update the version file
+        update_version_file(version_to_assign)
     # Add the `content_from_changesets` to the content_to_write
     for key, items in content_from_changesets.items():
         content_to_write.append(f"### {key}\n\n")
         for item in items:
             content_to_write.append(item)
         content_to_write.append("\n")
     # Try to find a changelog file
```

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/changeset.py` & `sempyver-0.1.0/sempyver/cli_application/modules/changeset.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/modules/commit.py` & `sempyver-0.1.0/sempyver/cli_application/modules/commit.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/utilities/tags_for_change.py` & `sempyver-0.1.0/sempyver/cli_application/utilities/tags_for_change.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver/cli_application/utilities/theme.py` & `sempyver-0.1.0/sempyver/cli_application/utilities/theme.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.1/sempyver.egg-info/SOURCES.txt` & `sempyver-0.1.0/sempyver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 sempyver/cli_application/cli_app.py
 sempyver/cli_application/modules/__init__.py
 sempyver/cli_application/modules/changelog_generator.py
 sempyver/cli_application/modules/changeset.py
 sempyver/cli_application/modules/commit.py
 sempyver/cli_application/utilities/__init__.py
 sempyver/cli_application/utilities/tags_for_change.py
-sempyver/cli_application/utilities/theme.py
+sempyver/cli_application/utilities/theme.py
+sempyver/helpers/__init__.py
+sempyver/helpers/cache_generator.py
+sempyver/helpers/toml_reader.py
+sempyver/helpers/update_version.py
```

### Comparing `sempyver-0.0.1/setup.py` & `sempyver-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,28 +21,42 @@
     if version_coincidence is None:
         raise TypeError("Couldn't find the version in the given file.")
     version = version_coincidence.group(1)
     # Return the version
     return version
 
 
+def long_description() -> str:
+    """Open the `README.md` file and return the long description
+
+    Returns:
+        - All the `README.md` as a simple and large string
+    """
+    with open("./README.md", encoding="utf-8") as file:
+        description = file.readlines()
+    return "".join(line for line in description)
+
+
 setup(
     name='sempyver',
     version=read_version(),
-    description='Setting up a python package',
-    long_description="",  # ! TO BE ADDED
+    description='Tool for teams to manage the CHANGELOG given a list of different changes.',
+    long_description=long_description(),
+    long_description_content_type='text/markdown',
     author='Ricardo Leal',
     author_email='ricardo.lealpz@gmail.com',
     maintainer='Ricardo Leal',
     maintainer_email='ricardo.lealpz@gmail.com',
     url='',  # ! TO BE ADDED
-    packages=find_packages(include=['sempyver', 'sempyver.*']),
+    packages=find_packages(
+        include=['sempyver', 'sempyver.*', 'sempyver.helpers']),
+    include_package_data=True,
     install_requires=[
         'click~=8.1',
         'inquirer~=3.1',
         'colorama==0.4.6',
         'faker~=17.6'
     ],
     entry_points={
-        'console_scripts': ['sempyver=sempyver.__main__:run']
+        'console_scripts': ['semver=sempyver.__main__:run']
     }
 )
```

