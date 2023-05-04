# Comparing `tmp/pytest-github-actions-annotate-failures-0.1.8.tar.gz` & `tmp/pytest-github-actions-annotate-failures-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-github-actions-annotate-failures-0.1.8.tar", last modified: Mon Dec 19 15:53:26 2022, max compression
+gzip compressed data, was "pytest-github-actions-annotate-failures-0.2.0.tar", last modified: Thu May  4 11:05:02 2023, max compression
```

## Comparing `pytest-github-actions-annotate-failures-0.1.8.tar` & `pytest-github-actions-annotate-failures-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/plugin_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-19 15:53:26.000000 pytest-github-actions-annotate-failures-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-19 15:53:20.000000 pytest-github-actions-annotate-failures-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:05:02.585419 pytest-github-actions-annotate-failures-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:05:02.581419 pytest-github-actions-annotate-failures-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:05:02.581419 pytest-github-actions-annotate-failures-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-04 11:05:02.585419 pytest-github-actions-annotate-failures-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:05:02.581419 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:05:02.585419 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 11:05:02.000000 pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:05:02.585419 pytest-github-actions-annotate-failures-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 11:04:47.000000 pytest-github-actions-annotate-failures-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-github-actions-annotate-failures-0.1.8/CHANGELOG.md` & `pytest-github-actions-annotate-failures-0.2.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## 0.2.0 (2023-05-04)
+
+### Incompatible changes
+
+- Require python 3.7+ #66 (thanks to @ssbarnea)
+
+### Other changes
+
+- Fix publish package workflow #74
+- Handle cases where pytest itself fails #70 (thanks to @edgarrmondragon)
+- Adopt PEP-621 for packaging #65 (thanks to @ssbarnea)
+- Bump pre-commit/action from 2.0.0 to 3.0.0 #56
+
 ## 0.1.8 (2022-12-20)
 
 No functionality change.
 - Change URL of PyPI project link #61
 - Fix CI environment #62 (thanks to @henryiii, @nicoddemus)
 
 ## 0.1.7 (2022-07-02)
```

### Comparing `pytest-github-actions-annotate-failures-0.1.8/LICENSE` & `pytest-github-actions-annotate-failures-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-github-actions-annotate-failures-0.1.8/PKG-INFO` & `pytest-github-actions-annotate-failures-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 Metadata-Version: 2.1
 Name: pytest-github-actions-annotate-failures
-Version: 0.1.8
+Version: 0.2.0
 Summary: pytest plugin to annotate failed tests with a workflow command for GitHub Actions
-Home-page: https://github.com/pytest-dev/pytest-github-actions-annotate-failures
-Author: utgwkk
-Author-email: utagawakiki@gmail.com
+Author-email: utgwkk <utagawakiki@gmail.com>
+Maintainer-email: utgwkk <utagawakiki@gmail.com>
 License: MIT
+Project-URL: homepage, https://github.com/pytest-dev/pytest-github-actions-annotate-failures
+Project-URL: repository, https://github.com/pytest-dev/pytest-github-actions-annotate-failures
+Project-URL: changelog, https://github.com/pytest-dev/pytest-github-actions-annotate-failures/releases
+Keywords: ansible,testing,molecule,plugin
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-github-actions-annotate-failures
 [Pytest](https://pypi.org/project/pytest/) plugin to annotate failed tests with a [workflow command for GitHub Actions](https://help.github.com/en/actions/reference/workflow-commands-for-github-actions)
 
 ## Usage
```

### Comparing `pytest-github-actions-annotate-failures-0.1.8/README.md` & `pytest-github-actions-annotate-failures-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-github-actions-annotate-failures-0.1.8/plugin_test.py` & `pytest-github-actions-annotate-failures-0.2.0/plugin_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,36 @@
     )
     testdir.monkeypatch.setenv("GITHUB_ACTIONS", "true")
     result = testdir.runpytest_subprocess()
 
     no_fnmatch_line(result, "::error file=test_annotation_succeed_no_output.py")
 
 
