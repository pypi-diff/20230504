# Comparing `tmp/asf_search-6.3.1.tar.gz` & `tmp/asf_search-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-6.3.1.tar", last modified: Wed Apr  5 22:21:58 2023, max compression
+gzip compressed data, was "asf_search-6.4.0.tar", last modified: Thu May  4 17:20:15 2023, max compression
```

## Comparing `asf_search-6.3.1.tar` & `asf_search-6.4.0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.801260 asf_search-6.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-05 22:21:45.000000 asf_search-6.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.777259 asf_search-6.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.781259 asf_search-6.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.781259 asf_search-6.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-05 22:21:45.000000 asf_search-6.3.1/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-05 22:21:45.000000 asf_search-6.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-04-05 22:21:45.000000 asf_search-6.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-05 22:21:45.000000 asf_search-6.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-05 22:21:58.801260 asf_search-6.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-05 22:21:45.000000 asf_search-6.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.781259 asf_search-6.3.1/asf_search/
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.789260 asf_search-6.3.1/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.789260 asf_search-6.3.1/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.789260 asf_search-6.3.1/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-05 22:21:45.000000 asf_search-6.3.1/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.785260 asf_search-6.3.1/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-05 22:21:58.000000 asf_search-6.3.1/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-05 22:21:58.000000 asf_search-6.3.1/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:21:58.000000 asf_search-6.3.1/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-05 22:21:58.000000 asf_search-6.3.1/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 22:21:58.000000 asf_search-6.3.1/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-05 22:21:45.000000 asf_search-6.3.1/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-05 22:21:45.000000 asf_search-6.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 22:21:58.801260 asf_search-6.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-05 22:21:45.000000 asf_search-6.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.793260 asf_search-6.3.1/tests/download/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.797260 asf_search-6.3.1/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:21:58.801260 asf_search-6.3.1/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23270 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)    46703 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (123)    38376 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (123)   350912 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-04-05 22:21:45.000000 asf_search-6.3.1/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.125105 asf_search-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 17:20:05.000000 asf_search-6.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.101104 asf_search-6.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.105104 asf_search-6.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.105104 asf_search-6.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 17:20:05.000000 asf_search-6.4.0/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-04 17:20:05.000000 asf_search-6.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-04 17:20:05.000000 asf_search-6.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 17:20:05.000000 asf_search-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-05-04 17:20:15.125105 asf_search-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-04 17:20:05.000000 asf_search-6.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.105104 asf_search-6.4.0/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.109104 asf_search-6.4.0/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.109104 asf_search-6.4.0/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.109104 asf_search-6.4.0/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.109104 asf_search-6.4.0/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.113104 asf_search-6.4.0/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.113104 asf_search-6.4.0/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.113104 asf_search-6.4.0/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.113104 asf_search-6.4.0/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.113104 asf_search-6.4.0/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-04 17:20:05.000000 asf_search-6.4.0/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.109104 asf_search-6.4.0/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-05-04 17:20:15.000000 asf_search-6.4.0/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-04 17:20:15.000000 asf_search-6.4.0/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:20:15.000000 asf_search-6.4.0/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-04 17:20:15.000000 asf_search-6.4.0/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 17:20:15.000000 asf_search-6.4.0/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-04 17:20:05.000000 asf_search-6.4.0/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 17:20:05.000000 asf_search-6.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:20:15.125105 asf_search-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-04 17:20:05.000000 asf_search-6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.117105 asf_search-6.4.0/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:20:15.125105 asf_search-6.4.0/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    46703 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    38828 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-05-04 17:20:05.000000 asf_search-6.4.0/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-05-04 17:20:06.000000 asf_search-6.4.0/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-6.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-6.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-6.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/.github/workflows/prod-request-merged.yml` & `asf_search-6.4.0/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/.github/workflows/pypi-publish.yml` & `asf_search-6.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/.github/workflows/run-pytest.yml` & `asf_search-6.4.0/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/.gitignore` & `asf_search-6.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/CHANGELOG.md` & `asf_search-6.4.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,27 @@
 
 ### Removed:
 -
 
 -->
 
 ------
+## [v6.4.0](https://github.com/asfadmin/Discovery-asf_search/compare/v6.3.1...v6.4.0)
+### Added
+- Burst product downloads now supported
+- `IPFVersion` field added to `ASFProduct` properties
+### Fixed
+- `BURST` product `url`, `fileName`, and `bytes` properties populated again
+- `search_count()` now uses `ASFSearchOptions.host` when building query url
+### Changed:
+- `BURST` product baseline stackng now uses `fullBurstID` and `polarization` for getting initial stack
+- Changed order of entries in `ASFSession`'s `User-Agent` header
+- `BURST` `filename` field uses "`sceneName`.`extension`" format
+
+------
 ## [v6.3.1](https://github.com/asfadmin/Discovery-asf_search/compare/v6.3.0...v6.3.1)
 ### Changed
 - Changed `CMR_PAGE_SIZE` constant from 500 to 250
 
 ------
 ## [v6.3.0](https://github.com/asfadmin/Discovery-asf_search/compare/v6.2.0...v6.3.0)
 ### Added
```

### Comparing `asf_search-6.3.1/LICENSE` & `asf_search-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/PKG-INFO` & `asf_search-6.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 6.3.1
+Version: 6.4.0
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.3.1/README.md` & `asf_search-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFProduct.py` & `asf_search-6.4.0/asf_search/ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-6.4.0/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-6.4.0/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFSearchOptions/validators.py` & `asf_search-6.4.0/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFSearchResults.py` & `asf_search-6.4.0/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/ASFSession.py` & `asf_search-6.4.0/asf_search/ASFSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from asf_search.exceptions import ASFAuthenticationError
 
 class ASFSession(requests.Session):
 
     def __init__(self):
         super().__init__()
         user_agent = '; '.join([
-            f"{asf_name}/{asf_version}",
             f'Python/{platform.python_version()}',
-            f'{requests.__name__}/{requests.__version__}'])
+            f'{requests.__name__}/{requests.__version__}',
+            f'{asf_name}/{asf_version}'])
 
         self.headers.update({'User-Agent': user_agent})  # For all hosts
         self.headers.update({'Client-Id': f"{asf_name}_v{asf_version}"})  # For CMR
 
     def __eq__(self, other):
         return self.auth == other.auth \
            and self.headers == other.headers \
