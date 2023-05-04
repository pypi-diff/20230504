# Comparing `tmp/openxes_cli_py-0.1.6.tar.gz` & `tmp/openxes_cli_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxes_cli_py-0.1.6.tar", max compression
+gzip compressed data, was "openxes_cli_py-0.1.7.tar", max compression
```

## Comparing `openxes_cli_py-0.1.6.tar` & `openxes_cli_py-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      615 2023-05-04 13:13:35.117868 openxes_cli_py-0.1.6/README.md
--rw-r--r--   0        0        0  3717515 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/lib/openxes-cli.jar
--rw-r--r--   0        0        0      481 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/src/openxes_cli/__init__.py
--rw-r--r--   0        0        0     1196 2023-05-04 13:13:35.145870 openxes_cli_py-0.1.6/src/openxes_cli/lib.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      744 2023-05-04 15:18:32.209949 openxes_cli_py-0.1.7/README.md
+-rw-r--r--   0        0        0  3717515 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/lib/openxes-cli.jar
+-rw-r--r--   0        0        0      481 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/src/openxes_cli/__init__.py
+-rw-r--r--   0        0        0     1216 2023-05-04 15:18:32.233950 openxes_cli_py-0.1.7/src/openxes_cli/lib.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.7/PKG-INFO
```

### Comparing `openxes_cli_py-0.1.6/lib/openxes-cli.jar` & `openxes_cli_py-0.1.7/lib/openxes-cli.jar`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.6/src/openxes_cli/lib.py` & `openxes_cli_py-0.1.7/src/openxes_cli/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 import os
 
 from pathlib import Path
 
 logging.basicConfig(level=logging.INFO)
 
-jar_file = Path(__file__).parent.parent.parent / "lib/openxes-cli.jar"
+jar_file = Path(__file__).parent.parent / "lib/openxes-cli.jar"
 
 
 def xes_to_csv(xes_path: Path, csv_path: Path, jar_file: Path = jar_file):
     """
     Converts XES to CSV using openxes-cli.jar. Java 8 is required.
 
     :param xes_path: Event log in XES format either with the .xes or .xes.gz extension.
     :param csv_path: Output path for the CSV file.
     :param jar_file: Path to the openxes-cli.jar file. Default: lib/openxes-cli.jar.
     :return: Exit code of the Java process.
     """
     return run_jar(jar_file, "-f", str(xes_path), "-t", "csv", "-o", str(csv_path))
 
 
-def csv_to_xes(csv_path: Path, xes_path: Path):
+def csv_to_xes(csv_path: Path, xes_path: Path, jar_file: Path = jar_file):
     """
     Converts CSV to XES using openxes-cli.jar. Java 8 is required.
 
     :param csv_path: Event log in CSV format.
     :param xes_path: Output path for the XES file.
     :return: Exit code of the Java process.
     """
```

### Comparing `openxes_cli_py-0.1.6/PKG-INFO` & `openxes_cli_py-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxes-cli-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Ihar Suvorau
 Author-email: ihar.suvorau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,12 +15,21 @@
 
 ![OpenXES-CLI](https://github.com/AutomatedProcessImprovement/openxes-cli-py/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/openxes-cli-py)
 
 These are Python bindings for the [OpenXES-CLI](https://github.com/AutomatedProcessImprovement/openxes-cli) application. It allows you to convert XES files to CSV files and vice
 versa from your Python code.
 
+## Installation
+
+The package requires **Python 3.9+**. You can install it from PyPI: 
+
+
+```shell
+pip install openxes-cli-py
+```
+
 ## Releases
 
 You can browse compiled releases which include the underlying jar file in the [Releases](https://github.com/AutomatedProcessImprovement/openxes-cli-py/releases)
 section.
```

