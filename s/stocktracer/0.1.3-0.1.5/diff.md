# Comparing `tmp/stocktracer-0.1.3.tar.gz` & `tmp/stocktracer-0.1.5.tar.gz`

## Comparing `stocktracer-0.1.3.tar` & `stocktracer-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 stocktracer-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 stocktracer-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 stocktracer-0.1.3/Makefile
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stocktracer-0.1.3/Pipfile
--rw-r--r--   0        0        0    67701 2020-02-02 00:00:00.000000 stocktracer-0.1.3/Pipfile.lock
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 stocktracer-0.1.3/SECURITY.md
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 stocktracer-0.1.3/auto-format.sh
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stocktracer-0.1.3/conftest.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 stocktracer-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 stocktracer-0.1.3/pydocktest.json
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 stocktracer-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 stocktracer-0.1.3/requirements.txt
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/release.yml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/cleanup.yml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/python.yml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/release-test.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/getting-started.md
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/index.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/analysis.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/caching.md
--rw-r--r--   0        0        0    20504 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/data-retrieval.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/index.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/reference.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/design/report.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/javascripts/tablesort.js
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 stocktracer-0.1.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/__main__.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/cli.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/analysis/__init__.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/analysis/diluted_eps.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/analysis/stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/data/__init__.py
--rw-r--r--   0        0        0    19444 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/stocktracer/data/sec.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/test_filter.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/test_sec.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/test_sec_network.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/test_xbrl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/analysis/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/analysis/test_diluted_eps.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/analysis/test_stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/fixtures/network/__init__.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 stocktracer-0.1.3/src/tests/fixtures/network/sec.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 stocktracer-0.1.3/.gitignore
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 stocktracer-0.1.3/LICENSE
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 stocktracer-0.1.3/README.md
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 stocktracer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    20896 2020-02-02 00:00:00.000000 stocktracer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 stocktracer-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 stocktracer-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 stocktracer-0.1.5/Makefile
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stocktracer-0.1.5/Pipfile
+-rw-r--r--   0        0        0    67701 2020-02-02 00:00:00.000000 stocktracer-0.1.5/Pipfile.lock
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 stocktracer-0.1.5/SECURITY.md
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 stocktracer-0.1.5/auto-format.sh
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stocktracer-0.1.5/conftest.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 stocktracer-0.1.5/mkdocs.yml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 stocktracer-0.1.5/pydocktest.json
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 stocktracer-0.1.5/requirements-dev.txt
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 stocktracer-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/release.yml
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/cleanup.yml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/python.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/release-test.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/getting-started.md
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/index.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/analysis.md
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/caching.md
+-rw-r--r--   0        0        0    20504 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/data-retrieval.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/index.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/reference.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/design/report.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/javascripts/tablesort.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 stocktracer-0.1.5/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/__main__.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/cli.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/analysis/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/analysis/diluted_eps.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/analysis/stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/data/__init__.py
+-rw-r--r--   0        0        0    19444 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/stocktracer/data/sec.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/test_filter.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/test_sec.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/test_sec_network.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/test_xbrl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/analysis/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/analysis/test_diluted_eps.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/analysis/test_stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/fixtures/network/__init__.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 stocktracer-0.1.5/src/tests/fixtures/network/sec.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 stocktracer-0.1.5/.gitignore
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 stocktracer-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 stocktracer-0.1.5/README.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 stocktracer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    21104 2020-02-02 00:00:00.000000 stocktracer-0.1.5/PKG-INFO
```

### Comparing `stocktracer-0.1.3/CODE_OF_CONDUCT.md` & `stocktracer-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/CONTRIBUTING.md` & `stocktracer-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/Pipfile` & `stocktracer-0.1.5/Pipfile`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/Pipfile.lock` & `stocktracer-0.1.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/mkdocs.yml` & `stocktracer-0.1.5/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-site_name: Ticker - Fundamental Analysis
+site_name: StockTracer
 theme:
   name: material
   palette:
     scheme: default
     primary: green
   icon:
     repo: fontawesome/brands/github
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-site_name: Ticker - Fundamental Analysis theme: name: material palette: scheme:
-default primary: green icon: repo: fontawesome/brands/github edit: material/
-pencil view: material/eye features: - content.action.edit - navigation.instant
-- navigation.tracking - navigation.sections - navigation.footer # -
+site_name: StockTracer theme: name: material palette: scheme: default primary:
+green icon: repo: fontawesome/brands/github edit: material/pencil view:
+material/eye features: - content.action.edit - navigation.instant -
+navigation.tracking - navigation.sections - navigation.footer # -
 navigation.indexes - toc.follow - toc.integrate # - navigation.expand -
 navigation.tabs - navigation.top # - header.autohide repo_url: https://
 github.com/gyund/fundamental-analysis repo_name: gyund/fundamental-analysis
 edit_uri: edit/main/docs/docs/ plugins: - search - tags - gen-files: scripts: -
 docs/gen_ref_pages.py - mkdocstrings - literate-nav: nav_file: SUMMARY.md -
 section-index markdown_extensions: - tables - admonition - pymdownx.details -
 pymdownx.superfences: custom_fences: - name: mermaid class: mermaid format:
```

