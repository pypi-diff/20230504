# Comparing `tmp/tmmc-lnpy-0.3.0.tar.gz` & `tmp/tmmc-lnpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmmc-lnpy-0.3.0.tar", last modified: Wed May  3 03:05:36 2023, max compression
+gzip compressed data, was "tmmc-lnpy-0.3.1.tar", last modified: Thu May  4 19:23:43 2023, max compression
```

## Comparing `tmmc-lnpy-0.3.0.tar` & `tmmc-lnpy-0.3.1.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.321590 tmmc-lnpy-0.3.0/
--rw-r--r--   0 wpk      (42033)    36681     1478 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.editorconfig
--rw-r--r--   0 wpk      (42033)    36681     1324 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3681 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.3.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     1834 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9178 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11319 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     7758 2023-05-03 03:05:36.322018 tmmc-lnpy-0.3.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     3274 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.249916 tmmc-lnpy-0.3.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.250654 tmmc-lnpy-0.3.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.252360 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.266048 tmmc-lnpy-0.3.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      961 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      317 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     6157 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.272827 tmmc-lnpy-0.3.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      396 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681      290 2023-05-03 03:05:36.323648 tmmc-lnpy-0.3.0/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.0/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.236716 tmmc-lnpy-0.3.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.276264 tmmc-lnpy-0.3.0/src/lnPi/
--rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/collectionlnpiutils.py
--rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnPi/stability.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.291583 tmmc-lnpy-0.3.0/src/lnpy/
--rw-r--r--   0 wpk      (42033)    36681     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/bracket.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.297421 tmmc-lnpy-0.3.0/src/lnpy/data/
--rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.0/src/lnpy/data/hsmix_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/lj_sub_example.json
--rw-r--r--   0 wpk      (42033)    36681    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/lj_sup_example.json
--rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.0/src/lnpy/data/ljmix_sup_example.json.gz
--rw-r--r--   0 wpk      (42033)    36681    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/src/lnpy/data/watermof_example.json
--rw-r--r--   0 wpk      (42033)    36681     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/docstrings.py
--rw-r--r--   0 wpk      (42033)    36681    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/ensembles.py
--rw-r--r--   0 wpk      (42033)    36681     4997 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/examples.py
--rw-r--r--   0 wpk      (42033)    36681    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/extensions.py
--rw-r--r--   0 wpk      (42033)    36681    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpicollectionutils.py
--rw-r--r--   0 wpk      (42033)    36681    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpidata.py
--rw-r--r--   0 wpk      (42033)    36681    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpienergy.py
--rw-r--r--   0 wpk      (42033)    36681    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/lnpiseries.py
--rw-r--r--   0 wpk      (42033)    36681    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/maskedlnpi_legacy.py
--rw-r--r--   0 wpk      (42033)    36681     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/molfrac.py
--rw-r--r--   0 wpk      (42033)    36681     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/options.py
--rw-r--r--   0 wpk      (42033)    36681    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/segment.py
--rw-r--r--   0 wpk      (42033)    36681    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/src/lnpy/stability.py
--rw-r--r--   0 wpk      (42033)    36681    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.0/src/lnpy/utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.305162 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     7758 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2061 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-14 22:53:56.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033)    36681      112 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       10 2023-05-03 03:05:36.000000 tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.312001 tmmc-lnpy-0.3.0/tests/
--rw-r--r--   0 wpk      (42033)    36681     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_hs_mix.py
--rw-r--r--   0 wpk      (42033)    36681       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.3.0/tests/test_import.py
--rw-r--r--   0 wpk      (42033)    36681     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_lj_mix_0.py
--rw-r--r--   0 wpk      (42033)    36681     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033)    36681     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_single_comp_sub.py
--rw-r--r--   0 wpk      (42033)    36681     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tests/test_single_comp_super.py
--rw-r--r--   0 wpk      (42033)    36681     2801 2023-04-15 00:15:07.000000 tmmc-lnpy-0.3.0/tests/test_water_cluster.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-03 03:05:36.320558 tmmc-lnpy-0.3.0/tests/water_cluster/
--rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_0.csv
--rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_0_dw.csv
--rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_1.csv
--rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/data_1_dw.csv
--rw-r--r--   0 wpk      (42033)    36681      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_ensemble.json
--rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_example.csv
--rw-r--r--   0 wpk      (42033)    36681     3774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.829684 tmmc-lnpy-0.3.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1489 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.editorconfig
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      684 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.3.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1834 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9663 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11319 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7674 2023-05-04 19:23:43.829048 tmmc-lnpy-0.3.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3245 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.789692 tmmc-lnpy-0.3.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.790416 tmmc-lnpy-0.3.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.791513 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.797149 tmmc-lnpy-0.3.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      961 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      317 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6102 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.801244 tmmc-lnpy-0.3.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      840 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:23:43.829922 tmmc-lnpy-0.3.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.781344 tmmc-lnpy-0.3.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.802922 tmmc-lnpy-0.3.1/src/lnPi/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/collectionlnpiutils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/stability.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.810538 tmmc-lnpy-0.3.1/src/lnpy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/bracket.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.813876 tmmc-lnpy-0.3.1/src/lnpy/data/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.1/src/lnpy/data/hsmix_example.json.gz
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/lj_sub_example.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/lj_sup_example.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.1/src/lnpy/data/ljmix_sup_example.json.gz
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/watermof_example.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/docstrings.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/ensembles.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4997 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/examples.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/extensions.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpicollectionutils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpidata.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpienergy.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpiseries.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/maskedlnpi_legacy.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/molfrac.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/options.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/segment.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/stability.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/utils.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.817842 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7674 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2083 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      112 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       10 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:23:42.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.822594 tmmc-lnpy-0.3.1/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_hs_mix.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.3.1/tests/test_import.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_lj_mix_0.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_single_comp_sub.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_single_comp_super.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2801 2023-04-15 00:15:07.000000 tmmc-lnpy-0.3.1/tests/test_water_cluster.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.828035 tmmc-lnpy-0.3.1/tests/water_cluster/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_0.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_0_dw.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_1.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_1_dw.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_ensemble.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_example.csv
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3947 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/tox.ini
```

### Comparing `tmmc-lnpy-0.3.0/.cruft.json` & `tmmc-lnpy-0.3.1/.cruft.json`

 * *Files 10% similar despite different names*

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

### Comparing `tmmc-lnpy-0.3.0/.editorconfig` & `tmmc-lnpy-0.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/.gitignore` & `tmmc-lnpy-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/.pre-commit-config.yaml` & `tmmc-lnpy-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/CHANGELOG.md` & `tmmc-lnpy-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/CONTRIBUTING.md` & `tmmc-lnpy-0.3.1/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -384,7 +384,18 @@
 
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

