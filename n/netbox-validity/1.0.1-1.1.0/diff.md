# Comparing `tmp/netbox-validity-1.0.1.tar.gz` & `tmp/netbox-validity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.0.1.tar", last modified: Thu Apr 20 18:36:48 2023, max compression
+gzip compressed data, was "netbox-validity-1.1.0.tar", last modified: Wed May  3 23:20:04 2023, max compression
```

## Comparing `netbox-validity-1.0.1.tar` & `netbox-validity-1.1.0.tar`

### file list

```diff
@@ -1,123 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.360661 netbox-validity-1.0.1/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/config_compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/commands/linkscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.360661 netbox-validity-1.0.1/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/nameset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_vdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_scripts/test_run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_utils/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/validity/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/device_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.942199 netbox-validity-1.1.0/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/nameset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/test_result.py
```

### Comparing `netbox-validity-1.0.1/LICENSE` & `netbox-validity-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/PKG-INFO` & `netbox-validity-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.0.1
+Version: 1.1.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 License-File: LICENSE
 
 # Validity: vendor-agnostic configuration compliance
 
 ![CI](https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg)
 ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json)
 ![Python version](https://img.shields.io/badge/Python-3.10+-blue.svg)
-![NetBox version](https://img.shields.io/badge/NetBox-3.4-blue.svg)
+![NetBox version](https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg)
 
 <!--mkdocs-start-->
 ## What?
 Validity is the [NetBox](https://netbox.dev) plugin to deal with configuration compliance. You define compliance tests and Validity checks network device configuration files against these tests. As a result you can find out which devices are provisioned properly (according to the tests you have written) and which are not.
 
 To use validity you need:
 
@@ -85,7 +85,14 @@
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
+
+
+## Quick Start
+
+The short video about first steps with Validity:
+
+[![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
```

### Comparing `netbox-validity-1.0.1/README.md` & `netbox-validity-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Validity: vendor-agnostic configuration compliance
 
 ![CI](https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg)
 ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json)
 ![Python version](https://img.shields.io/badge/Python-3.10+-blue.svg)
-![NetBox version](https://img.shields.io/badge/NetBox-3.4-blue.svg)
+![NetBox version](https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg)
 
 <!--mkdocs-start-->
 ## What?
 Validity is the [NetBox](https://netbox.dev) plugin to deal with configuration compliance. You define compliance tests and Validity checks network device configuration files against these tests. As a result you can find out which devices are provisioned properly (according to the tests you have written) and which are not.
 
 To use validity you need:
 
@@ -37,7 +37,14 @@
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
+
+
+## Quick Start
+
+The short video about first steps with Validity:
+
+[![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
```

### Comparing `netbox-validity-1.0.1/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.1.0/netbox_validity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.0.1
+Version: 1.1.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 License-File: LICENSE
 
 # Validity: vendor-agnostic configuration compliance
 
 ![CI](https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg)
 ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json)
 ![Python version](https://img.shields.io/badge/Python-3.10+-blue.svg)
-![NetBox version](https://img.shields.io/badge/NetBox-3.4-blue.svg)
+![NetBox version](https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg)
 
 <!--mkdocs-start-->
 ## What?
 Validity is the [NetBox](https://netbox.dev) plugin to deal with configuration compliance. You define compliance tests and Validity checks network device configuration files against these tests. As a result you can find out which devices are provisioned properly (according to the tests you have written) and which are not.
 
 To use validity you need:
 
@@ -85,7 +85,14 @@
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
+
+
+## Quick Start
+
+The short video about first steps with Validity:
+
+[![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
```

### Comparing `netbox-validity-1.0.1/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-1.1.0/netbox_validity.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 validity/tables.py
 validity/urls.py
 validity/api/__init__.py
 validity/api/helpers.py
 validity/api/serializers.py
 validity/api/urls.py
 validity/api/views.py
-validity/config_compliance/device_config.py
 validity/config_compliance/dynamic_pairs.py
 validity/config_compliance/exceptions.py
+validity/config_compliance/device_config/__init__.py
+validity/config_compliance/device_config/base.py
+validity/config_compliance/device_config/routeros.py
+validity/config_compliance/device_config/ttp.py
+validity/config_compliance/device_config/yaml.py
 validity/config_compliance/eval/__init__.py
 validity/config_compliance/eval/default_nameset.py
 validity/config_compliance/eval/eval.py
 validity/config_compliance/eval/eval_defaults.py
 validity/forms/__init__.py
 validity/forms/filterset.py
 validity/forms/general.py
@@ -79,14 +83,16 @@
 validity/tests/test_models/test_git_link.py
 validity/tests/test_models/test_git_repo.py
 validity/tests/test_models/test_selector.py
 validity/tests/test_models/test_vdevice.py
 validity/tests/test_scripts/conftest.py
 validity/tests/test_scripts/test_run_tests.py
 validity/tests/test_utils/test_git.py
+validity/tests/test_utils/test_misc.py
+validity/utils/config.py
 validity/utils/git.py
 validity/utils/misc.py
 validity/utils/password.py
 validity/views/__init__.py
 validity/views/device.py
 validity/views/git_repo.py
 validity/views/nameset.py
```

### Comparing `netbox-validity-1.0.1/pyproject.toml` & `netbox-validity-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.0.1"
+version = "1.1.0"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-1.0.1/validity/__init__.py` & `netbox-validity-1.1.0/validity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.0.1"
+    version = "1.1.0"
     base_url = "validity"
     django_apps = ["bootstrap5"]
 
     def ready(self):
         try:
             os.makedirs(settings.git_folder, exist_ok=True)
         except OSError as e:
```

### Comparing `netbox-validity-1.0.1/validity/api/helpers.py` & `netbox-validity-1.1.0/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/api/serializers.py` & `netbox-validity-1.1.0/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/api/urls.py` & `netbox-validity-1.1.0/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/api/views.py` & `netbox-validity-1.1.0/validity/api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from http import HTTPStatus
 
-from drf_yasg.utils import swagger_auto_schema
 from netbox.api.viewsets import NetBoxModelViewSet
+from netbox.settings import VERSION
 from rest_framework.exceptions import NotFound
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from validity import filtersets, models
 from validity.config_compliance.device_config import DeviceConfig
 from ..config_compliance.exceptions import DeviceConfigError
 from . import serializers
 
 
+if VERSION.split(".") < ["3", "5"]:
+    from drf_yasg.utils import swagger_auto_schema as extend_schema
+else:
+    from drf_spectacular.utils import extend_schema
+
+
 class ReadOnlyNetboxViewSet(NetBoxModelViewSet):
     http_method_names = ["get", "head", "options", "trace"]
 
 
 class ComplianceSelectorViewSet(NetBoxModelViewSet):
     queryset = models.ComplianceSelector.objects.prefetch_related(
         "tag_filter",
@@ -71,15 +77,15 @@
 
     def get_object(self, pk):
         try:
             return self.queryset.get(pk=pk)
         except models.VDevice.DoesNotExist:
             raise NotFound
 
-    @swagger_auto_schema(
+    @extend_schema(
         responses={200: serializers.SerializedConfigSerializer()}, operation_id="dcim_devices_serialized_config"
     )
     def get(self, request, pk):
         device = self.get_object(pk)
         try:
             config = DeviceConfig.from_device(device)
             serializer = serializers.SerializedConfigSerializer(config, context={"request": request})
```

### Comparing `netbox-validity-1.0.1/validity/choices.py` & `netbox-validity-1.1.0/validity/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     MIDDLE = "MIDDLE", _("MIDDLE"), "yellow"
     HIGH = "HIGH", _("HIGH"), "red"
 
 
 class ConfigExtractionChoices(TextChoices, metaclass=ColoredChoiceMeta):
     TTP = "TTP", "TTP", "purple"
     YAML = "YAML", "YAML", "info"
+    ROUTEROS = "ROUTEROS", "ROUTEROS", "green"
 
 
 class DeviceGroupByChoices(TextChoices):
     DEVICE = "device__name", _("Device")
     DEVICE_TYPE = "device__device_type__slug", _("Device Type")
     MANUFACTURER = "device__device_type__manufacturer__slug", _("Manufacturer")
     DEVICE_ROLE = "device__device_role__slug", _("Device Role")
```

### Comparing `netbox-validity-1.0.1/validity/config_compliance/dynamic_pairs.py` & `netbox-validity-1.1.0/validity/config_compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/config_compliance/eval/default_nameset.py` & `netbox-validity-1.1.0/validity/config_compliance/eval/default_nameset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from builtins import *  # noqa
 
 import jq as pyjq
 
-from validity.utils.misc import config  # noqa
+from validity.utils.config import config  # noqa
 
 
 builtins = [
     "abs",
     "all",
     "any",
     "ascii",
```

### Comparing `netbox-validity-1.0.1/validity/config_compliance/eval/eval.py` & `netbox-validity-1.1.0/validity/config_compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/config_compliance/eval/eval_defaults.py` & `netbox-validity-1.1.0/validity/config_compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/filtersets.py` & `netbox-validity-1.1.0/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/forms/filterset.py` & `netbox-validity-1.1.0/validity/forms/filterset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dcim.models import Device, DeviceRole, DeviceType, Location, Manufacturer, Platform, Site
-from django.forms import CharField, Form, NullBooleanField
+from django.forms import CharField, Form, NullBooleanField, Select
 from django.utils.translation import gettext_lazy as _
-from netbox.forms import NetBoxModelFilterSetForm, StaticSelect
+from netbox.forms import NetBoxModelFilterSetForm
 from tenancy.models import Tenant
 from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
 from utilities.forms.fields import DynamicModelMultipleChoiceField
 
 from validity import models
 from validity.choices import (
     BoolOperationChoices,
@@ -85,26 +85,24 @@
         choices=DeviceGroupByChoices.choices,
     )
 
 
 class NameSetFilterForm(NetBoxModelFilterSetForm):
     model = models.NameSet
     name = CharField(required=False)
-    _global = NullBooleanField(
-        label=_("Global"), required=False, widget=StaticSelect(choices=BOOLEAN_WITH_BLANK_CHOICES)
-    )
+    _global = NullBooleanField(label=_("Global"), required=False, widget=Select(choices=BOOLEAN_WITH_BLANK_CHOICES))
     repo_id = DynamicModelMultipleChoiceField(
         label=_("Git Repository"), queryset=models.GitRepo.objects.all(), required=False
     )
 
 
 class GitRepoFilterForm(NetBoxModelFilterSetForm):
     model = models.GitRepo
     name = CharField(required=False)
-    default = NullBooleanField(required=False, widget=StaticSelect(choices=BOOLEAN_WITH_BLANK_CHOICES))
+    default = NullBooleanField(required=False, widget=Select(choices=BOOLEAN_WITH_BLANK_CHOICES))
     username = CharField(required=False)
     branch = CharField(required=False)
     head_hash = CharField(required=False)
 
 
 class ComplianceSelectorFilterForm(NetBoxModelFilterSetForm):
     model = models.ComplianceSelector
```

### Comparing `netbox-validity-1.0.1/validity/forms/general.py` & `netbox-validity-1.1.0/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/forms/helpers.py` & `netbox-validity-1.1.0/validity/forms/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Sequence
 
-from django.forms import ChoiceField
-from utilities.forms import StaticSelect
+from django.forms import ChoiceField, Select
 
 
-class SelectWithPlaceholder(StaticSelect):
+class SelectWithPlaceholder(Select):
+    def __init__(self, attrs=None, choices=()) -> None:
+        super().__init__(attrs, choices)
+        self.attrs["class"] = "netbox-static-select"
+
     def create_option(self, name, value, label, selected, index: int, subindex=..., attrs=...):
         option = super().create_option(name, value, label, selected, index, subindex, attrs)
         if index == 0:
             option["attrs"]["data-placeholder"] = "true"
         return option
```

### Comparing `netbox-validity-1.0.1/validity/management/commands/linkscripts.py` & `netbox-validity-1.1.0/validity/management/commands/linkscripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/managers.py` & `netbox-validity-1.1.0/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/migrations/0001_initial.py` & `netbox-validity-1.1.0/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/migrations/0002_custom_fields.py` & `netbox-validity-1.1.0/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/base.py` & `netbox-validity-1.1.0/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/device.py` & `netbox-validity-1.1.0/validity/models/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 
 from validity.config_compliance.device_config import DeviceConfig
 from validity.managers import VDeviceQS
 from .repo import GitRepo
 from .serializer import ConfigSerializer
 
 
+def encrypted_password_to_field(json_repo: dict) -> None:
+    json_repo["encrypted_password"] = GitRepo._meta.get_field("encrypted_password").to_python(
+        json_repo["encrypted_password"]
+    )
+
+
 class VDevice(Device):
     objects = VDeviceQS.as_manager()
 
     class Meta:
         proxy = True
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.selector = None
 
     def annotated_repo(self) -> GitRepo | None:
         if not getattr(self, "json_repo", None):
             return
-        self.json_repo["encrypted_password"] = GitRepo._meta.get_field("encrypted_password").to_python(
-            self.json_repo["encrypted_password"]
-        )
+        encrypted_password_to_field(self.json_repo)
         return GitRepo(**self.json_repo)
 
     @cached_property
     def repo(self) -> GitRepo | None:
         if annotated := self.annotated_repo():
             return annotated
         default = GitRepo.objects.filter(default=True).first()
@@ -39,14 +43,15 @@
         except AttributeError:
             return
 
     def annotated_serializer(self) -> ConfigSerializer | None:
         if not getattr(self, "json_serializer", None):
             return
         if getattr(self, "json_serializer_repo", None):
+            encrypted_password_to_field(self.json_serializer_repo)
             self.json_serializer["repo"] = GitRepo(**self.json_serializer_repo)
         return ConfigSerializer(**self.json_serializer)
 
     @cached_property
     def serializer(self) -> ConfigSerializer | None:
         if annotated := self.annotated_serializer():
             return annotated
```

### Comparing `netbox-validity-1.0.1/validity/models/nameset.py` & `netbox-validity-1.1.0/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/repo.py` & `netbox-validity-1.1.0/validity/models/repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/selector.py` & `netbox-validity-1.1.0/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/serializer.py` & `netbox-validity-1.1.0/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/test.py` & `netbox-validity-1.1.0/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/models/test_result.py` & `netbox-validity-1.1.0/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/navigation.py` & `netbox-validity-1.1.0/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/scripts/git.py` & `netbox-validity-1.1.0/validity/scripts/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/scripts/run_tests.py` & `netbox-validity-1.1.0/validity/scripts/run_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import builtins
 import time
 from inspect import getmembers
 from itertools import chain
 from typing import Any, Callable, Generator, Iterable
 
 import yaml
+from dcim.models import Device
 from django.db.models import QuerySet
 from django.utils.translation import gettext as __
 from extras.choices import ObjectChangeActionChoices
 from extras.scripts import BooleanVar, MultiObjectVar, Script
 from extras.webhooks import enqueue_object
 from netbox.context import webhooks_queue
 from simpleeval import InvalidExpression
@@ -37,15 +38,26 @@
     sync_repos = BooleanVar(
         required=False,
         default=False,
         label=__("Sync Repositories"),
         description=__("Pull updates from all available git repositories before running the tests"),
     )
     make_report = BooleanVar(default=True, label=__("Make Compliance Report"))
-    selectors = MultiObjectVar(model=ComplianceSelector, required=False, label=__("Specific selectors"))
+    selectors = MultiObjectVar(
+        model=ComplianceSelector,
+        required=False,
+        label=__("Specific selectors"),
+        description=__("Run the tests only for specific selectors"),
+    )
+    devices = MultiObjectVar(
+        model=Device,
+        required=False,
+        label=__("Specific devices"),
+        description=__("Run the tests only for specific devices"),
+    )
 
     class Meta:
         name = __("Run Compliance Tests")
         description = __("Execute compliance tests and save the results")
 
     def __init__(self):
         super().__init__()
@@ -87,14 +99,15 @@
         tests_qs: QuerySet[ComplianceTest],
         device: VDevice,
         report: ComplianceReport | None,
     ) -> Generator[ComplianceTestResult, None, None]:
         for test in tests_qs:
             explanation = []
             try:
+                device.config
                 passed, explanation = self.run_test(device, test)
             except (InvalidExpression, EvalError) as e:
                 self.log_failure(f"Failed to execute test *{test}* for device *{device}*, `{type(e).__name__}: {e}`")
                 passed = False
                 explanation.append((f"{type(e).__name__}: {e}", None))
             self.results_count += 1
             self.results_passed += int(passed)
@@ -105,17 +118,23 @@
                 explanation=explanation,
                 report=report,
                 dynamic_pair=device.dynamic_pair,
             )
             time.sleep(self._sleep_between_tests)
 
     def run_tests_for_selector(
-        self, selector: ComplianceSelector, report: ComplianceReport | None
+        self,
+        selector: ComplianceSelector,
+        report: ComplianceReport | None,
+        device_ids: list[int],
     ) -> Generator[ComplianceTestResult, None, None]:
-        for device in selector.devices.select_related().annotate_json_serializer().annotate_json_repo():
+        qs = selector.devices.select_related().annotate_json_serializer().annotate_json_repo()
+        if device_ids:
+            qs = qs.filter(pk__in=device_ids)
+        for device in qs:
             try:
                 device.selector = selector
                 yield from self.run_tests_for_device(selector.tests.all(), device, report)
             except DeviceConfigError as e:
                 self.log_failure(f"`{e}`, ignoring all tests for *{device}*")
                 continue
 
@@ -132,17 +151,20 @@
 
     def run(self, data, commit):
         if data.get("sync_repos"):
             self.update_git_repos(GitRepo.objects.all())
         with null_request():
             report = ComplianceReport.objects.create() if data.get("make_report") else None
         selectors = ComplianceSelector.objects.prefetch_related("tests", "tests__namesets")
+        device_ids = data.get("devices", [])
         if specific_selectors := data.get("selectors"):
             selectors = selectors.filter(pk__in=specific_selectors)
-        results = [*chain.from_iterable(self.run_tests_for_selector(selector, report) for selector in selectors)]
+        results = [
+            *chain.from_iterable(self.run_tests_for_selector(selector, report, device_ids) for selector in selectors)
+        ]
         self.save_to_db(results, report)
         output = {"results": {"all": self.results_count, "passed": self.results_passed}}
         if report:
             self.log_info(f"See [Compliance Report]({report.get_absolute_url()}) for detailed statistics")
             self.fire_report_webhook(report.pk)
         return yaml.dump(output, sort_keys=False)
```

### Comparing `netbox-validity-1.0.1/validity/tables.py` & `netbox-validity-1.1.0/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/compliance_results.html` & `netbox-validity-1.1.0/validity/templates/validity/compliance_results.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/compliancereport.html` & `netbox-validity-1.1.0/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/complianceselector.html` & `netbox-validity-1.1.0/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/compliancetest.html` & `netbox-validity-1.1.0/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.1.0/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/configserializer.html` & `netbox-validity-1.1.0/validity/templates/validity/configserializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/device_config.html` & `netbox-validity-1.1.0/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/gitrepo.html` & `netbox-validity-1.1.0/validity/templates/validity/gitrepo.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templates/validity/nameset.html` & `netbox-validity-1.1.0/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/templatetags/validity.py` & `netbox-validity-1.1.0/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/base.py` & `netbox-validity-1.1.0/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/conftest.py` & `netbox-validity-1.1.0/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/factories.py` & `netbox-validity-1.1.0/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_api.py` & `netbox-validity-1.1.0/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_config_compliance/test_dynamic_pairs.py` & `netbox-validity-1.1.0/validity/tests/test_config_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_config_compliance/test_eval.py` & `netbox-validity-1.1.0/validity/tests/test_config_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_models/test_clean.py` & `netbox-validity-1.1.0/validity/tests/test_models/test_clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
 
 
 class TestSerializer(BaseTestClean):
     factory = SerializerGitFactory
 
     right_kwargs = [
         {"extraction_method": "TTP", "ttp_template": "interface {{ interface }}", "repo": None, "file_path": ""},
-        {"extraction_method": "JSON", "repo": None, "file_path": ""},
+        {"extraction_method": "YAML", "repo": None, "file_path": ""},
     ]
     wrong_kwargs = [
         {"extraction_method": "TTP", "ttp_template": "", "repo": None, "file_path": ""},
         {"extraction_method": "TTP", "ttp_template": "qwerty", "file_path": ""},
-        {"extraction_method": "JSON"},
+        {"extraction_method": "YAML"},
     ]
 
 
 class TestTest(BaseTestClean):
     factory = CompTestGitFactory
 
     right_kwargs = [{"expression": "a==1", "repo": None, "file_path": ""}, {}]
```

### Comparing `netbox-validity-1.0.1/validity/tests/test_models/test_git_link.py` & `netbox-validity-1.1.0/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_models/test_git_repo.py` & `netbox-validity-1.1.0/validity/tests/test_models/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_models/test_selector.py` & `netbox-validity-1.1.0/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_models/test_vdevice.py` & `netbox-validity-1.1.0/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-1.1.0/validity/tests/test_scripts/test_run_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         name="selector",
         **{
             "devices.select_related.return_value"
             ".annotate_json_serializer.return_value.annotate_json_repo.return_value": devices
         }
     )
     report = Mock()
-    list(script.run_tests_for_selector(selector, report))
+    list(script.run_tests_for_selector(selector, report, []))
     assert script.run_tests_for_device.call_count == len(devices)
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[0], report)
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[1], report)
     assert devices[0].selector == selector
 
 
 @pytest.mark.django_db
```

### Comparing `netbox-validity-1.0.1/validity/tests/test_utils/test_git.py` & `netbox-validity-1.1.0/validity/tests/test_utils/test_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/tests/test_views.py` & `netbox-validity-1.1.0/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/urls.py` & `netbox-validity-1.1.0/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/utils/git.py` & `netbox-validity-1.1.0/validity/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/utils/misc.py` & `netbox-validity-1.1.0/validity/utils/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from contextlib import contextmanager
 
-from dcim.models import Device
 from django.utils.html import format_html
 from netbox.context import current_request
 
-from validity.models import VDevice
-
 
 def colorful_percentage(percent: float) -> str:
     levels = {75: "warning", 50: "orange", 25: "danger"}
     badge_color = "success"
     for level, color in levels.items():
         if level <= percent:
             break
@@ -18,15 +15,25 @@
     return format_html('<span class="badge rounded-pill bg-{}">{}%</span>', badge_color, percent)
 
 
 @contextmanager
 def null_request():
     ctx = current_request.get()
     current_request.set(None)
-    yield
-    current_request.set(ctx)
+    try:
+        yield
+    finally:
+        current_request.set(ctx)
 
 
-def config(device: Device) -> dict | list | None:
-    vdevice = VDevice()
-    vdevice.__dict__ = device.__dict__.copy()
-    return vdevice.config
+@contextmanager
+def reraise(catch: type[Exception] | tuple[type[Exception], ...], raise_: type[Exception], msg: str | None = None):
+    try:
+        yield
+    except raise_:
+        raise
+    except catch as e:
+        if msg:
+            msg = msg.format(str(e))
+        else:
+            msg = str(e)
+        raise raise_(msg) from e
```

### Comparing `netbox-validity-1.0.1/validity/utils/password.py` & `netbox-validity-1.1.0/validity/utils/password.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/__init__.py` & `netbox-validity-1.1.0/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/device.py` & `netbox-validity-1.1.0/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/git_repo.py` & `netbox-validity-1.1.0/validity/views/git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/nameset.py` & `netbox-validity-1.1.0/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/report.py` & `netbox-validity-1.1.0/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/selector.py` & `netbox-validity-1.1.0/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/serializer.py` & `netbox-validity-1.1.0/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/test.py` & `netbox-validity-1.1.0/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.1/validity/views/test_result.py` & `netbox-validity-1.1.0/validity/views/test_result.py`

 * *Files identical despite different names*

