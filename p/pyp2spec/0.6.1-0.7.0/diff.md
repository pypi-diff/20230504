# Comparing `tmp/pyp2spec-0.6.1.tar.gz` & `tmp/pyp2spec-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyp2spec-0.6.1.tar", last modified: Mon Aug  1 12:15:24 2022, max compression
+gzip compressed data, was "pyp2spec-0.7.0.tar", last modified: Thu May  4 07:51:59 2023, max compression
```

## Comparing `pyp2spec-0.6.1.tar` & `pyp2spec-0.7.0.tar`

### file list

```diff
@@ -1,68 +1,49 @@
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.672428 pyp2spec-0.6.1/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1103 2021-08-25 12:47:30.000000 pyp2spec-0.6.1/LICENSE-MIT
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      954 2022-07-27 08:57:40.000000 pyp2spec-0.6.1/LICENSE-MIT-0
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      139 2021-12-10 09:31:28.000000 pyp2spec-0.6.1/MANIFEST.in
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7020 2022-08-01 12:15:24.672428 pyp2spec-0.6.1/PKG-INFO
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6319 2022-07-27 08:57:40.000000 pyp2spec-0.6.1/README.md
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.665428 pyp2spec-0.6.1/pyp2spec/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        0 2021-11-11 11:05:59.000000 pyp2spec-0.6.1/pyp2spec/__init__.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6912 2021-12-08 16:04:46.000000 pyp2spec-0.6.1/pyp2spec/classifiers_to_fedora.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6176 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/pyp2spec/conf2spec.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    16241 2022-08-01 11:03:52.000000 pyp2spec-0.6.1/pyp2spec/pyp2conf.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1791 2022-02-21 13:40:02.000000 pyp2spec-0.6.1/pyp2spec/pyp2spec.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2604 2022-03-21 16:56:13.000000 pyp2spec-0.6.1/pyp2spec/rpmversion.py
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1728 2022-03-30 13:46:14.000000 pyp2spec-0.6.1/pyp2spec/template.spec
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.666428 pyp2spec-0.6.1/pyp2spec.egg-info/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7020 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/PKG-INFO
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     3648 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/SOURCES.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        1 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/dependency_links.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      122 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/entry_points.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)       88 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/requires.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)        9 2022-08-01 12:15:24.000000 pyp2spec-0.6.1/pyp2spec.egg-info/top_level.txt
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2021-11-11 11:13:11.000000 pyp2spec-0.6.1/pyproject.toml
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1122 2022-08-01 12:15:24.672428 pyp2spec-0.6.1/setup.cfg
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.666428 pyp2spec-0.6.1/tests/
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.667428 pyp2spec-0.6.1/tests/expected_specfiles/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1283 2022-07-25 10:01:33.000000 pyp2spec-0.6.1/tests/expected_specfiles/python-click.spec
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1829 2022-03-30 13:46:14.000000 pyp2spec-0.6.1/tests/expected_specfiles/python-markdown-it-py.spec
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.663428 pyp2spec-0.6.1/tests/fixtures/
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.671428 pyp2spec-0.6.1/tests/fixtures/cassettes/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-12-08 16:04:46.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_OSI_Approved_is_ignored.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    59383 2022-02-11 13:16:09.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    10087 2021-11-03 12:34:18.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    21336 2021-11-03 12:34:18.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-11-29 16:49:28.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_bad_license_if_compliant_is_not_returned.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-11-29 16:49:28.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_bad_license_if_not_compliant_is_returned.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-11-29 16:49:28.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_compliant_license_is_returned.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    10087 2021-11-03 12:34:18.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-12-08 16:04:46.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_license_classifier_read_correctly.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-11-29 16:49:28.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_mix_non_compliant_licenses_wont_work_if_strict.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-11-29 16:49:28.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_mix_non_compliant_licenses_work_if_not_strict.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    24449 2021-12-10 09:20:26.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_no_homepage_in_metadata.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15265 2021-12-08 16:04:46.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_no_license_classifiers_and_no_license_keyword.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    15039 2021-11-03 12:34:18.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_package_without_license_is_not_processed.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5702 2022-08-01 11:03:52.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_name_with_capital_letter_is_normalized.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    11584 2022-08-01 11:03:52.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_name_with_underscore_is_normalized.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    11289 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[django-apistar-0.5.40-0-0.5.40-0].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    11249 2022-02-11 13:42:30.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[django-apistar-0.5.40-0-0.5.40^post0].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    17332 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[javascript-1!0.2.13-1!0.2.13].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    16934 2022-02-11 13:42:30.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[javascript-1!0.2.13-1-0.2.13].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    21402 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[markdown-it-py-1.1.0-%{version}].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    21402 2022-02-11 13:42:30.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[markdown-it-py-1.1.0-1.1.0].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5522 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[python3-wget-0.0.2-beta1-0.0.2-beta1].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5520 2022-02-11 13:42:30.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[python3-wget-0.0.2-beta1-0.0.2~b1].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    16325 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[tomli-None-%{version}].json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7714 2022-01-12 08:17:45.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_summary_is_generated_if_not_in_upstream.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     8839 2022-01-12 08:17:45.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_summary_is_generated_if_upstream_data_is_multiline.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)    17319 2021-12-08 16:04:46.000000 pyp2spec-0.6.1/tests/fixtures/cassettes/test_pyp2conf.test_zip_sdist_is_added_to_source_macro.json
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4790 2022-02-11 13:16:09.000000 pyp2spec-0.6.1/tests/test_conf2spec.py
-drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2022-08-01 12:15:24.672428 pyp2spec-0.6.1/tests/test_configs/
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      515 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_aionotion.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      754 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_boutdata.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      856 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_click.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      918 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_jupyter-packaging.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1047 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_markdown-it-py.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      603 2022-03-30 13:24:16.000000 pyp2spec-0.6.1/tests/test_configs/customized_tornado.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      485 2022-07-25 10:01:33.000000 pyp2spec-0.6.1/tests/test_configs/default_python-aionotion.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)      455 2022-07-25 10:01:33.000000 pyp2spec-0.6.1/tests/test_configs/default_python-click.conf
--rw-r--r--   0 ksurma    (1000) ksurma    (1000)     7636 2022-08-01 11:03:52.000000 pyp2spec-0.6.1/tests/test_pyp2conf.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.131534 pyp2spec-0.7.0/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1103 2022-12-02 12:41:04.000000 pyp2spec-0.7.0/LICENSE-MIT
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      954 2022-12-02 12:41:04.000000 pyp2spec-0.7.0/LICENSE-MIT-0
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)       64 2023-05-03 08:15:20.000000 pyp2spec-0.7.0/MANIFEST.in
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6638 2023-05-04 07:51:59.131534 pyp2spec-0.7.0/PKG-INFO
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5937 2023-05-03 08:15:20.000000 pyp2spec-0.7.0/README.md
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.128534 pyp2spec-0.7.0/pyp2spec/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        0 2022-12-02 12:41:04.000000 pyp2spec-0.7.0/pyp2spec/__init__.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     5862 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/pyp2spec/classifiers_to_fedora.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6074 2023-05-03 13:21:26.000000 pyp2spec-0.7.0/pyp2spec/conf2spec.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6562 2023-05-03 13:21:26.000000 pyp2spec-0.7.0/pyp2spec/license_processor.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    14597 2023-05-03 13:21:18.000000 pyp2spec-0.7.0/pyp2spec/pyp2conf.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      568 2023-05-03 13:21:18.000000 pyp2spec-0.7.0/pyp2spec/pyp2spec.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2604 2023-02-09 12:00:51.000000 pyp2spec-0.7.0/pyp2spec/rpmversion.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1669 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/pyp2spec/template.spec
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.128534 pyp2spec-0.7.0/pyp2spec.egg-info/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     6638 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/PKG-INFO
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1483 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/SOURCES.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        1 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/dependency_links.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      122 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/entry_points.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      135 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/requires.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)        9 2023-05-04 07:51:59.000000 pyp2spec-0.7.0/pyp2spec.egg-info/top_level.txt
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)       89 2022-12-02 12:41:04.000000 pyp2spec-0.7.0/pyproject.toml
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1164 2023-05-04 07:51:59.132534 pyp2spec-0.7.0/setup.cfg
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.129534 pyp2spec-0.7.0/tests/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      608 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/conftest.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.129534 pyp2spec-0.7.0/tests/expected_specfiles/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1234 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/expected_specfiles/python-click.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     1765 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/expected_specfiles/python-markdown-it-py.spec
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     8236 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/fedora_license_data.json
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.126534 pyp2spec-0.7.0/tests/fixtures/
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.131534 pyp2spec-0.7.0/tests/fixtures/cassettes/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    65864 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    11369 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)    25105 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)   381661 2023-04-25 08:18:22.000000 pyp2spec-0.7.0/tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     2869 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     4790 2023-03-07 19:31:45.000000 pyp2spec-0.7.0/tests/test_conf2spec.py
+drwxr-xr-x   0 ksurma    (1000) ksurma    (1000)        0 2023-05-04 07:51:59.131534 pyp2spec-0.7.0/tests/test_configs/
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      386 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_aionotion.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      624 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_boutdata.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      721 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_click.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      791 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_jupyter-packaging.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      928 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_markdown-it-py.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      474 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/customized_tornado.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      372 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/default_python-aionotion.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)      351 2023-04-26 08:33:53.000000 pyp2spec-0.7.0/tests/test_configs/default_python-click.conf
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     3965 2023-04-27 14:27:49.000000 pyp2spec-0.7.0/tests/test_license_processor.py
+-rw-r--r--   0 ksurma    (1000) ksurma    (1000)     9382 2023-04-28 12:11:50.000000 pyp2spec-0.7.0/tests/test_pyp2conf.py
```

### Comparing `pyp2spec-0.6.1/LICENSE-MIT` & `pyp2spec-0.7.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.6.1/LICENSE-MIT-0` & `pyp2spec-0.7.0/LICENSE-MIT-0`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.6.1/PKG-INFO` & `pyp2spec-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp2spec
-Version: 0.6.1
+Version: 0.7.0
 Summary: Generate a valid Fedora specfile from Python package from PyPI
 Home-page: https://github.com/befeleme/pyp2spec/
 Author: Karolina Surma
 Author-email: ksurma@redhat.com
 License: MIT, MIT-0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -100,22 +100,19 @@
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
 | python_name | pypi_name prepended with `python-` | string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
-| release | Fedora package release | string |
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
-| changelog_head | spec file changelog header (date, name, e-mail) | string |
-| changelog_msg | spec file changelog message | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
 
@@ -133,35 +130,32 @@
 | doc_files     | list doc files from the package     | list |
 | archful | package contains compiled extensions | bool |
 
 
 ### Example config file generated by pyp2spec
 
 ```
