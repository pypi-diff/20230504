# Comparing `tmp/analphipy-0.1.0.tar.gz` & `tmp/analphipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analphipy-0.1.0.tar", last modified: Tue Apr 25 03:08:15 2023, max compression
+gzip compressed data, was "analphipy-0.2.0.tar", last modified: Thu May  4 18:50:22 2023, max compression
```

## Comparing `analphipy-0.1.0.tar` & `analphipy-0.2.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.086929 analphipy-0.1.0/
--rw-r--r--   0 wpk      (42033)    36681     1502 2023-04-25 03:05:00.000000 analphipy-0.1.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      513 2023-04-25 03:05:00.000000 analphipy-0.1.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.941852 analphipy-0.1.0/.github/
--rw-r--r--   0 wpk      (42033)    36681      361 2023-04-25 03:05:00.000000 analphipy-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1313 2023-04-25 03:05:00.000000 analphipy-0.1.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-04-25 03:05:00.000000 analphipy-0.1.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3549 2023-04-25 03:05:00.000000 analphipy-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-04-25 03:05:00.000000 analphipy-0.1.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      131 2023-04-19 04:41:12.000000 analphipy-0.1.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      967 2023-04-25 03:05:00.000000 analphipy-0.1.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9146 2023-04-25 03:05:00.000000 analphipy-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2022-09-26 16:03:57.000000 analphipy-0.1.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-04-25 03:05:00.000000 analphipy-0.1.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    10568 2023-04-25 03:05:00.000000 analphipy-0.1.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     6596 2023-04-25 03:08:15.087669 analphipy-0.1.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2966 2023-04-25 03:05:00.000000 analphipy-0.1.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.942689 analphipy-0.1.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.943590 analphipy-0.1.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.945373 analphipy-0.1.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.957554 analphipy-0.1.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1201 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.916256 analphipy-0.1.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.958915 analphipy-0.1.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.961143 analphipy-0.1.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      837 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.975721 analphipy-0.1.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.982266 analphipy-0.1.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.986764 analphipy-0.1.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-14 18:58:52.000000 analphipy-0.1.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-template.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.988405 analphipy-0.1.0/docs/_templates/test/
--rw-r--r--   0 wpk      (42033)    36681     1166 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/test/class-1.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14667 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.991160 analphipy-0.1.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      887 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/create-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681       58 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.992727 analphipy-0.1.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   113096 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/usage/usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681      224 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      768 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      170 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.994331 analphipy-0.1.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      324 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/reference/index.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.009710 analphipy-0.1.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      929 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      381 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      552 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      430 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       50 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      208 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681      124 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      182 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      168 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.011342 analphipy-0.1.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-04-25 03:05:00.000000 analphipy-0.1.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.012467 analphipy-0.1.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   113096 2023-04-25 03:05:00.000000 analphipy-0.1.0/examples/usage/usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681     5428 2023-04-25 03:05:00.000000 analphipy-0.1.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.015821 analphipy-0.1.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-25 03:05:00.000000 analphipy-0.1.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-04-25 03:05:00.000000 analphipy-0.1.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681      290 2023-04-25 03:08:15.089612 analphipy-0.1.0/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-25 03:05:00.000000 analphipy-0.1.0/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.924342 analphipy-0.1.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.035095 analphipy-0.1.0/src/analphipy/
--rw-r--r--   0 wpk      (42033)    36681     1074 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     1031 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_attrs_utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.048091 analphipy-0.1.0/src/analphipy/_docfiller/
--rw-r--r--   0 wpk      (42033)    36681    19472 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_docfiller/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    23552 2023-03-22 17:48:12.000000 analphipy-0.1.0/src/analphipy/_docfiller/docscrape.py
--rw-r--r--   0 wpk      (42033)    36681     2526 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681      478 2022-09-27 20:23:36.000000 analphipy-0.1.0/src/analphipy/_typing.py
--rw-r--r--   0 wpk      (42033)    36681    12807 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/base_potential.py
--rw-r--r--   0 wpk      (42033)    36681     6297 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/cached_decorators.py
--rw-r--r--   0 wpk      (42033)    36681    12925 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/measures.py
--rw-r--r--   0 wpk      (42033)    36681    15134 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/norofrenkel.py
--rw-r--r--   0 wpk      (42033)    36681    14197 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/potential.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 17:48:12.000000 analphipy-0.1.0/src/analphipy/py.typed
--rw-r--r--   0 wpk      (42033)    36681     9878 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.045326 analphipy-0.1.0/src/analphipy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     6596 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     3074 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-07 19:52:25.000000 analphipy-0.1.0/src/analphipy.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033)    36681       73 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       10 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.060512 analphipy-0.1.0/tests/
--rw-r--r--   0 wpk      (42033)    36681       39 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     6600 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.085562 analphipy-0.1.0/tests/data/
--rw-r--r--   0 wpk      (42033)    36681     1175 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681      671 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     1273 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681      862 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681      110 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_hs_.csv
--rw-r--r--   0 wpk      (42033)    36681    15874 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681     5137 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     2479 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_stockmayer_.csv
--rw-r--r--   0 wpk      (42033)    36681    14148 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681     5317 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681    18038 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_hs_.csv
--rw-r--r--   0 wpk      (42033)    36681    21577 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681     7033 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     3284 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_stockmayer_.csv
--rw-r--r--   0 wpk      (42033)    36681     9423 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681     4247 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681     2145 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_generic.py
--rw-r--r--   0 wpk      (42033)    36681      735 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_js.py
--rw-r--r--   0 wpk      (42033)    36681     1738 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_nf_derivs.py
--rw-r--r--   0 wpk      (42033)    36681     3035 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_norofrenkel.py
--rw-r--r--   0 wpk      (42033)    36681     2027 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_potentials.py
--rw-r--r--   0 wpk      (42033)    36681     3353 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_secondvirial.py
--rw-r--r--   0 wpk      (42033)    36681     4569 2023-04-25 03:05:00.000000 analphipy-0.1.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.205371 analphipy-0.2.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1513 2023-05-04 18:49:45.000000 analphipy-0.2.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-04 18:49:45.000000 analphipy-0.2.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.158523 analphipy-0.2.0/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      361 2023-05-01 20:48:47.000000 analphipy-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-04 18:49:45.000000 analphipy-0.2.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-25 03:05:00.000000 analphipy-0.2.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3804 2023-05-04 18:49:45.000000 analphipy-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-25 03:05:00.000000 analphipy-0.2.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      561 2023-05-04 18:49:45.000000 analphipy-0.2.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      131 2023-04-19 04:41:12.000000 analphipy-0.2.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1195 2023-05-04 18:49:45.000000 analphipy-0.2.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9682 2023-05-04 18:49:45.000000 analphipy-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2022-09-26 16:03:57.000000 analphipy-0.2.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-25 03:05:00.000000 analphipy-0.2.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11455 2023-05-04 18:49:45.000000 analphipy-0.2.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6769 2023-05-04 18:50:22.204728 analphipy-0.2.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2966 2023-04-25 03:05:00.000000 analphipy-0.2.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.159393 analphipy-0.2.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-25 03:05:00.000000 analphipy-0.2.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.159895 analphipy-0.2.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.161183 analphipy-0.2.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-25 03:05:00.000000 analphipy-0.2.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-25 03:05:00.000000 analphipy-0.2.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-25 03:05:00.000000 analphipy-0.2.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.167701 analphipy-0.2.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-04 18:49:45.000000 analphipy-0.2.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.145327 analphipy-0.2.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.168300 analphipy-0.2.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.169536 analphipy-0.2.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      837 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.172402 analphipy-0.2.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.174545 analphipy-0.2.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.175898 analphipy-0.2.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-14 18:58:52.000000 analphipy-0.2.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.176324 analphipy-0.2.0/docs/_templates/test/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1166 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/_templates/test/class-1.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14667 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.176715 analphipy-0.2.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       58 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.177123 analphipy-0.2.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   113096 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/examples/usage/usage.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      768 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      170 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.177766 analphipy-0.2.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      324 2023-04-25 03:05:00.000000 analphipy-0.2.0/docs/reference/index.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-03-22 17:48:12.000000 analphipy-0.2.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.182258 analphipy-0.2.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      929 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      409 2023-05-04 18:49:45.000000 analphipy-0.2.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      552 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      458 2023-05-04 18:49:45.000000 analphipy-0.2.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       50 2023-05-02 04:00:17.000000 analphipy-0.2.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      236 2023-05-04 18:49:45.000000 analphipy-0.2.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      124 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      210 2023-05-04 18:49:45.000000 analphipy-0.2.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-25 03:05:00.000000 analphipy-0.2.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      196 2023-05-04 18:49:45.000000 analphipy-0.2.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.182647 analphipy-0.2.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-25 03:05:00.000000 analphipy-0.2.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.183021 analphipy-0.2.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   113096 2023-04-25 03:05:00.000000 analphipy-0.2.0/examples/usage/usage.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6140 2023-05-04 18:49:45.000000 analphipy-0.2.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.186090 analphipy-0.2.0/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      840 2023-05-04 18:49:45.000000 analphipy-0.2.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-04 18:49:45.000000 analphipy-0.2.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-25 03:05:00.000000 analphipy-0.2.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-04 18:49:45.000000 analphipy-0.2.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 18:49:45.000000 analphipy-0.2.0/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-04 18:49:45.000000 analphipy-0.2.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-25 03:05:00.000000 analphipy-0.2.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 18:50:22.205578 analphipy-0.2.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.148853 analphipy-0.2.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.190194 analphipy-0.2.0/src/analphipy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1074 2023-04-25 03:05:00.000000 analphipy-0.2.0/src/analphipy/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1031 2023-04-25 03:05:00.000000 analphipy-0.2.0/src/analphipy/_attrs_utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2562 2023-05-04 18:49:45.000000 analphipy-0.2.0/src/analphipy/_docstrings.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      478 2022-09-27 20:23:36.000000 analphipy-0.2.0/src/analphipy/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12800 2023-05-04 18:49:45.000000 analphipy-0.2.0/src/analphipy/base_potential.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12706 2023-05-04 18:49:45.000000 analphipy-0.2.0/src/analphipy/measures.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15297 2023-05-04 18:49:45.000000 analphipy-0.2.0/src/analphipy/norofrenkel.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14197 2023-04-25 03:05:00.000000 analphipy-0.2.0/src/analphipy/potential.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-03-22 17:48:12.000000 analphipy-0.2.0/src/analphipy/py.typed
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10105 2023-05-04 18:49:45.000000 analphipy-0.2.0/src/analphipy/utils.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.192828 analphipy-0.2.0/src/analphipy.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6769 2023-05-04 18:50:22.000000 analphipy-0.2.0/src/analphipy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3036 2023-05-04 18:50:22.000000 analphipy-0.2.0/src/analphipy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 18:50:22.000000 analphipy-0.2.0/src/analphipy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       95 2023-05-04 18:50:22.000000 analphipy-0.2.0/src/analphipy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       10 2023-05-04 18:50:22.000000 analphipy-0.2.0/src/analphipy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 18:50:21.000000 analphipy-0.2.0/src/analphipy.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.196455 analphipy-0.2.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       39 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6600 2023-04-25 03:05:00.000000 analphipy-0.2.0/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 18:50:22.203847 analphipy-0.2.0/tests/data/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1175 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/crit_eff_lj_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      671 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/crit_eff_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1273 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/crit_eff_sw_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      862 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/crit_eff_yukawa_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      110 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_hs_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15874 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_lj_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5137 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2479 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_stockmayer_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14148 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_sw_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5317 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/eff_yukawa_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18038 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_hs_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21577 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_lj_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7033 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3284 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_stockmayer_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9423 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_sw_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4247 2022-09-26 16:03:57.000000 analphipy-0.2.0/tests/data/vir_yukawa_.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2145 2023-03-22 17:48:12.000000 analphipy-0.2.0/tests/test_generic.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      735 2023-04-25 03:05:00.000000 analphipy-0.2.0/tests/test_js.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1738 2023-03-22 17:48:12.000000 analphipy-0.2.0/tests/test_nf_derivs.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3035 2023-04-25 03:05:00.000000 analphipy-0.2.0/tests/test_norofrenkel.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2027 2023-03-22 17:48:12.000000 analphipy-0.2.0/tests/test_potentials.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3353 2023-04-25 03:05:00.000000 analphipy-0.2.0/tests/test_secondvirial.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3962 2023-05-04 18:49:45.000000 analphipy-0.2.0/tox.ini
```

### Comparing `analphipy-0.1.0/.cruft.json` & `analphipy-0.2.0/.cruft.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9162280701754386%*

 * *Differences: {"'commit'": "'10a9fe1a4f0b341184e41953433c344020f92c72'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(6, "*

 * *              "'changelog.d/templates/*.j2'), (7, "*

 * *              "'changelog.d/templates/auto-changelog/*.jinja2')], delete: [7, 6]}}}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "f7522615a7ab432e28a39c485f4110b86b9e37af",
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

### Comparing `analphipy-0.1.0/.editorconfig` & `analphipy-0.2.0/.editorconfig`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 [LICENSE]
 insert_final_newline = false
 
 [Makefile]
 indent_style = tab
 
+[*.mk]
+indent_style = tab
+
 [*.{yaml,yml}]
 indent_size = 2
 
 [*.ini]
 indent_size = 4
 
 [*.json]
```

### Comparing `analphipy-0.1.0/.gitignore` & `analphipy-0.2.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
-dist-conda/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -105,8 +104,9 @@
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
 /docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/
+/dist-conda/*
+!/dist-conda/Makefile
```

### Comparing `analphipy-0.1.0/.pre-commit-config.yaml` & `analphipy-0.2.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,24 @@
         args: ["-e", "lint-mypy"]
         language: system
         pass_filenames: false
         # additional_dependencies: [tox]
         types: [python]
         require_serial: true
         stages: [manual]
+      - id: pyright
+        name: pyright
+        entry: pyright
+        args: []
+        language: system
+        pass_filenames: true
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
   # isort, pyupgrade, flake8 defer to ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         stages: [manual]
   - repo: https://github.com/asottile/pyupgrade
```

### Comparing `analphipy-0.1.0/CONTRIBUTING.md` & `analphipy-0.2.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -289,41 +289,45 @@
 ## Building the docs
 
 We use [tox] to isolate the documentation build. Useful commands are as follows.
 
 - Build the docs:
 
   ```bash
-  tox -e docs-build
+  tox -e docs -- build
   ```
 
 - Spellcheck the docs:
 
   ```bash
-  tox -e docs-spelling
+  tox -e docs -- spelling
   ```
 
 - Create a release of the docs:
 
   ```bash
-  tox -e docs-release
+  tox -e docs -- release
   ```
 
   If you make any changes to `docs/examples`, you should run:
 
   ```bash
   make docs-examples-symlink
   ```
 
   to update symlinks from `docs/examples` to `examples`.
 
   After this, the docs can be pushed to the correct branch for distribution.
 
 - Live documentation updates using
 
+  ```bash
+  make docs-livehtml
+  ```
+
 ## Using tox
 
 The package is setup to use tox to test, build and release pip and conda
 distributions, and release the docs. Most of these tasks have a command in the
 `Makefile`. To test against multiple versions, use:
 
 ```bash
@@ -335,15 +339,15 @@
 ```bash
 make docs-build
 ```
 
 To release the documentation use:
 
 ```bash
-make docs-release posargs='-m "commit message" -r origin -p'
+make docs-release release_args='-m "commit message" -r origin -p'
 ```
 
 Where posargs is are passed to ghp-import. Note that the branch created is
 called `nist-pages`. This can be changed in `tox.ini`.
 
 To build the distribution, use:
 
@@ -377,11 +381,22 @@
 
 where one options in the brackets should be choosen.
 
 ## Package version
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
-Versioning is handled with [setuptools_scm]. The pacakge version is set by the
+Versioning is handled with [setuptools_scm].The pacakge version is set by the
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

### Comparing `analphipy-0.1.0/LICENSE` & `analphipy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/Makefile` & `analphipy-0.2.0/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 	pre-commit run --all-files --hook-stage manual pyupgrade
 	pre-commit run --all-files --hook-stage manual nbqa-pyupgrade
 	pre-commit run --all-files --hook-stage manual nbqa-isort
 
 pre-commit-mypy: ## run mypy
 	pre-commit run --all-files --hook-stage manual mypy
 
+pre-commit-pyright: ## run pyright
+	pre-commit run --all-files --hook-stage manual pyright
+
 pre-commit-codespell: ## run codespell. Note that this imports allowed words from docs/spelling_wordlist.txt
 	pre-commit run --all-files --hook-stage manual codespell
 
 
 ################################################################################
 # my convenience functions
 ################################################################################
@@ -138,31 +141,31 @@
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
 ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
-PRETTIER = pre-commit run prettier --files
+PRETTIER = bash scripts/run-prettier.sh
 
 
 environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
 	conda-merge $^ > $@
-	-$(PRETTIER) $@ &> /dev/null || true
+	$(PRETTIER) $@
 
 environment/dev.yaml: ## development environment yaml file
 environment/test.yaml: ## testing environment yaml file
 enviornment/docs.yaml: ## docs environment yaml file
 
 
 # special for linters
 environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
 	echo $^
 	conda-merge $^ > $@
-	-$(PRETTIER) $@ &> /dev/null || true
+	$(PRETTIER) $@
 
 ENVIRONMENTS += environment/lint.yaml
 
 .PHONY: environment-files-clean
 environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
 	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
@@ -185,106 +188,118 @@
 
 mamba-dev-update: environment/dev.yaml ## update development environment
 	mamba env update -f $<
 
 ################################################################################
 # TOX
 ###############################################################################
-tox_posargs?=-v
+tox_args?=-v
 version?=
-TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_posargs)
+TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
 
 .PHONY: tox-ipykernel-display-name
 tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
 	bash ./scripts/tox-ipykernel-display-name.sh analphipy
 
 ## dev env
 .PHONY: dev-env
 dev-env: environment/dev.yaml ## create development environment using tox
 	tox -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox
+test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
 	$(TOX) -- $(posargs)
 
-
 ## docs
 .PHONY: docs-examples-symlink
 docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
 	bash ./scripts/docs-examples-symlinks.sh
 
 
-.PHONY: docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-open docs-live docs-clean-build docs-linkcheck
-posargs=
+.PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use posargs=... to override stuff
-	$(TOX) -e $@ -- $(posargs)
+docs-release: ## release docs.  use release_args=... to override stuff
+	$(TOX) -e docs -- release
+docs-command: ## run command with command=...
+	$(TOX) -e docs -- command
+
+.PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e $@ -- $(posargs)
-docs-nist-pages: ## do both build and releas
-	$(TOX) -e $@ -- $(posargs)
-docs-live: ## use autobuild for docs
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- spelling
+docs-livehtml: ## use autobuild for docs
+	$(TOX) -e docs -- livehtml
 docs-open: ## open the build
 	$(BROWSER) docs/_build/html/index.html
 docs-linkcheck: ## check links
-	$(TOX) -e docs-build -- linkcheck
+	$(TOX) -e docs -- linkcheck
 
-docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-live: environment/docs.yaml
+docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
+## linting
+.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
+lint-mypy: ## run mypy mypy_args=...
+	$(TOX) -e lint -- mypy
+lint-pyright: ## run pyright pyright_args=...
+	$(TOX) -e lint -- pyright
+lint-pytype: ## run pytype pytype_args=...
+	$(TOX) -e lint -- pytype
+lint-all:
+	$(TOX) -e lint -- all
+lint-command:
+	$(TOX) -e lint -- command
+
+lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
 
 ## distribution
-.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-conda-recipe dist-conda-build
+.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
-posargs=
-dist-pypi-build: ## build dist, can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-testrelease: ## test release on testpypi. can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
+dist-pypi-build: ## build dist
+	$(TOX) -e dist-pypi -- build
+dist-pypi-testrelease: ## test release on testpypi
+	$(TOX) -e dist-pypi -- testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-build dist-pypi-testrelease dist-pypi-release: environment/dist-pypi.yaml
+	$(TOX) -e dist-pypi -- release
+dist-pypi-command: ## run command with command=...
+	$(TOX) -e dist-pypi -- command
+dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
+.PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e dist-conda -- recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(pasargs)
-dist-conda-build dist-conda-recipe: environment/dist-conda.yaml
+	$(TOX) -e dist-conda -- build
+dist-conda-command: ## run command with command=...
+	$(TOX) -e dist-conda -- command
+dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
-.PHONY: test-dist-pypi-remote test-dist-conda-remote test-dist-pypi-local test-dist-conda-local
+.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-test-dist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
+testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-test-dist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
+testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
+testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 
-
-test-dist-pypi: environment/test.
-
+testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
 
 ## list all options
 .PHONY: tox-list
-
 tox-list:
 	$(TOX) -a
 
 
 ################################################################################
 # installation
 ################################################################################
```

### Comparing `analphipy-0.1.0/PKG-INFO` & `analphipy-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: analphipy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities to perform stat mech analysis of pair potentials
-Home-page: https://github.com/usnistgov/analphipy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/analphipy
 Project-URL: documentation, https://pages.nist.gov/analphipy/
 Keywords: analphipy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -134,14 +133,26 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/analphipy)
 
 <!-- scriv-insert-here -->
 
+## v0.2.0 — 2023-05-04
+
+### Removed
+
+- Removed `cached_decorator` module.
+- Removed `docfiller` module.
+
+### Added
+
+- Now use [module-utilities](https://pypi.org/project/module-utilities/) to
+  handle caching and docfilling.
+
 ## v0.1.0 — 2023-04-24
 
 ### Changed
 
 - Update package layout
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `analphipy-0.1.0/README.md` & `analphipy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/changelog.d/templates/auto-changelog/template.jinja2` & `analphipy-0.2.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/Makefile` & `analphipy-0.2.0/docs/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -14,33 +14,39 @@
 ALLSPHINXAUTOOPTS = $(ALLSPHINXOPTS) \
 	--ignore "*/$(BUILDDIR)/*" \
 	--ignore "*/generated/*" \
 	--ignore "*/jupyter_execute/*" \
 	--ignore "*/.ipynb_checkpoints/*"
 
 
+
+.PHONY: help Makefile clean-all build livehtml showlinks release command
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(ALLSPHINXOPTS) $(O)
 
-
-allclean: clean
-	rm -rf $(BUILDDIR)/*
-	rm -rf generated/*
-	rm -rf reference/generated/*
-
-.PHONY: help Makefile allclean
-
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(ALLSPHINXOPTS) $(O)
 
+clean-all: clean
+	rm -rf $(BUILDDIR)/*
+	rm -rf generated/*
+	rm -rf reference/generated/*
+
+# Alias to html
+build: html
 
-.PHONY: livehtml
 livehtml:
 	$(SPHINXAUTOBUILD) "$(SOURCEDIR)" "$(BUILDDIR)/html" $(ALLSPHINXAUTOOPTS) $(O)
 
-
-.PHONY: showlinks
 showlinks:
 	python -m sphinx.ext.intersphinx $(BUILDDIR)/html/objects.inv
+
+release_args ?= -m "update docs" -b nist-pages
+release:
+	ghp-import -o -n $(release_args) $(BUILDDIR)/html
+
+command ?= @echo pass "command=..."
+command:
+	$(command)
```

### Comparing `analphipy-0.1.0/docs/_static/css/nist-combined.css` & `analphipy-0.2.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_static/js/leave_notice.js` & `analphipy-0.2.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_static/js/nist-header-footer.js` & `analphipy-0.2.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/autosummary/class.rst` & `analphipy-0.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/autosummary/module.rst` & `analphipy-0.2.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/class-individual-pages.rst` & `analphipy-0.2.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/class-single-page.rst` & `analphipy-0.2.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/custom-module-template.rst` & `analphipy-0.2.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/module-custom-imported.rst` & `analphipy-0.2.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/module-custom.rst` & `analphipy-0.2.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/module-single.rst` & `analphipy-0.2.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/module-template.rst` & `analphipy-0.2.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/_templates/test/class-1.rst` & `analphipy-0.2.0/docs/_templates/test/class-1.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/conf.py` & `analphipy-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/examples/usage/usage.ipynb` & `analphipy-0.2.0/docs/examples/usage/usage.ipynb`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/installation.md` & `analphipy-0.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/docs/make.bat` & `analphipy-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/environment/dev-extras.yaml` & `analphipy-0.2.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/environment/docs-extras.yaml` & `analphipy-0.2.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/examples/usage/usage.ipynb` & `analphipy-0.2.0/examples/usage/usage.ipynb`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/pyproject.toml` & `analphipy-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "analphipy"
 authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
-license = { text = "NIST license" }
+license = { text = "NIST-PD" }
 description = "Utilities to perform stat mech analysis of pair potentials"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["analphipy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -28,14 +28,15 @@
 dependencies = [
     # additional packages
     "attrs",
     "typing-extensions",
     "numpy",
     "scipy",
     "custom-inherit",
+    "module-utilities >= 0.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/analphipy"
 documentation = "https://pages.nist.gov/analphipy/"
 
 [project.optional-dependencies]
@@ -43,24 +44,23 @@
     "pandas",
     "pytest",
     # "pytest-mypy",
     # "mypy",
 
 ]
 
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
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
@@ -234,19 +234,48 @@
 files = ["src/analphipy", "tests"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
 exclude = [".eggs", ".tox", "doc", "docs"]
 
+# check_untyped_defs = true
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
     "custom_inherit",
     "scipy.integrate.*",
     "scipy.optimize.*",
     "scipy.misc.*"
 ]
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = []
+
+[tool.pyright]
+include = ["src", "tests"]
+exclude = ["**/__pycache__", ".tox/**", "**/.mypy_cache"]
+pythonVersion = "3.10"
+typeCheckingMode = "basic"
+# enable subset of "strict"
+reportDuplicateImport = true
+reportInvalidStubStatement = true
+reportOverlappingOverload = true
+reportPropertyTypeMismatch = true
+reportUntypedClassDecorator = true
+reportUntypedFunctionDecorator = true
+reportUntypedNamedTuple = true
+reportUnusedImport = true
+# disable subset of "basic"
+reportGeneralTypeIssues = false
+reportMissingModuleSource = false
+reportOptionalCall = false
+reportOptionalIterable = false
+reportOptionalMemberAccess = false
+reportOptionalOperand = false
+reportOptionalSubscript = false
+reportPrivateImportUsage = false
+reportUnboundVariable = false
+
+[tool.pytype]
+inputs = ["src", "tests"]
```

### Comparing `analphipy-0.1.0/scripts/docs-examples-symlinks.sh` & `analphipy-0.2.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/src/analphipy/__init__.py` & `analphipy-0.2.0/src/analphipy/__init__.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/src/analphipy/_attrs_utils.py` & `analphipy-0.2.0/src/analphipy/_attrs_utils.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/src/analphipy/_docstrings.py` & `analphipy-0.2.0/src/analphipy/_docstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# type: ignore
 """Common docstrings."""
 
 from __future__ import annotations
 
-from ._docfiller import DocFiller
+# from ._docfiller import DocFiller
+from module_utilities.docfiller import DocFiller
 
 _docstrings_shared = """
 Parameters
 ----------
 segments : sequence of int
     Integration limits. For ``n = len(segments)`` integration will be performed over ranges
     ``(segments[0], segments[1]), (segments[1], segments[2]), ..., (segments[n-2], segments[n-]])``
```

### Comparing `analphipy-0.1.0/src/analphipy/base_potential.py` & `analphipy-0.2.0/src/analphipy/base_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     #: Value of ``phi`` at minimum.
     phi_min: float | None = _kw_only_field(
         converter=optional_converter(float), repr=field_formatter()
     )
 
     #: Integration limits
-    segments: Sequence[float] | None = _kw_only_field(
+    segments: Sequence[float] = _kw_only_field(
         converter=segments_converter,
     )
 
     def asdict(self) -> dict:
         """Convert object to dictionary"""
         return attrs.asdict(self, filter=self._get_smart_filter())
```

### Comparing `analphipy-0.1.0/src/analphipy/measures.py` & `analphipy-0.2.0/src/analphipy/measures.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,38 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Mapping, Sequence, Union, cast
 
 import numpy as np
-from custom_inherit import doc_inherit
 
-from analphipy.cached_decorators import gcached
+# from custom_inherit import doc_inherit
+from module_utilities import cached
 
-from ._docstrings import docfiller_shared  # type: ignore
+from ._docstrings import DOCFILLER_SHARED
 
+# from module_utilities.docfiller import DocFiller
 if TYPE_CHECKING:
     from ._typing import ArrayLike, Float_or_ArrayLike, Phi_Signature
 from .utils import TWO_PI, add_quad_kws, combine_segmets, quad_segments
 
 __all__ = [
     "Measures",
     "secondvirial",
     "secondvirial_dbeta",
     "secondvirial_sw",
     "diverg_kl_cont",
     "diverg_js_cont",
 ]
 
+docfiller = DOCFILLER_SHARED
 
-@docfiller_shared
+
+@docfiller.decorate
 def secondvirial(
     phi: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
     **kws,
@@ -76,15 +79,15 @@
         sum_errors=True,
         err=err,
         full_output=full_output,
         **kws,
     )
 
 
-@docfiller_shared
+@docfiller.decorate
 def secondvirial_dbeta(
     phi: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
     **kws,
@@ -128,15 +131,15 @@
         sum_errors=True,
         err=err,
         full_output=full_output,
         **kws,
     )
 
 
-@docfiller_shared
+@docfiller.decorate
 def secondvirial_sw(beta: float, sig: float, eps: float, lam: float):
     r"""
     Second virial coefficient for a square well (SW) fluid. Note that this assumes that
     the SW fluid is defined by the potential:
 
     .. math::
 
@@ -186,29 +189,29 @@
 
     if volume is not None:
         out *= np.asarray(volume)
 
     return out
 
 
-@docfiller_shared
+@docfiller(summary="Calculate discrete Kullback-Leibler divergence")
 def diverg_kl_disc(
     P: Float_or_ArrayLike, Q: Float_or_ArrayLike, axis: int | None = None
 ) -> float | np.ndarray:
     """
-    Calculate discrete Kullback–Leibler divergence
+    {summary}
 
     Parameters
     ----------
     P, Q : array-like
         Probabilities to consider
     Returns
     -------
-    result : float or ndarray
-        value of KB divergence
+    results : float or ndarray
+        Value of divergence.
 
     References
     ----------
     {kl_link}
     """
 
     P, Q = np.asarray(P), np.asarray(Q)
@@ -232,27 +235,29 @@
             raise ValueError("unknown dimension")
     else:
         assert callable(volume)
 
     return volume
 
 
-@docfiller_shared
+@docfiller(
+    summary="Calculate continuous Kullback–Leibler divergence for continuous pdf"
+)
 def diverg_kl_cont(
     p: Callable,
     q: Callable,
     segments: ArrayLike,
     segments_q: ArrayLike | None = None,
     volume: str | Callable | None = None,
     err: bool = False,
     full_output: bool = False,
     **kws,
 ):
     """
-    Calculate continuous Kullback–Leibler divergence for continuous pdf
+    {summary}
 
     Parameters
     ----------
     p, q: callable
         Probabilities to consider
     {volume_int_func}
     {segments}
@@ -260,15 +265,15 @@
         if supplied, build total segments by combining segments and segments_q
     {err}
     {full_output}
 
     Returns
     -------
     result : float or ndarray
-        value of KB divergence
+        value of divergence
     {error_summed}
     {full_output_summed}
 
     References
     ----------
     {kl_link}
     """
@@ -287,31 +292,19 @@
         sum_errors=True,
         err=err,
         full_output=full_output,
         **kws,
     )
 
 
