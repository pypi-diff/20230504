# Comparing `tmp/molfeat-0.8.7.tar.gz` & `tmp/molfeat-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.7.tar", last modified: Mon Apr 24 16:37:54 2023, max compression
+gzip compressed data, was "molfeat-0.8.8.tar", last modified: Wed May  3 22:38:44 2023, max compression
```

## Comparing `molfeat-0.8.7.tar` & `molfeat-0.8.8.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 16:37:36.000000 molfeat-0.8.7/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.444288 molfeat-0.8.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.444288 molfeat-0.8.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.448288 molfeat-0.8.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 16:35:03.000000 molfeat-0.8.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 16:37:36.000000 molfeat-0.8.7/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 16:37:36.000000 molfeat-0.8.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-24 16:37:36.000000 molfeat-0.8.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-24 16:35:03.000000 molfeat-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-24 16:37:54.472288 molfeat-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-24 16:35:03.000000 molfeat-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.448288 molfeat-0.8.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.440288 molfeat-0.8.7/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-24 16:35:03.000000 molfeat-0.8.7/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-24 16:35:03.000000 molfeat-0.8.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.460288 molfeat-0.8.7/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33499 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:37:45.000000 molfeat-0.8.7/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 16:35:03.000000 molfeat-0.8.7/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 16:35:03.000000 molfeat-0.8.7/plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 16:35:03.000000 molfeat-0.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 16:35:03.000000 molfeat-0.8.7/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:37:54.472288 molfeat-0.8.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 22:38:28.000000 molfeat-0.8.8/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 22:37:10.000000 molfeat-0.8.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 22:38:28.000000 molfeat-0.8.8/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 22:38:28.000000 molfeat-0.8.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-03 22:38:28.000000 molfeat-0.8.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 22:37:10.000000 molfeat-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-03 22:38:44.558586 molfeat-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-03 22:37:10.000000 molfeat-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.530587 molfeat-0.8.8/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-03 22:37:10.000000 molfeat-0.8.8/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-03 22:37:10.000000 molfeat-0.8.8/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16348 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:38:36.000000 molfeat-0.8.8/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 22:37:10.000000 molfeat-0.8.8/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 22:37:10.000000 molfeat-0.8.8/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-03 22:37:10.000000 molfeat-0.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 22:37:10.000000 molfeat-0.8.8/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:38:44.558586 molfeat-0.8.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_viz.py
```

### Comparing `molfeat-0.8.7/.authors.yml` & `molfeat-0.8.8/.authors.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 - name: maclandrol
   email: emmanuel.noutahi@hotmail.ca
+  alternate_emails:
+  - maclandrol@users.noreply.github.com
   num_commits: 0
   first_commit: 2021-04-06 11:53:10
 - name: Cas Wognum
   email: caswognum@outlook.com
   aliases:
   - cwognum
   num_commits: 0
@@ -27,7 +29,16 @@
   email: sauravvmaheshkar@gmail.com
   num_commits: 0
   first_commit: 2023-04-04 07:44:44
 - name: rbyrne-momatx
   email: 113197924+rbyrne-momatx@users.noreply.github.com
   num_commits: 0
   first_commit: 2023-04-22 17:53:52
+- name: dessygil
+  email: desmondgilmour@gmail.com
+  num_commits: 0
+  first_commit: 2023-04-22 21:22:11
+- name: DomInvivo
+  email: dominique@invivoai.com
+  num_commits: 0
+  first_commit: 2023-05-02 21:07:10
+  github: DomInvivo
```

### Comparing `molfeat-0.8.7/.github/CODE_OF_CONDUCT.md` & `molfeat-0.8.8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.8.8/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.8.8/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.8.8/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.8.8/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.8.8/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/workflows/doc.yml` & `molfeat-0.8.8/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/workflows/release.yml` & `molfeat-0.8.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.github/workflows/test.yml` & `molfeat-0.8.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.gitignore` & `molfeat-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/.mailmap` & `molfeat-0.8.8/.mailmap`

 * *Files 20% similar despite different names*

```diff
@@ -6,13 +6,15 @@
 #
 # You can skip bad-name if it is the same as good-name and is unique in the repo.
 #
 # This file is up-to-date if the command git log --format="%aN <%aE>" | sort -u
 # gives no duplicates.
 
 Cas Wognum <caswognum@outlook.com> cwognum <caswognum@outlook.com>