-changelog_msg = "Package generated with pyp2spec"
-changelog_head = "Tue Sep 21 2021 Name Surname <email@address>"
 description = "This is package 'aionotion' generated automatically by pyp2spec."
 summary = "A simple Python 3 library for Notion Home Monitoring"
 version = "2.0.3"
 license = "MIT"
-release = "1"
 pypi_name = "aionotion"
 pypi_version = %{version}
 python_name = "python-aionotion"
 url = "https://github.com/bachya/aionotion"
 source = "%{pypi_source aionotion}"
 archive_name = "aionotion"
 ```
 
 ### Spec file generated using the example config
 
 ```
 Name:           python-aionotion
 Version:        3.0.2
-Release:        1%{?dist}
+Release:        %autorelease
 Summary:        A simple Python 3 library for Notion Home Monitoring
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        MIT
 URL:            https://github.com/bachya/aionotion
 Source:         %{pypi_source aionotion}
@@ -204,16 +198,15 @@
 %pyproject_check_import
 
 
 %files -n python3-aionotion -f %{pyproject_files}
 
 
 %changelog
-* Tue Sep 21 2021 Name Surname <email@address> - 3.0.2-1
-- Package generated with pyp2spec
+%autochangelog
 ```
 
 
 ## License
 
 The code is licensed under **MIT**.
```