-@doc_inherit(diverg_kl_disc, style="numpy_with_merge")
+# @doc_inherit(diverg_kl_disc, style="numpy_with_merge")
+@docfiller(diverg_kl_disc, summary="Discrete Jensen–Shannon divergence")
 def diverg_js_disc(
     P: Float_or_ArrayLike, Q: Float_or_ArrayLike, axis: int | None = None
 ) -> float | np.ndarray:
-    """
-    Discrete Jensen–Shannon divergence
-
-    Returns
-    -------
-    result : float or ndarray
-        value of JS divergence
-
-    References
-    ----------
-    {js_link}
-    """
-
     P, Q = np.asarray(P), np.asarray(Q)
 
     M = 0.5 * (P + Q)
 
     out = 0.5 * (diverg_kl_disc(P, M, axis=axis) + diverg_kl_disc(Q, M, axis=axis))
     return cast(Union[float, np.ndarray], out)
 
@@ -330,40 +323,25 @@
 
     if volume is not None:
         out *= np.asarray(volume)
 
     return cast(np.ndarray, out)
 
 
-@doc_inherit(diverg_kl_cont, style="numpy_with_merge")
-@docfiller_shared
+@docfiller(diverg_kl_cont, summary="Continuous Jensen–Shannon divergence")
 def diverg_js_cont(
     p: Callable,
     q: Callable,
     segments: ArrayLike,
     segments_q: ArrayLike | None = None,
     volume: str | Callable | None = None,
     err: bool = False,
     full_output: bool = False,
     **kws,
 ):