+def test_annotation_pytest_error(testdir):
+    testdir.makepyfile(
+        """
+        import pytest
+        pytest_plugins = 'pytest_github_actions_annotate_failures'
+
+        @pytest.fixture
+        def fixture():
+            return 1
+
+        def test_error():
+            assert fixture() == 1
+        """
+    )
+    testdir.monkeypatch.setenv("GITHUB_ACTIONS", "true")
+    result = testdir.runpytest_subprocess()
+
+    result.stderr.re_match_lines(
+        [r"::error file=test_annotation_pytest_error\.py,line=8::test_error.*",]
+    )
+
+
 def test_annotation_fail(testdir):
     testdir.makepyfile(
         """
         import pytest
         pytest_plugins = 'pytest_github_actions_annotate_failures'
 
         def test_fail():
```

### Comparing `pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures/plugin.py` & `pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # -*- coding: utf-8 -*-
-from __future__ import print_function
+
+from __future__ import annotations
 
 import os
 import sys
 from collections import OrderedDict
+from typing import TYPE_CHECKING
+
+from _pytest._code.code import ExceptionRepr
 
 import pytest
 
+if TYPE_CHECKING:
+    from _pytest.nodes import Item
+    from _pytest.reports import CollectReport
+
+
 # Reference:
 # https://docs.pytest.org/en/latest/writing_plugins.html#hookwrapper-executing-around-other-hooks
 # https://docs.pytest.org/en/latest/writing_plugins.html#hook-function-ordering-call-example
 # https://docs.pytest.org/en/stable/reference.html#pytest.hookspec.pytest_runtest_makereport
 #
 # Inspired by:
 # https://github.com/pytest-dev/pytest/blob/master/src/_pytest/terminal.py
 
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
-def pytest_runtest_makereport(item, call):
+def pytest_runtest_makereport(item: Item, call):
     # execute all other hooks to obtain the report object
     outcome = yield
-    report = outcome.get_result()
+    report: CollectReport = outcome.get_result()
 
     # enable only in a workflow of GitHub Actions
     # ref: https://help.github.com/en/actions/configuring-and-managing-workflows/using-environment-variables#default-environment-variables
     if os.environ.get("GITHUB_ACTIONS") != "true":
         return
 
     if report.when == "call" and report.failed:
@@ -53,21 +62,22 @@
             # 0-index to 1-index
             lineno += 1
 
         # get the name of the current failed test, with parametrize info
         longrepr = report.head_line or item.name
 
         # get the error message and line number from the actual error
-        if hasattr(report.longrepr, "reprcrash"):
-            longrepr += "\n\n" + report.longrepr.reprcrash.message
-            traceback_entries = report.longrepr.reprtraceback.reprentries
-            if len(traceback_entries) > 1:
+        if isinstance(report.longrepr, ExceptionRepr):
+            if report.longrepr.reprcrash is not None:
+                longrepr += "\n\n" + report.longrepr.reprcrash.message
+            tb_entries = report.longrepr.reprtraceback.reprentries
+            if len(tb_entries) > 1 and tb_entries[0].reprfileloc is not None:
                 # Handle third-party exceptions
-                lineno = traceback_entries[0].reprfileloc.lineno
-            else:
+                lineno = tb_entries[0].reprfileloc.lineno
+            elif report.longrepr.reprcrash is not None:
                 lineno = report.longrepr.reprcrash.lineno
         elif isinstance(report.longrepr, tuple):
             _, lineno, message = report.longrepr
             longrepr += "\n\n" + message
         elif isinstance(report.longrepr, str):
             longrepr += "\n\n" + report.longrepr
```

### Comparing `pytest-github-actions-annotate-failures-0.1.8/pytest_github_actions_annotate_failures.egg-info/PKG-INFO` & `pytest-github-actions-annotate-failures-0.2.0/pytest_github_actions_annotate_failures.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 Metadata-Version: 2.1
 Name: pytest-github-actions-annotate-failures
-Version: 0.1.8
+Version: 0.2.0
 Summary: pytest plugin to annotate failed tests with a workflow command for GitHub Actions
-Home-page: https://github.com/pytest-dev/pytest-github-actions-annotate-failures
-Author: utgwkk
-Author-email: utagawakiki@gmail.com
+Author-email: utgwkk <utagawakiki@gmail.com>
+Maintainer-email: utgwkk <utagawakiki@gmail.com>
 License: MIT
+Project-URL: homepage, https://github.com/pytest-dev/pytest-github-actions-annotate-failures
+Project-URL: repository, https://github.com/pytest-dev/pytest-github-actions-annotate-failures
+Project-URL: changelog, https://github.com/pytest-dev/pytest-github-actions-annotate-failures/releases
+Keywords: ansible,testing,molecule,plugin
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Pytest
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-github-actions-annotate-failures
 [Pytest](https://pypi.org/project/pytest/) plugin to annotate failed tests with a [workflow command for GitHub Actions](https://help.github.com/en/actions/reference/workflow-commands-for-github-actions)
 
 ## Usage
```