### Comparing `pyp2spec-0.6.1/README.md` & `pyp2spec-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,19 @@
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
 | python_name | pypi_name prepended with `python-` | string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
-| release | Fedora package release | string |
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
-| changelog_head | spec file changelog header (date, name, e-mail) | string |
-| changelog_msg | spec file changelog message | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
 
@@ -113,35 +110,32 @@
 | doc_files     | list doc files from the package     | list |
 | archful | package contains compiled extensions | bool |
 
 
 ### Example config file generated by pyp2spec
 
 ```
-changelog_msg = "Package generated with pyp2spec"
-changelog_head = "Tue Sep 21 2021 Name Surname <email@address>"
 description = "This is package 'aionotion' generated automatically by pyp2spec."
 summary = "A simple Python 3 library for Notion Home Monitoring"
 version = "2.0.3"
 license = "MIT"
-release = "1"
 pypi_name = "aionotion"
 pypi_version = %{version}
 python_name = "python-aionotion"
 url = "https://github.com/bachya/aionotion"
 source = "%{pypi_source aionotion}"
 archive_name = "aionotion"
 ```
 
 ### Spec file generated using the example config
 
 ```
 Name:           python-aionotion
 Version:        3.0.2
-Release:        1%{?dist}
+Release:        %autorelease
 Summary:        A simple Python 3 library for Notion Home Monitoring
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        MIT
 URL:            https://github.com/bachya/aionotion
 Source:         %{pypi_source aionotion}
@@ -184,16 +178,15 @@
 %pyproject_check_import
 
 
 %files -n python3-aionotion -f %{pyproject_files}
 
 
 %changelog
-* Tue Sep 21 2021 Name Surname <email@address> - 3.0.2-1
-- Package generated with pyp2spec
+%autochangelog
 ```
 
 
 ## License
 
 The code is licensed under **MIT**.
```

### Comparing `pyp2spec-0.6.1/pyp2spec/conf2spec.py` & `pyp2spec-0.7.0/pyp2spec/conf2spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from importlib.resources import read_text
 from textwrap import fill
 
 import click
-import tomli
+
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
 
 from jinja2 import Template
 
 
 TEMPLATE_FILENAME = "template.spec"
 
 
@@ -18,15 +22,15 @@
         self.contents = self.load_configuration
 
     @property
     def load_configuration(self):
         """Return loaded TOML configuration file contents."""
 
         with open(self.filename, "rb") as configuration_file:
-            loaded_contents = tomli.load(configuration_file)
+            loaded_contents = tomllib.load(configuration_file)
 
         return loaded_contents
 
     def get_string(self, key):
         """Return a value for given key. Validate the value is a string.
         Raise TypeError otherwise."""
 
@@ -141,26 +145,23 @@
 
     spec_template = Template(read_text("pyp2spec", TEMPLATE_FILENAME))
 
     result = spec_template.render(
         archful=config.get_bool("archful"),
         archive_name=config.get_string("archive_name"),
         binary_files=config.get_list("binary_files"),
-        changelog_head=config.get_string("changelog_head"),
-        changelog_msg=config.get_string("changelog_msg"),
         description=wrap_description(config),
         doc_files=" ".join(config.get_list("doc_files")),
         extra_build_requires=generate_extra_build_requires(config),
         license_files=" ".join(config.get_list("license_files")),
         license=config.get_string("license"),
         manual_build_requires=config.get_list("manual_build_requires"),
         name=config.get_string("pypi_name"),
         python_name=config.get_string("python_name"),
         pypi_version=config.get_string("pypi_version"),
-        release=config.get_string("release"),
         source=config.get_string("source"),
         summary=config.get_string("summary"),
         test_method=generate_check(config),
         test_top_level=config.get_bool("test_top_level"),
         url=config.get_string("url"),
         version=config.get_string("version"),
     )
```

### Comparing `pyp2spec-0.6.1/pyp2spec/pyp2conf.py` & `pyp2spec-0.7.0/pyp2spec/pyp2conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from datetime import date
-from importlib.resources import open_text
-from subprocess import check_output
-import json
+from functools import wraps
 import re
 import sys
 
 import click
 import requests
 import tomli_w
 
 from pyp2spec.rpmversion import RpmVersion
+from pyp2spec.license_processor import classifiers_to_spdx_identifiers
+from pyp2spec.license_processor import license_keyword_to_spdx_identifiers, good_for_fedora
+
+
+class NoLicenseDetectedError(ValueError):
+    """Raised when there's no valid license detected"""
 
 
 class PypiPackage:
-    """Get and save package data from PyPI."""
+    """Store and process the package data obtained from PyPI."""
 