-    """
-    Continuous Jensen–Shannon divergence
-
-
-    Returns
-    -------
-    result : float or ndarray
-        value of JS divergence
-
-    References
-    ----------
-    {js_link}
-    """
-
     volume = _check_volume_func(volume)
 
     if segments_q is not None:
         segments = combine_segmets(segments, segments_q)
 
     def func(x):
         return diverg_js_integrand(p(x), q(x), volume(x))
@@ -375,15 +353,15 @@
         sum_errors=True,
         err=err,
         full_output=full_output,
         **kws,
     )
 
 
-@docfiller_shared
+@docfiller.decorate
 class Measures:
     """
     Convenience class for calculating measures
 
     Parameters
     ----------
     {phi}
@@ -400,17 +378,17 @@
     ) -> None:
         self.phi = phi
         self.segments = segments
         if quad_kws is None:
             quad_kws = {}
         self.quad_kws = quad_kws
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
-    @docfiller_shared
+    @docfiller.decorate
     def secondvirial(self, beta, err=False, full_output=False, **kws):
         """
         Calculate second virial coefficient.
 
         Parameters
         ----------
         {beta}
@@ -436,17 +414,17 @@
             beta=beta,
             segments=self.segments,
             err=err,
             full_output=full_output,
             **kws,
         )
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
-    @docfiller_shared
+    @docfiller.decorate
     def secondvirial_dbeta(self, beta, err=False, full_output=False, **kws):
         """
         Calculate ``beta`` derivative of second virial coefficient.
 
         Parameters
         ----------
         {beta}
@@ -470,15 +448,15 @@
             beta=beta,
             segments=self.segments,
             err=err,
             full_output=full_output,
             **kws,
         )
 
-    @docfiller_shared
+    @docfiller.decorate
     @add_quad_kws
     def boltz_diverg_js(
         self,
         other,
         beta: float,
         beta_other: float | None = None,
         volume: str | Callable = "3d",
```

### Comparing `analphipy-0.1.0/src/analphipy/norofrenkel.py` & `analphipy-0.2.0/src/analphipy/norofrenkel.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,55 +14,61 @@
 
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
 import numpy as np
-from custom_inherit import doc_inherit
+from module_utilities import cached
 
-from ._docstrings import DOCFILLER_SHARED, docfiller_shared  # type: ignore
-from .cached_decorators import gcached
+from ._docstrings import DOCFILLER_SHARED, docfiller_shared
 from .measures import secondvirial, secondvirial_dbeta, secondvirial_sw
 from .utils import TWO_PI, add_quad_kws, minimize_phi, quad_segments
 
 if TYPE_CHECKING:
     from ._typing import ArrayLike, Float_or_Array, Float_or_ArrayLike, Phi_Signature
     from .base_potential import PhiBase  # type: ignore
 # Hack to document module level docstring
-__doc__ = __doc__.format(**DOCFILLER_SHARED.data)
+__doc__ = __doc__.format(**DOCFILLER_SHARED.data)  # pyright: ignore
 
 __all__ = [
     "sig_nf",
     "sig_nf_dbeta",
     "lam_nf",
     "lam_nf_dbeta",
     "NoroFrenkelPair",
 ]
 
+d = DOCFILLER_SHARED.update(
+    summary="Noro-Frenkel/Barker-Henderson effective hard sphere diameter.",
+    extended_summary=r"""
+    This is calculated using the formula [1]_ [2]_
 
