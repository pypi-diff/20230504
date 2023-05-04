# Comparing `tmp/ethpm-types-0.4.5.tar.gz` & `tmp/ethpm-types-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.4.5.tar", last modified: Tue May  2 12:41:47 2023, max compression
+gzip compressed data, was "ethpm-types-0.5.0.tar", last modified: Thu May  4 12:52:30 2023, max compression
```

## Comparing `ethpm-types-0.4.5.tar` & `ethpm-types-0.5.0.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.819101 ethpm-types-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)   220464 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/release-drafter.yml` & `ethpm-types-0.5.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/workflows/commitlint.yaml` & `ethpm-types-0.5.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/workflows/docs.yaml` & `ethpm-types-0.5.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/workflows/prtitle.yaml` & `ethpm-types-0.5.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/workflows/publish.yaml` & `ethpm-types-0.5.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.github/workflows/test.yaml` & `ethpm-types-0.5.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.gitignore` & `ethpm-types-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/.pre-commit-config.yaml` & `ethpm-types-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/CONTRIBUTING.md` & `ethpm-types-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/LICENSE` & `ethpm-types-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/PKG-INFO` & `ethpm-types-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.5
+Version: 0.5.0
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.4.5/README.md` & `ethpm-types-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/build_docs.py` & `ethpm-types-0.5.0/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/_static/custom.css` & `ethpm-types-0.5.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/_static/custom.js` & `ethpm-types-0.5.0/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/_templates/layout.html` & `ethpm-types-0.5.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/conf.py` & `ethpm-types-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/favicon.ico` & `ethpm-types-0.5.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/docs/logo.gif` & `ethpm-types-0.5.0/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/ethpm_types/__init__.py` & `ethpm-types-0.5.0/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/ethpm_types/abi.py` & `ethpm-types-0.5.0/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/ethpm_types/ast.py` & `ethpm-types-0.5.0/ethpm_types/ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from enum import Enum
-from typing import Iterator, List, Optional, Tuple, Union
+from typing import Iterator, List, Optional, Union
 
 from pydantic import root_validator
 
 from ethpm_types.base import BaseModel
 from ethpm_types.sourcemap import SourceMapItem
-
-SourceLocation = Tuple[int, int, int, int]
+from ethpm_types.utils import SourceLocation
 
 
 class ASTClassification(Enum):
     UNCLASSIFIED = 0
     """Unclassified AST type (default)."""
 
     FUNCTION = 1
```

### Comparing `ethpm-types-0.4.5/ethpm_types/base.py` & `ethpm-types-0.5.0/ethpm_types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, no_type_check
 
 from pydantic import BaseModel as _BaseModel
 
-from .utils import HexBytes
+from ethpm_types.utils import HexBytes
 
 
 class BaseModel(_BaseModel):
     def dict(self, *args, **kwargs) -> dict:
         # NOTE: We do this to accommodate the aliases needed for EIP-2678 compatibility
         if "by_alias" not in kwargs:
             kwargs["by_alias"] = True
```

### Comparing `ethpm-types-0.4.5/ethpm_types/contract_type.py` & `ethpm-types-0.5.0/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/ethpm_types/manifest.py` & `ethpm-types-0.5.0/ethpm_types/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List, Optional
 
 from pydantic import Field, root_validator, validator
 
 from .base import BaseModel
 from .contract_type import BIP122_URI, ContractInstance, ContractType
 from .source import Compiler, Source
-from .utils import AnyUrl
+from .utils import Algorithm, AnyUrl
 
 ALPHABET = set("abcdefghijklmnopqrstuvwxyz")
 NUMBERS = set("0123456789")
 
 
 class PackageName(str):
     """
@@ -161,19 +161,20 @@
         ):
             raise ValueError("Both `name` and `version` must be present if either is specified.")
 
         return values
 
     @root_validator
     def check_contract_source_ids(cls, values):
-        if values.get("contract_types") is not None and values.get("sources") is not None:
-            for alias in values["contract_types"]:
-                source_id = values["contract_types"][alias].source_id
-                if source_id and (source_id not in values["sources"]):
-                    raise ValueError(f"'{source_id}' missing from `sources`.")
+        contract_types = values.get("contract_types", {}) or {}
+        for alias in contract_types:
+            source_id = values["contract_types"][alias].source_id
+            sources = values.get("sources", {}) or {}
+            if source_id and (source_id not in sources):
+                raise ValueError(f"'{source_id}' missing from `sources`.")
 
         return values
 
     @validator("contract_types")
     def add_name_to_contract_types(cls, values):
         aliases = list(values.keys())
         # NOTE: Must manually inject names to types here
@@ -187,7 +188,30 @@
     def __getattr__(self, attr_name: str):
         # NOTE: **must** raise `AttributeError` or return here, or else Python breaks
         if self.contract_types and attr_name in self.contract_types:
             return self.contract_types[attr_name]
 
         else:
             raise AttributeError(f"{self.__class__.__name__} has no contract type '{attr_name}'")
+
+    def dict(self, *args, **kwargs) -> Dict:
+        res = super().dict()
+        sources = res.get("sources", {})
+        for source_id, src in sources.items():
+            if "content" in src and isinstance(src["content"], dict):
+                content = "\n".join(src["content"].values())
+                if content and not content.endswith("\n"):
+                    content = f"{content}\n"
+
+                src["content"] = content
+
+            elif "content" in src and src["content"] is None:
+                src["content"] = ""
+
+            if (
+                "checksum" in src
+                and "algorithm" in src["checksum"]
+                and isinstance(src["checksum"]["algorithm"], Algorithm)
+            ):
+                src["checksum"]["algorithm"] = src["checksum"]["algorithm"].value
+
+        return res
```

### Comparing `ethpm-types-0.4.5/ethpm_types/sourcemap.py` & `ethpm-types-0.5.0/ethpm_types/sourcemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Iterator, List, Optional, Union
 
 from pydantic import root_validator
 
 from ethpm_types.base import BaseModel
+from ethpm_types.utils import SourceLocation
 
 
 class SourceMapItem(BaseModel):
     """
     An object modeling a node in a source map; useful for mapping
     the source map string back to source code.
     """
@@ -119,14 +120,23 @@
 
     line_start: Optional[int] = None
     column_start: Optional[int] = None
     line_end: Optional[int] = None
     column_end: Optional[int] = None
     dev: Optional[str] = None
 
+    @property
+    def location(self) -> SourceLocation:
+        return (
+            (self.line_start or -1),
+            (self.column_start or -1),
+            (self.line_end or -1),
+            (self.column_end or -1),
+        )
+
 
 _RawPCMapItem = Dict[str, Optional[Union[str, List[Optional[int]]]]]
 _RawPCMap = Dict[str, _RawPCMapItem]
 
 
 class PCMap(BaseModel):
     """