### Comparing `tmmc-lnpy-0.3.0/LICENSE` & `tmmc-lnpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/Makefile` & `tmmc-lnpy-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/PKG-INFO` & `tmmc-lnpy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Analysis of lnPi results from TMMC simulation
-Home-page: https://github.com/usnistgov/tmmc-lnpy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -52,16 +51,14 @@
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
 <!-- other links -->
 
 # `tmmc-lnpy`
 
-A Python package for stuff.
-
 ## Overview
 
 A package to analyze $\ln \Pi(N)$ data from Transition Matrix Monte Carlo
 simulation. The main output from TMMC simulations, $\ln \Pi(N)$, provides a
 means to calculate a host of thermodynamic properties. Moreover, if $\ln \Pi(N)$
 is calculated at a specific chemical potential, it can be reweighted to provide
 thermodynamic information at a different chemical potential
```

### Comparing `tmmc-lnpy-0.3.0/README.md` & `tmmc-lnpy-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
 <!-- other links -->
 
 # `tmmc-lnpy`
 
-A Python package for stuff.
-
 ## Overview
 
 A package to analyze $\ln \Pi(N)$ data from Transition Matrix Monte Carlo
 simulation. The main output from TMMC simulations, $\ln \Pi(N)$, provides a
 means to calculate a host of thermodynamic properties. Moreover, if $\ln \Pi(N)$
 is calculated at a specific chemical potential, it can be reweighted to provide
 thermodynamic information at a different chemical potential
```

### Comparing `tmmc-lnpy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2` & `tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/environment/dev-extras.yaml` & `tmmc-lnpy-0.3.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/environment/docs-extras.yaml` & `tmmc-lnpy-0.3.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/environment/docs.yaml` & `tmmc-lnpy-0.3.1/environment/docs.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/pyproject.toml` & `tmmc-lnpy-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmmc-lnpy"
 authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