-@docfiller_shared
+    .. math::
+
+        \sigma_{{\rm BH}}(\beta) = \int_0^{{\infty}} dr \left( 1 - \exp[-\beta \phi_{{\rm rep}}(r)]\right)
+
+    where :math:`\phi_{{\rm rep}}(r)` is the repulsive part of the potential [3]_.
+    """,
+).dedent()
+
+
+@d.decorate
 def sig_nf(
     phi_rep: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
     **kws,
 ):
     r"""
-    Noro-Frenkel/Barker-Henderson effective hard sphere diameter.
-
-    This is calculated using the formula [1]_ [2]_
-
-    .. math::
-
-        \sigma_{{\rm BH}}(\beta) = \int_0^{{\infty}} dr \left( 1 - \exp[-\beta \phi_{{\rm rep}}(r)]\right)
+    {summary}
 
-    where :math:`\phi_{{\rm rep}}(r)` is the repulsive part of the potential [3]_.
+    {extended_summary}
 
     Parameters
     ----------
     {phi_rep}
     {beta}
     {segments}
     phi_rep : callable
@@ -103,39 +109,36 @@
         sum_errors=True,
         err=err,
         full_output=full_output,
         **kws,
     )
 
 
-@doc_inherit(sig_nf, style="numpy_with_merge")
+d = DOCFILLER_SHARED.update(
+    summary="Derivative with respect to inverse temperature ``beta`` of ``sig_nf``.",
+    extended_summary=r"""
+    See refs [1]_ [2]_ [3]_
+
+    .. math::
+
+        \frac{d \sigma_{\rm BH}}{d\beta} = \int_0^{\infty} dr \phi_{\rm rep}(r) \exp[-\beta \phi_{\rm rep}(r)]
+    """,
+).dedent()
+
+
+# @doc_inherit(sig_nf, style="numpy_with_merge")
+@d(sig_nf)
 def sig_nf_dbeta(
     phi_rep: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
     **kws,
 ):