### Comparing `stocktracer-0.1.3/requirements-dev.txt` & `stocktracer-0.1.5/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/requirements.txt` & `stocktracer-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `stocktracer-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/workflows/cleanup.yml` & `stocktracer-0.1.5/.github/workflows/cleanup.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/workflows/docs.yml` & `stocktracer-0.1.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/workflows/publish-pypi.yml` & `stocktracer-0.1.5/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/workflows/python.yml` & `stocktracer-0.1.5/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.github/workflows/release-test.yml` & `stocktracer-0.1.5/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 # separate terms of service, privacy policy, and support
 # documentation.
 
 # GitHub recommends pinning actions to a commit SHA.
 # To get a newer version, you will need to update the SHA.
 # You can also reference a tag or branch, but the action may change without warning.
 
-name: Test - Upload Python Package
+name: Upload Python Package
 
 on:
-  push:
-    branches:
-      - 16-publish-package
+  release:
+    types: [published]
 
 jobs:
   deploy:
     permissions:
-      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
+        id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     uses: ./.github/workflows/publish-pypi.yml
     with:
-        ENVIRONMENT: release-test
+        ENVIRONMENT: release
```

### Comparing `stocktracer-0.1.3/.github/workflows/release.yml` & `stocktracer-0.1.5/.github/workflows/release-test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 # separate terms of service, privacy policy, and support
 # documentation.
 
 # GitHub recommends pinning actions to a commit SHA.
 # To get a newer version, you will need to update the SHA.
 # You can also reference a tag or branch, but the action may change without warning.
 
-name: Upload Python Package
+name: Test - Upload Python Package
 
 on:
-  release:
-    types: [published]
+  push:
+    branches:
+      - release-*
 
 jobs:
   deploy:
     permissions:
-        id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     uses: ./.github/workflows/publish-pypi.yml
     with:
-        ENVIRONMENT: release
+        ENVIRONMENT: release-test
```

### Comparing `stocktracer-0.1.3/docs/gen_ref_pages.py` & `stocktracer-0.1.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/getting-started.md` & `stocktracer-0.1.5/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/index.md` & `stocktracer-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/design/analysis.md` & `stocktracer-0.1.5/docs/design/analysis.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/design/caching.md` & `stocktracer-0.1.5/docs/design/caching.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/design/data-retrieval.md` & `stocktracer-0.1.5/docs/design/data-retrieval.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/design/reference.md` & `stocktracer-0.1.5/docs/design/reference.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/design/report.md` & `stocktracer-0.1.5/docs/design/report.md`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/docs/stylesheets/extra.css` & `stocktracer-0.1.5/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/stocktracer/cli.py` & `stocktracer-0.1.5/src/stocktracer/cli.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/stocktracer/filter.py` & `stocktracer-0.1.5/src/stocktracer/filter.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/stocktracer/analysis/diluted_eps.py` & `stocktracer-0.1.5/src/stocktracer/analysis/diluted_eps.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/stocktracer/analysis/stub.py` & `stocktracer-0.1.5/src/stocktracer/analysis/stub.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/stocktracer/data/sec.py` & `stocktracer-0.1.5/src/stocktracer/data/sec.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/test_filter.py` & `stocktracer-0.1.5/src/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/test_sec.py` & `stocktracer-0.1.5/src/tests/test_sec.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/test_sec_network.py` & `stocktracer-0.1.5/src/tests/test_sec_network.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/test_xbrl.py` & `stocktracer-0.1.5/src/tests/test_xbrl.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/analysis/test_diluted_eps.py` & `stocktracer-0.1.5/src/tests/analysis/test_diluted_eps.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/analysis/test_stub.py` & `stocktracer-0.1.5/src/tests/analysis/test_stub.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/src/tests/fixtures/network/sec.py` & `stocktracer-0.1.5/src/tests/fixtures/network/sec.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/.gitignore` & `stocktracer-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/LICENSE` & `stocktracer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stocktracer-0.1.3/README.md` & `stocktracer-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 <p align="center">
     <a href='https://github.com/gyund/fundamental-analysis/blob/main/LICENSE'><img alt="License" src="https://img.shields.io/github/license/gyund/fundamental-analysis"></a>
     <img alt="License" src="https://img.shields.io/badge/python-3.10%2B-blue">
     <a href='https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml'><img alt="Test Status" src="https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml/badge.svg?service=github"></a>
     <a href='https://coveralls.io/github/gyund/fundamental-analysis?branch=main'><img src='https://coveralls.io/repos/github/gyund/fundamental-analysis/badge.svg?branch=main&service=github' alt='Coverage Status' /></a>
-    <img alt="Development Status" src="https://img.shields.io/badge/status-early%20development-red">
+    <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/stocktracer?">
 </p>
 
-# Ticker - Stock Analysis Framework
+# StockTracer
+
+**Stock Analysis Framework**
 
 The goal of this project is aggregate a variety of ways to consume information about a particular equity traded on the US stock market and provide a modular mechanism to process it. Core tenants of this project include:
 
 - **Heavy data caching** - don't download static data more than once
 - **Efficient use of storage** - leave data compressed while not in use
 - **Batch Processing** - We can't store all information in memory, so break problems up
 - **Speed** - Find and avoid bottlenecks of big data processing
 
 ## Requirements
 
 - `python 3.10+`
 
 ## Getting Started
 
+### Users
+
+```sh
+pip install stocktracer
+
+# Perform analysis (not supported yet)
+stocktracer analyze --tickers aapl,msft
+
+# Help
+stocktracer
+
+```
+
+### Developers
+
 Make sure you have `pipenv` installed through a package manager or through pip. You may also use the generated `requirements.txt` but note that these are generated using `pipenv` when we make changes to to dependencies.
 
 ```sh
 pipenv install --dev
 
 # Perform analysis (not supported yet)
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-   [License] [License] [Test_Status] [Coverage_Status] [Development Status]
-# Ticker - Stock Analysis Framework The goal of this project is aggregate a
-variety of ways to consume information about a particular equity traded on the
-US stock market and provide a modular mechanism to process it. Core tenants of
-this project include: - **Heavy data caching** - don't download static data
-more than once - **Efficient use of storage** - leave data compressed while not
-in use - **Batch Processing** - We can't store all information in memory, so
-break problems up - **Speed** - Find and avoid bottlenecks of big data
-processing ## Requirements - `python 3.10+` ## Getting Started Make sure you
-have `pipenv` installed through a package manager or through pip. You may also
-use the generated `requirements.txt` but note that these are generated using
-`pipenv` when we make changes to to dependencies. ```sh pipenv install --dev #
-Perform analysis (not supported yet) PYTHONPATH=src pipenv run python -
-m stocktracer analyze --tickers aapl,msft # Help PYTHONPATH=src pipenv run
-python -m stocktracer # Run Unit Tests pipenv run pytest ``` More information
-can be found in our [documentation](https://gyund.github.io/fundamental-
-analysis/) ## Disclaimer This project seeks to use publicly available
-information to perform security analysis and help perform long term risk
-analysis. Results provided from this project are generally for academic use
-only and are not considered advice or recommendations. This project makes no
-performance claims or guarantees. Please read the [license](LICENSE) for this
-project. Usage of any data is at your own risk.
+      [License] [License] [Test_Status] [Coverage_Status] [PyPI - Status]
+# StockTracer **Stock Analysis Framework** The goal of this project is
+aggregate a variety of ways to consume information about a particular equity
+traded on the US stock market and provide a modular mechanism to process it.
+Core tenants of this project include: - **Heavy data caching** - don't download
+static data more than once - **Efficient use of storage** - leave data
+compressed while not in use - **Batch Processing** - We can't store all
+information in memory, so break problems up - **Speed** - Find and avoid
+bottlenecks of big data processing ## Requirements - `python 3.10+` ## Getting
+Started ### Users ```sh pip install stocktracer # Perform analysis (not
+supported yet) stocktracer analyze --tickers aapl,msft # Help stocktracer ```
+### Developers Make sure you have `pipenv` installed through a package manager
+or through pip. You may also use the generated `requirements.txt` but note that
+these are generated using `pipenv` when we make changes to to dependencies.
+```sh pipenv install --dev # Perform analysis (not supported yet)
+PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft #
+Help PYTHONPATH=src pipenv run python -m stocktracer # Run Unit Tests pipenv
+run pytest ``` More information can be found in our [documentation](https://
+gyund.github.io/fundamental-analysis/) ## Disclaimer This project seeks to use
+publicly available information to perform security analysis and help perform
+long term risk analysis. Results provided from this project are generally for
+academic use only and are not considered advice or recommendations. This
+project makes no performance claims or guarantees. Please read the [license]
+(LICENSE) for this project. Usage of any data is at your own risk.
```

### Comparing `stocktracer-0.1.3/pyproject.toml` & `stocktracer-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src/stocktracer"]
 sources = ["src"]
 
 [project]
 name = "stocktracer"