-    def __init__(self, package, session=None):
-        self.package = package
-        self.package_data = self.get_package_metadata(session)
+    def __init__(self, package_name, *, package_metadata=None, session=None):
+        self.package_name = package_name
+        # package_metadata - custom dictionary with package metadata - used for testing
+        # in the typical app run it's not set,
+        # meaning we jump to the other sources package metadata data (eg. PyPI)
+        self.package_data = package_metadata or self.get_package_metadata(session=session)
         self.sdist_filename = None
 
     @property
     def pypi_name(self):
         """Return normalized PyPI package name (as defined in PEP 503).
         The resulting string better conforms with Fedora's Packaging Guidelines.
         """
@@ -29,24 +35,23 @@
         return self.normalize(self.package_data["info"]["name"])
 
     def normalize(self, package_name):
         """Normalize given package name as defined in PEP 503"""
 
         return re.sub(r"[-_.]+", "-", package_name).lower()
 
-    def get_package_metadata(self, session):
-        pkg_index = f"https://pypi.org/pypi/{self.package}/json"
+    def get_package_metadata(self, *,session=None):
+        pkg_index = f"https://pypi.org/pypi/{self.package_name}/json"
         s = session or requests.Session()
-        try:
-            response = s.get(pkg_index).json()
-        except json.decoder.JSONDecodeError:
-            click.secho(f"'{self.package}' was not found on PyPI, did you spell it correctly?", fg="red")
+        response = s.get(pkg_index)
+        if not response.ok:
+            click.secho(f"'{self.package_name}' was not found on PyPI, did you spell it correctly?", fg="red")
             sys.exit(1)
         else:
-            return response
+            return response.json()
 
     def python_name(self):
         if self.pypi_name.startswith("python"):
             return self.pypi_name
         else:
             return f"python-{self.pypi_name}"
 
@@ -87,79 +92,78 @@
         In such case return version string as from PyPI.
         """
         rpm_version = convert_version_to_rpm_scheme(version)
         if version == rpm_version:
             return "%{version}"
         return version
 
-    def license(self, compliant=False):
+    def filter_license_classifiers(self):
+        """Return the list of license classifiers defined for the package.
+
+        Filter out the parent categories `OSI-/DFSG Approved` which don't have any meaning.
+        """
+
+        return  [
+            c for c in self.package_data["info"]["classifiers"]
+            if (
+                c.startswith("License")
+                and c not in ("License :: OSI Approved", "License :: DFSG approved")
+            )
+        ]
+
+    def transform_to_spdx(self):
+        """Return SPDX identifiers and expression based on the found
+        package license metadata (classifiers or license keyword).
+        
+        If multiple identifiers are found, create an expression that's the safest option (with AND as joining operator).
+        Raise ValueError if no valid SPDX identifiers are found.
+        """
+
+        if (license_classifiers := self.filter_license_classifiers()):
+            identifiers = classifiers_to_spdx_identifiers(license_classifiers)
+            if identifiers:
+                expression = " AND ".join(identifiers)
+                return (identifiers, expression)
+
+        license_keyword = self.package_data["info"]["license"]
+        identifiers = license_keyword_to_spdx_identifiers(license_keyword)
+
+        # No more options to detect licenses left, hence explicit fail
+        if not identifiers:
+            raise NoLicenseDetectedError()
+        return (identifiers, license_keyword)
+
+    def license(self, *, check_compliance=False, session=None, licenses_dict=None):
         """Return the license string from package metadata.
 
-        First, check trove classifiers which are the current Python standard:
-        https://www.python.org/dev/peps/pep-0301/#distutils-trove-classification
-        If argument `compliant` is set to True, perform the approximate compliance
-        check of the parsed classifiers with Fedora Good Licenses.
+        If `check_compliance` is set to True, check each of the found
+        SPDX identifiers against the Fedora allowed licenses.
         This isn't a 100% reliable solution and in case of ambiguous results,
         the license is discarded as invalid.