-    r"""
-    Derivative with respect to inverse temperature ``beta`` of ``sig_nf``.
-
-
-    See refs [1]_ [2]_ [3]_
-
-    .. math::
-
-        \frac{d \sigma_{\rm BH}}{d\beta} = \int_0^{\infty} dr \phi_{\rm rep}(r) \exp[-\beta \phi_{\rm rep}(r)]
-
-    See Also
-    --------
-    sig_nf
-
-    """
-
     def integrand(r):
         v = phi_rep(r)
         if np.isinf(v):
             return 0.0
         else:
             return v * np.exp(-beta * v)
 
@@ -416,52 +419,57 @@
                 segments=phi.segments,
                 r_min=r_min,
                 bounds=bounds,
                 quad_kws=quad_kws,
                 **kws,
             )
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def secondvirial(self, beta: float, **kws):
         """
         Second virial coefficient.
 
         See Also
         --------
         ~analphipy.measures.secondvirial
         """
         return secondvirial(phi=self.phi, beta=beta, segments=self.segments, **kws)
 
-    @gcached()
-    def _segments_rep(self) -> list:
+    @cached.prop
+    def _segments_rep(self) -> list[float]:
         return [x for x in self.segments if x < self.r_min] + [self.r_min]
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def sig(self, beta: float, **kws):
         """
         Effective hard sphere diameter.
 
         See Also
         --------
         ~analphipy.norofrenkel.sig_nf
 
         """