+DomInvivo <dominique@invivoai.com>
 Hadrien Mary <hadrien.mary@gmail.com> Hadrien Mary <hadim@users.noreply.github.com>
 Honore Hounwanou <mercuryseries@gmail.com>
 Saurav Maheshkar <sauravvmaheshkar@gmail.com>
 Therence <38595485+Therence1@users.noreply.github.com>
-maclandrol <emmanuel.noutahi@hotmail.ca>
+dessygil <desmondgilmour@gmail.com>
+maclandrol <emmanuel.noutahi@hotmail.ca> maclandrol <maclandrol@users.noreply.github.com>
 rbyrne-momatx <113197924+rbyrne-momatx@users.noreply.github.com>
```

### Comparing `molfeat-0.8.7/CHANGELOG.rst` & `molfeat-0.8.8/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,39 @@
 ==================
 molfeat Change Log
 ==================
 
 .. current developments
 
+v0.8.8
+====================
+
+**Added:**
+
+* A model named Molt5
+* Existing plugins to a the `plugin.yml` file
+* Documents missing featurizers
+
+**Changed:**
+
+* Different docs style, with Tabs on the top for `Overview`, `Usage`, `Tutorials`, `API`, `Contribute`, `License`
+* Small updates in docs
+
+**Fixed:**
+
+* Fix #43: Pretrained models should now work better with `batch_transform`,  allowing efficient parallelization, while retaining all cached features.
+
+**Authors:**
+
+* DomInvivo
+* dessygil
+* maclandrol
+
+
+
 v0.8.7
 ====================
 
 **Added:**
 
 * Support for `ignore_padding` in Graphormer
 * More flexibility overall for graphormer embeddings
```

### Comparing `molfeat-0.8.7/LICENSE` & `molfeat-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/PKG-INFO` & `molfeat-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.7
+Version: 0.8.8
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -100,15 +100,15 @@
 - To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
 ### Installing Plugins
 
