# Comparing `tmp/github_reserved_names-1.0.1.tar.gz` & `tmp/github_reserved_names-2023.5.1.tar.gz`

## Comparing `github_reserved_names-1.0.1.tar` & `github_reserved_names-2023.5.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.flake8
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/github_reserved_names.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/noxfile.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/test_github_reserved_names.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/.github/workflows/cron.yml
--rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/bin/check_for_differences
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/bin/parse_source_data
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/source_data/reserved-names.json
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/COPYING
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/README.rst
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 github_reserved_names-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.flake8
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/github_reserved_names.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/noxfile.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/test_github_reserved_names.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/release.yml
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/workflows/cron.yml
+-rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/bin/check_for_differences
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/bin/parse_source_data
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/source_data/reserved-names.json
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/COPYING
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/README.rst
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/PKG-INFO
```

### Comparing `github_reserved_names-1.0.1/.pre-commit-config.yaml` & `github_reserved_names-2023.5.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,31 +9,31 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
-    rev: v5.11.3
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/PyCQA/flake8
-    rev: "5.0.4"
+    rev: "6.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/yesqa
     rev: v1.4.0
     hooks:
       - id: yesqa
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.2
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 23.1.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.4"
     hooks:
```

### Comparing `github_reserved_names-1.0.1/github_reserved_names.py` & `github_reserved_names-2023.5.1/github_reserved_names.py`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/noxfile.py` & `github_reserved_names-2023.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/.github/SECURITY.md` & `github_reserved_names-2023.5.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/.github/workflows/ci.yml` & `github_reserved_names-2023.5.1/.github/workflows/ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions |
             grep '^* ' |
             cut -d ' ' -f 2- |
             jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
@@ -57,41 +57,41 @@
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
+    environment:
+      name: PyPI
+      url: https://pypi.org/p/github-reserved-names
+    permissions:
+      contents: write
+      id-token: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: python -m pip install build
       - name: Create packages
         run: python -m build .
       - name: Publish to PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
       - name: Create a Release
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: actions/github-script@v6
+        uses: softprops/action-gh-release@v1
         with:
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-
-          script: |
-            await github.request(`POST /repos/${{ github.repository }}/releases`, {
-              tag_name: "${{ github.ref }}",
-              generate_release_notes: true
-            });
+          files: |
+            dist/*
+          generate_release_notes: true
```

### Comparing `github_reserved_names-1.0.1/bin/check_for_differences` & `github_reserved_names-2023.5.1/bin/check_for_differences`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/source_data/reserved-names.json` & `github_reserved_names-2023.5.1/source_data/reserved-names.json`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/COPYING` & `github_reserved_names-2023.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/README.rst` & `github_reserved_names-2023.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/pyproject.toml` & `github_reserved_names-2023.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_reserved_names-1.0.1/PKG-INFO` & `github_reserved_names-2023.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github_reserved_names
-Version: 1.0.1
+Version: 2023.5.1
 Summary: A list of paths that GitHub uses which aren't real users
 Project-URL: Homepage, https://github.com/Julian/github-reserved-names
 Project-URL: Issues, https://github.com/Julian/github-reserved-names/issues/
 Project-URL: Source, https://github.com/Julian/github-reserved-names
 Author: Julian Berman
 Author-email: Julian+github_reserved_names@GrayVines.com
 License: MIT
```