-        return sig_nf(self.phi_rep, beta=beta, segments=self._segments_rep, **kws)
+        return sig_nf(
+            self.phi_rep,
+            beta=beta,
+            segments=self._segments_rep,  # pyright: ignore
+            **kws,
+        )
 
-    def eps(self, beta: float, **kws) -> float:
+    def eps(self, beta: float, **kws) -> float:  # pyright: ignore
         """
         Effective square well epsilon.
 
         This is equal to the minimum in ``phi``.
         """
         return cast(float, self.phi_min)
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def lam(self, beta: float, **kws):
         """
         Effective square well lambda.
 
         See Also
         --------
@@ -470,51 +478,51 @@
         return lam_nf(
             beta=beta,
             sig=self.sig(beta, **kws),
             eps=self.eps(beta, **kws),
             B2=self.secondvirial(beta, **kws),
         )
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def sw_dict(self, beta: float, **kws) -> dict[str, float]:
         """Dictionary view of Noro-Frenkel parameters."""
         sig = self.sig(beta, **kws)
         eps = self.eps(beta, **kws)
         lam = lam_nf(beta=beta, sig=sig, eps=eps, B2=self.secondvirial(beta, **kws))
         return {"sig": sig, "eps": eps, "lam": lam}
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def secondvirial_dbeta(self, beta: float, **kws):
         """
         Derivative of ``secondvirial`` with respect to ``beta``
 
         See Also
         --------
         ~analphipy.measures.secondvirial_dbeta
         """
         return secondvirial_dbeta(
             phi=self.phi, beta=beta, segments=self.segments, **kws
         )
 
-    @gcached(prop=False)
+    @cached.meth
     @add_quad_kws
     def sig_dbeta(self, beta: float, **kws):
         """
         Derivative of effective hard-sphere diameter with respect to ``beta``
 
         See Also
         --------
         ~analphipy.norofrenkel.sig_nf_dbeta
 
         """
         return sig_nf_dbeta(self.phi_rep, beta=beta, segments=self.segments, **kws)
 
-    @gcached(prop=False)
+    @cached.meth
     def lam_dbeta(self, beta: float, **kws):
         """
         Derivative of effective lambda parameter with respect to ``beta``.
 
         See Also
         --------
         ~analphipy.norofrenkel.lam_nf_dbeta
@@ -525,15 +533,15 @@
             eps=self.eps(beta, **kws),
             lam=self.lam(beta, **kws),
             B2=self.secondvirial(beta, **kws),
             B2_dbeta=self.secondvirial_dbeta(beta, **kws),
             sig_dbeta=self.sig_dbeta(beta, **kws),
         )
 
