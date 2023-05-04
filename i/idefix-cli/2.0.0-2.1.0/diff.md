# Comparing `tmp/idefix_cli-2.0.0.tar.gz` & `tmp/idefix_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.0.0.tar", last modified: Wed Apr 26 19:41:39 2023, max compression
+gzip compressed data, was "idefix_cli-2.1.0.tar", last modified: Thu May  4 13:22:53 2023, max compression
```

## Comparing `idefix_cli-2.0.0.tar` & `idefix_cli-2.1.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.039720 idefix_cli-2.0.0/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_write.py
```

### Comparing `idefix_cli-2.0.0/LICENSE` & `idefix_cli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/PKG-INFO` & `idefix_cli-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.0.0
+Version: 2.1.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-2.0.0/README.md` & `idefix_cli-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/__main__.py` & `idefix_cli-2.1.0/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_backports.py` & `idefix_cli-2.1.0/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/clean.py` & `idefix_cli-2.1.0/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/clone.py` & `idefix_cli-2.1.0/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/conf.py` & `idefix_cli-2.1.0/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/read.py` & `idefix_cli-2.1.0/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/run.py` & `idefix_cli-2.1.0/idefix_cli/_commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 import subprocess
 import sys
 from copy import deepcopy
 from enum import auto
 from multiprocessing import cpu_count
 from pathlib import Path
-from subprocess import CalledProcessError, check_call
 from tempfile import NamedTemporaryFile
 from time import sleep, time
 from typing import Final
 
 import inifix
 from rich.prompt import Confirm
 
@@ -22,14 +21,15 @@
     get_config_file,
     get_option,
     print_err,
     print_subcommand,
     print_success,
     print_warning,
     requires_idefix,
+    run_subcommand,
 )
 
 if sys.version_info >= (3, 11):
     from contextlib import chdir
     from enum import StrEnum
     from typing import assert_never
 else:
@@ -106,21 +106,15 @@
 )
 
 
 @requires_idefix()
 def build_idefix(directory) -> int:
     ncpus = 2 ** min(3, cpu_count().bit_length())
     cmd = ["make", "-j", str(ncpus)]