-        Only if a package doesn't define the license in the classifiers, the "license"
-        keyword is checked. There isn't any check whether that value is compliant
-        with Fedora, it is passed to the config file for the user to validate.
-        Some packages fill in "license" with the whole license text.
-        This is indicated by the multiline value and such is discarded as invalid.
-
-        If the license can't be determined from both classifiers and "license"
-        keyword, this fact is logged and the script ended.
+        If the license can't be determined, this fact is printed to stdout and the script ends.
         """
-        click.secho("Attempting to get license from Classifiers", fg="cyan")
-        self.classifiers = self.read_license_classifiers()
-        # Process classifiers further if there are some
-        if self.classifiers:
-            return self.get_license_from_classifiers(compliant)
-        else:
-            click.secho("License in Classifiers not found, looking for the 'License' keyword", fg="cyan")
-            pkg_license = self.package_data["info"]["license"]
-            # Check if license isn't empty and is only one line
-            if pkg_license and len(pkg_license.split("\n")) == 1:
-                return pkg_license
-            else:
-                click.secho("Invalid license field value length, cannot reliably determine the license", fg="red")
 
-        click.secho("License not found. Specify --license explicitly. Quitting", fg="red")
-        sys.exit(1)
+        try:
+            identifiers, expression = self.transform_to_spdx()
+        except NoLicenseDetectedError:
+            click.secho("No valid license detected, Quitting", fg="red")
+            sys.exit(1)
+        except Exception as err:
+            click.secho(err, fg="red")
+            sys.exit(1)
+        if check_compliance:
+            is_compliant, bad_identifiers = good_for_fedora(identifiers, session=session, licenses_dict=licenses_dict)
+            if not is_compliant:
+                if bad_identifiers:
+                    err_string = "The detected licenses: `{0}` aren't allowed in Fedora."
+                    click.secho(err_string.format(", ".join(bad_identifiers), fg="red"))
+                click.secho("Could not create a compliant license field, Quitting", fg="red")
+                sys.exit(1)
 
-    def get_license_from_classifiers(self, compliant):
-        license_map = self.read_license_map()
-        licenses = []
-        for classifier in self.classifiers:
-            short_license, fedora_status = license_map[classifier]
-            # "OSI Approved" is a top-level category which doesn't bring
-            # any valuable information, let's just ignore it when encountered
-            if short_license == "OSI Approved":
-                continue
-            if compliant:
-                # "???" are APSL, Artistic, Eiffel - some versions are Fedora OK,
-                # some not. On PyPI there are <100 packages with them, rather than
-                # adding another layer of decision matrix, just skip them all.
-                if fedora_status in ["BAD", "UNKNOWN", "???"]:
-                    click.secho(f"License '{short_license}' is or may not be allowed in Fedora, quitting", fg="red")
-                    sys.exit(1)
-                else:
-                    licenses.append(short_license)
-            else:
-                licenses.append(short_license)
-        return " and ".join(licenses)
-
-    def read_license_map(self):
-        with open_text("pyp2spec", "classifiers_to_fedora.json") as f:
-            license_map = json.load(f)
-        return license_map
-
-    def read_license_classifiers(self):
-        classifiers = self.package_data["info"]["classifiers"]
-        return [c for c in classifiers if c.startswith("License")]
+        return expression
 
     def summary(self):
         summary = self.package_data["info"]["summary"]
         # summary may not be filled in the upstream data or it can consist of
         # more than one line - in both cases use the autogenerated string
         if not summary or len(summary.split("\n")) > 1:
             summary = "..."
@@ -216,40 +220,14 @@
         for suffix in (".tar.gz", ".zip"):
             edited_sdist_filename = edited_sdist_filename.removesuffix(suffix)
         # Second, get rid of the version string and the delimiter "-"
         archive_name = edited_sdist_filename.replace("-" + version, "")
         return archive_name
 
 
-def changelog_head(email, name, changelog_date):
-    """Return f'{date} {name} <{email}>'"""
-
-    # Date is set for the tests
-    if not changelog_date:
-        changelog_date = (date.today()).strftime("%a %b %d %Y")
-
-    if email or name:
-        return f"{changelog_date} {name} <{email}>"
-
-    try:
-        result = check_output(["rpmdev-packager"])
-        result = result.decode().strip()
-    except FileNotFoundError:
-        # Set a dummy value not to fail on missing changelog data
-        result = "mockbuilder"
-
-    return f"{changelog_date} {result}"
-
-
-def changelog_msg():
-    """Return a default changelog message."""
-
-    return "Initial package"
-
-
 def get_description(package):
     """Return a default package description."""
 
     return f"This is package '{package}' generated automatically by pyp2spec."
 
 
 def convert_version_to_rpm_scheme(version):
@@ -276,83 +254,65 @@
     click.secho(f"Assuming '{package}' is a package name", fg="yellow")
     return True
 
 
 def create_config_contents(
     package,
     description=None,
-    release=None,
-    message=None,
-    email=None,
-    name=None,
     version=None,
     summary=None,
-    date=None,
     session=None,
     license=None,
     compliant=False,
     top_level=False,
     archful=False,
 ):
     """Use `package` and provided kwargs to create the whole config contents.
     Return contents dictionary.
     """
     contents = {}
 
     # a package name was given as the `package`, look for it on PyPI
     if is_package_name(package):
-        pkg = PypiPackage(package, session)
+        pkg = PypiPackage(package, session=session)
         click.secho(f"Querying PyPI for package '{package}'", fg="cyan")
     # a URL was given as the `package`
     else:
         raise NotImplementedError
 
-    # If the arguments weren't provided via CLI,
-    # get them from the stored package object data or the default values
-    if message is None:
-        message = changelog_msg()
-        click.secho(f"Assuming changelog --message={message}", fg="yellow")
-
     if description is None:
         description = get_description(package)
         click.secho(f"Assuming --description={description}", fg="yellow")
 
     if summary is None:
         summary = pkg.summary()
         click.secho(f"Assuming --summary={summary}", fg="yellow")
 
     if version is None:
         version = pkg.version()
         click.secho(f"Assuming PyPI --version={version}", fg="yellow")
 
     if license is None:
-        license = pkg.license(compliant)
+        license = pkg.license(check_compliance=compliant, session=session)
         click.secho(f"Assuming --license={license}", fg="yellow")
 
-    if release is None:
-        release = "1"
-        click.secho(f"Assuming --release={release}", fg="yellow")
-
     if top_level:
         click.secho("Only top-level modules will be checked", fg="yellow")
         contents["test_top_level"] = True
 
     if archful:
         click.secho("Package is set to --archful", fg="magenta")
         click.secho("You may need to specify manual_build_requires in the config file", fg="magenta")
         contents["archful"] = archful
 
-    contents["changelog_msg"] = message
-    contents["changelog_head"] = changelog_head(email, name, date)
     contents["description"] = description
     contents["summary"] = summary
     contents["version"] = convert_version_to_rpm_scheme(version)
     contents["pypi_version"] = pkg.pypi_version_or_macro(version)
     contents["license"] = license
-    contents["release"] = release
     contents["pypi_name"] = pkg.pypi_name
     contents["python_name"] = pkg.python_name()
     contents["url"] = pkg.project_url()
     contents["source"] = pkg.source(version)
     contents["archive_name"] = pkg.archive_name(version)
 
     return contents
@@ -375,77 +335,64 @@
 
 def create_config(options):
     """Create and save config file."""
 
     contents = create_config_contents(
         options["package"],
         description=options["description"],
-        release=options["release"],
-        message=options["message"],
-        email=options["email"],
-        name=options["packager"],
         version=options["version"],
         summary=options["summary"],
         license=options["license"],
         compliant=options["fedora_compliant"],
         top_level=options["top_level"],
         archful=options["archful"],
     )
     return save_config(contents, options["config_output"])
 
 
+def pypconf_args(func):
+    @click.argument("package")
+    @click.option(
+        "--config-output", "-c",
+        help="Provide custom output for configuration file",
+    )
+    @click.option(
+        "--description", "-d",
+        help="Provide description for the package",
+    )
+    @click.option(
+        "--version", "-v",
+        help="Provide package version to query PyPI for, default: latest",
+    )
+    @click.option(
+        "--summary", "-s",
+        help="Provide custom package summary",
+    )
+    @click.option(
+        "--license", "-l",
+        help="Provide license name",
+    )
+    @click.option(
+        "--fedora-compliant", is_flag=True,
+        help="Check whether license is compliant with Fedora",
+    )
+    @click.option(
+        "--top-level", "-t", is_flag=True,
+        help="Test only top-level modules in %check",
+    )
+    @click.option(
+        "--archful", "-a", is_flag=True,
+        help="Set if the resulting RPM should be arched",
+    )
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+    return wrapper
+
 @click.command()
-@click.argument("package")
-@click.option(
-    "--config-output", "-c",
-    help="Provide custom output for configuration file",
-)
-@click.option(
-    "--description", "-d",
-    help="Provide description for the package",
-)
-@click.option(
-    "--release", "-r",
-    help="Provide Fedora release, default: 1",
-)
-@click.option(
-    "--message", "-m",
-    help="Provide custom changelog message for the package",
-)
-@click.option(
-    "--email", "-e",
-    help="Provide e-mail for changelog, default: output of `rpmdev-packager`",
-)
-@click.option(
-    "--packager", "-p",
-    help="Provide packager name for changelog, default: output of `rpmdev-packager`",
-)
-@click.option(
-    "--version", "-v",
-    help="Provide package version to query PyPI for, default: latest",
-)
-@click.option(
-    "--summary", "-s",
-    help="Provide custom package summary",
-)
-@click.option(
-    "--license", "-l",
-    help="Provide license name",
-)
-@click.option(
-    "--fedora-compliant", is_flag=True,
-    help="Check whether license is compliant with Fedora",
-)
-@click.option(
-    "--top-level", "-t", is_flag=True,
-    help="Test only top-level modules in %check",
-)
-@click.option(
-    "--archful", "-a", is_flag=True,
-    help="Set if the resulting RPM should be arched",
-)
+@pypconf_args
 def main(**options):
     create_config(options)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyp2spec-0.6.1/pyp2spec/rpmversion.py` & `pyp2spec-0.7.0/pyp2spec/rpmversion.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.6.1/pyp2spec/template.spec` & `pyp2spec-0.7.0/pyp2spec/template.spec`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name:           {{python_name}}
 Version:        {{version}}
-Release:        {{release}}%{?dist}
+Release:        %autorelease
 Summary:        {{summary}}
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        {{license}}
 URL:            {{url}}
 Source:         {{source}}
@@ -66,9 +66,8 @@
 {% if binary_files -%}
 {% for bf in binary_files -%}
 %{_bindir}/{{bf}}
 {% endfor -%}
 {% endif %}
 
 %changelog
-* {{changelog_head}} - {{version}}-{{release}}
-- {{changelog_msg}}
+%autochangelog
```

### Comparing `pyp2spec-0.6.1/pyp2spec.egg-info/PKG-INFO` & `pyp2spec-0.7.0/pyp2spec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp2spec
-Version: 0.6.1
+Version: 0.7.0
 Summary: Generate a valid Fedora specfile from Python package from PyPI
 Home-page: https://github.com/befeleme/pyp2spec/
 Author: Karolina Surma
 Author-email: ksurma@redhat.com
 License: MIT, MIT-0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -100,22 +100,19 @@
 | Field  | Description | Type |
 | -------- | -------- | -------- |
 | pypi_name | package name as stored in PyPI  | string   |
 | python_name | pypi_name prepended with `python-` | string |
 | archive_name | source tarball name, stripped of version and file extension  | string |
 | version | package version to create spec file for (RPM format) | string |
 | pypi_version | package version string as in PyPI, '%{version}' if the same as version | string
-| release | Fedora package release | string |
 | summary | short package summary | string |
 | license | license name | string |
 | url | project URL | string |
 | source | %{pypi_source} macro with optional arguments (tarball URL can be used instead) | string |
 | description | long package description | multiline string |
-| changelog_head | spec file changelog header (date, name, e-mail) | string |
-| changelog_msg | spec file changelog message | string |
 
 
 ### Optional fields
 
 - Not generated by pyp2conf
 - Can be also added to config files generated by pyp2conf
 
@@ -133,35 +130,32 @@
 | doc_files     | list doc files from the package     | list |
 | archful | package contains compiled extensions | bool |
 
 
 ### Example config file generated by pyp2spec
 
 ```
-changelog_msg = "Package generated with pyp2spec"
-changelog_head = "Tue Sep 21 2021 Name Surname <email@address>"
 description = "This is package 'aionotion' generated automatically by pyp2spec."
 summary = "A simple Python 3 library for Notion Home Monitoring"
 version = "2.0.3"
 license = "MIT"
-release = "1"
 pypi_name = "aionotion"
 pypi_version = %{version}
 python_name = "python-aionotion"
 url = "https://github.com/bachya/aionotion"
 source = "%{pypi_source aionotion}"
 archive_name = "aionotion"
 ```
 
 ### Spec file generated using the example config
 
 ```
 Name:           python-aionotion
 Version:        3.0.2
-Release:        1%{?dist}
+Release:        %autorelease
 Summary:        A simple Python 3 library for Notion Home Monitoring
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        MIT
 URL:            https://github.com/bachya/aionotion
 Source:         %{pypi_source aionotion}
@@ -204,16 +198,15 @@
 %pyproject_check_import
 
 
 %files -n python3-aionotion -f %{pyproject_files}
 
 
 %changelog
-* Tue Sep 21 2021 Name Surname <email@address> - 3.0.2-1
-- Package generated with pyp2spec
+%autochangelog
 ```
 
 
 ## License
 
 The code is licensed under **MIT**.
```

### Comparing `pyp2spec-0.6.1/pyp2spec.egg-info/SOURCES.txt` & `pyp2spec-0.7.0/pyp2spec.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,56 +3,37 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 pyp2spec/__init__.py
 pyp2spec/classifiers_to_fedora.json
 pyp2spec/conf2spec.py
+pyp2spec/license_processor.py
 pyp2spec/pyp2conf.py
 pyp2spec/pyp2spec.py
 pyp2spec/rpmversion.py
 pyp2spec/template.spec
 pyp2spec.egg-info/PKG-INFO
 pyp2spec.egg-info/SOURCES.txt
 pyp2spec.egg-info/dependency_links.txt
 pyp2spec.egg-info/entry_points.txt
 pyp2spec.egg-info/requires.txt
 pyp2spec.egg-info/top_level.txt
+tests/conftest.py
+tests/fedora_license_data.json
 tests/test_conf2spec.py
+tests/test_license_processor.py
 tests/test_pyp2conf.py
 tests/expected_specfiles/python-click.spec
 tests/expected_specfiles/python-markdown-it-py.spec
-tests/fixtures/cassettes/test_pyp2conf.test_OSI_Approved_is_ignored.json
 tests/fixtures/cassettes/test_pyp2conf.test_archful_package.json
 tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[aionotion-2.0.3].json
 tests/fixtures/cassettes/test_pyp2conf.test_automatically_generated_config_is_valid[click-7.1.2].json
-tests/fixtures/cassettes/test_pyp2conf.test_bad_license_if_compliant_is_not_returned.json
-tests/fixtures/cassettes/test_pyp2conf.test_bad_license_if_not_compliant_is_returned.json
-tests/fixtures/cassettes/test_pyp2conf.test_compliant_license_is_returned.json
 tests/fixtures/cassettes/test_pyp2conf.test_config_with_customization_is_valid.json
-tests/fixtures/cassettes/test_pyp2conf.test_license_classifier_read_correctly.json
-tests/fixtures/cassettes/test_pyp2conf.test_mix_non_compliant_licenses_wont_work_if_strict.json
-tests/fixtures/cassettes/test_pyp2conf.test_mix_non_compliant_licenses_work_if_not_strict.json
-tests/fixtures/cassettes/test_pyp2conf.test_no_homepage_in_metadata.json
-tests/fixtures/cassettes/test_pyp2conf.test_no_license_classifiers_and_no_license_keyword.json
-tests/fixtures/cassettes/test_pyp2conf.test_package_without_license_is_not_processed.json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_name_with_capital_letter_is_normalized.json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_name_with_underscore_is_normalized.json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[django-apistar-0.5.40-0-0.5.40-0].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[django-apistar-0.5.40-0-0.5.40^post0].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[javascript-1!0.2.13-1!0.2.13].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[javascript-1!0.2.13-1-0.2.13].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[markdown-it-py-1.1.0-%{version}].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[markdown-it-py-1.1.0-1.1.0].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[python3-wget-0.0.2-beta1-0.0.2-beta1].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[python3-wget-0.0.2-beta1-0.0.2~b1].json
-tests/fixtures/cassettes/test_pyp2conf.test_pypi_version_is_converted_to_rpm[tomli-None-%{version}].json
-tests/fixtures/cassettes/test_pyp2conf.test_summary_is_generated_if_not_in_upstream.json
-tests/fixtures/cassettes/test_pyp2conf.test_summary_is_generated_if_upstream_data_is_multiline.json
-tests/fixtures/cassettes/test_pyp2conf.test_zip_sdist_is_added_to_source_macro.json
+tests/fixtures/cassettes/test_pyp2conf.test_non_existent_package.json
 tests/test_configs/customized_aionotion.conf
 tests/test_configs/customized_boutdata.conf
 tests/test_configs/customized_click.conf
 tests/test_configs/customized_jupyter-packaging.conf
 tests/test_configs/customized_markdown-it-py.conf
 tests/test_configs/customized_tornado.conf
 tests/test_configs/default_python-aionotion.conf
```

### Comparing `pyp2spec-0.6.1/tests/expected_specfiles/python-click.spec` & `pyp2spec-0.7.0/tests/expected_specfiles/python-click.spec`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Name:           python-click
 Version:        7.1.2
-Release:        1%{?dist}
+Release:        %autorelease
 Summary:        Composable command line interface toolkit
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
-License:        BSD
+License:        BSD-3-Clause
 URL:            https://palletsprojects.com/p/click/
 Source:         %{pypi_source click}
 
 BuildArch:      noarch
 BuildRequires:  python3-devel
 
 
@@ -49,9 +49,8 @@
 %pyproject_check_import
 
 
 %files -n python3-click -f %{pyproject_files}
 
 
 %changelog
-* Wed Nov 03 2021 Packager <packager@maint.com> - 7.1.2-1
-- Initial package
+%autochangelog
```

### Comparing `pyp2spec-0.6.1/tests/expected_specfiles/python-markdown-it-py.spec` & `pyp2spec-0.7.0/tests/expected_specfiles/python-markdown-it-py.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Name:           python-markdown-it-py
 Version:        1.1.0
-Release:        3%{?dist}
+Release:        %autorelease
 Summary:        Python port of markdown-it
 
 # Check if the automatically generated License and its spelling is correct for Fedora
 # https://docs.fedoraproject.org/en-US/packaging-guidelines/LicensingGuidelines/
 License:        MIT
 URL:            https://github.com/executablebooks/markdown-it-py
 Source:         %{url}/archive/v%{version}/markdown-it-py-%{version}.tar.gz
@@ -61,9 +61,8 @@
 %files -n python3-markdown-it-py -f %{pyproject_files}
 %doc README.md
 %license LICENSE LICENSE.markdown-it
 %{_bindir}/markdown-it
 
 
 %changelog
-* Fri Jul 23 2021 Package Maintainer <package@maintainer.com> - 1.1.0-3
-- Rebuilt
+%autochangelog
```

### Comparing `pyp2spec-0.6.1/tests/test_conf2spec.py` & `pyp2spec-0.7.0/tests/test_conf2spec.py`

 * *Files identical despite different names*

### Comparing `pyp2spec-0.6.1/tests/test_configs/customized_boutdata.conf` & `pyp2spec-0.7.0/tests/test_configs/customized_boutdata.conf`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 pypi_name = "boutdata"
 pypi_version = "%{version}"
 python_name = "python-boutdata"
 version = "0.1.3"
-release = "0.2"
 summary = "Python package for collecting BOUT++ data"
 license = "LGPLv3+"
 url = "http://boutproject.github.io"
 source = "%{pypi_source boutdata}"
 archive_name = "boutdata"
 description = '''
 Python interface for reading bout++ data files.
@@ -18,10 +17,7 @@
     "python3dist(pytest)",
 ]
 
 test_method = "pytest"
 test_top_level = true
 license_files = ["LICENSE"]
 doc_files = ["README.md"]
-
-changelog_head = "Fri Sep 18 2020 Package Maintainer <package@maintainer.org>"
-changelog_msg = "Initial package."
```

### Comparing `pyp2spec-0.6.1/tests/test_configs/customized_click.conf` & `pyp2spec-0.7.0/tests/test_configs/customized_click.conf`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 pypi_name = "click"
 pypi_version = "%{version}"
 python_name = "python-click"
 version = "7.1.2"
-release = "6"
 summary = "Simple wrapper around optparse for powerful command line utilities"
 license = "BSD"
 url = "https://github.com/mitsuhiko/click"
 source = "%{url}/archive/%{version}/click-%{version}.tar.gz"
 archive_name = "click"
 description = '''
 click is a Python package for creating beautiful command line
@@ -16,10 +15,7 @@
 '''
 
 extra_build_requires = ["tox"]
 test_method = "tox"
 
 license_files = ["LICENSE.rst"]
 doc_files = ["README.rst", "CHANGES.rst"]
-
-changelog_head = "Wed Jun 02 2021 Package Maintainer <package@maintainer.com>"
-changelog_msg = "Rebuilt for Python 3.10"
```

### Comparing `pyp2spec-0.6.1/tests/test_configs/customized_jupyter-packaging.conf` & `pyp2spec-0.7.0/tests/test_configs/customized_jupyter-packaging.conf`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 pypi_name = "jupyter-packaging"
 pypi_version = "%{version}"
 python_name = "python-jupyter-packaging"
 version = "0.10.4"
-release = "2"
 summary = "Tools to help build and install Jupyter Python packages"
 license = "BSD"
 url = "https://github.com/jupyter/jupyter-packaging"
 source = "%{pypi_source jupyter_packaging}"
 archive_name = "jupyter_packaging"
 description = "This package contains utilities for making Python packages with and without accompanying JavaScript packages."
 
@@ -22,10 +21,7 @@
     "test_install",
     "test_install_hybrid",
     "test_run",
 ]
 
 license_files = ["LICENSE"]
 doc_files = ["README.md"]
-
-changelog_head = "Fri Jul 23 2021 Package Maintainer <package@maintainer.com>"
-changelog_msg = "Initial package"
```

### Comparing `pyp2spec-0.6.1/tests/test_configs/customized_markdown-it-py.conf` & `pyp2spec-0.7.0/tests/test_configs/customized_markdown-it-py.conf`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 pypi_name = "markdown-it-py"
 pypi_version = "%{version}"
 python_name = "python-markdown-it-py"
 version = "1.1.0"
-release = "3"
 summary = "Python port of markdown-it"
 license = "MIT"
 url = "https://github.com/executablebooks/markdown-it-py"
 source = "%{url}/archive/v%{version}/markdown-it-py-%{version}.tar.gz"
 archive_name = "markdown-it-py"
 description = '''
 Markdown parser done right. Its features:
@@ -28,10 +27,7 @@
     "test_file",
     "test_linkify",
 ]
 
 license_files = ["LICENSE", "LICENSE.markdown-it"]
 doc_files = ["README.md"]
 binary_files = ["markdown-it"]
-
-changelog_head = "Fri Jul 23 2021 Package Maintainer <package@maintainer.com>"
-changelog_msg = "Rebuilt"
```