-    @gcached(prop=False)
+    @cached.meth
     def secondvirial_sw(self, beta: float, **kws):
         """
         Second virial coefficient of effective square well fluid.
 
         For testing.  This should be the same of value from :meth:`secondvirial`
         """
         return secondvirial_sw(
```

### Comparing `analphipy-0.1.0/src/analphipy/potential.py` & `analphipy-0.2.0/src/analphipy/potential.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/src/analphipy/utils.py` & `analphipy-0.2.0/src/analphipy/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Utilities module (:mod:`analphipy.utils`)
 =========================================
 """
 
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Mapping
+from typing import TYPE_CHECKING, Any, Callable
 
 import numpy as np
 from scipy.integrate import quad
 from scipy.optimize import minimize
 
-from ._docstrings import docfiller_shared  # type: ignore
+from ._docstrings import docfiller_shared
 
 if TYPE_CHECKING:
-    from ._typing import ArrayLike, Float_or_ArrayLike
+    from ._typing import ArrayLike
 
 # from typing_extensions import Protocol
 
 # ArrayLike = Union[Sequence[float], NDArray[np.float_]]
 # Float_or_ArrayLike = Union[float, ArrayLike]
 # Float_or_Array = Union[float, NDArray[np.float_]]
 
@@ -216,214 +216,214 @@
 
 
 def segments_to_segments_cut(segments, rcut):
     """Update segments for 'cut' potential"""
     return [x for x in segments if x < rcut] + [rcut]
 
 
-def phi_to_phi_cut(
-    rcut: float,
-    phi: Callable,
-    dphidr: Callable | None = None,
-    meta: Mapping | None = None,
-):
-    r"""
-    Create callable ``phi`` and ``dphidr`` cut potentials.
+# def phi_to_phi_cut(
+#     rcut: float,
+#     phi: Callable,
+#     dphidr: Callable | None = None,
+#     meta: Mapping | None = None,
+# ):
+#     r"""
+#     Create callable ``phi`` and ``dphidr`` cut potentials.
 
-    Parameters
-    ----------
-    rcut : float
-        Position of cut.
-    phi : callable
-        input callable function.
-    dphidr : callable, optional
-    input callable for :math:`d\phi/dr`
+#     Parameters
+#     ----------
+#     rcut : float
+#         Position of cut.
+#     phi : callable
+#         input callable function.
+#     dphidr : callable, optional
+#     input callable for :math:`d\phi/dr`
 
-    Returns
-    -------
-    phi_cut : callable
-    dphidr_cut : callable or None
-        Note that ``dphidr_cut`` is always returned, even if it is None.
-    """
+#     Returns
+#     -------
+#     phi_cut : callable
+#     dphidr_cut : callable or None
+#         Note that ``dphidr_cut`` is always returned, even if it is None.
+#     """
 
-    vcut = phi(rcut)
+#     vcut = phi(rcut)
 
-    def phi_cut(r):
-        r = np.asarray(r)
-        v = np.empty_like(r)
+#     def phi_cut(r):
+#         r = np.asarray(r)
+#         v = np.empty_like(r)
 
-        left = r <= rcut
-        right = ~left
+#         left = r <= rcut
+#         right = ~left
 
-        v[right] = 0.0
+#         v[right] = 0.0
 
-        if np.any(left):
-            v[left] = phi(r[left]) - vcut
-        return v
+#         if np.any(left):
+#             v[left] = phi(r[left]) - vcut
+#         return v
 
-    if dphidr:
+#     if dphidr:
 
-        def dphidr_cut(r):
-            r = np.asarray(r)
-            dvdbeta = np.empty_like(r)
+#         def dphidr_cut(r):
+#             r = np.asarray(r)
+#             dvdbeta = np.empty_like(r)
 
-            left = r <= rcut
-            right = ~left
+#             left = r <= rcut
+#             right = ~left
 
-            dvdbeta[right] = 0
+#             dvdbeta[right] = 0
 
-            if np.any(left):
-                dvdbeta[left] = dphidr(r[left])
+#             if np.any(left):
+#                 dvdbeta[left] = dphidr(r[left])
 
-            return dvdbeta
+#             return dvdbeta
 
-    else:
-        dphidr_cut = None  # type: ignore
+#     else:
+#         dphidr_cut = None
 
-    if meta is not None:
-        meta = dict(meta, rcut=rcut)
-        meta["style"] = meta.get("style", ()) + ("cut",)
+#     if meta is not None:
+#         meta = dict(meta, rcut=rcut)
+#         meta["style"] = meta.get("style", ()) + ("cut",)
 
-    return phi_cut, dphidr_cut, meta
+#     return phi_cut, dphidr_cut, meta
 
 
-def phi_to_phi_lfs(
-    rcut: float,
-    phi: Callable,
-    dphidr: Callable,
-    meta: Mapping | None = None,
-):
-    r"""
-    Create callable ``phi`` and ``dphidr`` cut potentials.
+# def phi_to_phi_lfs(
+#     rcut: float,
+#     phi: Callable,
+#     dphidr: Callable,
+#     meta: Mapping | None = None,
+# ):
+#     r"""
+#     Create callable ``phi`` and ``dphidr`` cut potentials.
 
-    Parameters
-    ----------
-    rcut : float
-        Position of cut.
-    phi : callable
-        input callable function.
-    dphidr : callable, optional
-    input callable for :math:`d\phi/dr`
+#     Parameters
+#     ----------
+#     rcut : float
+#         Position of cut.
+#     phi : callable
+#         input callable function.
+#     dphidr : callable, optional
+#     input callable for :math:`d\phi/dr`
 
-    Returns
-    -------
-    phi_cut : callable
-    dphidr_cut : callable or None
-        Note that ``dphidr_cut`` is always returned, even if it is None.
-    """
+#     Returns
+#     -------
+#     phi_cut : callable
+#     dphidr_cut : callable or None
+#         Note that ``dphidr_cut`` is always returned, even if it is None.
+#     """
 
-    vcut = phi(rcut)
-    dvdrcut = dphidr(rcut)
+#     vcut = phi(rcut)
+#     dvdrcut = dphidr(rcut)
 
-    def phi_cut(r):
-        r = np.asarray(r)
-        v = np.empty_like(r)
+#     def phi_cut(r):
+#         r = np.asarray(r)
+#         v = np.empty_like(r)
 
-        left = r <= rcut
-        right = ~left
+#         left = r <= rcut
+#         right = ~left
 
-        v[right] = 0.0
+#         v[right] = 0.0
 
-        if np.any(left):
-            v[left] = phi(r[left]) - vcut - dvdrcut * (r - rcut)
-        return v
+#         if np.any(left):
+#             v[left] = phi(r[left]) - vcut - dvdrcut * (r - rcut)
+#         return v
 
-    def dphidr_cut(r):
-        r = np.asarray(r)
-        dvdbeta = np.empty_like(r)
+#     def dphidr_cut(r):
+#         r = np.asarray(r)
+#         dvdbeta = np.empty_like(r)
 
-        left = r <= rcut
-        right = ~left
+#         left = r <= rcut
+#         right = ~left
 
-        dvdbeta[right] = 0
+#         dvdbeta[right] = 0
 
-        if np.any(left):
-            dvdbeta[left] = dphidr(r[left]) - dvdrcut
+#         if np.any(left):
+#             dvdbeta[left] = dphidr(r[left]) - dvdrcut
 
-        return dvdbeta
+#         return dvdbeta
 
-    if meta is not None:
-        meta = dict(meta, rcut=rcut)
-        meta["style"] = meta.get("style", ()) + ("lfs",)
+#     if meta is not None:
+#         meta = dict(meta, rcut=rcut)
+#         meta["style"] = meta.get("style", ()) + ("lfs",)
 
-    return phi_cut, dphidr_cut, meta
+#     return phi_cut, dphidr_cut, meta
 
 
-def wca_decomp_rep(phi, dphidr, r_min, phi_min, meta):
-    def phi_rep(r: Float_or_ArrayLike) -> np.ndarray:
-        """WCA repulsive potential"""
-        r = np.array(r)
-        v = np.empty_like(r)
+# def wca_decomp_rep(phi, dphidr, r_min, phi_min, meta):
+#     def phi_rep(r: Float_or_ArrayLike) -> np.ndarray:
+#         """WCA repulsive potential"""
+#         r = np.array(r)
+#         v = np.empty_like(r)
 
-        left = r <= r_min
-        right = ~left
+#         left = r <= r_min
+#         right = ~left
 
-        v[left] = phi(r[left]) - phi_min
-        v[right] = 0.0
-        return v
+#         v[left] = phi(r[left]) - phi_min
+#         v[right] = 0.0
+#         return v
 
-    if dphidr is not None:
+#     if dphidr is not None:
 
-        def dphidr_rep(r: Float_or_ArrayLike) -> np.ndarray:
-            r = np.array(r)
-            dvdr = np.empty_like(r)
+#         def dphidr_rep(r: Float_or_ArrayLike) -> np.ndarray:
+#             r = np.array(r)
+#             dvdr = np.empty_like(r)
 
-            left = r <= r_min
-            right = ~left
+#             left = r <= r_min
+#             right = ~left
 
-            dvdr[left] = dphidr(r[left])
-            dvdr[right] = 0.0
+#             dvdr[left] = dphidr(r[left])
+#             dvdr[right] = 0.0
 
-            return dvdr
+#             return dvdr
 
-    else:
-        dphidr_rep = None
+#     else:
+#         dphidr_rep = None
 
-    if meta is not None:
-        meta = dict(meta)
-        meta["style"] = meta.get("style", ()) + ("wca_rep",)
+#     if meta is not None:
+#         meta = dict(meta)
+#         meta["style"] = meta.get("style", ()) + ("wca_rep",)
 
-    return phi_rep, dphidr_rep, meta
+#     return phi_rep, dphidr_rep, meta
 
 
-def wca_decomp_att(phi, dphidr, r_min, phi_min, meta):
-    def phi_att(r: Float_or_ArrayLike) -> np.ndarray:
-        """WCA repulsive potential"""
-        r = np.array(r)
-        v = np.empty_like(r)
+# def wca_decomp_att(phi, dphidr, r_min, phi_min, meta):
+#     def phi_att(r: Float_or_ArrayLike) -> np.ndarray:
+#         """WCA repulsive potential"""
+#         r = np.array(r)
+#         v = np.empty_like(r)
 
-        left = r <= r_min
-        right = ~left
+#         left = r <= r_min
+#         right = ~left
 
-        v[left] = phi_min
-        v[right] = phi(r[right])
-        return v
+#         v[left] = phi_min
+#         v[right] = phi(r[right])
+#         return v
 
-    if dphidr is not None:
+#     if dphidr is not None:
 
-        def dphidr_att(r: Float_or_ArrayLike) -> np.ndarray:
-            r = np.array(r)
-            dvdr = np.empty_like(r)
+#         def dphidr_att(r: Float_or_ArrayLike) -> np.ndarray:
+#             r = np.array(r)
+#             dvdr = np.empty_like(r)
 
-            left = r <= r_min
-            right = ~left
+#             left = r <= r_min
+#             right = ~left
 
-            dvdr[left] = 0.0
-            dvdr[right] = dphidr(r[right])
+#             dvdr[left] = 0.0
+#             dvdr[right] = dphidr(r[right])
 
-            return dvdr
+#             return dvdr
 
-    else:
-        dphidr_att = None
+#     else:
+#         dphidr_att = None
 
-    if meta is not None:
-        meta = dict(meta)
-        meta["style"] = meta.get("style", ()) + ("wca_att",)
+#     if meta is not None:
+#         meta = dict(meta)
+#         meta["style"] = meta.get("style", ()) + ("wca_att",)
 
-    return phi_att, dphidr_att, meta
+#     return phi_att, dphidr_att, meta
 
 
 def add_quad_kws(func: Callable) -> Callable:
     @wraps(func)
     def wrapped(self, *args, **kws):
         kws = dict(self.quad_kws, **kws)
         return func(self, *args, **kws)
```

### Comparing `analphipy-0.1.0/src/analphipy.egg-info/PKG-INFO` & `analphipy-0.2.0/src/analphipy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: analphipy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities to perform stat mech analysis of pair potentials
-Home-page: https://github.com/usnistgov/analphipy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/analphipy
 Project-URL: documentation, https://pages.nist.gov/analphipy/
 Keywords: analphipy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -134,14 +133,26 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/analphipy)
 
 <!-- scriv-insert-here -->
 
