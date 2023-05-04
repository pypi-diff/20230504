# Comparing `tmp/aws_clipper-0.0.7.tar.gz` & `tmp/aws_clipper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_clipper-0.0.7.tar", max compression
+gzip compressed data, was "aws_clipper-0.0.8.tar", max compression
```

## Comparing `aws_clipper-0.0.7.tar` & `aws_clipper-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2603 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      672 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/README.md
--rw-r--r--   0        0        0     2059 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2789 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/__init__.py
--rw-r--r--   0        0        0       65 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/__main__.py
--rw-r--r--   0        0        0     1323 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/cli.py
--rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 aws_clipper-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2887 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/LICENSE
+-rw-r--r--   0        0        0      789 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/README.md
+-rw-r--r--   0        0        0     2216 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2789 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/src/aws_clipper/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/src/aws_clipper/__main__.py
+-rw-r--r--   0        0        0     1323 2023-05-04 07:00:01.519643 aws_clipper-0.0.8/src/aws_clipper/cli.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 aws_clipper-0.0.8/PKG-INFO
```

### Comparing `aws_clipper-0.0.7/CHANGELOG.md` & `aws_clipper-0.0.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [v0.0.8](https://github.com/kai2nenobu/aws-clipper/compare/v0.0.7...v0.0.8) - 2023-05-04
+- Add MIT license file by @kai2nenobu in https://github.com/kai2nenobu/aws-clipper/pull/31
+- Test multiple versions by tox by @kai2nenobu in https://github.com/kai2nenobu/aws-clipper/pull/33
+
 ## [v0.0.7](https://github.com/kai2nenobu/aws-clipper/compare/v0.0.6...v0.0.7) - 2023-04-26
 - Enrich project info by @kai2nenobu in https://github.com/kai2nenobu/aws-clipper/pull/28
 
 ## [v0.0.6](https://github.com/kai2nenobu/aws-clipper/compare/v0.0.5...v0.0.6) - 2023-04-26
 - Use src layout for a project structure by @kai2nenobu in https://github.com/kai2nenobu/aws-clipper/pull/25
 - Build single executables by PyInstaller by @kai2nenobu in https://github.com/kai2nenobu/aws-clipper/pull/24
```

### Comparing `aws_clipper-0.0.7/pyproject.toml` & `aws_clipper-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 [tool.poetry]
 name = "aws-clipper"
-version = "0.0.7"
+version = "0.0.8"
 description = "`aws-clipper` dumps AWS CLI config from a simple YAML file."
 authors = ["kai2nenobu <kai2nenobu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_clipper", from = "src"}]
 homepage = "https://github.com/kai2nenobu/aws-clipper"
 repository = "https://github.com/kai2nenobu/aws-clipper"
 keywords = ["aws"]
-include = ["README.md", "CHANGELOG.md"]
+include = [
+    { path = "CHANGELOG.md", format = "sdist" }
+]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/kai2nenobu/aws-clipper/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/kai2nenobu/aws-clipper/issues"
 
 [tool.poetry.scripts]
 aws-clipper = 'aws_clipper.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = "^6.0"
 
 
 [tool.poetry.group.dev.dependencies]
+tox = [
+    {version = "^3.20.0", python = "<3.8"},
+    {version = "^4.0.0", python = ">=3.8"}
+]
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 
-
 [tool.poetry.group.lint.dependencies]
 pre-commit = [
     {version = "^2.21.0", python = "<3.8"},
     {version = "^3.2.0", python = ">=3.8"}
 ]
 black = "^23.1.0"
 isort = [
```

### Comparing `aws_clipper-0.0.7/src/aws_clipper/__init__.py` & `aws_clipper-0.0.8/src/aws_clipper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import configparser
 from typing import Any, TextIO
 
 import yaml
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 
 def _expand_value(v: Any, variables: dict[str, Any] = {}) -> str:
     """
     In AWS CLI config, nested settings (like S3 settings) are indented as below.
 
     [default]
```

### Comparing `aws_clipper-0.0.7/src/aws_clipper/cli.py` & `aws_clipper-0.0.8/src/aws_clipper/cli.py`

 * *Files identical despite different names*

### Comparing `aws_clipper-0.0.7/PKG-INFO` & `aws_clipper-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-clipper
-Version: 0.0.7
+Version: 0.0.8
 Summary: `aws-clipper` dumps AWS CLI config from a simple YAML file.
 Home-page: https://github.com/kai2nenobu/aws-clipper
 License: MIT
 Keywords: aws
 Author: kai2nenobu
 Author-email: kai2nenobu@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -20,17 +20,21 @@
 Project-URL: Changelog, https://github.com/kai2nenobu/aws-clipper/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/kai2nenobu/aws-clipper
 Description-Content-Type: text/markdown
 
 [![PyPI][pypi_badge]][pypi_project] ![PythonVersions][pyversions] ![LICENSE][license_badge] [![CI][actions_status]][ci_workflow]
 
 [pypi_project]: https://pypi.org/project/aws-clipper/
-[pypi_badge]: https://img.shields.io/badge/pypi-v0.0.7-orange
+[pypi_badge]: https://img.shields.io/badge/pypi-v0.0.8-orange
 [license_badge]: https://img.shields.io/badge/license-MIT-green
 [pyversions]: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
 [actions_status]: https://github.com/kai2nenobu/aws-clipper/actions/workflows/ci.yml/badge.svg
 [ci_workflow]: https://github.com/kai2nenobu/aws-clipper/actions/workflows/ci.yml
 
 # aws-clipper
 
 `aws-clipper` dumps AWS CLI config from a simple YAML file.
 
+## License
+
+This project is developed and distributed under MIT license. See [LICENCE](./LICENSE) for more details.
+
```