-license = { text = "NIST license" }
+license = { text = "NIST-PD" }
 description = "Analysis of lnPi results from TMMC simulation"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["tmmc-lnpy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -42,24 +42,24 @@
 documentation = "https://pages.nist.gov/tmmc-lnpy/"
 
 [project.optional-dependencies]
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

### Comparing `tmmc-lnpy-0.3.0/scripts/docs-examples-symlinks.sh` & `tmmc-lnpy-0.3.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnPi/__init__.py` & `tmmc-lnpy-0.3.1/src/lnPi/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/__init__.py` & `tmmc-lnpy-0.3.1/src/lnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/bracket.py` & `tmmc-lnpy-0.3.1/src/lnpy/bracket.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/data/hsmix_example.json.gz` & `tmmc-lnpy-0.3.1/src/lnpy/data/hsmix_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/data/lj_sub_example.json` & `tmmc-lnpy-0.3.1/src/lnpy/data/lj_sub_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/data/lj_sup_example.json` & `tmmc-lnpy-0.3.1/src/lnpy/data/lj_sup_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/data/ljmix_sup_example.json.gz` & `tmmc-lnpy-0.3.1/src/lnpy/data/ljmix_sup_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/data/watermof_example.json` & `tmmc-lnpy-0.3.1/src/lnpy/data/watermof_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/docstrings.py` & `tmmc-lnpy-0.3.1/src/lnpy/docstrings.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/ensembles.py` & `tmmc-lnpy-0.3.1/src/lnpy/ensembles.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/examples.py` & `tmmc-lnpy-0.3.1/src/lnpy/examples.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/extensions.py` & `tmmc-lnpy-0.3.1/src/lnpy/extensions.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/lnpicollectionutils.py` & `tmmc-lnpy-0.3.1/src/lnpy/lnpicollectionutils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/lnpidata.py` & `tmmc-lnpy-0.3.1/src/lnpy/lnpidata.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/lnpienergy.py` & `tmmc-lnpy-0.3.1/src/lnpy/lnpienergy.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/lnpiseries.py` & `tmmc-lnpy-0.3.1/src/lnpy/lnpiseries.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/maskedlnpi_legacy.py` & `tmmc-lnpy-0.3.1/src/lnpy/maskedlnpi_legacy.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/molfrac.py` & `tmmc-lnpy-0.3.1/src/lnpy/molfrac.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/options.py` & `tmmc-lnpy-0.3.1/src/lnpy/options.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/segment.py` & `tmmc-lnpy-0.3.1/src/lnpy/segment.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/stability.py` & `tmmc-lnpy-0.3.1/src/lnpy/stability.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/lnpy/utils.py` & `tmmc-lnpy-0.3.1/src/lnpy/utils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/PKG-INFO` & `tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Analysis of lnPi results from TMMC simulation
-Home-page: https://github.com/usnistgov/tmmc-lnpy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -52,16 +51,14 @@
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
 <!-- other links -->
 
 # `tmmc-lnpy`
 
-A Python package for stuff.
-
 ## Overview
 
 A package to analyze $\ln \Pi(N)$ data from Transition Matrix Monte Carlo
 simulation. The main output from TMMC simulations, $\ln \Pi(N)$, provides a
 means to calculate a host of thermodynamic properties. Moreover, if $\ln \Pi(N)$
 is calculated at a specific chemical potential, it can be reweighted to provide
 thermodynamic information at a different chemical potential
```

### Comparing `tmmc-lnpy-0.3.0/src/tmmc_lnpy.egg-info/SOURCES.txt` & `tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 environment/dev-extras.yaml
 environment/dev.yaml
@@ -31,14 +30,15 @@
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
 src/lnPi/__init__.py
 src/lnPi/collectionlnpiutils.py
 src/lnPi/stability.py
 src/lnpy/__init__.py
 src/lnpy/bracket.py
@@ -60,17 +60,17 @@
 src/lnpy/data/lj_sub_example.json
 src/lnpy/data/lj_sup_example.json
 src/lnpy/data/ljmix_sup_example.json.gz
 src/lnpy/data/watermof_example.json
 src/tmmc_lnpy.egg-info/PKG-INFO
 src/tmmc_lnpy.egg-info/SOURCES.txt
 src/tmmc_lnpy.egg-info/dependency_links.txt
-src/tmmc_lnpy.egg-info/not-zip-safe
 src/tmmc_lnpy.egg-info/requires.txt
 src/tmmc_lnpy.egg-info/top_level.txt
+src/tmmc_lnpy.egg-info/zip-safe
 tests/test_hs_mix.py
 tests/test_import.py
 tests/test_lj_mix_0.py
 tests/test_lnPi.py
 tests/test_single_comp_sub.py
 tests/test_single_comp_super.py
 tests/test_water_cluster.py
```

### Comparing `tmmc-lnpy-0.3.0/tests/test_hs_mix.py` & `tmmc-lnpy-0.3.1/tests/test_hs_mix.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/test_lj_mix_0.py` & `tmmc-lnpy-0.3.1/tests/test_lj_mix_0.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/test_lnPi.py` & `tmmc-lnpy-0.3.1/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/test_single_comp_sub.py` & `tmmc-lnpy-0.3.1/tests/test_single_comp_sub.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/test_single_comp_super.py` & `tmmc-lnpy-0.3.1/tests/test_single_comp_super.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/test_water_cluster.py` & `tmmc-lnpy-0.3.1/tests/test_water_cluster.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/water_cluster/data_0.csv` & `tmmc-lnpy-0.3.1/tests/water_cluster/data_0.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/water_cluster/data_1.csv` & `tmmc-lnpy-0.3.1/tests/water_cluster/data_1.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/water_cluster/data_1_dw.csv` & `tmmc-lnpy-0.3.1/tests/water_cluster/data_1_dw.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tests/water_cluster/water_MOF_example.csv` & `tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_example.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.0/tox.ini` & `tmmc-lnpy-0.3.1/tox.ini`

 * *Files 3% similar despite different names*

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
@@ -89,17 +96,17 @@
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