```

### Comparing `asf_search-6.3.1/asf_search/CMR/MissionList.py` & `asf_search-6.4.0/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/CMR/field_map.py` & `asf_search-6.4.0/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/CMR/subquery.py` & `asf_search-6.4.0/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/CMR/translate.py` & `asf_search-6.4.0/asf_search/CMR/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
         'polarization': get(umm, 'AdditionalAttributes', ('Name', 'POLARIZATION'), 'Values', 0),
         'processingDate': get(umm, 'DataGranule', 'ProductionDateTime'),
         'processingLevel': get(umm, 'AdditionalAttributes', ('Name', 'PROCESSING_TYPE'), 'Values', 0),
         'sceneName': get(umm, 'DataGranule', 'Identifiers', ('IdentifierType', 'ProducerGranuleId'), 'Identifier'),
         'sensor': get(umm, 'Platforms', 0, 'Instruments', 0, 'ShortName'),
         'startTime': get(umm, 'TemporalExtent', 'RangeDateTime', 'BeginningDateTime'),
         'stopTime': get(umm, 'TemporalExtent', 'RangeDateTime', 'EndingDateTime'),
-        'url': get(umm, 'RelatedUrls', ('Type', 'GET DATA'), 'URL')
+        'url': get(umm, 'RelatedUrls', ('Type', 'GET DATA'), 'URL'),
+        'pgeVersion': get(umm, 'PGEVersionClass', 'PGEVersion')
     }
     
     if properties['beamModeType'] is None:
         properties['beamModeType'] = get(umm, 'AdditionalAttributes', ('Name', 'BEAM_MODE'), 'Values', 0)
 
     positions = {}
     velocities = {}
@@ -213,14 +214,20 @@
             'samplesPerBurst': cast(int, get(umm, 'AdditionalAttributes', ('Name', 'SAMPLES_PER_BURST'), 'Values', 0)),
             'subswath': get(umm, 'AdditionalAttributes', ('Name', 'SUBSWATH_NAME'), 'Values', 0),
             'azimuthTime': get(umm, 'AdditionalAttributes', ('Name', 'AZIMUTH_TIME'), 'Values', 0),
             'azimuthAnxTime': get(umm, 'AdditionalAttributes', ('Name', 'AZIMUTH_ANX_TIME'), 'Values', 0),
         }
         properties['burst'] = burst
         properties['sceneName'] = properties['fileID']
+        properties['bytes'] = cast(int, get(umm, 'AdditionalAttributes', ('Name', 'BYTE_LENGTH'),  'Values', 0))
+
+        urls = get(umm, 'RelatedUrls', ('Type', [('USE SERVICE API', 'URL')]), 0)
+        if urls is not None:
+            properties['url'] = urls[0]
+            properties['fileName'] = properties['fileID'] + '.' + urls[0].split('.')[-1]
 
     return {'geometry': geometry, 'properties': properties, 'type': 'Feature', 'baseline': baseline}
 
 def get_additional_fields(umm, *field_path):
     return get(umm, *field_path)
 
 def cast(f, v):
```

### Comparing `asf_search-6.3.1/asf_search/WKT/validate_wkt.py` & `asf_search-6.4.0/asf_search/WKT/validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/__init__.py` & `asf_search-6.4.0/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/baseline/calc.py` & `asf_search-6.4.0/asf_search/baseline/calc.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/baseline/stack.py` & `asf_search-6.4.0/asf_search/baseline/stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/constants/BEAMMODE.py` & `asf_search-6.4.0/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-6.4.0/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/download/download.py` & `asf_search-6.4.0/asf_search/download/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Iterable
 from multiprocessing import Pool
 import os.path
 import urllib.parse
+from requests import Response
 from requests.exceptions import HTTPError
 import warnings
+import regex as re
 
 from asf_search.exceptions import ASFAuthenticationError, ASFDownloadError
 from asf_search import ASFSession
 from remotezip import RemoteZip
+from tenacity import retry, stop_after_delay, retry_if_result, wait_fixed
 
 def _download_url(arg):
     url, path, session = arg
     download_url(
         url=url,
         path=path,
         session=session)
@@ -47,38 +50,30 @@
 
     :param url: URL from which to download
     :param path: Local path in which to save the product
     :param filename: Optional filename to be used, extracted from the URL by default
     :param session: The session to use, in most cases should be authenticated beforehand
     :return:
     """
-
+    
     if filename is None:
         filename = os.path.split(urllib.parse.urlparse(url).path)[1]
-
+    
     if not os.path.isdir(path):
         raise ASFDownloadError(f'Error downloading {url}: directory not found: {path}')
 
     if os.path.isfile(os.path.join(path, filename)):
         warnings.warn(f'File already exists, skipping download: {os.path.join(path, filename)}')
         return
 
     if session is None:
         session = ASFSession()
 
-    response = session.get(url, stream=True, hooks={'response': strip_auth_if_aws})
-
-    try:
-        response.raise_for_status()
-    except HTTPError as e:
-        if 400 <= response.status_code <= 499:
-            raise ASFAuthenticationError(f'HTTP {e.response.status_code}: {e.response.text}')
-        
-        raise e   
-
+    response = _try_get_response(session=session, url=url)
+    
     with open(os.path.join(path, filename), 'wb') as f:
         for chunk in response.iter_content(chunk_size=8192):
             f.write(chunk)
 
 def remotezip(url: str, session: ASFSession) -> RemoteZip:
     """
     :param url: the url to the zip product
