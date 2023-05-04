# Comparing `tmp/ivoire-0.3.1.tar.gz` & `tmp/ivoire-0.3.2.tar.gz`

## Comparing `ivoire-0.3.1.tar` & `ivoire-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ivoire-0.3.1/.coveragerc
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ivoire-0.3.1/.flake8
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 ivoire-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 ivoire-0.3.1/FAQ.rst
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ivoire-0.3.1/noxfile.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ivoire-0.3.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 ivoire-0.3.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ivoire-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ivoire-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.1/examples/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 ivoire-0.3.1/examples/calculator_spec.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ivoire-0.3.1/examples/next_spec.py
--rw-r--r--   0        0        0    25614 2020-02-02 00:00:00.000000 ivoire-0.3.1/examples/img/calculator_spec_output.png
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/__main__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/load.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/manager.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/result.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/run.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/standalone.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/__init__.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/context_manager_spec.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/context_spec.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/describe_spec.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/example_spec.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/load_spec.py
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/result_spec.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/run_spec.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/spec/unit/transform_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/tests/__init__.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/tests/test_result.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/tests/test_standalone.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/tests/test_transform.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ivoire-0.3.1/ivoire/tests/util.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ivoire-0.3.1/COPYING
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 ivoire-0.3.1/README.rst
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ivoire-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ivoire-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ivoire-0.3.2/.coveragerc
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ivoire-0.3.2/.flake8
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ivoire-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 ivoire-0.3.2/FAQ.rst
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ivoire-0.3.2/noxfile.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ivoire-0.3.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 ivoire-0.3.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ivoire-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 ivoire-0.3.2/.github/release.yml
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ivoire-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.2/examples/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 ivoire-0.3.2/examples/calculator_spec.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ivoire-0.3.2/examples/next_spec.py
+-rw-r--r--   0        0        0    25614 2020-02-02 00:00:00.000000 ivoire-0.3.2/examples/img/calculator_spec_output.png
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/__main__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/load.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/manager.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/result.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/run.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/standalone.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/__init__.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/context_manager_spec.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/context_spec.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/describe_spec.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/example_spec.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/load_spec.py
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/result_spec.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/run_spec.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/spec/unit/transform_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/tests/__init__.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/tests/test_result.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/tests/test_standalone.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/tests/test_transform.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ivoire-0.3.2/ivoire/tests/util.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ivoire-0.3.2/COPYING
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 ivoire-0.3.2/README.rst
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ivoire-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ivoire-0.3.2/PKG-INFO
```

### Comparing `ivoire-0.3.1/.pre-commit-config.yaml` & `ivoire-0.3.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/flake8
     rev: "6.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.1.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.4"
     hooks:
```

### Comparing `ivoire-0.3.1/FAQ.rst` & `ivoire-0.3.2/FAQ.rst`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/noxfile.py` & `ivoire-0.3.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/.github/SECURITY.md` & `ivoire-0.3.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/.github/workflows/ci.yml` & `ivoire-0.3.2/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,70 +8,91 @@
   schedule:
     # Daily at 4:21
     - cron: "21 4 * * *"
 
 env:
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_PYTHON_VERSION_WARNING: "1"
-  PYTHON_LATEST: "3.11"
 
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - uses: pre-commit/action@v3.0.0
 
+  list:
+    runs-on: ubuntu-latest
+    outputs:
+      noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up nox
+        uses: wntrblm/nox@2023.04.22
+      - id: noxenvs-matrix
+        run: |
+          echo >>$GITHUB_OUTPUT noxenvs=$(
+            nox --list-sessions |
+            grep '^* ' |
+            cut -d ' ' -f 2- |
+            jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
+          )
+
   ci:
+    needs: list
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
+        noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
 
     steps:
       - uses: actions/checkout@v3
       - name: Install dependencies
         run: sudo apt-get update && sudo apt-get install -y libenchant-2-dev
-        if: runner.os == 'Linux'
+        if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
-        if: runner.os == 'macOS'
+        if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
-        run: nox
+        run: nox -s "${{ matrix.noxenv }}"
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
+    environment:
+      name: PyPI
+      url: https://pypi.org/p/ivoire
+    permissions:
+      contents: write
+      id-token: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - name: Install dependencies
         run: python -m pip install build
       - name: Create packages
         run: python -m build .
-      - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
       - name: Publish to PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
       - name: Create a Release
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
         uses: softprops/action-gh-release@v1
         with:
           files: |
             dist/*
           generate_release_notes: true
```

### Comparing `ivoire-0.3.1/examples/calculator_spec.py` & `ivoire-0.3.2/examples/calculator_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/examples/next_spec.py` & `ivoire-0.3.2/examples/next_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/examples/img/calculator_spec_output.png` & `ivoire-0.3.2/examples/img/calculator_spec_output.png`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/__init__.py` & `ivoire-0.3.2/ivoire/__init__.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/load.py` & `ivoire-0.3.2/ivoire/load.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/manager.py` & `ivoire-0.3.2/ivoire/manager.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/result.py` & `ivoire-0.3.2/ivoire/result.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/run.py` & `ivoire-0.3.2/ivoire/run.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/standalone.py` & `ivoire-0.3.2/ivoire/standalone.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/transform.py` & `ivoire-0.3.2/ivoire/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
             kw_defaults=[],
             kwonlyargs=[],
             posonlyargs=[],
         )
 
 
 class ExampleLoader(SourceFileLoader):
-
     suffix = "_spec.py"
 
     @classmethod
     def register(cls):
         """
         Register the path hook.
```

### Comparing `ivoire-0.3.1/ivoire/spec/unit/context_manager_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/context_manager_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/context_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/context_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/describe_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/describe_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/example_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/example_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/load_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/load_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/result_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/result_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/run_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/run_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/spec/unit/transform_spec.py` & `ivoire-0.3.2/ivoire/spec/unit/transform_spec.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/tests/test_result.py` & `ivoire-0.3.2/ivoire/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/tests/test_standalone.py` & `ivoire-0.3.2/ivoire/tests/test_standalone.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/ivoire/tests/test_transform.py` & `ivoire-0.3.2/ivoire/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/COPYING` & `ivoire-0.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/README.rst` & `ivoire-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/pyproject.toml` & `ivoire-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ivoire-0.3.1/PKG-INFO` & `ivoire-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivoire
-Version: 0.3.1
+Version: 0.3.2
 Summary: A simple RSpec-like testing framework.
 Project-URL: Homepage, https://github.com/Julian/Ivoire
 Project-URL: Issues, https://github.com/Julian/Ivoire/issues/
 Project-URL: Source, https://github.com/Julian/Ivoire
 Author: Julian Berman
 Author-email: Julian+Ivoire@GrayVines.com
 License: MIT
```