-    print_subcommand(cmd, loc=Path(directory))
-    try:
-        with chdir(directory):
-            return check_call(cmd)
-    except CalledProcessError as exc:
-        print_err("failed to build idefix")
-        return exc.returncode
+    return run_subcommand(cmd, loc=Path(directory), err="failed to build idefix")
 
 
 def add_arguments(parser) -> None:
     parser.add_argument("--dir", dest="directory", default=".", help="target directory")
     parser.add_argument(
         "-i",
         dest="inifile",
```

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/stamp.py` & `idefix_cli-2.1.0/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/_commands/write.py` & `idefix_cli-2.1.0/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/idefix_cli/lib.py` & `idefix_cli-2.1.0/idefix_cli/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,20 +195,20 @@
     elif THEME is Theme.BABALLE:
         emoji = ":guide_dog:"
     else:
         assert_never(THEME)
     console.print(f"{emoji}[bold chartreuse1] {message}[/]")
 
 
-def print_subcommand(cmd: list[str], *, loc: Path | None = None) -> None:
+def print_subcommand(cmd: list[str], *, loc: os.PathLike[str] | None = None) -> None:
     """Print a command, which is to be executed as a subprocess.
 
     Args:
         cmd (list[str]): equivalent argument to be passed to, e.g., subprocess.run
-        loc (pathlib.Path | None): the directory (other than cwd)
+        loc (os.PathLike[str] | None): the directory (other than cwd)
             from which the command is meant to be executed.
 
     Returns:
         None
 
     Examples:
         >>> import os
@@ -216,32 +216,64 @@
         >>> from pathlib import Path
         >>> def my_command() -> int:
         ...    cmd = ["which", "gcc"]
         ...    print_subcommand(cmd, loc=Path.home())
         ...    subprocess.run(cmd)
         ...    return 0
         >>> my_command()
-        🚀 running (from ...) which gcc
+        🚀 running which gcc (from ...)
         ...
     """
     msg = " ".join(cmd)
-
-    header = "running"
-    if loc is not None and loc.resolve() != Path.cwd():
-        header += f" (from {loc}{os.sep})"
+    trailer = ""
+    if loc is not None and Path(loc).resolve() != Path.cwd():
+        trailer = f" (from {loc}{os.sep})"
 
     console = Console(width=500, highlight=False)
     THEME = get_theme()
     if THEME is Theme.DEFAULT:
         emoji = ":rocket:"
     elif THEME is Theme.BABALLE:
         emoji = ":dog_face:"
     else:
         assert_never(THEME)
-    console.print(f"{emoji}[italic cornflower_blue] {header}[/] [bold]{msg}[/]")
+    console.print(f"{emoji}[italic cornflower_blue] running[/] [bold]{msg}[/]{trailer}")
+
+
+def run_subcommand(
+    cmd: list[str], *, loc: os.PathLike[str] | None = None, err: str | None = None
+) -> int:
+    """
+    Convenience function to run subprocess while logging with print_subcommand
+
+    Args:
+        cmd (list[str]): equivalent argument to be passed to subprocess.run
+        loc (os.PathLike[str] | None): the directory (other than cwd)
+            from which the command is meant to be executed.
+        err (str | None): error message to be printed in case the subprocess fails
+
+    Returns:
+      retcode (int): the return code of the subprocess
+    """
+    from subprocess import CalledProcessError, run
+
+    chdir = __getattr__("chdir")
+    if loc is None:
+        loc = Path.cwd()
+    print_subcommand(cmd, loc=loc)
+    try:
+        with chdir(loc):
+            p = run(cmd, check=True)
+    except CalledProcessError as exc:
+        if err is None:
+            err = f"failed to run {' '.join(cmd)!r}"
+        print_err(err)
+        return exc.returncode
+    else:
+        return p.returncode
 
 
 def files_from_patterns(source, *patterns, recursive: bool = False) -> list[str]:
     """
     Args:
         source (os.PathLike[str]): path to the directory to inspect
         patterns (str): file patterns (e.g. "*.py", "*.txt" ...)
```

### Comparing `idefix_cli-2.0.0/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.1.0/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.0.0
+Version: 2.1.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-2.0.0/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.1.0/idefix_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 idefix_cli/_commands/__init__.py
 idefix_cli/_commands/clean.py
 idefix_cli/_commands/clone.py
 idefix_cli/_commands/conf.py
 idefix_cli/_commands/read.py
 idefix_cli/_commands/run.py
 idefix_cli/_commands/stamp.py
+idefix_cli/_commands/switch.py
 idefix_cli/_commands/write.py
 tests/test_app_structure.py
 tests/test_clean.py
 tests/test_clone.py
 tests/test_commons.py
 tests/test_conf.py
+tests/test_lib.py
 tests/test_read.py
 tests/test_run.py
 tests/test_stamp.py
 tests/test_ux.py
 tests/test_write.py
```

### Comparing `idefix_cli-2.0.0/pyproject.toml` & `idefix_cli-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "2.0.0"
+version = "2.1.0"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
```

### Comparing `idefix_cli-2.0.0/tests/test_app_structure.py` & `idefix_cli-2.1.0/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_clean.py` & `idefix_cli-2.1.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_clone.py` & `idefix_cli-2.1.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_commons.py` & `idefix_cli-2.1.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_conf.py` & `idefix_cli-2.1.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_read.py` & `idefix_cli-2.1.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_run.py` & `idefix_cli-2.1.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_stamp.py` & `idefix_cli-2.1.0/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.0.0/tests/test_ux.py` & `idefix_cli-2.1.0/tests/test_ux.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from idefix_cli.__main__ import main
 
 if sys.version_info >= (3, 10):
     OPTIONAL_SEC = "options"
 else:
     OPTIONAL_SEC = "optional arguments"
 HELP_MESSAGE = (
-    "usage: idfx [-h] [-v] {clean,clone,conf,read,run,stamp,write} ...\n"
+    "usage: idfx [-h] [-v] {clean,clone,conf,read,run,stamp,switch,write} ...\n"
     "\n"
     f"{OPTIONAL_SEC}:\n"
     "  -h, --help            show this help message and exit\n"
     "  -v, --version         show program's version number and exit\n"
     "\n"
     "commands:\n"
-    "  {clean,clone,conf,read,run,stamp,write}\n"
+    "  {clean,clone,conf,read,run,stamp,switch,write}\n"
     "    clean               remove compilation files\n"
     "    clone               clone a problem directory\n"
     "    conf                configure Idefix\n"
     "    read                read an Idefix inifile and print it to json format\n"
     "    run                 run an Idefix problem\n"
     "    stamp               print relevant data for reproduction to stdout\n"
+    "    switch              switch git branch in $IDEFIX_DIR using git checkout\n"
     "    write               write an Idefix inifile from a json string\n"
 )
 
 
 @pytest.mark.usefixtures("isolated_conf_dir")
 def test_no_command_passed(capsys):
     ret = main([])
```

### Comparing `idefix_cli-2.0.0/tests/test_write.py` & `idefix_cli-2.1.0/tests/test_write.py`

 * *Files identical despite different names*