@@ -89,7 +84,29 @@
     return RemoteZip(url, session=session)
 
 def strip_auth_if_aws(r, *args, **kwargs):
     if 300 <= r.status_code <= 399 and 'amazonaws.com' in urllib.parse.urlparse(r.headers['location']).netloc:
         location = r.headers['location']
         r.headers.clear()
         r.headers['location'] = location
+
+# if it's an unprocessed burst product it'll return a 202 and we'll have to query again 
+# https://sentinel1-burst-docs.asf.alaska.edu/
+def _is_burst_processing(response: Response):
+    return response.status_code == 202
+
+@retry(retry=retry_if_result(_is_burst_processing),
+       wait=wait_fixed(1),
+       stop=stop_after_delay(90),
+    )
+def _try_get_response(session: ASFSession, url: str):
+    response = session.get(url, stream=True, hooks={'response': strip_auth_if_aws})
+
+    try:
+        response.raise_for_status()
+    except HTTPError as e:
+        if 400 <= response.status_code <= 499:
+            raise ASFAuthenticationError(f'HTTP {e.response.status_code}: {e.response.text}')
+
+        raise e
+
+    return response
```

### Comparing `asf_search-6.3.1/asf_search/exceptions.py` & `asf_search-6.4.0/asf_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/export/csv.py` & `asf_search-6.4.0/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/export/export_translators.py` & `asf_search-6.4.0/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/export/geojson.py` & `asf_search-6.4.0/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/export/jsonlite.py` & `asf_search-6.4.0/asf_search/export/jsonlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,16 @@
             'productTypeDisplay': p['processingTypeDisplay'],
             'sizeMB': p['sizeMB'],
             'stackSize': p.get('insarStackSize'), # Used for datasets with precalculated stacks
             'startTime': p['startTime'],
             'stopTime': p['stopTime'],
             'thumb': p['thumb'],
             'wkt': wrapped,
-            'wkt_unwrapped': unwrapped
+            'wkt_unwrapped': unwrapped,
+            'pgeVersion': p['pgeVersion']
         }
         
         for key in result.keys():
             if result[key] in [ 'NA', 'NULL']:
                 result[key] = None
 
         if 'temporalBaseline' in p.keys() or 'perpendicularBaseline' in p.keys():
```

### Comparing `asf_search-6.3.1/asf_search/export/jsonlite2.py` & `asf_search-6.4.0/asf_search/export/jsonlite2.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             'ptd': p['productTypeDisplay'],
             's': p['sizeMB'],
             'ss': p['stackSize'], # Used for datasets with precalculated stacks
             'st': p['startTime'],
             'stp': p['stopTime'],
             't': p['thumb'].replace(p['granuleName'], '{gn}') if p['thumb'] is not None else p['thumb'],
             'w': p['wkt'],
-            'wu': p['wkt_unwrapped']
+            'wu': p['wkt_unwrapped'],
+            'pge': p['pgeVersion']
         }
 
         if 'temporalBaseline' in p.keys() or 'perpendicularBaseline' in p.keys():
             result['tb'] = p['temporalBaseline']
             result['pb'] = p['perpendicularBaseline']
 
         if p.get('burst') is not None: # is a burst product
```

### Comparing `asf_search-6.3.1/asf_search/export/kml.py` & `asf_search-6.4.0/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/export/metalink.py` & `asf_search-6.4.0/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/health/health.py` & `asf_search-6.4.0/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/baseline_search.py` & `asf_search-6.4.0/asf_search/search/baseline_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,26 +80,29 @@
     if reference.properties['platform'] in precalc_platforms:
         if reference.properties['insarStackId'] not in [None, 'NA', 0, '0']:
             stack_opts.insarStackId = reference.properties['insarStackId']
             return stack_opts
         raise ASFBaselineError(f'Requested reference product needs a baseline stack ID but does not have one: {reference.properties["fileID"]}')
 
     # build a stack from scratch if it's a non-precalc dataset with state vectors
-    if reference.properties['platform'].upper() in [PLATFORM.SENTINEL1A.upper(), PLATFORM.SENTINEL1B.upper()]:
+    
+    if reference.properties['processingLevel'] == 'BURST':
+        stack_opts.fullBurstID = reference.properties['burst']['fullBurstID']
+        stack_opts.polarization = [reference.properties['polarization']]
+        return stack_opts
+    elif reference.properties['platform'].upper() in [PLATFORM.SENTINEL1A.upper(), PLATFORM.SENTINEL1B.upper()]:
         stack_opts.platform = [PLATFORM.SENTINEL1A, PLATFORM.SENTINEL1B]
         
         stack_opts.beamMode = [reference.properties['beamModeType']]
         stack_opts.flightDirection = reference.properties['flightDirection']
         stack_opts.relativeOrbit = [int(reference.properties['pathNumber'])]  # path
         
-        is_burst = reference.properties['processingLevel'] == 'BURST'
-        
-        if reference.properties['polarization'] in ['HH', 'HH+HV'] and not is_burst:
+        if reference.properties['polarization'] in ['HH', 'HH+HV']:
             stack_opts.polarization = ['HH','HH+HV']
-        elif reference.properties['polarization'] in ['VV', 'VV+VH'] and not is_burst:
+        elif reference.properties['polarization'] in ['VV', 'VV+VH']:
             stack_opts.polarization = ['VV','VV+VH']
         else:
             stack_opts.polarization = [reference.properties['polarization']]
         
         stack_opts.intersectsWith = reference.centroid().wkt
         
         return stack_opts
```

### Comparing `asf_search-6.3.1/asf_search/search/campaigns.py` & `asf_search-6.4.0/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/error_reporting.py` & `asf_search-6.4.0/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/geo_search.py` & `asf_search-6.4.0/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/granule_search.py` & `asf_search-6.4.0/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/product_search.py` & `asf_search-6.4.0/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/search.py` & `asf_search-6.4.0/asf_search/search/search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search/search/search_count.py` & `asf_search-6.4.0/asf_search/search/search_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     kw_opts = ASFSearchOptions(**kwargs)
 
     # Anything passed in as kwargs has priority over anything in opts:
     opts.merge_args(**dict(kw_opts))
 
     preprocess_opts(opts)
 