+## v0.2.0 — 2023-05-04
+
+### Removed
+
+- Removed `cached_decorator` module.
+- Removed `docfiller` module.
+
+### Added
+
+- Now use [module-utilities](https://pypi.org/project/module-utilities/) to
+  handle caching and docfilling.
+
 ## v0.1.0 — 2023-04-24
 
 ### Changed
 
 - Update package layout
 - New linters via pre-commit
 - Development env now handled by tox
```

### Comparing `analphipy-0.1.0/src/analphipy.egg-info/SOURCES.txt` & `analphipy-0.2.0/src/analphipy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
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
@@ -47,15 +46,14 @@
 docs/_templates/autodocsumm/module-inherit.rst
 docs/_templates/autodocsumm/module-noindex.rst
 docs/_templates/autodocsumm/module.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/_templates/test/class-1.rst
-docs/examples/create-symlinks.sh
 docs/examples/index.md
 docs/examples/usage/usage.ipynb
 docs/reference/index.rst
 environment/dev-extras.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
@@ -64,35 +62,37 @@
 environment/lint-extras.yaml
 environment/lint.yaml
 environment/test-extras.yaml
 environment/test.yaml
 environment/tools.yaml
 examples/README.md
 examples/usage/usage.ipynb
+scripts/dist-conda.mk
+scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
+scripts/lint.mk
+scripts/recipe-append.sh
+scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/analphipy/__init__.py
 src/analphipy/_attrs_utils.py
 src/analphipy/_docstrings.py
 src/analphipy/_typing.py
 src/analphipy/base_potential.py
-src/analphipy/cached_decorators.py
 src/analphipy/measures.py
 src/analphipy/norofrenkel.py
 src/analphipy/potential.py
 src/analphipy/py.typed
 src/analphipy/utils.py
 src/analphipy.egg-info/PKG-INFO
 src/analphipy.egg-info/SOURCES.txt
 src/analphipy.egg-info/dependency_links.txt
-src/analphipy.egg-info/not-zip-safe
 src/analphipy.egg-info/requires.txt
 src/analphipy.egg-info/top_level.txt
-src/analphipy/_docfiller/__init__.py
-src/analphipy/_docfiller/docscrape.py
+src/analphipy.egg-info/zip-safe
 tests/__init__.py
 tests/conftest.py
 tests/test_generic.py
 tests/test_js.py
 tests/test_nf_derivs.py
 tests/test_norofrenkel.py
 tests/test_potentials.py
```

### Comparing `analphipy-0.1.0/tests/conftest.py` & `analphipy-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/crit_eff_lj_.csv` & `analphipy-0.2.0/tests/data/crit_eff_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/crit_eff_lj_nm_.csv` & `analphipy-0.2.0/tests/data/crit_eff_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/crit_eff_sw_.csv` & `analphipy-0.2.0/tests/data/crit_eff_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/crit_eff_yukawa_.csv` & `analphipy-0.2.0/tests/data/crit_eff_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/eff_lj_.csv` & `analphipy-0.2.0/tests/data/eff_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/eff_lj_nm_.csv` & `analphipy-0.2.0/tests/data/eff_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/eff_stockmayer_.csv` & `analphipy-0.2.0/tests/data/eff_stockmayer_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/eff_sw_.csv` & `analphipy-0.2.0/tests/data/eff_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/eff_yukawa_.csv` & `analphipy-0.2.0/tests/data/eff_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_hs_.csv` & `analphipy-0.2.0/tests/data/vir_hs_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_lj_.csv` & `analphipy-0.2.0/tests/data/vir_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_lj_nm_.csv` & `analphipy-0.2.0/tests/data/vir_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_stockmayer_.csv` & `analphipy-0.2.0/tests/data/vir_stockmayer_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_sw_.csv` & `analphipy-0.2.0/tests/data/vir_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/data/vir_yukawa_.csv` & `analphipy-0.2.0/tests/data/vir_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_generic.py` & `analphipy-0.2.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_js.py` & `analphipy-0.2.0/tests/test_js.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_nf_derivs.py` & `analphipy-0.2.0/tests/test_nf_derivs.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_norofrenkel.py` & `analphipy-0.2.0/tests/test_norofrenkel.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_potentials.py` & `analphipy-0.2.0/tests/test_potentials.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.1.0/tests/test_secondvirial.py` & `analphipy-0.2.0/tests/test_secondvirial.py`

 * *Files identical despite different names*

