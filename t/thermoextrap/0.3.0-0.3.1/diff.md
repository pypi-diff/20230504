# Comparing `tmp/thermoextrap-0.3.0.tar.gz` & `tmp/thermoextrap-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoextrap-0.3.0.tar", last modified: Wed May  3 20:15:44 2023, max compression
+gzip compressed data, was "thermoextrap-0.3.1.tar", last modified: Thu May  4 19:38:10 2023, max compression
```

## Comparing `thermoextrap-0.3.0.tar` & `thermoextrap-0.3.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.728277 thermoextrap-0.3.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1480 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.editorconfig
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      104 2023-04-11 02:16:02.000000 thermoextrap-0.3.0/.gitmodules
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      163 2023-04-24 16:24:54.000000 thermoextrap-0.3.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1386 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9227 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-10 21:01:10.000000 thermoextrap-0.3.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11351 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9570 2023-05-03 20:15:44.728674 thermoextrap-0.3.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5362 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.692236 thermoextrap-0.3.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.692571 thermoextrap-0.3.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.693235 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.697698 thermoextrap-0.3.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       11 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/environment/conda-spec.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      985 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      423 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      638 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      337 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       36 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      328 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      369 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6719 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.700635 thermoextrap-0.3.0/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      399 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      293 2023-05-03 20:15:44.730206 thermoextrap-0.3.0/setup.cfg
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/setup.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.684145 thermoextrap-0.3.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.706335 thermoextrap-0.3.0/src/thermoextrap/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1583 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18791 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/adaptive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    17295 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/beta.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.709989 thermoextrap-0.3.0/src/thermoextrap/core/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/core/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4998 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/_attrs_utils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12082 2023-04-11 02:16:02.000000 thermoextrap-0.3.0/src/thermoextrap/core/_deprecate.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      322 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/sputils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3159 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/xrutils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    52780 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3513 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/docstrings.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.711784 thermoextrap-0.3.0/src/thermoextrap/gpr_active/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      717 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    89013 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/active_utils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    56361 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/gp_models.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3377 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/ig_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3003 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/sine_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10310 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/idealgas.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.718196 thermoextrap-0.3.0/src/thermoextrap/legacy/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      629 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9563 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/extrap.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18311 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/gpr.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16775 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/gpr_stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5547 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/ig.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16626 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9580 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/old_scripts.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21063 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/recursive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8609 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/reweight.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10983 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/utilities.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12877 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/lnpi.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32051 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/models.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21933 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/recursive_interp.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18752 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5827 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/volume.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4387 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/volume_idealgas.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.708269 thermoextrap-0.3.0/src/thermoextrap.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9570 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2466 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-10 21:05:09.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      360 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       13 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.726147 thermoextrap-0.3.0/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9072 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.726702 thermoextrap-0.3.0/tests/lnpi_data/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   794879 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/lnpi_data/sample_data.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23103 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_GPs.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    25332 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_active.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32495 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_beta.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2259 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1421 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_idealgas.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3437 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2094 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/test_stack.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7641 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_u_data.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2046 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/test_u_equations.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2703 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_volume.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3981 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.874773 thermoextrap-0.3.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1491 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.editorconfig
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      104 2023-04-11 02:16:02.000000 thermoextrap-0.3.1/.gitmodules
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      371 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      163 2023-04-24 16:24:54.000000 thermoextrap-0.3.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1386 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9712 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-10 21:01:10.000000 thermoextrap-0.3.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11351 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9470 2023-05-04 19:38:10.873805 thermoextrap-0.3.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5362 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.769447 thermoextrap-0.3.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.770453 thermoextrap-0.3.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.772243 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.799553 thermoextrap-0.3.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       11 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/environment/conda-spec.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      985 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      423 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      638 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      337 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       36 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      328 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      369 2023-05-03 20:14:50.000000 thermoextrap-0.3.1/environment.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6622 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.805756 thermoextrap-0.3.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      843 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:38:10.874984 thermoextrap-0.3.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.756856 thermoextrap-0.3.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.815184 thermoextrap-0.3.1/src/thermoextrap/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1583 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18791 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/adaptive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    17295 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/beta.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.842126 thermoextrap-0.3.1/src/thermoextrap/core/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/core/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4998 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/_attrs_utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12082 2023-04-11 02:16:02.000000 thermoextrap-0.3.1/src/thermoextrap/core/_deprecate.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      322 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/sputils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3159 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/core/xrutils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    52780 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3513 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/docstrings.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.846590 thermoextrap-0.3.1/src/thermoextrap/gpr_active/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      717 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    89013 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/active_utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    56361 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/gp_models.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3377 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/ig_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3003 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/gpr_active/sine_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10310 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/idealgas.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.857939 thermoextrap-0.3.1/src/thermoextrap/legacy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      629 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9563 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/extrap.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18311 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/gpr.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16775 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/gpr_stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5547 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/ig.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16626 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9580 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/old_scripts.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21063 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/recursive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8609 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/reweight.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10983 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/src/thermoextrap/legacy/utilities.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12877 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/lnpi.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32051 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/models.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21933 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/recursive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18752 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5827 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/volume.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4387 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/src/thermoextrap/volume_idealgas.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.837724 thermoextrap-0.3.1/src/thermoextrap.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9470 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2488 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      360 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       13 2023-05-04 19:38:10.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:38:09.000000 thermoextrap-0.3.1/src/thermoextrap.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.869899 thermoextrap-0.3.1/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9072 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:38:10.870737 thermoextrap-0.3.1/tests/lnpi_data/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   794879 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/lnpi_data/sample_data.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23103 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_GPs.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    25332 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32495 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_beta.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2259 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1421 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_idealgas.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3437 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2094 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/test_stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7641 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_u_data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2046 2023-05-03 20:14:51.000000 thermoextrap-0.3.1/tests/test_u_equations.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2703 2023-04-10 21:01:11.000000 thermoextrap-0.3.1/tests/test_volume.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4154 2023-05-04 19:37:23.000000 thermoextrap-0.3.1/tox.ini
```

### Comparing `thermoextrap-0.3.0/.cruft.json` & `thermoextrap-0.3.1/.cruft.json`

 * *Files 5% similar despite different names*

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

### Comparing `thermoextrap-0.3.0/.editorconfig` & `thermoextrap-0.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/.gitignore` & `thermoextrap-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/.pre-commit-config.yaml` & `thermoextrap-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/CHANGELOG.md` & `thermoextrap-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/CONTRIBUTING.md` & `thermoextrap-0.3.1/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -385,7 +385,18 @@
 
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

