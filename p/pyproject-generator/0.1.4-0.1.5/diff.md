# Comparing `tmp/pyproject-generator-0.1.4.tar.gz` & `tmp/pyproject-generator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.4.tar", last modified: Wed May  3 20:45:51 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.5.tar", last modified: Thu May  4 18:16:42 2023, max compression
```

## Comparing `pyproject-generator-0.1.4.tar` & `pyproject-generator-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.787041 pyproject-generator-0.1.4/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-05-03 20:45:51.787178 pyproject-generator-0.1.4/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.4/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.4/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-03 20:45:51.788104 pyproject-generator-0.1.4/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.759606 pyproject-generator-0.1.4/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.766649 pyproject-generator-0.1.4/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-05-03 20:45:40.000000 pyproject-generator-0.1.4/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-03 20:45:03.000000 pyproject-generator-0.1.4/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3494 2023-05-02 21:04:44.000000 pyproject-generator-0.1.4/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.769282 pyproject-generator-0.1.4/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.4/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.4/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1312 2023-05-03 20:35:21.000000 pyproject-generator-0.1.4/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    14894 2023-05-03 20:38:37.000000 pyproject-generator-0.1.4/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2727 2023-05-03 18:55:58.000000 pyproject-generator-0.1.4/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.781844 pyproject-generator-0.1.4/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.4/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.4/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.4/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.4/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.4/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.4/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.786280 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      956 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.786811 pyproject-generator-0.1.4/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.4/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.780785 pyproject-generator-0.1.5/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.5/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3564 2023-05-04 18:16:42.780945 pyproject-generator-0.1.5/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3023 2023-05-04 18:03:16.000000 pyproject-generator-0.1.5/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-04 02:13:28.000000 pyproject-generator-0.1.5/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-04 18:16:42.785353 pyproject-generator-0.1.5/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.737608 pyproject-generator-0.1.5/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.746989 pyproject-generator-0.1.5/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-03 20:58:26.000000 pyproject-generator-0.1.5/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-04 18:16:36.000000 pyproject-generator-0.1.5/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3530 2023-05-04 13:38:47.000000 pyproject-generator-0.1.5/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.749914 pyproject-generator-0.1.5/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.5/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.5/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1314 2023-05-04 13:50:03.000000 pyproject-generator-0.1.5/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15640 2023-05-04 13:37:51.000000 pyproject-generator-0.1.5/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-04 01:29:47.000000 pyproject-generator-0.1.5/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.769211 pyproject-generator-0.1.5/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.5/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.5/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.5/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      986 2023-05-04 02:20:31.000000 pyproject-generator-0.1.5/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.5/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.5/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.5/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.779674 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3564 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1061 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.780513 pyproject-generator-0.1.5/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.5/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.4/setup.cfg` & `pyproject-generator-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject/cli.py` & `pyproject-generator-0.1.5/src/pyproject/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import typing
 from typing import Optional
 
-from .project_builder import Action, ProjectBuilder
 from .__version__ import __version__
+from .project_builder import LICENSE_NAME_MAPPER, Action, ProjectBuilder
 
 ACTIONS = list(typing.get_args(Action))
