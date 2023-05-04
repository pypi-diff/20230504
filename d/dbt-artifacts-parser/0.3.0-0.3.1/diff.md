# Comparing `tmp/dbt-artifacts-parser-0.3.0.tar.gz` & `tmp/dbt-artifacts-parser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-artifacts-parser-0.3.0.tar", last modified: Wed Apr 19 10:29:21 2023, max compression
+gzip compressed data, was "dbt-artifacts-parser-0.3.1.tar", last modified: Thu May  4 02:37:27 2023, max compression
```

## Comparing `dbt-artifacts-parser-0.3.0.tar` & `dbt-artifacts-parser-0.3.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0      804 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1824 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2319 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1158 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1896 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.gitignore
--rw-r--r--   0        0        0     1371 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14055 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pylintrc
--rw-r--r--   0        0        0      150 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.pypirc
--rw-r--r--   0        0        0       32 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/.style.yapf
--rw-r--r--   0        0        0    11357 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/LICENSE
--rw-r--r--   0        0        0      159 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/MANIFEST.in
--rw-r--r--   0        0        0      879 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/Makefile
--rw-r--r--   0        0        0     8681 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/README.md
--rw-r--r--   0        0        0      859 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    11501 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    40546 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47751 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48519 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52861 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35031 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0    39455 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     4274 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   135379 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138301 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157234 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159202 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163790 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   174833 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json
--rw-r--r--   0        0        0   115570 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0   129190 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json
--rw-r--r--   0        0        0     4622 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9816 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10271 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     5568 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6789 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7248 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/utils.py
--rwxr-xr-x   0        0        0     1121 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/clean.sh
--rwxr-xr-x   0        0        0     1021 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/format_python.sh
--rw-r--r--   0        0        0     3162 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/generate_parser_classes.sh
--rw-r--r--   0        0        0      978 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/dev/test_python.sh
--rw-r--r--   0        0        0     1545 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      830 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/setup.py
--rw-r--r--   0        0        0      792 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      796 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/parsers/__init__.py
--rw-r--r--   0        0        0     6001 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/parsers/test_utils.py
--rw-r--r--   0        0        0    11587 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/catalog.json
--rw-r--r--   0        0        0   226551 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/manifest.json
--rw-r--r--   0        0        0     4688 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   265840 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15168 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   289190 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15738 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   269797 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    14576 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   817922 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v5/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   352436 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v6/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   412717 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v7/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   394308 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   401315 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json
--rw-r--r--   0        0        0  1234064 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json
--rw-r--r--   0        0        0      938 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_basic.py
--rw-r--r--   0        0        0     6671 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_parser.py
--rw-r--r--   0        0        0     1090 2023-04-19 10:29:21.000000 dbt-artifacts-parser-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0    10459 1970-01-01 00:00:00.000000 dbt-artifacts-parser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1824 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2319 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1158 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1896 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1371 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14055 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pylintrc
+-rw-r--r--   0        0        0      150 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pypirc
+-rw-r--r--   0        0        0       32 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/LICENSE
+-rw-r--r--   0        0        0      159 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/MANIFEST.in
+-rw-r--r--   0        0        0      879 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/Makefile
+-rw-r--r--   0        0        0     8681 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/README.md
+-rw-r--r--   0        0        0      859 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    11513 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1887 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    39709 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    40546 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    41294 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    46633 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    47751 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    48519 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    52861 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    35031 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    39455 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1719 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1755 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3346 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3458 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2044 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2327 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2441 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     4274 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   135379 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138301 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157234 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159202 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163790 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9816 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10271 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     5568 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6789 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7248 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/utils.py
+-rwxr-xr-x   0        0        0     1121 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/clean.sh
+-rwxr-xr-x   0        0        0     1021 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/format_python.sh
+-rw-r--r--   0        0        0     3162 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/generate_parser_classes.sh
+-rw-r--r--   0        0        0      978 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1391 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/publish.sh
+-rwxr-xr-x   0        0        0     1023 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/test_python.sh
+-rw-r--r--   0        0        0     1545 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/setup.py
+-rw-r--r--   0        0        0      792 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     6001 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/parsers/test_utils.py
+-rw-r--r--   0        0        0    11587 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/catalog.json
+-rw-r--r--   0        0        0   226551 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0     4688 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   265840 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    15168 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   289190 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    15738 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   269797 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0    14576 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/run_results.json
+-rw-r--r--   0        0        0   817922 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v5/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   352436 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v6/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   412717 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v7/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   394308 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop/manifest.json
+-rw-r--r--   0        0        0   401315 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json
+-rw-r--r--   0        0        0  1234064 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json
+-rw-r--r--   0        0        0      938 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_basic.py
+-rw-r--r--   0        0        0     6671 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_parser.py
+-rw-r--r--   0        0        0     1090 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0    10459 1970-01-01 00:00:00.000000 dbt-artifacts-parser-0.3.1/PKG-INFO
```

### Comparing `dbt-artifacts-parser-0.3.0/.github/CODEOWNERS` & `dbt-artifacts-parser-0.3.1/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.github/workflows/publish.yml` & `dbt-artifacts-parser-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.github/workflows/test-publish.yml` & `dbt-artifacts-parser-0.3.1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.github/workflows/test.yml` & `dbt-artifacts-parser-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.gitignore` & `dbt-artifacts-parser-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.pre-commit-config.yaml` & `dbt-artifacts-parser-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/.pylintrc` & `dbt-artifacts-parser-0.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/LICENSE` & `dbt-artifacts-parser-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/Makefile` & `dbt-artifacts-parser-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/README.md` & `dbt-artifacts-parser-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parser.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 #
 # manifest
 #
 def parse_manifest(
     manifest: dict
 ) -> Union[ManifestV1, ManifestV2, ManifestV3, ManifestV4, ManifestV5,
-           ManifestV6, ManifestV7, ManifestV8]:
+           ManifestV6, ManifestV7, ManifestV8, ManifestV9]:
     """Parse manifest.json
 
     Args:
         manifest: A dict of manifest.json
 
     Returns:
        Union[ManifestV1, ManifestV2, ManifestV3, ManifestV4]
```

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/base.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/sources/sources_v3.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/utils.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/parsers/version_map.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/version_map.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dbt_artifacts_parser/utils.py` & `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/clean.sh` & `dbt-artifacts-parser-0.3.1/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/format_python.sh` & `dbt-artifacts-parser-0.3.1/dev/format_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/generate_parser_classes.sh` & `dbt-artifacts-parser-0.3.1/dev/generate_parser_classes.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/lint_python.sh` & `dbt-artifacts-parser-0.3.1/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/publish.sh` & `dbt-artifacts-parser-0.3.1/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/setup.sh` & `dbt-artifacts-parser-0.3.1/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/dev/test_python.sh` & `dbt-artifacts-parser-0.3.1/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/pyproject.toml` & `dbt-artifacts-parser-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/setup.py` & `dbt-artifacts-parser-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/__init__.py` & `dbt-artifacts-parser-0.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/parsers/__init__.py` & `dbt-artifacts-parser-0.3.1/tests/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/parsers/test_utils.py` & `dbt-artifacts-parser-0.3.1/tests/parsers/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/catalog.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/catalog.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v1/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v2/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v3/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v4/jaffle_shop/run_results.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/run_results.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v5/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v5/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v6/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v6/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v7/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v7/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json` & `dbt-artifacts-parser-0.3.1/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/test_basic.py` & `dbt-artifacts-parser-0.3.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/test_parser.py` & `dbt-artifacts-parser-0.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/tests/test_utils.py` & `dbt-artifacts-parser-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.0/PKG-INFO` & `dbt-artifacts-parser-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.3.0
+Version: 0.3.1
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.3.0 Summary: A dbt
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.3.1 Summary: A dbt
 artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
```

