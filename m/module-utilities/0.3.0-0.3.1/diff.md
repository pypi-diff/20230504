# Comparing `tmp/module-utilities-0.3.0.tar.gz` & `tmp/module-utilities-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.3.0.tar", last modified: Wed May  3 20:30:10 2023, max compression
+gzip compressed data, was "module-utilities-0.3.1.tar", last modified: Thu May  4 19:05:27 2023, max compression
```

## Comparing `module-utilities-0.3.0.tar` & `module-utilities-0.3.1.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.798253 module-utilities-0.3.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1358 2023-05-03 02:36:13.000000 module-utilities-0.3.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.741254 module-utilities-0.3.0/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1307 2023-05-02 03:09:02.000000 module-utilities-0.3.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3581 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.3.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.3.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      495 2023-05-03 20:28:18.000000 module-utilities-0.3.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9267 2023-05-03 02:36:13.000000 module-utilities-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-27 23:45:36.000000 module-utilities-0.3.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.3.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11367 2023-05-03 02:36:13.000000 module-utilities-0.3.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6060 2023-05-03 20:30:10.798663 module-utilities-0.3.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2844 2023-05-03 02:36:13.000000 module-utilities-0.3.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.742133 module-utilities-0.3.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.742900 module-utilities-0.3.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.743970 module-utilities-0.3.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.3.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.3.0/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.749812 module-utilities-0.3.0/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.728433 module-utilities-0.3.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.750500 module-utilities-0.3.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.752436 module-utilities-0.3.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.758369 module-utilities-0.3.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.763003 module-utilities-0.3.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.765680 module-utilities-0.3.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.767992 module-utilities-0.3.0/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1675 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/example-usage-1.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1667 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       89 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.769562 module-utilities-0.3.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-05-03 20:28:18.000000 module-utilities-0.3.0/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      937 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.770407 module-utilities-0.3.0/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-05-03 02:36:13.000000 module-utilities-0.3.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.780300 module-utilities-0.3.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      232 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      349 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-27 23:45:36.000000 module-utilities-0.3.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-05-02 03:09:02.000000 module-utilities-0.3.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.781523 module-utilities-0.3.0/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.3.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.783594 module-utilities-0.3.0/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.0/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.0/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6202 2023-05-03 02:36:13.000000 module-utilities-0.3.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.788777 module-utilities-0.3.0/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      403 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-27 23:45:36.000000 module-utilities-0.3.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-02 03:09:02.000000 module-utilities-0.3.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-27 23:45:36.000000 module-utilities-0.3.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      297 2023-05-03 20:30:10.799712 module-utilities-0.3.0/setup.cfg
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-27 23:45:36.000000 module-utilities-0.3.0/setup.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.732011 module-utilities-0.3.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.792346 module-utilities-0.3.0/src/module_utilities/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      683 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23552 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_docscrape.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20974 2023-05-03 20:28:18.000000 module-utilities-0.3.0/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.3.0/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.795136 module-utilities-0.3.0/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6060 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2670 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-25 12:55:39.000000 module-utilities-0.3.0/src/module_utilities.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       48 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-05-03 20:30:10.000000 module-utilities-0.3.0/src/module_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:30:10.797558 module-utilities-0.3.0/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.3.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.0/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.3.0/tests/test_cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.3.0/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-05-02 03:09:02.000000 module-utilities-0.3.0/tests/test_module_utilities.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4013 2023-05-03 02:36:13.000000 module-utilities-0.3.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.786108 module-utilities-0.3.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1369 2023-05-04 19:04:22.000000 module-utilities-0.3.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.729675 module-utilities-0.3.1/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1307 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3581 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-05-04 19:04:22.000000 module-utilities-0.3.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.3.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      495 2023-05-03 20:28:18.000000 module-utilities-0.3.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9752 2023-05-04 19:04:22.000000 module-utilities-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-27 23:45:36.000000 module-utilities-0.3.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.3.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11367 2023-05-03 02:36:13.000000 module-utilities-0.3.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5998 2023-05-04 19:05:27.785460 module-utilities-0.3.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2844 2023-05-03 02:36:13.000000 module-utilities-0.3.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.730570 module-utilities-0.3.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.731454 module-utilities-0.3.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.733002 module-utilities-0.3.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.3.1/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.742537 module-utilities-0.3.1/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.711377 module-utilities-0.3.1/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.743007 module-utilities-0.3.1/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.744198 module-utilities-0.3.1/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.748213 module-utilities-0.3.1/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.750821 module-utilities-0.3.1/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.752387 module-utilities-0.3.1/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.754264 module-utilities-0.3.1/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1675 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/example-usage-1.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1667 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       89 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.755312 module-utilities-0.3.1/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      937 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.756420 module-utilities-0.3.1/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.763826 module-utilities-0.3.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      232 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      349 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.764729 module-utilities-0.3.1/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.3.1/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.766352 module-utilities-0.3.1/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.1/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.1/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6147 2023-05-04 19:04:22.000000 module-utilities-0.3.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.772182 module-utilities-0.3.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      847 2023-05-04 19:04:22.000000 module-utilities-0.3.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-27 23:45:36.000000 module-utilities-0.3.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:04:22.000000 module-utilities-0.3.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-27 23:45:36.000000 module-utilities-0.3.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:05:27.786317 module-utilities-0.3.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.715616 module-utilities-0.3.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.778045 module-utilities-0.3.1/src/module_utilities/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      683 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23552 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_docscrape.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20974 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.782030 module-utilities-0.3.1/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5998 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2692 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       48 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.784679 module-utilities-0.3.1/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.3.1/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.1/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.3.1/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.3.1/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-05-02 03:09:02.000000 module-utilities-0.3.1/tests/test_module_utilities.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4186 2023-05-04 19:04:22.000000 module-utilities-0.3.1/tox.ini
```

### Comparing `module-utilities-0.3.0/.cruft.json` & `module-utilities-0.3.1/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8994736842105263%*

 * *Differences: {"'commit'": "'10a9fe1a4f0b341184e41953433c344020f92c72'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(6, "*

 * *              "'changelog.d/templates/*.j2'), (7, "*

 * *              "'changelog.d/templates/auto-changelog/*.jinja2')], delete: [7, 6]}}}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "cb20a32f67dadb4142be54898a87de1efdce6bd6",
+    "commit": "10a9fe1a4f0b341184e41953433c344020f92c72",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
                 "docs/_static/css/*",
                 "docs/_static/js/*",
-                "changelog.d/templates/*",
-                "changelog.d/templates/auto-changlog/*"
+                "changelog.d/templates/*.j2",
+                "changelog.d/templates/auto-changelog/*.jinja2"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
```

### Comparing `module-utilities-0.3.0/.editorconfig` & `module-utilities-0.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/.gitignore` & `module-utilities-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/.pre-commit-config.yaml` & `module-utilities-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/CONTRIBUTING.md` & `module-utilities-0.3.1/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -386,7 +386,18 @@
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
 Versioning is handled with [setuptools_scm].The pacakge version is set by the
 git tag. For convenience, you can override the version in the makefile (calling
 tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
 the docs, etc.
+
+## Creating conda recipe
+
+[grayskull]: https://github.com/conda/grayskull
+
+For the most part, we use [grayskull] to create the conda recipe. However, I've
+had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
+variables. So, we use grayskull to build the majority of the recipe, and append
+the file `.recipe-append.yaml`. For some edge cases (install name different from
+package name, etc), you'll need to manually edit this file to create the final
+recipe.
```

### Comparing `module-utilities-0.3.0/LICENSE` & `module-utilities-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/Makefile` & `module-utilities-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/PKG-INFO` & `module-utilities-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of utilities to aid working with python modules.
-Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `module-utilities-0.3.0/README.md` & `module-utilities-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.3.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/Makefile` & `module-utilities-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_static/css/nist-combined.css` & `module-utilities-0.3.1/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_static/js/leave_notice.js` & `module-utilities-0.3.1/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_static/js/nist-header-footer.js` & `module-utilities-0.3.1/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/autosummary/class.rst` & `module-utilities-0.3.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/autosummary/module.rst` & `module-utilities-0.3.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/class-individual-pages.rst` & `module-utilities-0.3.1/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/class-single-page.rst` & `module-utilities-0.3.1/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/custom-module-template.rst` & `module-utilities-0.3.1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/module-custom-imported.rst` & `module-utilities-0.3.1/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/module-custom.rst` & `module-utilities-0.3.1/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/module-single.rst` & `module-utilities-0.3.1/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/_templates/module-template.rst` & `module-utilities-0.3.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/conf.py` & `module-utilities-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/examples/example-usage-1.rst` & `module-utilities-0.3.1/docs/examples/example-usage-1.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/examples/example-usage.md` & `module-utilities-0.3.1/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/examples/usage/cached.ipynb` & `module-utilities-0.3.1/docs/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/examples/usage/docfiller.ipynb` & `module-utilities-0.3.1/docs/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/installation.md` & `module-utilities-0.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/docs/make.bat` & `module-utilities-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/environment/dev-extras.yaml` & `module-utilities-0.3.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/environment/docs-extras.yaml` & `module-utilities-0.3.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/examples/usage/cached.ipynb` & `module-utilities-0.3.1/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/examples/usage/docfiller.ipynb` & `module-utilities-0.3.1/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/pyproject.toml` & `module-utilities-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "module-utilities"
 authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
-license = { text = "NIST license" }
+license = { text = "NIST-PD" }
 description = "Collection of utilities to aid working with python modules."
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["module-utilities"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -33,24 +33,24 @@
 
 [project.optional-dependencies]
 test = ["pytest"]
 attrs = ["attrs"]
 
 # dev = []
 # docs = []
-## Defer this to setup.cfg
-## Will transition when everything works (grayskull in particular)
-## and will remove setup.py
-# [tool.setuptools]
-# zip-safe = true # if using mypy, must be False
-# include-package-data = true
-# license-files = ["LICENSE"]
-# [tool.setuptools.packages.find]
-# namespaces = true
-# where = ["src"]
+## grayskull still messes some things up, but use scripts/recipe-append.sh for this
+[tool.setuptools]
+zip-safe = true # if using mypy, must be False
+include-package-data = true
+license-files = ["LICENSE"]
+
+[tool.setuptools.packages.find]
+namespaces = true
+where = ["src"]
+
 ## include = []
 ## exclude = []
 ##
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
```

### Comparing `module-utilities-0.3.0/scripts/docs-examples-symlinks.sh` & `module-utilities-0.3.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/__init__.py` & `module-utilities-0.3.1/src/module_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/_doc.py` & `module-utilities-0.3.1/src/module_utilities/_doc.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/_docscrape.py` & `module-utilities-0.3.1/src/module_utilities/_docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/attributedict.py` & `module-utilities-0.3.1/src/module_utilities/attributedict.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/cached.py` & `module-utilities-0.3.1/src/module_utilities/cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities/docfiller.py` & `module-utilities-0.3.1/src/module_utilities/docfiller.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.3.1/src/module_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of utilities to aid working with python modules.
-Home-page: https://github.com/usnistgov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `module-utilities-0.3.0/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.3.1/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 .cruft.json
 .editorconfig
 .gitignore
 .markdownlint.yaml
 .pre-commit-config.yaml
 .prettierrc.yaml
+.recipe-append.yaml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 conftest.py
 environment.yaml
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
 .github/ISSUE_TEMPLATE.md
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
@@ -71,28 +70,29 @@
 examples/README.md
 examples/usage/cached.ipynb
 examples/usage/docfiller.ipynb
 scripts/dist-conda.mk
 scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
 scripts/lint.mk
+scripts/recipe-append.sh
 scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/module_utilities/__init__.py
 src/module_utilities/_doc.py
 src/module_utilities/_docscrape.py
 src/module_utilities/_typing.py
 src/module_utilities/attributedict.py
 src/module_utilities/cached.py
 src/module_utilities/docfiller.py
 src/module_utilities/py.typed
 src/module_utilities.egg-info/PKG-INFO
 src/module_utilities.egg-info/SOURCES.txt
 src/module_utilities.egg-info/dependency_links.txt
-src/module_utilities.egg-info/not-zip-safe
 src/module_utilities.egg-info/requires.txt
 src/module_utilities.egg-info/top_level.txt
+src/module_utilities.egg-info/zip-safe
 tests/__init__.py
 tests/conftest.py
 tests/test_cached.py
 tests/test_docfiller.py
 tests/test_module_utilities.py
```

### Comparing `module-utilities-0.3.0/tests/test_cached.py` & `module-utilities-0.3.1/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/tests/test_docfiller.py` & `module-utilities-0.3.1/tests/test_docfiller.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.0/tox.ini` & `module-utilities-0.3.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -27,21 +27,28 @@
     python --version
     python -c 'import {[base]import_name}; print( {[base]import_name}.__version__)'
     bash -ec 'echo $PWD'
 
 [testenv]
 passenv =
         SETUPTOOLS_SCM_PRETEND_VERSION
+        TEST_VERSION
+        # general command
         command
+        # linting
         mypy_args
         pyright_args
         pytype_args
         release_args
+        # dist-conda stuff
         project_name
-        TEST_VERSION
+        sdist_path
+        grayskull_args
+        recipe_base_path
+        recipe_append_path
 usedevelop =
     test: True
 conda_env =
     test: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
@@ -98,17 +105,17 @@
     recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
-changedir    = {toxinidir}/dist-conda
+changedir    = {toxinidir}
 commands     =
-    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={[base]package_name}
+    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={env:project_name:{[base]package_name}}
 
 [testenv:testdist-{pypi, conda}-{local,remote}-py3{8, 9, 10, 11}]
 conda_channels =
     {[base]conda_channels}
 description =
     Test install from
     pypi: pypi
```