-    url = '/'.join(s.strip('/') for s in [f'https://{INTERNAL.CMR_HOST}', f'{INTERNAL.CMR_GRANULE_PATH}'])
+    url = '/'.join(s.strip('/') for s in [f'https://{opts.host}', f'{INTERNAL.CMR_GRANULE_PATH}'])
 
     count = 0
     for query in build_subqueries(opts):
         translated_opts = translate_opts(query)
         idx = translated_opts.index(('page_size', INTERNAL.CMR_PAGE_SIZE))
         translated_opts[idx] = ('page_size', 0)
```

### Comparing `asf_search-6.3.1/asf_search/search/search_generator.py` & `asf_search-6.4.0/asf_search/search/search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/asf_search.egg-info/PKG-INFO` & `asf_search-6.4.0/asf_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf-search
-Version: 6.3.1
+Version: 6.4.0
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.3.1/asf_search.egg-info/SOURCES.txt` & `asf_search-6.4.0/asf_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/0-Intro.md` & `asf_search-6.4.0/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/1-Basic_Overview.ipynb` & `asf_search-6.4.0/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/2-Geographic_Search.ipynb` & `asf_search-6.4.0/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/3-Granule_Search.ipynb` & `asf_search-6.4.0/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/4-Baseline_Search.ipynb` & `asf_search-6.4.0/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/5-Download.ipynb` & `asf_search-6.4.0/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/6-Outro.md` & `asf_search-6.4.0/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/examples/hello_world.py` & `asf_search-6.4.0/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/setup.py` & `asf_search-6.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     "requests",
     "shapely",
     "python-dateutil",
     "pytz",
     "importlib_metadata",
     "numpy",
     "dateparser",
-    "remotezip >= 0.10.0"
+    "remotezip >= 0.10.0",
+    "tenacity == 8.2.2"
 ]
 
 test_requirements = [
     "pytest < 7.2.0",
     "pytest-automation",
     "pytest-cov",
     "pytest-xdist",
```

### Comparing `asf_search-6.3.1/tests/ASFProduct/test_ASFProduct.py` & `asf_search-6.4.0/tests/ASFProduct/test_ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-6.4.0/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-6.4.0/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/ASFSession/test_ASFSession.py` & `asf_search-6.4.0/tests/ASFSession/test_ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-6.4.0/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/BaselineSearch/test_baseline_search.py` & `asf_search-6.4.0/tests/BaselineSearch/test_baseline_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,18 @@
     params = get_stack_opts(reference)
 
     original_properties = product['properties']
     assert(original_properties['polarization'] in params.polarization)
     
     if reference.properties['processingLevel'] == 'BURST':
         assert([reference.properties['polarization']] == params.polarization)
+        assert([reference.properties['burst']['fullBurstID']] == params.fullBurstID)
     else:
         assert(['VV', 'VV+VH'] == params.polarization if reference.properties['polarization'] in ['VV', 'VV+VH'] else ['HH','HH+HV'] == params.polarization)
-    assert(len(dict(params)) == 7)
+        assert(len(dict(params)) == 7)
 
 def run_get_stack_opts_invalid_insarStackId(product):
     invalid_reference = ASFProduct(product)
     
     invalid_reference.properties['insarStackId'] = '0'
 
     with pytest.raises(ASFBaselineError):
```

### Comparing `asf_search-6.3.1/tests/CMR/test_MissionList.py` & `asf_search-6.4.0/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/Search/test_search.py` & `asf_search-6.4.0/tests/Search/test_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/Search/test_search_generator.py` & `asf_search-6.4.0/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/Serialization/test_serialization.py` & `asf_search-6.4.0/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/WKT/test_validate_wkt.py` & `asf_search-6.4.0/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/pytest-config.yml` & `asf_search-6.4.0/tests/pytest-config.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/pytest-managers.py` & `asf_search-6.4.0/tests/pytest-managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import pathlib
 import yaml
 
 from WKT.test_validate_wkt import run_test_search_wkt_prep, run_test_validate_wkt_get_shape_coords, run_test_validate_wkt_clamp_geometry, run_test_validate_wkt_valid_wkt, run_test_validate_wkt_convex_hull, run_test_validate_wkt_counter_clockwise_reorientation, run_test_validate_wkt_invalid_wkt_error, run_test_validate_wkt_merge_overlapping_geometry, run_test_simplify_aoi
 from ASFSearchOptions.test_ASFSearchOptions import run_test_ASFSearchOptions_validator, run_test_validator_map_validate
 from BaselineSearch.Stack.test_stack import run_test_find_new_reference, run_test_get_baseline_from_stack, run_test_get_default_product_type, run_test_valid_state_vectors
 
-from download.test_download import run_test_download_url_auth_error
+from download.test_download import run_test_download_url, run_test_download_url_auth_error
 from Serialization.test_serialization import run_test_serialization
 import nbformat
 from nbconvert.preprocessors import ExecutePreprocessor
 
 
 # asf_search.ASFProduct Tests
 def test_ASFProduct(**args) -> None:
@@ -334,15 +334,17 @@
     test_info = args["test_info"]
     url = test_info["url"]
     path = test_info["path"]
     filename = test_info["filename"]
         
     if filename == "error":
         run_test_download_url_auth_error(url, path, filename)
-
+    else:
+        run_test_download_url(url, path, filename)
+        
 def test_find_new_reference(**args) -> None:
     """
     Test asf_search.baseline.calc.find_new_reference
     """
     test_info = args["test_info"]
     stack = get_resource(test_info["stack"])
     output_index = get_resource(test_info["output_index"])
```

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         "sceneName": "ALPSRS279162650",
         "sensor": "PALSAR",
         "startTime": "2011-04-21T20:23:11.000Z",
         "stopTime": "2011-04-21T20:23:36.000Z",
         "url": "https://datapool.asf.alaska.edu/L1.0/A3/ALPSRS279162650-L1.0.zip",
         "fileName": "ALPSRS279162650-L1.0.zip",
         "frameNumber": 2650,
+        "pgeVersion": null
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-147.788, 49.629],
@@ -234,14 +235,15 @@
         "sceneName": "ALPSRS279162650",
         "sensor": "PALSAR",
         "startTime": "2011-04-21T20:23:11.000Z",
         "stopTime": "2011-04-21T20:23:36.000Z",
         "url": "https://datapool.asf.alaska.edu/L1.5/A3/ALPSRS279162650-L1.5.zip",
         "fileName": "ALPSRS279162650-L1.5.zip",
         "frameNumber": 2650,
+        "pgeVersion": null
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-147.788, 49.629],
@@ -446,14 +448,15 @@
         "sceneName": "ALPSRS279162600",
         "sensor": "PALSAR",
         "startTime": "2011-04-21T20:22:30.000Z",
         "stopTime": "2011-04-21T20:22:55.000Z",
         "url": "https://datapool.asf.alaska.edu/L1.0/A3/ALPSRS279162600-L1.0.zip",
         "fileName": "ALPSRS279162600-L1.0.zip",
         "frameNumber": 2600,
+        "pgeVersion": null
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-147.166, 52.088],
```

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         "sceneName": "S1B_IW_GRDH_1SDV_20211216T032038_20211216T032103_030045_039655_2335",
         "sensor": "C-SAR",
         "startTime": "2021-12-16T03:20:38.000Z",
         "stopTime": "2021-12-16T03:21:03.000Z",
         "url": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211216T032038_20211216T032103_030045_039655_2335.zip",
         "fileName": "S1B_IW_GRDH_1SDV_20211216T032038_20211216T032103_030045_039655_2335.zip",
         "frameNumber": 210,
+        "pgeVersion": "003.40"
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-150.147552, 65.464966],
@@ -168,14 +169,15 @@
         "ProviderDates":
           [
             { "Date": "2021-12-17T09:29:15.000Z", "Type": "Insert" },
             { "Date": "2021-12-17T09:29:15.000Z", "Type": "Update" },
           ],
         "CollectionReference":
           { "ShortName": "SENTINEL-1B_DP_GRD_HIGH", "Version": "1" },