-The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
+The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](docs/developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
 ## API tour
 
 ```python
 import datamol as dm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.7 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.8 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -75,24 +75,24 @@
 pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
-more details on how to [create](developers/create-plugin.md) your own plugins.
-However, this does imply that the installation of a plugin is plugin-dependent:
-please consult the relevant documentation to learn more. ## API tour ```python
-import datamol as dm from molfeat.calc import FPCalculator from molfeat.trans
-import MoleculeTransformer from molfeat.store.modelstore import ModelStore #
-Load some dummy data data = dm.data.freesolv().sample(100).smiles.values #
-Featurize a single molecule calc = FPCalculator("ecfp") calc(data[0]) # Define
-a parallelized featurization pipeline mol_transf = MoleculeTransformer(calc,
-n_jobs=-1) mol_transf(data) # Easily save and load featurizers
-mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
+more details on how to [create](docs/developers/create-plugin.md) your own
+plugins. However, this does imply that the installation of a plugin is plugin-
+dependent: please consult the relevant documentation to learn more. ## API tour
+```python import datamol as dm from molfeat.calc import FPCalculator from
+molfeat.trans import MoleculeTransformer from molfeat.store.modelstore import
+ModelStore # Load some dummy data data = dm.data.freesolv().sample
+(100).smiles.values # Featurize a single molecule calc = FPCalculator("ecfp")
+calc(data[0]) # Define a parallelized featurization pipeline mol_transf =
+MoleculeTransformer(calc, n_jobs=-1) mol_transf(data) # Easily save and load
+featurizers mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
```

### Comparing `molfeat-0.8.7/README.md` & `molfeat-0.8.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 - To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
 ### Installing Plugins
 
-The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
+The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](docs/developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
 ## API tour
 
 ```python
 import datamol as dm
```

#### html2text {}

```diff
@@ -55,24 +55,24 @@
 pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
-more details on how to [create](developers/create-plugin.md) your own plugins.
-However, this does imply that the installation of a plugin is plugin-dependent:
-please consult the relevant documentation to learn more. ## API tour ```python
-import datamol as dm from molfeat.calc import FPCalculator from molfeat.trans
-import MoleculeTransformer from molfeat.store.modelstore import ModelStore #
-Load some dummy data data = dm.data.freesolv().sample(100).smiles.values #
-Featurize a single molecule calc = FPCalculator("ecfp") calc(data[0]) # Define
-a parallelized featurization pipeline mol_transf = MoleculeTransformer(calc,
-n_jobs=-1) mol_transf(data) # Easily save and load featurizers
-mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
+more details on how to [create](docs/developers/create-plugin.md) your own
+plugins. However, this does imply that the installation of a plugin is plugin-
+dependent: please consult the relevant documentation to learn more. ## API tour
+```python import datamol as dm from molfeat.calc import FPCalculator from
+molfeat.trans import MoleculeTransformer from molfeat.store.modelstore import
+ModelStore # Load some dummy data data = dm.data.freesolv().sample
+(100).smiles.values # Featurize a single molecule calc = FPCalculator("ecfp")
+calc(data[0]) # Define a parallelized featurization pipeline mol_transf =
+MoleculeTransformer(calc, n_jobs=-1) mol_transf(data) # Easily save and load
+featurizers mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
```

### Comparing `molfeat-0.8.7/docs/api/molfeat.calc.md` & `molfeat-0.8.8/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/assets/css/custom-molfeat.css` & `molfeat-0.8.8/docs/assets/css/custom-molfeat.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/assets/css/custom.css` & `molfeat-0.8.8/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/benchmark.ipynb` & `molfeat-0.8.8/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/developers/contribute.md` & `molfeat-0.8.8/docs/developers/contribute.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/developers/create-plugin.md` & `molfeat-0.8.8/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/developers/register-plugin.md` & `molfeat-0.8.8/docs/developers/register-plugin.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 The `molfeat` plugin registry aims to be the home for all publicly available `molfeat` plugins. It
 collects information on the type of plugins provided by your package and which `molfeat` versions it is compatible with.
 
 If you are starting to develop a new plugin or if you already have one, please register it here.
 We strongly encourage you to **register at early stages of development**, both to reserve the name of your plugin and to inform the community of your ongoing work.
 
 
-
 ## How to register a plugin
 
 1. Fork this repository
 2. Add your plugin to the end of the `plugins.yaml` file, e.g.
     ```
     ...
     molfeat-new:
@@ -29,16 +28,21 @@
 
 - __top-level key__ (required):
 the name under which your plugin will be distributed.
 By convention, names of molfeat plugins are lowercase and prefixed by `molfeat-` (e.g `molfeat-myplugin`)
 
 - __entry_point_prefix__ (required):
 the prefix of all entry points provided by the plugin.
-By convention, a plugin `molfeat-xxx` should use `entry_point_prefix: xxx`.
-For example: `molfeat-myplugin` uses the entry point prefix `myplugin` and provides numerous entry points, all of which start with `myplugin.`.
+By convention, a plugin `molfeat-xxx` should use `entry_point_prefix: xxx`. You can also use the module name of your plugin. For example: `molfeat-myplugin` uses the entry point prefix `myplugin` and provides numerous entry points, all of which start with `myplugin.`. The entry point is also how you signal to users how they can load your plugin through molfeat. 
+
+```python
+from molfeat.trans import MoleculeTransformer
+from molfeat.plugins import load_registered_plugins
+load_registered_plugins(add_submodules=True, plugins=["new"])
+```
 
 - __home_url__ (required):
 the link to the homepage of the plugin, for example its github repository.
 
 - __molfeat_version__ (required):
 the molfeat version required for your plugin to work.
 
@@ -55,15 +59,18 @@
 
 ```yaml
 # name of the featurizer, str
 name: awesome-featurizer 
 # description of your featurizer, str
 description: Concise description for the awesome-featurizer
 # type of input the featurizer takes, str
-inputs: smiles 
+inputs: smiles
+# which group does the featurizer belong to. 
+# This helps for the usage card. Ask a maintainer for help
+group: "rdkit"
 # link to the reference of the featurizer
 reference: https://link-to-the-awesome-paper/
 # type of featurizer, Literal["pretrained", "hand-crafted", "hashed"]
 type: "pretrained" 
 # output representation of the featurizer, Literal["graph", "line-notation", "vector", "tensor", "other"]
 representation: vector 
 # Whether 3D information are required, Optional[bool]
```

### Comparing `molfeat-0.8.7/docs/images/logo-black.png` & `molfeat-0.8.8/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/images/logo-black.svg` & `molfeat-0.8.8/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/images/logo-title.svg` & `molfeat-0.8.8/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/images/logo.png` & `molfeat-0.8.8/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/images/logo.svg` & `molfeat-0.8.8/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/index.md` & `molfeat-0.8.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/add_your_own.ipynb` & `molfeat-0.8.8/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/datacache.ipynb` & `molfeat-0.8.8/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/graphs.ipynb` & `molfeat-0.8.8/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/integrations.ipynb` & `molfeat-0.8.8/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.8.8/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/save_and_load.ipynb` & `molfeat-0.8.8/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.8.8/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.8.8/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/docs/usage.md` & `molfeat-0.8.8/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/env.yml` & `molfeat-0.8.8/env.yml`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
   # Optional: featurizers
   - dgl
   - dgllife
   - graphormer-pretrained >=0.2.3
   - transformers
   - tokenizers <0.13.2
+  - sentencepiece
   - biotite # required for ESM models
 
   # Optional: viz
   - nglview
   - ipywidgets
 
   # Dev
```

### Comparing `molfeat-0.8.7/mkdocs.yml` & `molfeat-0.8.8/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
   - License: license.md
 
 theme:
   name: material
   # NOTE(cwognum): to customize the material primary and secondary
   # color check `docs/assets/css/custom-molfeat.css`.
   features:
+    - navigation.tabs
     - navigation.expand
   favicon: images/logo-black.png
   logo: images/logo.svg
 
 extra_css:
   - assets/css/custom.css
   - assets/css/custom-molfeat.css
```

### Comparing `molfeat-0.8.7/molfeat/calc/__init__.py` & `molfeat-0.8.8/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/_atom_bond_features.py` & `molfeat-0.8.8/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/_map4.py` & `molfeat-0.8.8/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/_mhfp.py` & `molfeat-0.8.8/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/atom.py` & `molfeat-0.8.8/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/base.py` & `molfeat-0.8.8/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/bond.py` & `molfeat-0.8.8/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/cats.py` & `molfeat-0.8.8/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/descriptors.py` & `molfeat-0.8.8/molfeat/calc/descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/fingerprints.py` & `molfeat-0.8.8/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/pharmacophore.py` & `molfeat-0.8.8/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/shape.py` & `molfeat-0.8.8/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/skeys.py` & `molfeat-0.8.8/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/calc/tree.py` & `molfeat-0.8.8/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/data/cats_features.fdef` & `molfeat-0.8.8/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/data/elements.xz` & `molfeat-0.8.8/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/data/elements_completed.xz` & `molfeat-0.8.8/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/data/origin.xz` & `molfeat-0.8.8/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/data/skey_parameters.csv` & `molfeat-0.8.8/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/plugins/entry_point.py` & `molfeat-0.8.8/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/plugins/factories.py` & `molfeat-0.8.8/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/store/loader.py` & `molfeat-0.8.8/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/store/modelcard.py` & `molfeat-0.8.8/molfeat/store/modelcard.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,32 +13,44 @@
     """Get the model initialization code
 
     Args:
         card: model card to use
     """
     if card.group == "all" and card.type != "pretrained":
         import_statement = "from molfeat.trans import MoleculeTransformer"
-        loader_statement = f"MoleculeTransformer(featurizer='{card.name}')"
-    elif card.group in ["rdkit", "fp"]:
+        loader_statement = f"MoleculeTransformer(featurizer='{card.name}', dtype=float)"
+    elif card.group in ["rdkit", "fp", "shape"]:
         import_statement = f"from molfeat.trans.fp import FPVecTransformer"
-        loader_statement = f"FPVecTransformer(kind='{card.name}')"
+        loader_statement = f"FPVecTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "dgllife":
         import_statement = "from molfeat.trans.pretrained import PretrainedDGLTransformer"
-        loader_statement = f"PretrainedDGLTransformer(kind='{card.name}')"
+        loader_statement = f"PretrainedDGLTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "graphormer":
         import_statement = "from molfeat.trans.pretrained import GraphormerTransformer"
-        loader_statement = f"GraphormerTransformer(kind='{card.name}')"
+        loader_statement = f"GraphormerTransformer(kind='{card.name}', dtype=float)"
     elif card.group == "fcd":
         import_statement = "from molfeat.trans.pretrained import FCDTransformer"
         loader_statement = f"FCDTransformer()"
+    elif card.group == "pharmacophore":
+        name = card.name.split("-")[-1]
+        if card.require_3D:
+            import_class = "Pharmacophore3D"
+        else:
+            import_class = "Pharmacophore2D"
+        import_statement = f"from molfeat.trans.base import MoleculeTransformer\nfrom molfeat.calc.pharmacophore import {import_class}"
+        loader_statement = (
+            f"MoleculeTransformer(featurizer={import_class}(factory='{name}'), dtype=float)"
+        )
     elif card.group == "huggingface":
         import_statement = (
             "from molfeat.trans.pretrained.hf_transformers import PretrainedHFTransformer"
         )
-        loader_statement = f"PretrainedHFTransformer(kind='{card.name}', notation='{card.inputs}')"
+        loader_statement = (
+            f"PretrainedHFTransformer(kind='{card.name}', notation='{card.inputs}', dtype=float)"
+        )
     else:
         raise ValueError(f"Unknown model group {card.group}")
     return import_statement, loader_statement
 
 
 class ModelInfo(BaseModel):
     name: str
@@ -84,16 +96,20 @@
             self_content = {k: self_content.get(k) for k in match_only}
             new_content = {k: new_content.get(k) for k in match_only}
         return self_content == new_content
 
     def usage(self):
         """Return the usage of the model"""
         import_statement, loader_statement = get_model_init(self)
+        comment = "# sanitize and standardize your molecules if needed"
+        if self.require_3D:
+            comment += "\n# <generate 3D coordinates here> "
         usage = f"""
         import datamol as dm
         {import_statement}
-        data = dm.freesolv().iloc[:100]
+        smiles = dm.freesolv().iloc[:100].smiles
+        {comment}
         transformer = {loader_statement}
-        features = transformer(data["smiles"])
+        features = transformer(smiles)
         """
         usage = "\n".join([x.strip() for x in usage.split("\n")])
         return usage
```

### Comparing `molfeat-0.8.7/molfeat/store/modelstore.py` & `molfeat-0.8.8/molfeat/store/modelstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,17 @@
             model_name: name of the model to load
             load_fn: Custom loading function to load the model
             load_fn_kwargs: Optional dict of additional kwargs to provide to the loading function
             download_output_dir: Argument for download function to specify the download folder
             chunk_size: chunk size for download
             force: whether to reforce the download of the file
 
+        Returns:
+            model: Optional model, if the model requires download or loading weights
+            model_info: model information card
         """
         if isinstance(model_name, str):
             # find the model with the same name
             modelcard = self.search(name=model_name)[0]
         else:
             modelcard = model_name
         output_dir = self.download(
```

### Comparing `molfeat-0.8.7/molfeat/trans/base.py` & `molfeat-0.8.8/molfeat/trans/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,27 +475,27 @@
             and n_jobs not in [None, 0, 1]  # this is based on datamol sequential vs parallel
         )
         if use_mp_cache:
             # we need to change the cache system to one that works with multiprocessing
             # to have a shared memory
             new_cache = MPDataCache()
             new_cache.update(existing_cache)
-            transformer.cache = new_cache
+            setattr(transformer, cache_attr, new_cache)
 
         transformed = dm.parallelized(
             transformer,
             batched_mols,
             n_jobs=n_jobs,
             progress=progress,
             **parallel_kwargs,
         )
         if use_mp_cache:
             # we set back the original transformation while updating it with
             # all the missing values
-            existing_cache.update(transformer.cache)
+            existing_cache.update(getattr(transformer, cache_attr, {}))
             setattr(transformer, cache_attr, existing_cache)
 
         if concatenate:
             # if we ask for concatenation, then we would need to fix None values ideally
             fixed_transformations = []
             for computed_trans in transformed:
                 if computed_trans is None:
```

### Comparing `molfeat-0.8.7/molfeat/trans/concat.py` & `molfeat-0.8.8/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/fp.py` & `molfeat-0.8.8/molfeat/trans/fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         "mordred",
         "cats2D",
         "cats3D",
         "pharm2D",
         "pharm3D",
         "scaffoldkeys",
         "skeys",
+        "electroshape",
+        "usr",
+        "usrcat",
     ]
 
     def __init__(
         self,
         kind: str = "ecfp:4",
         length: int = 2000,
         n_jobs: int = 1,
```

### Comparing `molfeat-0.8.7/molfeat/trans/graph/adj.py` & `molfeat-0.8.8/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/graph/tree.py` & `molfeat-0.8.8/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/pretrained/base.py` & `molfeat-0.8.8/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.8.8/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/pretrained/fcd.py` & `molfeat-0.8.8/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.8.8/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.8.8/molfeat/trans/pretrained/hf_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import torch
 import tempfile
 import numpy as np
 import datamol as dm
 
 from dataclasses import dataclass
 from loguru import logger
+from transformers import EncoderDecoderModel
 from transformers import AutoTokenizer
 from transformers import AutoModel
 from transformers import AutoConfig
 from transformers import MODEL_MAPPING
 from transformers import PreTrainedModel
 from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
 from molfeat.trans.pretrained.base import PretrainedMolTransformer
@@ -217,14 +218,15 @@
 
     def __init__(
         self,
         kind: Union[str, HFModel] = "ChemBERTa-77M-MLM",
         notation: Optional[str] = "none",
         pooling: str = "mean",
         concat_layers: Union[List[int], int] = -1,
+        prefer_encoder: bool = True,
         dtype=np.float32,
         device="cpu",
         max_length: int = 128,
         ignore_padding: bool = True,
         preload: bool = False,
         n_jobs: int = 0,
         random_seed: Optional[int] = None,
@@ -244,14 +246,15 @@
 
         Args:
             kind: name of the featurizer as available in the model store
             notation: optional line notation to use. Only use if it cannot be found from the model card.
             pooling: type of pooling to use. One of ['default', 'mean', 'max', 'sum']. The value "default" corresponds to the default litterature pooling for each model type.
                 See `molfeat.utils.pooler.get_default_hf_pooler` for more details.
             concat_layers: Layer to concat to get the representation. By default the last hidden layer is returned.
+            prefer_encoder: For an encoder-decoder model, prefer the embeddings provided by the encoder.
             dtype: Data type to output
             device: Torch device on which to run the featurizer.
             max_length: Maximum length of the input sequence to consider. Please update this for large sequences
             ignore_padding: Whether to ignore padding in the representation (default: True) to avoid effect of batching
             preload: Whether to preload the model into memory or not
             n_jobs: number of jobs to use
             random_seed: random seed to use for reproducibility whenever a DNN pooler is used (e.g bert/roberta)
@@ -270,14 +273,15 @@
         self.concat_layers = concat_layers
         self.max_length = max_length
         self.ignore_padding = ignore_padding
         self._require_mols = False
         self.random_seed = random_seed
         self.preload = preload
         self.pooling = pooling
+        self.prefer_encoder = prefer_encoder
         self._pooling_obj = None
         if isinstance(kind, HFModel):
             self.kind = kind.name
             self.featurizer = kind
         else:
             self.kind = kind
             self.featurizer = HFModel(name=self.kind)
@@ -393,15 +397,21 @@
 
         attention_mask = inputs.get("attention_mask", None)
         if attention_mask is not None and self.ignore_padding:
             attention_mask = attention_mask.unsqueeze(-1)  # B, S, 1
         else:
             attention_mask = None
         with torch.no_grad():
-            out_dict = self.featurizer.model(output_hidden_states=True, **inputs)
+            if (
+                isinstance(self.featurizer.model, EncoderDecoderModel)
+                or hasattr(self.featurizer.model, "encoder")
+            ) and self.prefer_encoder:
+                out_dict = self.featurizer.model.encoder(output_hidden_states=True, **inputs)
+            else:
+                out_dict = self.featurizer.model(output_hidden_states=True, **inputs)
             hidden_state = out_dict["hidden_states"]
             emb_layers = []
             for layer in self.concat_layers:
                 emb = hidden_state[layer].detach().cpu()  # B, S, D
                 emb = self._pooling_obj(
                     emb,
                     inputs["input_ids"],
```

### Comparing `molfeat-0.8.7/molfeat/trans/struct/esm.py` & `molfeat-0.8.8/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/trans/struct/prot1D.py` & `molfeat-0.8.8/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/cache.py` & `molfeat-0.8.8/molfeat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/commons.py` & `molfeat-0.8.8/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/const.py` & `molfeat-0.8.8/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/converters.py` & `molfeat-0.8.8/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/datatype.py` & `molfeat-0.8.8/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/log.py` & `molfeat-0.8.8/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/parsing.py` & `molfeat-0.8.8/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/pooler.py` & `molfeat-0.8.8/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/requires.py` & `molfeat-0.8.8/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/utils/state.py` & `molfeat-0.8.8/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat/viz.py` & `molfeat-0.8.8/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/molfeat.egg-info/PKG-INFO` & `molfeat-0.8.8/molfeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.7
+Version: 0.8.8
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -100,15 +100,15 @@
 - To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
 ### Installing Plugins
 
-The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
+The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](docs/developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
 ## API tour
 
 ```python
 import datamol as dm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.7 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.8 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -75,24 +75,24 @@
 pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
-more details on how to [create](developers/create-plugin.md) your own plugins.
-However, this does imply that the installation of a plugin is plugin-dependent:
-please consult the relevant documentation to learn more. ## API tour ```python
-import datamol as dm from molfeat.calc import FPCalculator from molfeat.trans
-import MoleculeTransformer from molfeat.store.modelstore import ModelStore #
-Load some dummy data data = dm.data.freesolv().sample(100).smiles.values #
-Featurize a single molecule calc = FPCalculator("ecfp") calc(data[0]) # Define
-a parallelized featurization pipeline mol_transf = MoleculeTransformer(calc,
-n_jobs=-1) mol_transf(data) # Easily save and load featurizers
-mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
+more details on how to [create](docs/developers/create-plugin.md) your own
+plugins. However, this does imply that the installation of a plugin is plugin-
+dependent: please consult the relevant documentation to learn more. ## API tour
+```python import datamol as dm from molfeat.calc import FPCalculator from
+molfeat.trans import MoleculeTransformer from molfeat.store.modelstore import
+ModelStore # Load some dummy data data = dm.data.freesolv().sample
+(100).smiles.values # Featurize a single molecule calc = FPCalculator("ecfp")
+calc(data[0]) # Define a parallelized featurization pipeline mol_transf =
+MoleculeTransformer(calc, n_jobs=-1) mol_transf(data) # Easily save and load
+featurizers mol_transf.to_state_yaml_file("state_dict.yml") mol_transf =
 MoleculeTransformer.from_state_yaml_file("state_dict.yml") mol_transf(data) #
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
```

### Comparing `molfeat-0.8.7/molfeat.egg-info/SOURCES.txt` & `molfeat-0.8.8/molfeat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .mailmap
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE
 README.md
 env.yml
 mkdocs.yml
-plugin.yaml
+plugin.yml
 pyproject.toml
 rever.xsh
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/SECURITY.md
 .github/ISSUE_TEMPLATE/1_bug_report.yaml
```

### Comparing `molfeat-0.8.7/pyproject.toml` & `molfeat-0.8.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
 
 graphormer = [
     "graphormer-pretrained",
 ]
 
 transformer = [
     "tokenizers <0.13.2",
-    "transformers"
+    "transformers",
+    "sentencepiece",
 ]
 
 fcd = [
     "fcd_torch"
 ]
 
 viz = [
```

### Comparing `molfeat-0.8.7/tests/test_atom_bond_calculator.py` & `molfeat-0.8.8/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_descriptors.py` & `molfeat-0.8.8/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_fp.py` & `molfeat-0.8.8/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_graphs.py` & `molfeat-0.8.8/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_pharmacophore.py` & `molfeat-0.8.8/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_pretrained.py` & `molfeat-0.8.8/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_prot_embed.py` & `molfeat-0.8.8/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_state.py` & `molfeat-0.8.8/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.7/tests/test_utils.py` & `molfeat-0.8.8/tests/test_utils.py`

 * *Files identical despite different names*

