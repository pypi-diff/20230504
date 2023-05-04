# Comparing `tmp/evm-trace-0.1.0a8.tar.gz` & `tmp/evm-trace-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evm-trace-0.1.0a8.tar", last modified: Thu Sep  8 19:07:31 2022, max compression
+gzip compressed data, was "evm-trace-0.1.0a9.tar", last modified: Sat Sep 10 17:32:37 2022, max compression
```

## Comparing `evm-trace-0.1.0a8.tar` & `evm-trace-0.1.0a9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.736346 evm-trace-0.1.0a8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4977 2022-09-08 19:07:31.736346 evm-trace-0.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/evm_trace/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5402 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/display.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/gas.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/parity.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/evm_trace/vmtrace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/evm_trace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4977 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-08 19:07:31.000000 evm-trace-0.1.0a8/evm_trace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-08 19:07:31.736346 evm-trace-0.1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.732346 evm-trace-0.1.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.728345 evm-trace-0.1.0a8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 19:07:31.736346 evm-trace-0.1.0a8/tests/data/parity/
--rw-r--r--   0 runner    (1001) docker     (121)   137258 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/call.json
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/create.json
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/create_revert.json
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/error.json
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/revert.json
--rw-r--r--   0 runner    (1001) docker     (121)    10608 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/revert_with_message.json
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/data/parity/selfdestruct.json
--rw-r--r--   0 runner    (1001) docker     (121)    12817 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/test_call_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/test_parity_trace.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-08 19:07:03.000000 evm-trace-0.1.0a8/tests/test_trace_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.739202 evm-trace-0.1.0a9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-09-10 17:32:37.739202 evm-trace-0.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/evm_trace/
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5402 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/gas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/parity.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6263 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/evm_trace/vmtrace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/evm_trace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-10 17:32:37.000000 evm-trace-0.1.0a9/evm_trace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-10 17:32:37.739202 evm-trace-0.1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.739202 evm-trace-0.1.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.735201 evm-trace-0.1.0a9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 17:32:37.739202 evm-trace-0.1.0a9/tests/data/parity/
+-rw-r--r--   0 runner    (1001) docker     (121)   137258 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/call.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/create.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/create_revert.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/error.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/revert.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10608 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/revert_with_message.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/data/parity/selfdestruct.json
+-rw-r--r--   0 runner    (1001) docker     (121)    12817 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/test_call_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/test_parity_trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-10 17:32:16.000000 evm-trace-0.1.0a9/tests/test_trace_frame.py
```

### Comparing `evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/bug.md` & `evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 ---
 name: Bug report
 about: Report an error that you've encountered.
 labels: 'bug'
 ---
 ### Environment information
 
+* Python Version: x.x.x
+* OS: macOS/linux/win
+
+If using with `ape`, please provide:
+
 * `ape` and plugin versions:
 
 ```
 $ ape --version
 # ...copy and paste result of above command here...
 
 $ ape plugins list
 # ...copy and paste result of above command here...
 ```
 