+        'PGEVersionClass': {'PGEName': 'Sentinel-1 IPF', 'PGEVersion': '003.40'},
         "RelatedUrls":
           [
             {
               "Format": "Not provided",
               "Description": "This link provides direct download access to the granule.",
               "Type": "GET DATA",
               "URL": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211216T032038_20211216T032103_030045_039655_2335.zip",
@@ -264,14 +266,15 @@
         "sceneName": "S1B_IW_GRDH_1SDV_20211204T032038_20211204T032103_029870_0390CC_FC88",
         "sensor": "C-SAR",
         "startTime": "2021-12-04T03:20:38.000Z",
         "stopTime": "2021-12-04T03:21:03.000Z",
         "url": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211204T032038_20211204T032103_029870_0390CC_FC88.zip",
         "fileName": "S1B_IW_GRDH_1SDV_20211204T032038_20211204T032103_029870_0390CC_FC88.zip",
         "frameNumber": 210,
+        "pgeVersion": "003.40"
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-150.146927, 65.465103],
@@ -407,14 +410,15 @@
         "ProviderDates":
           [
             { "Date": "2021-12-04T10:04:34.000Z", "Type": "Insert" },
             { "Date": "2021-12-04T10:04:34.000Z", "Type": "Update" },
           ],
         "CollectionReference":
           { "ShortName": "SENTINEL-1B_DP_GRD_HIGH", "Version": "1" },
+        'PGEVersionClass': {'PGEName': 'Sentinel-1 IPF', 'PGEVersion': '003.40'},
         "RelatedUrls":
           [
             {
               "Format": "Not provided",
               "Description": "This link provides direct download access to the granule.",
               "Type": "GET DATA",
               "URL": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211204T032038_20211204T032103_029870_0390CC_FC88.zip",
@@ -503,14 +507,15 @@
         "sceneName": "S1B_IW_GRDH_1SDV_20211122T032039_20211122T032104_029695_038B4D_706D",
         "sensor": "C-SAR",
         "startTime": "2021-11-22T03:20:39.000Z",
         "stopTime": "2021-11-22T03:21:04.000Z",
         "url": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211122T032039_20211122T032104_029695_038B4D_706D.zip",
         "fileName": "S1B_IW_GRDH_1SDV_20211122T032039_20211122T032104_029695_038B4D_706D.zip",
         "frameNumber": 210,
+        "pgeVersion": "003.40"
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-150.147202, 65.465134],
@@ -646,14 +651,15 @@
         "ProviderDates":
           [
             { "Date": "2021-11-22T22:36:40.000Z", "Type": "Insert" },
             { "Date": "2021-11-22T22:36:40.000Z", "Type": "Update" },
           ],
         "CollectionReference":
           { "ShortName": "SENTINEL-1B_DP_GRD_HIGH", "Version": "1" },
+        'PGEVersionClass': {'PGEName': 'Sentinel-1 IPF', 'PGEVersion': '003.40'},
         "RelatedUrls":
           [
             {
               "Format": "Not provided",
               "Description": "This link provides direct download access to the granule.",
               "Type": "GET DATA",
               "URL": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211122T032039_20211122T032104_029695_038B4D_706D.zip",
@@ -742,14 +748,15 @@
         "sceneName": "S1B_IW_GRDH_1SDV_20211110T032039_20211110T032104_029520_0385E6_60DB",
         "sensor": "C-SAR",
         "startTime": "2021-11-10T03:20:39.000Z",
         "stopTime": "2021-11-10T03:21:04.000Z",
         "url": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211110T032039_20211110T032104_029520_0385E6_60DB.zip",
         "fileName": "S1B_IW_GRDH_1SDV_20211110T032039_20211110T032104_029520_0385E6_60DB.zip",
         "frameNumber": 210,
+        "pgeVersion": "003.40"
       },
     "geometry":
       {
         "coordinates":
           [
             [
               [-150.149414, 65.465057],
@@ -885,14 +892,15 @@
         "ProviderDates":
           [
             { "Date": "2021-11-10T08:57:13.000Z", "Type": "Insert" },
             { "Date": "2021-11-10T08:57:13.000Z", "Type": "Update" },
           ],
         "CollectionReference":
           { "ShortName": "SENTINEL-1B_DP_GRD_HIGH", "Version": "1" },
+        'PGEVersionClass': {'PGEName': 'Sentinel-1 IPF', 'PGEVersion': '003.40'},
         "RelatedUrls":
           [
             {
               "Format": "Not provided",
               "Description": "This link provides direct download access to the granule.",
               "Type": "GET DATA",
               "URL": "https://datapool.asf.alaska.edu/GRD_HD/SB/S1B_IW_GRDH_1SDV_20211110T032039_20211110T032104_029520_0385E6_60DB.zip",
```

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/S1_response.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,163 +1,171 @@
 {
   "properties":
     {
       "beamModeType": "IW",
       "browse": None,
       "bytes": None,
-      "centerLat": 56.66337474164923,
-      "centerLon": -139.0261243329513,
+      "centerLat": 57.37481196728577,
+      "centerLon": -133.71556178621003,
       "faradayRotation": None,
-      "fileID": "S1_105585_IW1_20200814T025429_VV_FBE6-BURST",
+      "fileID": "S1_167878_IW2_20150316T023730_VH_BAD9-BURST",
       "flightDirection": "ASCENDING",
-      "groupID": "S1A_IWDV_0182_0187_033897_050",
+      "groupID": "S1A_IWDV_0184_0190_005051_079",
       "granuleType": None,
       "insarStackId": None,
       "md5sum": None,
       "offNadirAngle": None,
-      "orbit": 33897,
-      "pathNumber": 50,
+      "orbit": 5051,
+      "pathNumber": 79,
       "platform": "SENTINEL-1A",
       "pointingAngle": None,
-      "polarization": "VV",
+      "polarization": "VH",
       "processingDate": None,
       "processingLevel": "BURST",
-      "sceneName": "S1_105585_IW1_20200814T025429_VV_FBE6-BURST",
+      "sceneName": "S1_167878_IW2_20150316T023730_VH_BAD9-BURST",
       "sensor": "C-SAR",
-      "startTime": "2020-08-14T02:54:30.254113Z",
-      "stopTime": "2020-08-14T02:54:31.128247Z",
-      "url": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20200814T025409_20200814T025439_033897_03EE6C_FBE6/IW1/VV/7.tiff",
-      "fileName": "7.tiff",
+      "startTime": "2015-03-16T02:37:31.036086Z",
+      "stopTime": "2015-03-16T02:37:32.077676Z",
+      "url": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20150316T023715_20150316T023745_005051_006577_BAD9/IW2/VH/5.tiff",
+      "fileName": "5.tiff",
       "frameNumber": None,
       "burst":
-        { "absoluteBurstID": 72806500, "relativeBurstID": 105585, "fullBurstID": "050_105585_IW1", "burstIndex": 7, "samplesPerBurst": 21182, "subswath": "IW1", "azimuthAnxTime": "929.3799213259" },
-    },
-  "geometry":
-    {
-      "coordinates":
-        [[[-139.685624, 56.488088], [-138.968891, 56.56747], [-138.302229, 56.637151], [-138.373742, 56.840058], [-139.042373, 56.765726], [-139.761172, 56.681661], [-139.685624, 56.488088]]],
-      "type": "Polygon",
-    },
-  "baseline":
-    {
-      "stateVectors":
         {
-          "positions":
-            {
-              "prePosition": [-3282115.87647, -2255237.128829, 5838881.870155],
-              "prePositionTime": "2020-08-14T02:54:29.000000",
-              "postPosition": [-3244772.904073, -2203087.927862, 5879428.79989],
-              "postPositionTime": "2020-08-14T02:54:39.000000",
-            },
-          "velocities":
-            {
-              "preVelocity": [3712.183926, 5205.103635, 4087.71388],
-              "preVelocityTime": "2020-08-14T02:54:29.000000",
-              "postVelocity": [3756.345419, 5224.628326, 4021.596137],
-              "postVelocityTime": "2020-08-14T02:54:39.000000",
-            },
+          "absoluteBurstID": 10847375,
+          "relativeBurstID": 167878,
+          "fullBurstID": "079_167878_IW2",
+          "burstIndex": 5,
+          "samplesPerBurst": 25023,
+          "subswath": "IW2",
+          "azimuthTime": "2015-03-16T02:37:30.005466",
+          "azimuthAnxTime": "936.0866766603999",
         },
-      "ascendingNodeTime": "2020-08-14T02:38:59.749279",
     },
   "meta":
     {
       "concept-type": "granule",
-      "concept-id": "G1257027271-ASFDEV",
+      "concept-id": "G1257175671-ASFDEV",
       "revision-id": 1,
-      "native-id": "S1_105585_IW1_20200814T025429_VV_FBE6-BURST",
+      "native-id": "S1_167878_IW2_20150316T023730_VH_BAD9-BURST",
       "provider-id": "ASFDEV",
       "format": "application/vnd.nasa.cmr.umm+json",
-      "revision-date": "2023-03-30T21:55:03.157Z",
+      "revision-date": "2023-04-11T00:34:07.016Z",
     },
   "umm":
     {
-      "TemporalExtent": { "RangeDateTime": { "BeginningDateTime": "2020-08-14T02:54:30.254113Z", "EndingDateTime": "2020-08-14T02:54:31.128247Z" } },
-      "OrbitCalculatedSpatialDomains": [{ "OrbitNumber": 33897 }],
-      "GranuleUR": "S1_105585_IW1_20200814T025429_VV_FBE6-BURST",
+      "TemporalExtent": { "RangeDateTime": { "BeginningDateTime": "2015-03-16T02:37:31.036086Z", "EndingDateTime": "2015-03-16T02:37:32.077676Z" } },
+      "OrbitCalculatedSpatialDomains": [{ "OrbitNumber": 5051 }],
+      "GranuleUR": "S1_167878_IW2_20150316T023730_VH_BAD9-BURST",
       "AdditionalAttributes":
         [
-          { "Name": "ASC_NODE_TIME", "Values": ["2020-08-14T02:38:59.749279"] },
+          { "Name": "ASC_NODE_TIME", "Values": ["2015-03-16T02:21:53.918789"] },
           { "Name": "ASCENDING_DESCENDING", "Values": ["ASCENDING"] },
-          { "Name": "AZIMUTH_ANX_TIME", "Values": ["929.3799213259"] },
-          { "Name": "AZIMUTH_TIME", "Values": ["2020-08-14T02:54:29.129200"] },
+          { "Name": "AZIMUTH_ANX_TIME", "Values": ["936.0866766603999"] },
+          { "Name": "AZIMUTH_TIME", "Values": ["2015-03-16T02:37:30.005466"] },
           { "Name": "BEAM_MODE", "Values": ["IW"] },
           {
             "Name": "BEAM_MODE_DESC",
             "Values": ["Interferometric Wide. 250 km swath, 5 m x 20 m spatial resolution and burst synchronization for interferometry. IW is considered to be the standard mode over land masses."],
           },
-          { "Name": "BURST_ID_ABSOLUTE", "Values": ["72806500"] },
-          { "Name": "BURST_ID_FULL", "Values": ["050_105585_IW1"] },
-          { "Name": "BURST_ID_RELATIVE", "Values": ["105585"] },
-          { "Name": "BURST_INDEX", "Values": ["7"] },
-          { "Name": "BYTE_LENGTH", "Values": ["127261456"] },
-          { "Name": "BYTE_OFFSET", "Values": ["890950667"] },
-          { "Name": "CENTER_LAT", "Values": ["56.66337474164923"] },
-          { "Name": "CENTER_LON", "Values": ["-139.0261243329513"] },
-          { "Name": "GROUP_ID", "Values": ["S1A_IWDV_0182_0187_033897_050"] },
-          { "Name": "LINES_PER_BURST", "Values": ["1502"] },
-          { "Name": "PATH_NUMBER", "Values": ["50"] },
-          { "Name": "POLARIZATION", "Values": ["VV"] },
+          { "Name": "BURST_ID_ABSOLUTE", "Values": ["10847375"] },
+          { "Name": "BURST_ID_FULL", "Values": ["079_167878_IW2"] },
+          { "Name": "BURST_ID_RELATIVE", "Values": ["167878"] },
+          { "Name": "BURST_INDEX", "Values": ["5"] },
+          { "Name": "BYTE_LENGTH", "Values": ["151439196"] },
+          { "Name": "BYTE_OFFSET", "Values": ["757317335"] },
+          { "Name": "CENTER_LAT", "Values": ["57.37481196728577"] },
+          { "Name": "CENTER_LON", "Values": ["-133.71556178621003"] },
+          { "Name": "GROUP_ID", "Values": ["S1A_IWDV_0184_0190_005051_079"] },
+          { "Name": "LINES_PER_BURST", "Values": ["1513"] },
+          { "Name": "PATH_NUMBER", "Values": ["79"] },
+          { "Name": "POLARIZATION", "Values": ["VH"] },
           { "Name": "PROCESSING_LEVEL", "Values": ["L1"] },
           { "Name": "PROCESSING_TYPE", "Values": ["BURST"] },
-          { "Name": "SAMPLES_PER_BURST", "Values": ["21182"] },
-          { "Name": "SUBSWATH_NAME", "Values": ["IW1"] },
-          { "Name": "SV_POSITION_POST", "Values": ["-3244772.904073,-2203087.927862,5879428.79989,2020-08-14T02:54:39.000000"] },
-          { "Name": "SV_POSITION_PRE", "Values": ["-3282115.87647,-2255237.128829,5838881.870155,2020-08-14T02:54:29.000000"] },
-          { "Name": "SV_VELOCITY_POST", "Values": ["3756.345419,5224.628326,4021.596137,2020-08-14T02:54:39.000000"] },
-          { "Name": "SV_VELOCITY_PRE", "Values": ["3712.183926,5205.103635,4087.71388,2020-08-14T02:54:29.000000"] },
+          { "Name": "SAMPLES_PER_BURST", "Values": ["25023"] },
+          { "Name": "SUBSWATH_NAME", "Values": ["IW2"] },
+          { "Name": "SV_POSITION_POST", "Values": ["-3078107.203128,-2429893.458311,5879766.359772,2015-03-16T02:37:34.000000"] },
+          { "Name": "SV_POSITION_PRE", "Values": ["-3111615.103481,-2484588.280656,5839224.145067,2015-03-16T02:37:24.000000"] },
+          { "Name": "SV_VELOCITY_POST", "Values": ["3372.083035,5480.744957,4021.123749,2015-03-16T02:37:34.000000"] },
+          { "Name": "SV_VELOCITY_PRE", "Values": ["3329.439778,5458.106882,4087.243253,2015-03-16T02:37:24.000000"] },
         ],
       "SpatialExtent":
         {
           "HorizontalSpatialDomain":
             {
               "Geometry":
                 {
                   "GPolygons":
                     [
                       {
                         "Boundary":
                           {
                             "Points":
                               [
-                                { "Latitude": 56.488088, "Longitude": -139.685624 },
-                                { "Latitude": 56.56747, "Longitude": -138.968891 },
-                                { "Latitude": 56.637151, "Longitude": -138.302229 },
-                                { "Latitude": 56.840058, "Longitude": -138.373742 },
-                                { "Latitude": 56.765726, "Longitude": -139.042373 },
-                                { "Latitude": 56.681661, "Longitude": -139.761172 },
-                                { "Latitude": 56.488088, "Longitude": -139.685624 },
+                                { "Latitude": 57.208768, "Longitude": -134.429185 },
+                                { "Latitude": 57.283638, "Longitude": -133.668191 },
+                                { "Latitude": 57.349892, "Longitude": -132.947782 },
+                                { "Latitude": 57.541739, "Longitude": -133.009124 },
+                                { "Latitude": 57.471188, "Longitude": -133.731915 },
+                                { "Latitude": 57.391995, "Longitude": -134.49532 },
+                                { "Latitude": 57.208768, "Longitude": -134.429185 },
                               ],
                           },
                       },
                     ],
                 },
             },
         },
-      "ProviderDates": [{ "Type": "Insert", "Date": "2023-03-30T21:55:02Z" }, { "Type": "Update", "Date": "2023-03-30T21:55:02Z" }],
-      "CollectionReference": { "ShortName": "SENTINEL-1_BURSTS_DEV9", "Version": "1" },
-      "PGEVersionClass": { "PGEName": "Sentinel-1 IPF", "PGEVersion": "003.31" },
+      "ProviderDates": [{ "Type": "Insert", "Date": "2023-04-11T00:34:06Z" }, { "Type": "Update", "Date": "2023-04-11T00:34:06Z" }],
+      "CollectionReference": { "ShortName": "SENTINEL-1_BURSTS_DEV10", "Version": "1" },
+      "PGEVersionClass": { "PGEName": "Sentinel-1 IPF", "PGEVersion": "002.72" },
       "RelatedUrls":
         [
           {
-            "URL": "www.asf.alaska.edu/sar-information/sentinel-1-documents-tools",
-            "Type": "VIEW RELATED INFORMATION",
-            "Description": "ASF DAAC Sentinel-1 User Guide and Technical Documentation",
+            "URL": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20150316T023715_20150316T023745_005051_006577_BAD9/IW2/VH/5.tiff",
+            "Type": "USE SERVICE API",
+            "Description": "Use the link to extract the burst as a GeoTIFF from the input granule.",
             "Format": "Not provided",
           },
-          { "URL": "www.asf.alaska.edu/sar-data-sets/sentinel-1", "Type": "VIEW RELATED INFORMATION", "Description": "ASF DAAC Sentinel-1 data set landing page", "Format": "Not provided" },
           {
-            "URL": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20200814T025409_20200814T025439_033897_03EE6C_FBE6/IW1/VV/7.tiff",
-            "Type": "GET DATA",
-            "Description": "Link to burst granule.",
-            "Format": "Not provided",
+            "URL": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20150316T023715_20150316T023745_005051_006577_BAD9/IW2/VH/5.xml",
+            "Type": "USE SERVICE API",
+            "Description": "Use the link to extract an extended metadata file of the burst from the input granule.",
+            "Format": "XML",
           },
           {
-            "URL": "https://sentinel1-burst.asf.alaska.edu/S1A_IW_SLC__1SDV_20200814T025409_20200814T025439_033897_03EE6C_FBE6/IW1/VV/7.xml",
-            "Type": "EXTENDED METADATA",
-            "Description": "Link to burst granule metadata.",
+            "URL": "https://sentinel1-burst-docs.asf.alaska.edu/",
+            "Type": "VIEW RELATED INFORMATION",
+            "Description": "Usage information for the API used to extract a burst product from a Sentinel-1 SLC granule.",
             "Format": "Not provided",
           },
         ],
-      "InputGranules": ["S1A_IW_SLC__1SDV_20200814T025409_20200814T025439_033897_03EE6C_FBE6-SLC"],
+      "InputGranules": ["S1A_IW_SLC__1SDV_20150316T023715_20150316T023745_005051_006577_BAD9-SLC"],
       "Platforms": [{ "Instruments": [{ "ShortName": "C-SAR", "Characteristics": [{ "Name": "LookDirection", "Value": "RIGHT" }] }], "ShortName": "SENTINEL-1A" }],
     },
+  "geometry":
+    {
+      "coordinates":
+        [[[-134.429185, 57.208768], [-133.668191, 57.283638], [-132.947782, 57.349892], [-133.009124, 57.541739], [-133.731915, 57.471188], [-134.49532, 57.391995], [-134.429185, 57.208768]]],
+      "type": "Polygon",
+    },
+  "baseline":
+    {
+      "stateVectors":
+        {
+          "positions":
+            {
+              "prePosition": [-3111615.103481, -2484588.280656, 5839224.145067],
+              "prePositionTime": "2015-03-16T02:37:24.000000",
+              "postPosition": [-3078107.203128, -2429893.458311, 5879766.359772],
+              "postPositionTime": "2015-03-16T02:37:34.000000",
+            },
+          "velocities":
+            {
+              "preVelocity": [3329.439778, 5458.106882, 4087.243253],
+              "preVelocityTime": "2015-03-16T02:37:24.000000",
+              "postVelocity": [3372.083035, 5480.744957, 4021.123749],
+              "postVelocityTime": "2015-03-16T02:37:34.000000",
+            },
+        },
+      "ascendingNodeTime": "2015-03-16T02:21:53.918789",
+    },
 }
```

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-6.4.0/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-6.4.0/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_ASFProduct.yml` & `asf_search-6.4.0/tests/yml_tests/test_ASFProduct.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-6.4.0/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-6.4.0/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_ASFSession.yml` & `asf_search-6.4.0/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_baseline_search.yml` & `asf_search-6.4.0/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_search.yml` & `asf_search-6.4.0/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_search_generator.yml` & `asf_search-6.4.0/tests/yml_tests/test_search_generator.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_serialization.yml` & `asf_search-6.4.0/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_stack.yml` & `asf_search-6.4.0/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.3.1/tests/yml_tests/test_validate_wkt.yml` & `asf_search-6.4.0/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*

