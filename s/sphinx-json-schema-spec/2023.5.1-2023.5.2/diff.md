# Comparing `tmp/sphinx_json_schema_spec-2023.5.1.tar.gz` & `tmp/sphinx_json_schema_spec-2023.5.2.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.5.1.tar` & `sphinx_json_schema_spec-2023.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.flake8
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/Makefile
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/index.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/requirements.in
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/README.rst
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.flake8
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/release.yml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/Makefile
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/index.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/requirements.in
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/README.rst
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.5.1/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/noxfile.py` & `sphinx_json_schema_spec-2023.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.5.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.5.2/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,15 @@
   packaging:
     needs: ci
     runs-on: ubuntu-latest
     environment:
       name: PyPI
       url: https://pypi.org/p/sphinx-json-schema-spec
     permissions:
+      contents: write
       id-token: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `sphinx_json_schema_spec-2023.5.1/docs/Makefile` & `sphinx_json_schema_spec-2023.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/docs/conf.py` & `sphinx_json_schema_spec-2023.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/docs/index.rst` & `sphinx_json_schema_spec-2023.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/docs/requirements.txt` & `sphinx_json_schema_spec-2023.5.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/.gitignore` & `sphinx_json_schema_spec-2023.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/COPYING` & `sphinx_json_schema_spec-2023.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/README.rst` & `sphinx_json_schema_spec-2023.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/pyproject.toml` & `sphinx_json_schema_spec-2023.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.1/PKG-INFO` & `sphinx_json_schema_spec-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Sphinx support for the JSON Schema specifications
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
 Author-email: Julian+sphinx-json-schema-spec@GrayVines.com
```