-LICENSES = ("apache", "mit")
+LICENSES = list(LICENSE_NAME_MAPPER.keys())
 
 
 def _parse_arg_to_set(string: Optional[str], sep: str = ",") -> set[str]:
     """Expects a delimited string of arguments, e.g. `a,b,c,d`. Transforms string
     into a set.
 
     Args:
```

### Comparing `pyproject-generator-0.1.4/src/pyproject/logger.py` & `pyproject-generator-0.1.5/src/pyproject/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
+
 import enum
 from typing import Callable, Optional
 
-from rich.console import Console
 import rich.pretty
+from rich.console import Console
+
 from .spinner import Spinner
 
 
 class Level(enum.Enum):
     ERROR = 1
     INFO = 2
```

### Comparing `pyproject-generator-0.1.4/src/pyproject/project_builder.py` & `pyproject-generator-0.1.5/src/pyproject/project_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 # Imports
 
 from __future__ import annotations
 
 import dataclasses
 import datetime
-import os
 import json
-from pathlib import Path
+import os
 import re
 import shutil
-import subprocess
 import string
+import subprocess
 import sys
+import venv
+from pathlib import Path
 from types import SimpleNamespace
 from typing import Literal, Optional, Union
-import venv
 
 import platformdirs
 from rich.panel import Panel
 
 from .logger import CustomConsole, Level
 
 # Globals
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
 USER_CONFIG_PATH = platformdirs.user_config_dir(
     appname="pyproject-generator", appauthor="cangyuanli"
 )
 
+LICENSE_NAME_MAPPER = {
+    "mit": "MIT",
+    "apache": "Apache",
+    "gpl_v3": "GPL v3",
+    "bsd3": "BSD 3-Clause",
+}
+
 # Types
 
 Action = Literal["init", "upload", "config"]
 PathLike = Union[Path, str]
 
 
 @dataclasses.dataclass
 class License:
     short_name: str
     proper_name: Optional[str] = None
 
     def __post_init__(self):
         if self.proper_name is None:
-            name_mapper = {"mit": "MIT", "apache": "Apache", "gpl_v3": "GPL v3"}
-            self.proper_name = name_mapper[self.short_name]
+            self.proper_name = LICENSE_NAME_MAPPER[self.short_name]
 
 
 @dataclasses.dataclass
 class Config:
     pypi_username: str
     pypi_password: str
     github_url: str
@@ -258,14 +264,17 @@
 
     def _init_config_files(self, proj_path: Path, templates: dict):
         (proj_path / "tox.ini").write_text(templates["tox"])
         (proj_path / "pyproject.toml").write_text(templates["pyproject"])
         (proj_path / "setup.cfg").write_text(templates["setup"])
         (proj_path / ".gitignore").write_text(templates["gitignore"])
         (proj_path / "README.md").write_text(templates["readme"])
+        (proj_path / ".pre-commit-config.yaml").write_text(
+            templates["pre_commit_config"]
+        )
 
         license = self._config.license.short_name
         (proj_path / "LICENSE").write_text(templates[f"license_{license}"])
 
     @staticmethod
     def _init_github_actions(proj_path, templates: dict):
         workflows_path = proj_path / ".github/workflows"
@@ -368,17 +377,36 @@
             self._console.spinner(
                 lambda: venv_builder.run_bin(
                     ["pip", "install", dep], stdout=subprocess.DEVNULL
                 ),
                 text=dep,
             )
 
+        self._console.info(Panel("Finalizing project..."), justify="left")
+
         # Create requirements_dev file
-        reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
-        (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
+        def _create_req_file():
+            reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
+            (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
+
+        self._console.spinner(
+            _create_req_file,
+            "Creating requirements_dev.txt",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # Ensure pre-commit is up to date
+        self._console.spinner(
+            lambda: venv_builder.run_bin(
+                ["pre-commit", "autoupdate"], stdout=subprocess.DEVNULL
+            ),
+            "Ensuring pre-commit config is up to date",
+            clear=True,
+        )
 
         self._console.info(f"Done setting up {project_name}!", style="green")
 
     def _parse_config_file(self, filename: PathLike) -> Config:
         if filename == "default_config.json":
             path = BASE_PATH / "config/default_config.json"
         elif filename == "config.json":
```

### Comparing `pyproject-generator-0.1.4/src/pyproject/spinner.py` & `pyproject-generator-0.1.5/src/pyproject/spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import time
 from typing import Optional
 
 from rich.console import Console
 
 BACKSPACE = "\b"
 CLEAR_LINE = "\033[K"
-CHECKMARK = "\u2713"
-XMARK = "\u274C"
+CHECKMARK = "[green]\u2713[/green]"
+XMARK = "[red]\u274C[/red]"
 
 
 class Spinner:
     def __init__(
         self,
         console: Console,
         text: str,
```

### Comparing `pyproject-generator-0.1.4/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.5/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.5/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.5/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.5/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.5/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.4/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.5/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/logger.py
 src/pyproject/project_builder.py
 src/pyproject/spinner.py
 src/pyproject/config/config.json
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/license_apache.template
+src/pyproject/templates/license_bsd3.template
 src/pyproject/templates/license_gpl_v3.template
 src/pyproject/templates/license_mit.template
+src/pyproject/templates/pre_commit_config.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
 src/pyproject_generator.egg-info/SOURCES.txt
```

