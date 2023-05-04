# Comparing `tmp/sphinx_json_schema_spec-2023.2.4.tar.gz` & `tmp/sphinx_json_schema_spec-2023.5.1.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.2.4.tar` & `sphinx_json_schema_spec-2023.5.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.flake8
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.readthedocs.yml
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.github/dependabot.yml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/Makefile
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/index.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/requirements.in
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/README.rst
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/pyproject.toml
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.2.4/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.flake8
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/release.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/Makefile
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/index.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/requirements.in
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/README.rst
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.2.4/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.5.1/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -14,10 +14,10 @@
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `sphinx_json_schema_spec-2023.2.4/noxfile.py` & `sphinx_json_schema_spec-2023.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.5.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.5.1/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

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
@@ -60,37 +60,40 @@
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
+      url: https://pypi.org/p/sphinx-json-schema-spec
+    permissions:
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
         uses: softprops/action-gh-release@v1
         with:
           files: |
             dist/*
           generate_release_notes: true
```

### Comparing `sphinx_json_schema_spec-2023.2.4/docs/Makefile` & `sphinx_json_schema_spec-2023.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/docs/conf.py` & `sphinx_json_schema_spec-2023.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/docs/index.rst` & `sphinx_json_schema_spec-2023.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/docs/requirements.txt` & `sphinx_json_schema_spec-2023.5.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/.gitignore` & `sphinx_json_schema_spec-2023.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/COPYING` & `sphinx_json_schema_spec-2023.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/README.rst` & `sphinx_json_schema_spec-2023.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/pyproject.toml` & `sphinx_json_schema_spec-2023.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.2.4/PKG-INFO` & `sphinx_json_schema_spec-2023.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.2.4
+Version: 2023.5.1
 Summary: Sphinx support for the JSON Schema specifications
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
 Author-email: Julian+sphinx-json-schema-spec@GrayVines.com
```