-* Python Version: x.x.x
-* OS: osx/linux/win
-
 ### What went wrong?
 
 Please include information like:
 
 * what command you ran
 * the code that caused the failure (see [this link](https://help.github.com/articles/basic-writing-and-formatting-syntax/) for help with formatting code)
 * full output of the error you received
```

### Comparing `evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/feature.md` & `evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/ISSUE_TEMPLATE/work-item.md` & `evm-trace-0.1.0a9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/release-drafter.yml` & `evm-trace-0.1.0a9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/workflows/commitlint.yaml` & `evm-trace-0.1.0a9/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/workflows/publish.yaml` & `evm-trace-0.1.0a9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/workflows/test.yaml` & `evm-trace-0.1.0a9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.github/workflows/title.yaml` & `evm-trace-0.1.0a9/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.gitignore` & `evm-trace-0.1.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/.pre-commit-config.yaml` & `evm-trace-0.1.0a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/CONTRIBUTING.md` & `evm-trace-0.1.0a9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/LICENSE` & `evm-trace-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/PKG-INFO` & `evm-trace-0.1.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # evm-trace
+Description: # Quick Start
         
         Ethereum Virtual Machine transaction tracing tool
         
         ## Dependencies
         
         * [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
```

### Comparing `evm-trace-0.1.0a8/README.md` & `evm-trace-0.1.0a9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# evm-trace
+# Quick Start
 
 Ethereum Virtual Machine transaction tracing tool
 
 ## Dependencies
 
 * [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
```

### Comparing `evm-trace-0.1.0a8/evm_trace/base.py` & `evm-trace-0.1.0a9/evm_trace/base.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/evm_trace/display.py` & `evm-trace-0.1.0a9/evm_trace/display.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/evm_trace/gas.py` & `evm-trace-0.1.0a9/evm_trace/gas.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/evm_trace/parity.py` & `evm-trace-0.1.0a9/evm_trace/parity.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/evm_trace/vmtrace.py` & `evm-trace-0.1.0a9/evm_trace/vmtrace.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 
 from typing import Any, Dict, Iterator, List, Optional, Type, Union
 
 from eth.vm.memory import Memory  # type: ignore
 from eth.vm.stack import Stack  # type: ignore
 from eth_utils import to_checksum_address
 from hexbytes import HexBytes
-
-try:
-    from msgspec import Struct  # type: ignore
-    from msgspec.json import Decoder  # type: ignore
-except ImportError as e:
-    raise ImportError("msgspec not found. install it with `pip install msgspec`") from e
+from msgspec import Struct  # type: ignore
+from msgspec.json import Decoder  # type: ignore
 
 # opcodes grouped by the number of items they pop from the stack
 # fmt: off
 POP_OPCODES = {
     1: ["EXTCODEHASH", "ISZERO", "NOT", "BALANCE", "CALLDATALOAD", "EXTCODESIZE", "BLOCKHASH", "POP", "MLOAD", "SLOAD", "JUMP", "SELFDESTRUCT"],  # noqa: E501
     2: ["SHL", "SHR", "SAR", "REVERT", "ADD", "MUL", "SUB", "DIV", "SDIV", "MOD", "SMOD", "EXP", "SIGNEXTEND", "LT", "GT", "SLT", "SGT", "EQ", "AND", "XOR", "OR", "BYTE", "SHA3", "MSTORE", "MSTORE8", "SSTORE", "JUMPI", "RETURN"],  # noqa: E501
     3: ["RETURNDATACOPY", "ADDMOD", "MULMOD", "CALLDATACOPY", "CODECOPY", "CREATE"],
```

### Comparing `evm-trace-0.1.0a8/evm_trace.egg-info/PKG-INFO` & `evm-trace-0.1.0a9/evm_trace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # evm-trace
+Description: # Quick Start
         
         Ethereum Virtual Machine transaction tracing tool
         
         ## Dependencies
         
         * [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
```

### Comparing `evm-trace-0.1.0a8/evm_trace.egg-info/SOURCES.txt` & `evm-trace-0.1.0a9/evm_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/pyproject.toml` & `evm-trace-0.1.0a9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `evm-trace-0.1.0a8/setup.py` & `evm-trace-0.1.0a9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/evm-trace",
     include_package_data=True,
     install_requires=[
-        "importlib-metadata ; python_version<'3.8'",
-        "pydantic>=1.10.1,<2.0",
-        "hexbytes>=0.3.0,<1.0.0",
-        "eth-utils>=2.0.0",
-        "ethpm-types>=0.3.7,<0.4.0",
+        "pydantic>=1.10.1,<2",
+        "hexbytes>=0.3.0,<1",
+        "eth-utils>=2",
+        "ethpm-types>=0.3.7,<0.4",
+        "msgspec>=0.8.0",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["evm_trace"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `evm-trace-0.1.0a8/tests/conftest.py` & `evm-trace-0.1.0a9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/call.json` & `evm-trace-0.1.0a9/tests/data/parity/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/create.json` & `evm-trace-0.1.0a9/tests/data/parity/create.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/create_revert.json` & `evm-trace-0.1.0a9/tests/data/parity/create_revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/error.json` & `evm-trace-0.1.0a9/tests/data/parity/error.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/revert.json` & `evm-trace-0.1.0a9/tests/data/parity/revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/revert_with_message.json` & `evm-trace-0.1.0a9/tests/data/parity/revert_with_message.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/data/parity/selfdestruct.json` & `evm-trace-0.1.0a9/tests/data/parity/selfdestruct.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/expected_traces.py` & `evm-trace-0.1.0a9/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/test_call_tree.py` & `evm-trace-0.1.0a9/tests/test_call_tree.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/test_gas_report.py` & `evm-trace-0.1.0a9/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/test_parity_trace.py` & `evm-trace-0.1.0a9/tests/test_parity_trace.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.0a8/tests/test_trace_frame.py` & `evm-trace-0.1.0a9/tests/test_trace_frame.py`

 * *Files identical despite different names*