```

### Comparing `ethpm-types-0.4.5/ethpm_types/utils.py` & `ethpm-types-0.5.0/ethpm_types/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from hashlib import md5, sha3_256, sha256
-from typing import Union
+from typing import Tuple, Union
 
 from hexbytes import HexBytes as BaseHexBytes
 from pydantic import AnyUrl as _AnyUrl
 from pydantic import FileUrl
 
 CONTENT_ADDRESSED_SCHEMES = {"ipfs"}
 AnyUrl = Union[_AnyUrl, FileUrl]
@@ -110,7 +110,10 @@
         return Hex.from_bytes(sha256(content).digest())
 
     # TODO: Support IPFS CIDv0 & CIDv1
     # TODO: Support keccak256 (if even necessary, mentioned in EIP but not used)
     # TODO: Explore other algorithms needed
     else:
         raise ValueError("Unsupported algorithm.")
+
+
+SourceLocation = Tuple[int, int, int, int]
```

### Comparing `ethpm-types-0.4.5/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.5.0/ethpm_types.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.5
+Version: 0.5.0
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.4.5/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.5.0/ethpm_types.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -58,11 +58,15 @@
 tests/test_contract_type.py
 tests/test_hexbytes.py
 tests/test_package_manifest.py
 tests/test_pc_map.py
 tests/test_schema_fuzzing.py
 tests/test_source.py
 tests/test_sourcemap.py
-tests/data/OpenZeppelinContracts.json
-tests/data/SolidityContract.json
-tests/data/TestStrategy.srcmap
-tests/data/VyperContract.json
+tests/data/Compiled/HasError.json
+tests/data/Compiled/OpenZeppelinContracts.json
+tests/data/Compiled/SolidityContract.json
+tests/data/Compiled/TestStrategy.srcmap
+tests/data/Compiled/VyperContract.json
+tests/data/Sources/HasError.sol
+tests/data/Sources/SolidityContract.sol
+tests/data/Sources/VyperContract.vy
```

### Comparing `ethpm-types-0.4.5/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.5.0/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/pyproject.toml` & `ethpm-types-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/setup.py` & `ethpm-types-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/data/OpenZeppelinContracts.json` & `ethpm-types-0.5.0/tests/data/Compiled/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/data/TestStrategy.srcmap` & `ethpm-types-0.5.0/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_ast.py` & `ethpm-types-0.5.0/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_cairo.py` & `ethpm-types-0.5.0/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_hexbytes.py` & `ethpm-types-0.5.0/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_package_manifest.py` & `ethpm-types-0.5.0/tests/test_package_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
     else:
         with pytest.raises(ValidationError):
             PackageManifest.parse_obj(example_json).dict()
 
 
 def test_open_zeppelin_contracts(oz_package, oz_package_manifest_dict):
-    assert oz_package.dict() == oz_package_manifest_dict
+    actual = oz_package.dict()
+    assert actual == oz_package_manifest_dict
 
     for source_name, source in oz_package.sources.items():
         # NOTE: Per EIP-2678, "Checksum is only required if content is missing"
         if not source.content:
             assert source.content_is_valid(), f"Invalid checksum for '{source_name}'"
```

### Comparing `ethpm-types-0.4.5/tests/test_pc_map.py` & `ethpm-types-0.5.0/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_schema_fuzzing.py` & `ethpm-types-0.5.0/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.5/tests/test_sourcemap.py` & `ethpm-types-0.5.0/tests/test_sourcemap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from pathlib import Path
 from typing import Iterator
 
 import pytest
 
 from ethpm_types.sourcemap import SourceMap, SourceMapItem
+from tests.conftest import COMPILED_BASE
 
-SOURCE_MAP_FILES = {p.stem: p for p in sorted(Path("tests/data").glob("*.srcmap"))}
+SOURCE_MAP_FILES = {p.stem: p for p in sorted(COMPILED_BASE.glob("*.srcmap"))}
 
 
 def serialize(sourcemap: Iterator[SourceMapItem]) -> str:
     result = ""
     previous_item = None
     for item in sourcemap:
         if item == previous_item:
```