### Comparing `thermoextrap-0.3.0/LICENSE` & `thermoextrap-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/Makefile` & `thermoextrap-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/PKG-INFO` & `thermoextrap-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.3.0
+Version: 0.3.1
 Summary: Thermodynamic extrapolation
-Home-page: https://github.com/usnistgov/thermoextrap
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
-License: "NIST license https://www.nist.gov/director/licensing"
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/thermoextrap
 Project-URL: documentation, https://pages.nist.gov/thermoextrap/
 Keywords: thermoextrap
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `thermoextrap-0.3.0/README.md` & `thermoextrap-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/changelog.d/templates/auto-changelog/template.jinja2` & `thermoextrap-0.3.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/environment/dev-extras.yaml` & `thermoextrap-0.3.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/environment/docs-extras.yaml` & `thermoextrap-0.3.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/environment/docs.yaml` & `thermoextrap-0.3.1/environment/docs.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/pyproject.toml` & `thermoextrap-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "thermoextrap"
 authors = [
     { name = "Jacob Monroe", email = "jacob.monroe@nist.gov" },
     { name = "William Krekelberg", email = "wpk@nist.gov" }
 ]
-license = { text = '"NIST license https://www.nist.gov/director/licensing"' }
+license = { text = "NIST-PD" }
 description = "Thermodynamic extrapolation"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["thermoextrap"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -56,24 +56,24 @@
     "thermoextrap[parallel]",
     "thermoextrap[viz]",
 ]
 test = ["pytest"]
 
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

### Comparing `thermoextrap-0.3.0/scripts/docs-examples-symlinks.sh` & `thermoextrap-0.3.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/__init__.py` & `thermoextrap-0.3.1/src/thermoextrap/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/adaptive_interp.py` & `thermoextrap-0.3.1/src/thermoextrap/adaptive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/beta.py` & `thermoextrap-0.3.1/src/thermoextrap/beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/core/_attrs_utils.py` & `thermoextrap-0.3.1/src/thermoextrap/core/_attrs_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/core/_deprecate.py` & `thermoextrap-0.3.1/src/thermoextrap/core/_deprecate.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/core/xrutils.py` & `thermoextrap-0.3.1/src/thermoextrap/core/xrutils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/data.py` & `thermoextrap-0.3.1/src/thermoextrap/data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/docstrings.py` & `thermoextrap-0.3.1/src/thermoextrap/docstrings.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/gpr_active/__init__.py` & `thermoextrap-0.3.1/src/thermoextrap/gpr_active/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/gpr_active/active_utils.py` & `thermoextrap-0.3.1/src/thermoextrap/gpr_active/active_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/gpr_active/gp_models.py` & `thermoextrap-0.3.1/src/thermoextrap/gpr_active/gp_models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/gpr_active/ig_active.py` & `thermoextrap-0.3.1/src/thermoextrap/gpr_active/ig_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/gpr_active/sine_active.py` & `thermoextrap-0.3.1/src/thermoextrap/gpr_active/sine_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/idealgas.py` & `thermoextrap-0.3.1/src/thermoextrap/idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/__init__.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/extrap.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/extrap.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/gpr.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/gpr.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/gpr_stack.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/gpr_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/ig.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/ig.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/interp.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/old_scripts.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/old_scripts.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/recursive_interp.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/reweight.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/reweight.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/legacy/utilities.py` & `thermoextrap-0.3.1/src/thermoextrap/legacy/utilities.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/lnpi.py` & `thermoextrap-0.3.1/src/thermoextrap/lnpi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/models.py` & `thermoextrap-0.3.1/src/thermoextrap/models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/recursive_interp.py` & `thermoextrap-0.3.1/src/thermoextrap/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/stack.py` & `thermoextrap-0.3.1/src/thermoextrap/stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/volume.py` & `thermoextrap-0.3.1/src/thermoextrap/volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap/volume_idealgas.py` & `thermoextrap-0.3.1/src/thermoextrap/volume_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/src/thermoextrap.egg-info/PKG-INFO` & `thermoextrap-0.3.1/src/thermoextrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.3.0
+Version: 0.3.1
 Summary: Thermodynamic extrapolation