-version = "0.1.3"
+version = "0.1.5"
 authors = [
   { name="Gary Yund", email="gary.yund@gmail.com" },
 ]
 description = "Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes caching SEC data dump processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = [ "sec-tools", "fundamental analysis", "stocks" ]
 classifiers = [
-    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Office/Business :: Financial :: Investment",
     "Intended Audience :: Science/Research",
     "Development Status :: 2 - Pre-Alpha",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 
 dynamic = ["dependencies"]
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
```

### Comparing `stocktracer-0.1.3/PKG-INFO` & `stocktracer-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocktracer
-Version: 0.1.3
+Version: 0.1.5
 Summary: Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes caching SEC data dump processing.
 Project-URL: Homepage, https://gyund.github.io/fundamental-analysis/
 Project-URL: Bug Tracker, https://github.com/gyund/fundamental-analysis/issues
 Author-email: Gary Yund <gary.yund@gmail.com>
 License: Eclipse Public License - v 2.0
         
             THE ACCOMPANYING PROGRAM IS PROVIDED UNDER THE TERMS OF THIS ECLIPSE
@@ -284,15 +284,16 @@
           You may add additional accurate notices of copyright ownership.
 License-File: LICENSE
 Keywords: fundamental analysis,sec-tools,stocks
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.10
 Requires-Dist: attrs==23.1.0; python_version >= '3.7'
 Requires-Dist: cattrs==22.2.0; python_version >= '3.7'
 Requires-Dist: certifi==2022.12.7; python_version >= '3.6'
 Requires-Dist: charset-normalizer==3.1.0; python_full_version >= '3.7.0'
@@ -315,32 +316,49 @@
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href='https://github.com/gyund/fundamental-analysis/blob/main/LICENSE'><img alt="License" src="https://img.shields.io/github/license/gyund/fundamental-analysis"></a>
     <img alt="License" src="https://img.shields.io/badge/python-3.10%2B-blue">
     <a href='https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml'><img alt="Test Status" src="https://github.com/gyund/fundamental-analysis/actions/workflows/python.yml/badge.svg?service=github"></a>
     <a href='https://coveralls.io/github/gyund/fundamental-analysis?branch=main'><img src='https://coveralls.io/repos/github/gyund/fundamental-analysis/badge.svg?branch=main&service=github' alt='Coverage Status' /></a>
-    <img alt="Development Status" src="https://img.shields.io/badge/status-early%20development-red">
+    <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/stocktracer?">
 </p>
 
-# Ticker - Stock Analysis Framework
+# StockTracer
+
+**Stock Analysis Framework**
 
 The goal of this project is aggregate a variety of ways to consume information about a particular equity traded on the US stock market and provide a modular mechanism to process it. Core tenants of this project include:
 
 - **Heavy data caching** - don't download static data more than once
 - **Efficient use of storage** - leave data compressed while not in use
 - **Batch Processing** - We can't store all information in memory, so break problems up
 - **Speed** - Find and avoid bottlenecks of big data processing
 
 ## Requirements
 
 - `python 3.10+`
 
 ## Getting Started
 
+### Users
+
+```sh
+pip install stocktracer
+
+# Perform analysis (not supported yet)
+stocktracer analyze --tickers aapl,msft
+
+# Help
+stocktracer
+
+```
+
+### Developers
+
 Make sure you have `pipenv` installed through a package manager or through pip. You may also use the generated `requirements.txt` but note that these are generated using `pipenv` when we make changes to to dependencies.
 
 ```sh
 pipenv install --dev
 
 # Perform analysis (not supported yet)
 PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
```