-Home-page: https://github.com/usnistgov/thermoextrap
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
-License: "NIST license https://www.nist.gov/director/licensing"
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/thermoextrap
 Project-URL: documentation, https://pages.nist.gov/thermoextrap/
 Keywords: thermoextrap
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `thermoextrap-0.3.0/src/thermoextrap.egg-info/SOURCES.txt` & `thermoextrap-0.3.1/src/thermoextrap.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 .cruft.json
 .editorconfig
 .gitignore
 .gitmodules
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
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 environment/conda-spec.txt
 environment/dev-extras.yaml
@@ -33,14 +32,15 @@
 environment/test-extras.yaml
 environment/test.yaml
 environment/tools.yaml
 scripts/dist-conda.mk
 scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
 scripts/lint.mk
+scripts/recipe-append.sh
 scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/thermoextrap/__init__.py
 src/thermoextrap/adaptive_interp.py
 src/thermoextrap/beta.py
 src/thermoextrap/data.py
 src/thermoextrap/docstrings.py
@@ -50,17 +50,17 @@
 src/thermoextrap/recursive_interp.py
 src/thermoextrap/stack.py
 src/thermoextrap/volume.py
 src/thermoextrap/volume_idealgas.py
 src/thermoextrap.egg-info/PKG-INFO
 src/thermoextrap.egg-info/SOURCES.txt
 src/thermoextrap.egg-info/dependency_links.txt
-src/thermoextrap.egg-info/not-zip-safe
 src/thermoextrap.egg-info/requires.txt
 src/thermoextrap.egg-info/top_level.txt
+src/thermoextrap.egg-info/zip-safe
 src/thermoextrap/core/__init__.py
 src/thermoextrap/core/_attrs_utils.py
 src/thermoextrap/core/_deprecate.py
 src/thermoextrap/core/sputils.py
 src/thermoextrap/core/xrutils.py
 src/thermoextrap/gpr_active/__init__.py
 src/thermoextrap/gpr_active/active_utils.py
```

### Comparing `thermoextrap-0.3.0/tests/conftest.py` & `thermoextrap-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/lnpi_data/sample_data.json` & `thermoextrap-0.3.1/tests/lnpi_data/sample_data.json`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_GPs.py` & `thermoextrap-0.3.1/tests/test_GPs.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_active.py` & `thermoextrap-0.3.1/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_beta.py` & `thermoextrap-0.3.1/tests/test_beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_data.py` & `thermoextrap-0.3.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_idealgas.py` & `thermoextrap-0.3.1/tests/test_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_lnPi.py` & `thermoextrap-0.3.1/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_stack.py` & `thermoextrap-0.3.1/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_u_data.py` & `thermoextrap-0.3.1/tests/test_u_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_u_equations.py` & `thermoextrap-0.3.1/tests/test_u_equations.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tests/test_volume.py` & `thermoextrap-0.3.1/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.3.0/tox.ini` & `thermoextrap-0.3.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,28 @@
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
@@ -91,17 +98,17 @@
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

