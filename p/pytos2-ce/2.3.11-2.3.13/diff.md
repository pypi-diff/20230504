# Comparing `tmp/pytos2-ce-2.3.11.tar.gz` & `tmp/pytos2-ce-2.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytos2-ce-2.3.11.tar", last modified: Thu May  4 12:57:39 2023, max compression
+gzip compressed data, was "pytos2-ce-2.3.13.tar", last modified: Thu May  4 13:08:02 2023, max compression
```

## Comparing `pytos2-ce-2.3.11.tar` & `pytos2-ce-2.3.13.tar`

### file list

```diff
@@ -1,560 +1,566 @@
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262896 pytos2-ce-2.3.11/
--rw-r--r--   0 ploch      (502) staff       (20)       80 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/.gitignore
--rw-r--r--   0 ploch      (502) staff       (20)      631 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/.gitlab-ci.yml
--rw-r--r--   0 ploch      (502) staff       (20)     5628 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/CHANGELOG.md
--rw-r--r--   0 ploch      (502) staff       (20)    10781 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/LICENSE
--rw-r--r--   0 ploch      (502) staff       (20)     8527 2023-05-04 12:57:39.262681 pytos2-ce-2.3.11/PKG-INFO
--rw-r--r--   0 ploch      (502) staff       (20)     8369 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/README.md
--rw-r--r--   0 ploch      (502) staff       (20)       44 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/dev-requirements.txt
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.068799 pytos2-ce-2.3.11/doc/
--rw-r--r--   0 ploch      (502) staff       (20)       72 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/.env
--rw-r--r--   0 ploch      (502) staff       (20)      222 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/Jupyter Notebook Setup.md
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.071541 pytos2-ce-2.3.11/doc/assets/
--rw-r--r--   0 ploch      (502) staff       (20)   176021 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-closed.png
--rw-r--r--   0 ploch      (502) staff       (20)   182801 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-1.png
--rw-r--r--   0 ploch      (502) staff       (20)   188759 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-1.png
--rw-r--r--   0 ploch      (502) staff       (20)   181652 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-2.png
--rw-r--r--   0 ploch      (502) staff       (20)   185275 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2.png
--rw-r--r--   0 ploch      (502) staff       (20)   187802 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-3.png
--rw-r--r--   0 ploch      (502) staff       (20)      640 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/init.py
--rw-r--r--   0 ploch      (502) staff       (20)    58633 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/pytos2-ce.ipynb
--rw-r--r--   0 ploch      (502) staff       (20)       89 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/mypy.ini
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.071925 pytos2-ce-2.3.11/pytos2/
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.072057 pytos2-ce-2.3.11/pytos2/api/
--rw-r--r--   0 ploch      (502) staff       (20)     4051 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/api/__init__.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.072329 pytos2-ce-2.3.11/pytos2/models/
--rw-r--r--   0 ploch      (502) staff       (20)     1197 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/models/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/py.typed
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.073418 pytos2-ce-2.3.11/pytos2/secureapp/
--rw-r--r--   0 ploch      (502) staff       (20)      112 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)      731 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/api.py
--rw-r--r--   0 ploch      (502) staff       (20)      713 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/application_identities.py
--rw-r--r--   0 ploch      (502) staff       (20)     1799 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/entrypoint.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.078412 pytos2-ce-2.3.11/pytos2/securechange/
--rw-r--r--   0 ploch      (502) staff       (20)      172 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)     4015 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/api.py
--rw-r--r--   0 ploch      (502) staff       (20)     8022 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/designer.py
--rw-r--r--   0 ploch      (502) staff       (20)     7928 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/designer_verifier_common.py
--rw-r--r--   0 ploch      (502) staff       (20)      205 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/device.py
--rw-r--r--   0 ploch      (502) staff       (20)     9789 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/entrypoint.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.079343 pytos2-ce-2.3.11/pytos2/securechange/fields/
--rw-r--r--   0 ploch      (502) staff       (20)    58171 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)      414 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/binding.py
--rw-r--r--   0 ploch      (502) staff       (20)    20740 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/rule_operation.py
--rw-r--r--   0 ploch      (502) staff       (20)    10020 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/network_object.py
--rw-r--r--   0 ploch      (502) staff       (20)     8168 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/risk_results.py
--rw-r--r--   0 ploch      (502) staff       (20)     2756 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/rule.py
--rw-r--r--   0 ploch      (502) staff       (20)   104439 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/service.py
--rw-r--r--   0 ploch      (502) staff       (20)    22932 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/ticket.py
--rw-r--r--   0 ploch      (502) staff       (20)    13112 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/trigger.py
--rw-r--r--   0 ploch      (502) staff       (20)     3309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/user.py
--rw-r--r--   0 ploch      (502) staff       (20)     4518 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/verifier.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.085095 pytos2-ce-2.3.11/pytos2/securetrack/
--rw-r--r--   0 ploch      (502) staff       (20)       77 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)    10363 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/api.py
--rw-r--r--   0 ploch      (502) staff       (20)     6456 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/device.py
--rw-r--r--   0 ploch      (502) staff       (20)      283 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/domain.py
--rw-r--r--   0 ploch      (502) staff       (20)    77507 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/entrypoint.py
--rw-r--r--   0 ploch      (502) staff       (20)      293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_device.py
--rw-r--r--   0 ploch      (502) staff       (20)      447 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_ignored_interface.py
--rw-r--r--   0 ploch      (502) staff       (20)      727 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_interface.py
--rw-r--r--   0 ploch      (502) staff       (20)      519 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_interface_customer.py
--rw-r--r--   0 ploch      (502) staff       (20)      620 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_route.py
--rw-r--r--   0 ploch      (502) staff       (20)      830 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_transparent_firewall.py
--rw-r--r--   0 ploch      (502) staff       (20)      582 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_vpn.py
--rw-r--r--   0 ploch      (502) staff       (20)     3325 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/interface.py
--rw-r--r--   0 ploch      (502) staff       (20)      368 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/join_cloud.py
--rw-r--r--   0 ploch      (502) staff       (20)    16797 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securetrack/network_object.py
--rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/policy_browser.py
--rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/revision.py
--rw-r--r--   0 ploch      (502) staff       (20)    14109 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/rule.py
--rw-r--r--   0 ploch      (502) staff       (20)     6998 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/service_object.py
--rw-r--r--   0 ploch      (502) staff       (20)      237 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/topology.py
--rw-r--r--   0 ploch      (502) staff       (20)     2677 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/zone.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.085550 pytos2-ce-2.3.11/pytos2/utils/
--rw-r--r--   0 ploch      (502) staff       (20)    13996 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/utils/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)     3127 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/utils/cache.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.086537 pytos2-ce-2.3.11/pytos2_ce.egg-info/
--rw-r--r--   0 ploch      (502) staff       (20)     8527 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/PKG-INFO
--rw-r--r--   0 ploch      (502) staff       (20)    23801 2023-05-04 12:57:39.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/SOURCES.txt
--rw-r--r--   0 ploch      (502) staff       (20)        1 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/dependency_links.txt
--rw-r--r--   0 ploch      (502) staff       (20)      129 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/requires.txt
--rw-r--r--   0 ploch      (502) staff       (20)        7 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/top_level.txt
--rw-r--r--   0 ploch      (502) staff       (20)      106 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/requirements.txt
--rw-r--r--   0 ploch      (502) staff       (20)       38 2023-05-04 12:57:39.263069 pytos2-ce-2.3.11/setup.cfg
--rw-r--r--   0 ploch      (502) staff       (20)      812 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/setup.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.087146 pytos2-ce-2.3.11/tests/
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)     4555 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/api_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.087828 pytos2-ce-2.3.11/tests/secureapp/
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)      914 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/conftest.py
--rw-r--r--   0 ploch      (502) staff       (20)      610 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/entrypoint_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.088008 pytos2-ce-2.3.11/tests/secureapp/json/
--rw-r--r--   0 ploch      (502) staff       (20)  1337893 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/json/application_identities.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.093084 pytos2-ce-2.3.11/tests/securechange/
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)     3511 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/api_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     8758 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/ar_service_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     8399 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/conftest.py
--rw-r--r--   0 ploch      (502) staff       (20)    25461 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/designer_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     3575 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/tests/securechange/entrypoint_test.py
--rw-r--r--   0 ploch      (502) staff       (20)    28797 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/fields_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.093364 pytos2-ce-2.3.11/tests/securechange/files/
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/files/test.pdf
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.094334 pytos2-ce-2.3.11/tests/securechange/json/
--rw-r--r--   0 ploch      (502) staff       (20)    35674 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/all_fields-workflow.json
--rw-r--r--   0 ploch      (502) staff       (20)      201 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/application_details.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.099419 pytos2-ce-2.3.11/tests/securechange/json/designer/
--rw-r--r--   0 ploch      (502) staff       (20)      663 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_icmp_service_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)     1854 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_group_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)      726 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_host_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)      755 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_range_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)      667 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_subnet_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)     9066 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)     4094 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule_any_service-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)     1721 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_service_group-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)      678 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_transport_service_object-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)     7682 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_251.json
--rw-r--r--   0 ploch      (502) staff       (20)    20023 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_instruction_update_rule.json
--rw-r--r--   0 ploch      (502) staff       (20)    19907 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results.json
--rw-r--r--   0 ploch      (502) staff       (20)   113035 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results_multi_instructions.json
--rw-r--r--   0 ploch      (502) staff       (20)      171 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/fully_implemented-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)      217 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/fully_implemented_since_no_security-instruction.json
--rw-r--r--   0 ploch      (502) staff       (20)    13618 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/update_rule-instruction.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.104958 pytos2-ce-2.3.11/tests/securechange/json/field/
--rw-r--r--   0 ploch      (502) staff       (20)      117 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/approve_reject-field.json
--rw-r--r--   0 ploch      (502) staff       (20)       91 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/checkbox-field.json
--rw-r--r--   0 ploch      (502) staff       (20)     1159 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/clone_server_policy_request-field.json
--rw-r--r--   0 ploch      (502) staff       (20)       84 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/date-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      262 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/drop_down_list-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      110 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/hyperlink-field.json
--rw-r--r--   0 ploch      (502) staff       (20)       78 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/manager-field.json
--rw-r--r--   0 ploch      (502) staff       (20)     3986 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request-field.json
--rw-r--r--   0 ploch      (502) staff       (20)     9895 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_all_service_types.json
--rw-r--r--   0 ploch      (502) staff       (20)     2128 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_designer_results-field.json
--rw-r--r--   0 ploch      (502) staff       (20)    21739 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json
--rw-r--r--   0 ploch      (502) staff       (20)    13017 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json.old
--rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_hyperlink-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      163 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_network_object-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      868 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_server_decommission_request-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      142 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_service-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      123 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_target-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      181 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_text_area-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      204 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_text_field-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multiple_selection-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      129 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/read_only-field.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.105141 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/
--rw-r--r--   0 ploch      (502) staff       (20)    43082 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/source_mod.json
--rw-r--r--   0 ploch      (502) staff       (20)    10726 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification_field-field.json
--rw-r--r--   0 ploch      (502) staff       (20)      119 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/text_area-field.json
--rw-r--r--   0 ploch      (502) staff       (20)       88 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/text_field-field.json
--rw-r--r--   0 ploch      (502) staff       (20)       78 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/time-field.json
--rw-r--r--   0 ploch      (502) staff       (20)    34462 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/risk_results_ticket.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.114620 pytos2-ce-2.3.11/tests/securechange/json/ticket/
--rw-r--r--   0 ploch      (502) staff       (20)    32220 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/all_fields-ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)     5565 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/closed_group_modify-ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)    12132 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/dynamic_assignment-ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)    50426 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_access_request-ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)    20839 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_group_modify-ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)      215 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/post_bad_ticket.json
--rw-r--r--   0 ploch      (502) staff       (20)    21757 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/redo.json
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/specific_workflow.json
--rw-r--r--   0 ploch      (502) staff       (20)      153 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_not_found.json
--rw-r--r--   0 ploch      (502) staff       (20)   346577 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_assigned.json
--rw-r--r--   0 ploch      (502) staff       (20)     5929 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_by_step_name.json
--rw-r--r--   0 ploch      (502) staff       (20)  5944047 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-0-99.json
--rw-r--r--   0 ploch      (502) staff       (20)  9501053 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-100-199.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.134088 pytos2-ce-2.3.11/tests/securechange/json/users/
--rw-r--r--   0 ploch      (502) staff       (20)  1525217 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/all_users.json
--rw-r--r--   0 ploch      (502) staff       (20)     2103 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/user_45.json
--rw-r--r--   0 ploch      (502) staff       (20)     2095 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/users_by_username.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.135711 pytos2-ce-2.3.11/tests/securechange/json/verifier/
--rw-r--r--   0 ploch      (502) staff       (20)    28476 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/verifier/verifier_result_199.json
--rw-r--r--   0 ploch      (502) staff       (20)     3617 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/object_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     1196 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/risk_results_test.py
--rw-r--r--   0 ploch      (502) staff       (20)    18093 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/ticket_test.py
--rw-r--r--   0 ploch      (502) staff       (20)    10874 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/trigger_test.py
--rw-r--r--   0 ploch      (502) staff       (20)      793 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/verifier_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.140766 pytos2-ce-2.3.11/tests/securetrack/
--rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/__init__.py
--rw-r--r--   0 ploch      (502) staff       (20)    21743 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/api_test.py
--rw-r--r--   0 ploch      (502) staff       (20)    26361 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/conftest.py
--rw-r--r--   0 ploch      (502) staff       (20)     1592 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/device_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     1726 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/domain_test.py
--rw-r--r--   0 ploch      (502) staff       (20)       31 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/entrypoint_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     3984 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_ignored_interface_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     7779 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_interface_customer_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     7252 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_interface_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     6468 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_route_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     6593 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_transparent_firewall_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     6232 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_vpn_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     1351 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/interface_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     3842 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/join_cloud_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.064874 pytos2-ce-2.3.11/tests/securetrack/json/
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.170568 pytos2-ce-2.3.11/tests/securetrack/json/devices/
--rw-r--r--   0 ploch      (502) staff       (20)      332 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/8.json
--rw-r--r--   0 ploch      (502) staff       (20)      455 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/ASAv.json
--rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-1.json
--rw-r--r--   0 ploch      (502) staff       (20)      241 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-10.json
--rw-r--r--   0 ploch      (502) staff       (20)      277 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-105.json
--rw-r--r--   0 ploch      (502) staff       (20)      226 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-11.json
--rw-r--r--   0 ploch      (502) staff       (20)      276 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-114.json
--rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-115.json
--rw-r--r--   0 ploch      (502) staff       (20)      263 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-119.json
--rw-r--r--   0 ploch      (502) staff       (20)      226 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-12.json
--rw-r--r--   0 ploch      (502) staff       (20)      292 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-120.json
--rw-r--r--   0 ploch      (502) staff       (20)      296 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-121.json
--rw-r--r--   0 ploch      (502) staff       (20)      295 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-123.json
--rw-r--r--   0 ploch      (502) staff       (20)      250 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-142.json
--rw-r--r--   0 ploch      (502) staff       (20)      274 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-144.json
--rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-156.json
--rw-r--r--   0 ploch      (502) staff       (20)      267 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-157.json
--rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-159.json
--rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-160.json
--rw-r--r--   0 ploch      (502) staff       (20)      275 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-161.json
--rw-r--r--   0 ploch      (502) staff       (20)      242 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-166.json
--rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-174.json
--rw-r--r--   0 ploch      (502) staff       (20)      301 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-179.json
--rw-r--r--   0 ploch      (502) staff       (20)      303 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-180.json
--rw-r--r--   0 ploch      (502) staff       (20)      298 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-181.json
--rw-r--r--   0 ploch      (502) staff       (20)      305 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-182.json
--rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-184.json
--rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-193.json
--rw-r--r--   0 ploch      (502) staff       (20)      243 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-194.json
--rw-r--r--   0 ploch      (502) staff       (20)      269 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-195.json
--rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-196.json
--rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-198.json
--rw-r--r--   0 ploch      (502) staff       (20)      242 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-20.json
--rw-r--r--   0 ploch      (502) staff       (20)      340 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-206.json
--rw-r--r--   0 ploch      (502) staff       (20)      212 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-207.json
--rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-208.json
--rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-209.json
--rw-r--r--   0 ploch      (502) staff       (20)      325 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-21.json
--rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-211.json
--rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-212.json
--rw-r--r--   0 ploch      (502) staff       (20)      248 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-213.json
--rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-214.json
--rw-r--r--   0 ploch      (502) staff       (20)      291 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-215.json
--rw-r--r--   0 ploch      (502) staff       (20)      293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-216.json
--rw-r--r--   0 ploch      (502) staff       (20)      286 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-217.json
--rw-r--r--   0 ploch      (502) staff       (20)      287 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-218.json
--rw-r--r--   0 ploch      (502) staff       (20)      235 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-219.json
--rw-r--r--   0 ploch      (502) staff       (20)      215 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-230.json
--rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-231.json
--rw-r--r--   0 ploch      (502) staff       (20)      259 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-232.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-233.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-234.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-235.json
--rw-r--r--   0 ploch      (502) staff       (20)      254 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-236.json
--rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-237.json
--rw-r--r--   0 ploch      (502) staff       (20)      213 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-239.json
--rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-240.json
--rw-r--r--   0 ploch      (502) staff       (20)      240 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-243.json
--rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-244.json
--rw-r--r--   0 ploch      (502) staff       (20)      275 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-245.json
--rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-246.json
--rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-32.json
--rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-348.json
--rw-r--r--   0 ploch      (502) staff       (20)      332 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-349.json
--rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-37.json
--rw-r--r--   0 ploch      (502) staff       (20)      225 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-38.json
--rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-408.json
--rw-r--r--   0 ploch      (502) staff       (20)      249 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-411.json
--rw-r--r--   0 ploch      (502) staff       (20)      237 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-416.json
--rw-r--r--   0 ploch      (502) staff       (20)      229 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-5.json
--rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-552.json
--rw-r--r--   0 ploch      (502) staff       (20)      219 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-553.json
--rw-r--r--   0 ploch      (502) staff       (20)      256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-554.json
--rw-r--r--   0 ploch      (502) staff       (20)      254 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-555.json
--rw-r--r--   0 ploch      (502) staff       (20)      291 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-556.json
--rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-557.json
--rw-r--r--   0 ploch      (502) staff       (20)      246 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-559.json
--rw-r--r--   0 ploch      (502) staff       (20)      211 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-561.json
--rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-562.json
--rw-r--r--   0 ploch      (502) staff       (20)      207 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-563.json
--rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-564.json
--rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-565.json
--rw-r--r--   0 ploch      (502) staff       (20)      262 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-566.json
--rw-r--r--   0 ploch      (502) staff       (20)      261 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-567.json
--rw-r--r--   0 ploch      (502) staff       (20)      286 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-568.json
--rw-r--r--   0 ploch      (502) staff       (20)      285 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-569.json
--rw-r--r--   0 ploch      (502) staff       (20)      289 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-570.json
--rw-r--r--   0 ploch      (502) staff       (20)      288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-571.json
--rw-r--r--   0 ploch      (502) staff       (20)      260 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-572.json
--rw-r--r--   0 ploch      (502) staff       (20)      277 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-573.json
--rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-574.json
--rw-r--r--   0 ploch      (502) staff       (20)      268 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-575.json
--rw-r--r--   0 ploch      (502) staff       (20)      269 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-576.json
--rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-577.json
--rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-579.json
--rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-58.json
--rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-580.json
--rw-r--r--   0 ploch      (502) staff       (20)      249 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-581.json
--rw-r--r--   0 ploch      (502) staff       (20)      243 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-582.json
--rw-r--r--   0 ploch      (502) staff       (20)      258 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-583.json
--rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-584.json
--rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-585.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-586.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-587.json
--rw-r--r--   0 ploch      (502) staff       (20)      283 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-588.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-589.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-59.json
--rw-r--r--   0 ploch      (502) staff       (20)      304 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-590.json
--rw-r--r--   0 ploch      (502) staff       (20)      280 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-591.json
--rw-r--r--   0 ploch      (502) staff       (20)      310 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-592.json
--rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-593.json
--rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-594.json
--rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-595.json
--rw-r--r--   0 ploch      (502) staff       (20)      230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-596.json
--rw-r--r--   0 ploch      (502) staff       (20)      205 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-598.json
--rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-60.json
--rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-61.json
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-62.json
--rw-r--r--   0 ploch      (502) staff       (20)      229 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-622.json
--rw-r--r--   0 ploch      (502) staff       (20)      440 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-637.json
--rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-65.json
--rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-7.json
--rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-75.json
--rw-r--r--   0 ploch      (502) staff       (20)      276 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-77.json
--rw-r--r--   0 ploch      (502) staff       (20)      233 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-8.json
--rw-r--r--   0 ploch      (502) staff       (20)      230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-89.json
--rw-r--r--   0 ploch      (502) staff       (20)      253 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-90.json
--rw-r--r--   0 ploch      (502) staff       (20)      288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-91.json
--rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-92.json
--rw-r--r--   0 ploch      (502) staff       (20)    69102 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/devices.json
--rw-r--r--   0 ploch      (502) staff       (20)     2508 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/for-rule-test.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.170973 pytos2-ce-2.3.11/tests/securetrack/json/domains/
--rw-r--r--   0 ploch      (502) staff       (20)      100 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/domains/domain-7.json
--rw-r--r--   0 ploch      (502) staff       (20)     1112 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/domains/domains.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.171610 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/
--rw-r--r--   0 ploch      (502) staff       (20)      309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/generic_devices.json
--rw-r--r--   0 ploch      (502) staff       (20)      133 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/generic_devices_filtered.json
--rw-r--r--   0 ploch      (502) staff       (20)      415 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/sample_generic_device.csv
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.171790 pytos2-ce-2.3.11/tests/securetrack/json/generic_ignored_interfaces/
--rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_ignored_interfaces/mgmt-10.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.172242 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/
--rw-r--r--   0 ploch      (502) staff       (20)      373 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/device-5.json
--rw-r--r--   0 ploch      (502) staff       (20)      166 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/int-cust-74.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.174434 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/
--rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-1.json
--rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-19.json
--rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-2.json
--rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-20.json
--rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-3.json
--rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-32.json
--rw-r--r--   0 ploch      (502) staff       (20)      777 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-1.json
--rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-21.json
--rw-r--r--   0 ploch      (502) staff       (20)      479 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-5.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.178393 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/
--rw-r--r--   0 ploch      (502) staff       (20)      481 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/mgmt-2.json
--rw-r--r--   0 ploch      (502) staff       (20)      527 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/mgmt-3.json
--rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-27.json
--rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-28.json
--rw-r--r--   0 ploch      (502) staff       (20)      265 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-29.json
--rw-r--r--   0 ploch      (502) staff       (20)      267 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-30.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.179241 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/
--rw-r--r--   0 ploch      (502) staff       (20)      337 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/data-17.json
--rw-r--r--   0 ploch      (502) staff       (20)      333 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/data-23.json
--rw-r--r--   0 ploch      (502) staff       (20)      904 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/device-9.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.180606 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/
--rw-r--r--   0 ploch      (502) staff       (20)      469 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/device-1.json
--rw-r--r--   0 ploch      (502) staff       (20)      417 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/device-3.json
--rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-17.json
--rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-22.json
--rw-r--r--   0 ploch      (502) staff       (20)      235 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-24.json
--rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-25.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.181252 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/
--rw-r--r--   0 ploch      (502) staff       (20)     3862 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-interfaces.json
--rw-r--r--   0 ploch      (502) staff       (20)     3195 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-objects.json
--rw-r--r--   0 ploch      (502) staff       (20)      348 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-topology-interfaces.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.181443 pytos2-ce-2.3.11/tests/securetrack/json/join_clouds/
--rw-r--r--   0 ploch      (502) staff       (20)       80 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/join_clouds/cloud-67.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.191650 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/
--rw-r--r--   0 ploch      (502) staff       (20)    79537 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/157.json
--rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/174.json
--rw-r--r--   0 ploch      (502) staff       (20)    73209 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/181.json
--rw-r--r--   0 ploch      (502) staff       (20)    42360 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/184.json
--rw-r--r--   0 ploch      (502) staff       (20)   103018 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20.json
--rw-r--r--   0 ploch      (502) staff       (20)      571 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json
--rw-r--r--   0 ploch      (502) staff       (20)   119194 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/243.json
--rw-r--r--   0 ploch      (502) staff       (20)    36452 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/5.json
--rw-r--r--   0 ploch      (502) staff       (20)      585 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json
--rw-r--r--   0 ploch      (502) staff       (20)     1649 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json
--rw-r--r--   0 ploch      (502) staff       (20)      553 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json
--rw-r--r--   0 ploch      (502) staff       (20)      859 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json
--rw-r--r--   0 ploch      (502) staff       (20)     1220 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/identity_awareness.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.193000 pytos2-ce-2.3.11/tests/securetrack/json/policies/
--rw-r--r--   0 ploch      (502) staff       (20)      356 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/policies/157.json
--rw-r--r--   0 ploch      (502) staff       (20)      337 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/policies/20.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.214947 pytos2-ce-2.3.11/tests/securetrack/json/revisions/
--rw-r--r--   0 ploch      (502) staff       (20)    17051 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/1-all.json
--rw-r--r--   0 ploch      (502) staff       (20)    15168 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/1.json
--rw-r--r--   0 ploch      (502) staff       (20)    18723 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-1.json
--rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-10.json
--rw-r--r--   0 ploch      (502) staff       (20)    31413 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-105.json
--rw-r--r--   0 ploch      (502) staff       (20)      928 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-11.json
--rw-r--r--   0 ploch      (502) staff       (20)    31074 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-114.json
--rw-r--r--   0 ploch      (502) staff       (20)     5017 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-115.json
--rw-r--r--   0 ploch      (502) staff       (20)      476 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-119.json
--rw-r--r--   0 ploch      (502) staff       (20)      935 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-12.json
--rw-r--r--   0 ploch      (502) staff       (20)     2748 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-120.json
--rw-r--r--   0 ploch      (502) staff       (20)     1385 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-121.json
--rw-r--r--   0 ploch      (502) staff       (20)      931 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-123.json
--rw-r--r--   0 ploch      (502) staff       (20)      477 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-142.json
--rw-r--r--   0 ploch      (502) staff       (20)     1387 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-144.json
--rw-r--r--   0 ploch      (502) staff       (20)       16 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-156.json
--rw-r--r--   0 ploch      (502) staff       (20)    24971 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-157.json
--rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-159.json
--rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-160.json
--rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-161.json
--rw-r--r--   0 ploch      (502) staff       (20)     5479 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-166.json
--rw-r--r--   0 ploch      (502) staff       (20)    46903 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-174.json
--rw-r--r--   0 ploch      (502) staff       (20)    76878 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-179.json
--rw-r--r--   0 ploch      (502) staff       (20)     4644 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-180.json
--rw-r--r--   0 ploch      (502) staff       (20)    77093 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-181.json
--rw-r--r--   0 ploch      (502) staff       (20)     1880 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-182.json
--rw-r--r--   0 ploch      (502) staff       (20)    54424 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-184.json
--rw-r--r--   0 ploch      (502) staff       (20)    16309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-193.json
--rw-r--r--   0 ploch      (502) staff       (20)    19380 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-194.json
--rw-r--r--   0 ploch      (502) staff       (20)    13012 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-195.json
--rw-r--r--   0 ploch      (502) staff       (20)    79890 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-196.json
--rw-r--r--   0 ploch      (502) staff       (20)    14883 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-198.json
--rw-r--r--   0 ploch      (502) staff       (20)    36540 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-20.json
--rw-r--r--   0 ploch      (502) staff       (20)      312 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-206.json
--rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-207.json
--rw-r--r--   0 ploch      (502) staff       (20)      905 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-208.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-209.json
--rw-r--r--   0 ploch      (502) staff       (20)     3895 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-21.json
--rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-211.json
--rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-212.json
--rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-213.json
--rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-214.json
--rw-r--r--   0 ploch      (502) staff       (20)     4177 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-215.json
--rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-216.json
--rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-217.json
--rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-218.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-219.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-220.json
--rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-221.json
--rw-r--r--   0 ploch      (502) staff       (20)     3055 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-32.json
--rw-r--r--   0 ploch      (502) staff       (20)     2446 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-37.json
--rw-r--r--   0 ploch      (502) staff       (20)      616 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-38.json
--rw-r--r--   0 ploch      (502) staff       (20)    13412 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-5.json
--rw-r--r--   0 ploch      (502) staff       (20)      609 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-58.json
--rw-r--r--   0 ploch      (502) staff       (20)     2109 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-59.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-60.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-61.json
--rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-62.json
--rw-r--r--   0 ploch      (502) staff       (20)      613 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-65.json
--rw-r--r--   0 ploch      (502) staff       (20)     6349 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-7.json
--rw-r--r--   0 ploch      (502) staff       (20)      979 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-75.json
--rw-r--r--   0 ploch      (502) staff       (20)    11188 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-77.json
--rw-r--r--   0 ploch      (502) staff       (20)      440 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8-latest-revision.json
--rw-r--r--   0 ploch      (502) staff       (20)    44184 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8.json
--rw-r--r--   0 ploch      (502) staff       (20)     2140 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-89.json
--rw-r--r--   0 ploch      (502) staff       (20)     3293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-90.json
--rw-r--r--   0 ploch      (502) staff       (20)     1491 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-91.json
--rw-r--r--   0 ploch      (502) staff       (20)     2136 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-92.json
--rw-r--r--   0 ploch      (502) staff       (20)      525 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2226.json
--rw-r--r--   0 ploch      (502) staff       (20)      351 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2285.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.258669 pytos2-ce-2.3.11/tests/securetrack/json/rules/
--rw-r--r--   0 ploch      (502) staff       (20)    71570 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)    62230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-10.json
--rw-r--r--   0 ploch      (502) staff       (20)   543520 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-105.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-11.json
--rw-r--r--   0 ploch      (502) staff       (20)   663431 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-114.json
--rw-r--r--   0 ploch      (502) staff       (20)   109786 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-115.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-119.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-12.json
--rw-r--r--   0 ploch      (502) staff       (20)   133714 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-120.json
--rw-r--r--   0 ploch      (502) staff       (20)    34804 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-121.json
--rw-r--r--   0 ploch      (502) staff       (20)     8212 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-123.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-142.json
--rw-r--r--   0 ploch      (502) staff       (20)     7255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-144.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-156.json
--rw-r--r--   0 ploch      (502) staff       (20)   157444 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-157.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-159.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-160.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-161.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-166.json
--rw-r--r--   0 ploch      (502) staff       (20)    12014 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-174.json
--rw-r--r--   0 ploch      (502) staff       (20)   194256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-179.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-180.json
--rw-r--r--   0 ploch      (502) staff       (20)    97136 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-181.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-182.json
--rw-r--r--   0 ploch      (502) staff       (20)    55631 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-184.json
--rw-r--r--   0 ploch      (502) staff       (20)    23897 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-193.json
--rw-r--r--   0 ploch      (502) staff       (20)   141460 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-194.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-195.json
--rw-r--r--   0 ploch      (502) staff       (20)   367349 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-196.json
--rw-r--r--   0 ploch      (502) staff       (20)    21047 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-198.json
--rw-r--r--   0 ploch      (502) staff       (20)   162520 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)   162511 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-with-uid.json
--rw-r--r--   0 ploch      (502) staff       (20)   137967 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-206.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-207.json
--rw-r--r--   0 ploch      (502) staff       (20)     5714 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-208.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-209.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-21-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-21.json
--rw-r--r--   0 ploch      (502) staff       (20)     2807 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-211.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-212.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-213.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-214.json
--rw-r--r--   0 ploch      (502) staff       (20)   388533 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-215.json
--rw-r--r--   0 ploch      (502) staff       (20)    21127 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-216.json
--rw-r--r--   0 ploch      (502) staff       (20)    33725 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-217.json
--rw-r--r--   0 ploch      (502) staff       (20)    35869 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-218.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-219.json
--rw-r--r--   0 ploch      (502) staff       (20)    26022 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-220.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-221.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-32.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-37.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-38.json
--rw-r--r--   0 ploch      (502) staff       (20)    32311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)    27756 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-58.json
--rw-r--r--   0 ploch      (502) staff       (20)    51831 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-59.json
--rw-r--r--   0 ploch      (502) staff       (20)    22759 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-60.json
--rw-r--r--   0 ploch      (502) staff       (20)    22802 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-61.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-62.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-65.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-7-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-7.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-75.json
--rw-r--r--   0 ploch      (502) staff       (20)    87482 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-77.json
--rw-r--r--   0 ploch      (502) staff       (20)   542053 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8-add-documentation.json
--rw-r--r--   0 ploch      (502) staff       (20)   479880 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-89.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-90.json
--rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-91.json
--rw-r--r--   0 ploch      (502) staff       (20)    28029 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-92.json
--rw-r--r--   0 ploch      (502) staff       (20)     3282 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/kwargify-rules-test-data.json
--rw-r--r--   0 ploch      (502) staff       (20)   127793 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/revision-2285-with-uid.json
--rw-r--r--   0 ploch      (502) staff       (20)  8342101 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-1.json
--rw-r--r--   0 ploch      (502) staff       (20)   619029 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-2.json
--rw-r--r--   0 ploch      (502) staff       (20)      147 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.260834 pytos2-ce-2.3.11/tests/securetrack/json/services/
--rw-r--r--   0 ploch      (502) staff       (20)   178425 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/1.json
--rw-r--r--   0 ploch      (502) staff       (20)   299824 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/aurora339.json
--rw-r--r--   0 ploch      (502) staff       (20)     6477 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json
--rw-r--r--   0 ploch      (502) staff       (20)      569 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.261041 pytos2-ce-2.3.11/tests/securetrack/json/topology/
--rw-r--r--   0 ploch      (502) staff       (20)       31 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/topology/status.json
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262025 pytos2-ce-2.3.11/tests/securetrack/json/zones/
--rw-r--r--   0 ploch      (502) staff       (20)      250 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-69.json
--rw-r--r--   0 ploch      (502) staff       (20)      256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-78.json
--rw-r--r--   0 ploch      (502) staff       (20)      693 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-descendants-80.json
--rw-r--r--   0 ploch      (502) staff       (20)      397 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-entries-78.json
--rw-r--r--   0 ploch      (502) staff       (20)    10385 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zones.json
--rw-r--r--   0 ploch      (502) staff       (20)     2937 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/network_object_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     5196 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/revision_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/rule_test.py
--rw-r--r--   0 ploch      (502) staff       (20)    11536 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/service_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     1624 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/zone_test.py
-drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262264 pytos2-ce-2.3.11/tests/utils/
--rw-r--r--   0 ploch      (502) staff       (20)     1863 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/utils/cache_test.py
--rw-r--r--   0 ploch      (502) staff       (20)     7383 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/utils_test.py
--rw-r--r--   0 ploch      (502) staff       (20)      344 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tox.ini
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.585440 pytos2-ce-2.3.13/
+-rw-r--r--   0 ploch      (502) staff       (20)       99 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/.gitignore
+-rw-r--r--   0 ploch      (502) staff       (20)      631 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/.gitlab-ci.yml
+-rw-r--r--   0 ploch      (502) staff       (20)      188 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/.pre-commit-config.yaml
+-rw-r--r--   0 ploch      (502) staff       (20)     6481 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/CHANGELOG.md
+-rw-r--r--   0 ploch      (502) staff       (20)    10781 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/LICENSE
+-rw-r--r--   0 ploch      (502) staff       (20)     3095 2023-05-04 13:08:02.585273 pytos2-ce-2.3.13/PKG-INFO
+-rw-r--r--   0 ploch      (502) staff       (20)     2937 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/README.md
+-rw-r--r--   0 ploch      (502) staff       (20)       71 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/dev-requirements.txt
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.476535 pytos2-ce-2.3.13/doc/
+-rw-r--r--   0 ploch      (502) staff       (20)    55728 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/doc/pytos2-ce.ipynb
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.477614 pytos2-ce-2.3.13/docs/
+-rw-r--r--   0 ploch      (502) staff       (20)       72 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/.env
+-rw-r--r--   0 ploch      (502) staff       (20)    10033 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/Basic Usage.ipynb
+-rw-r--r--   0 ploch      (502) staff       (20)      586 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/Jupyter Notebook Setup.md
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.479082 pytos2-ce-2.3.13/docs/assets/
+-rw-r--r--   0 ploch      (502) staff       (20)   176021 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-closed.png
+-rw-r--r--   0 ploch      (502) staff       (20)   182801 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-step-1.png
+-rw-r--r--   0 ploch      (502) staff       (20)   188759 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-step-2-edit-1.png
+-rw-r--r--   0 ploch      (502) staff       (20)   181652 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-step-2-edit-2.png
+-rw-r--r--   0 ploch      (502) staff       (20)   185275 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-step-2.png
+-rw-r--r--   0 ploch      (502) staff       (20)   187802 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/assets/securechange-step-3.png
+-rw-r--r--   0 ploch      (502) staff       (20)      660 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/basic_trigger.py
+-rw-r--r--   0 ploch      (502) staff       (20)      730 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/contributing.md
+-rw-r--r--   0 ploch      (502) staff       (20)      640 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/init.py
+-rw-r--r--   0 ploch      (502) staff       (20)    55750 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/docs/pytos2-ce.ipynb
+-rw-r--r--   0 ploch      (502) staff       (20)       89 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/mypy.ini
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.479339 pytos2-ce-2.3.13/pytos2/
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.479467 pytos2-ce-2.3.13/pytos2/api/
+-rw-r--r--   0 ploch      (502) staff       (20)     4051 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/api/__init__.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.479616 pytos2-ce-2.3.13/pytos2/models/
+-rw-r--r--   0 ploch      (502) staff       (20)     1197 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/models/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/py.typed
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.480224 pytos2-ce-2.3.13/pytos2/secureapp/
+-rw-r--r--   0 ploch      (502) staff       (20)      112 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/secureapp/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      731 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/secureapp/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)      713 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/secureapp/application_identities.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1799 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/secureapp/entrypoint.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.482312 pytos2-ce-2.3.13/pytos2/securechange/
+-rw-r--r--   0 ploch      (502) staff       (20)      172 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4015 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8022 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/designer.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7928 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/designer_verifier_common.py
+-rw-r--r--   0 ploch      (502) staff       (20)      205 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/device.py
+-rw-r--r--   0 ploch      (502) staff       (20)    11121 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/entrypoint.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.482771 pytos2-ce-2.3.13/pytos2/securechange/fields/
+-rw-r--r--   0 ploch      (502) staff       (20)    58249 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/fields/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      414 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/fields/binding.py
+-rw-r--r--   0 ploch      (502) staff       (20)    20740 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/fields/rule_operation.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10020 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/network_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8168 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/risk_results.py
+-rw-r--r--   0 ploch      (502) staff       (20)     2756 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/rule.py
+-rw-r--r--   0 ploch      (502) staff       (20)   104439 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/service.py
+-rw-r--r--   0 ploch      (502) staff       (20)    24159 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/ticket.py
+-rw-r--r--   0 ploch      (502) staff       (20)    13112 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/trigger.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3309 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/user.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4518 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securechange/verifier.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.486097 pytos2-ce-2.3.13/pytos2/securetrack/
+-rw-r--r--   0 ploch      (502) staff       (20)       77 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10363 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6456 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/device.py
+-rw-r--r--   0 ploch      (502) staff       (20)      283 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/domain.py
+-rw-r--r--   0 ploch      (502) staff       (20)    77507 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/entrypoint.py
+-rw-r--r--   0 ploch      (502) staff       (20)      293 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_device.py
+-rw-r--r--   0 ploch      (502) staff       (20)      447 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_ignored_interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      727 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      519 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_interface_customer.py
+-rw-r--r--   0 ploch      (502) staff       (20)      620 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_route.py
+-rw-r--r--   0 ploch      (502) staff       (20)      830 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_transparent_firewall.py
+-rw-r--r--   0 ploch      (502) staff       (20)      582 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/generic_vpn.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3325 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      368 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/join_cloud.py
+-rw-r--r--   0 ploch      (502) staff       (20)    17292 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/network_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/policy_browser.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/revision.py
+-rw-r--r--   0 ploch      (502) staff       (20)    14109 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/rule.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6998 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/service_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)      237 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/topology.py
+-rw-r--r--   0 ploch      (502) staff       (20)     2677 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/securetrack/zone.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.486371 pytos2-ce-2.3.13/pytos2/utils/
+-rw-r--r--   0 ploch      (502) staff       (20)    13996 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/utils/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3127 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/pytos2/utils/cache.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.487090 pytos2-ce-2.3.13/pytos2_ce.egg-info/
+-rw-r--r--   0 ploch      (502) staff       (20)     3095 2023-05-04 13:08:02.000000 pytos2-ce-2.3.13/pytos2_ce.egg-info/PKG-INFO
+-rw-r--r--   0 ploch      (502) staff       (20)    23921 2023-05-04 13:08:02.000000 pytos2-ce-2.3.13/pytos2_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 ploch      (502) staff       (20)        1 2023-05-04 13:08:02.000000 pytos2-ce-2.3.13/pytos2_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 ploch      (502) staff       (20)      129 2023-05-04 13:08:02.000000 pytos2-ce-2.3.13/pytos2_ce.egg-info/requires.txt
+-rw-r--r--   0 ploch      (502) staff       (20)        7 2023-05-04 13:08:02.000000 pytos2-ce-2.3.13/pytos2_ce.egg-info/top_level.txt
+-rw-r--r--   0 ploch      (502) staff       (20)      106 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/requirements.txt
+-rw-r--r--   0 ploch      (502) staff       (20)       38 2023-05-04 13:08:02.585512 pytos2-ce-2.3.13/setup.cfg
+-rw-r--r--   0 ploch      (502) staff       (20)      812 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/setup.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.487511 pytos2-ce-2.3.13/tests/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4555 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/api_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.487937 pytos2-ce-2.3.13/tests/secureapp/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/secureapp/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      914 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/secureapp/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)      610 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/secureapp/entrypoint_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.488086 pytos2-ce-2.3.13/tests/secureapp/json/
+-rw-r--r--   0 ploch      (502) staff       (20)  1337893 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/secureapp/json/application_identities.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.490608 pytos2-ce-2.3.13/tests/securechange/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3511 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/api_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8758 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/ar_service_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8399 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)    25461 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/designer_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     5508 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/entrypoint_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    28797 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/fields_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.490753 pytos2-ce-2.3.13/tests/securechange/files/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/files/test.pdf
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.491213 pytos2-ce-2.3.13/tests/securechange/json/
+-rw-r--r--   0 ploch      (502) staff       (20)    35674 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/all_fields-workflow.json
+-rw-r--r--   0 ploch      (502) staff       (20)      201 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/application_details.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.493801 pytos2-ce-2.3.13/tests/securechange/json/designer/
+-rw-r--r--   0 ploch      (502) staff       (20)      663 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_icmp_service_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1854 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_group_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      726 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_host_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      755 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_range_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      667 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_subnet_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     9066 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_new_rule-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4094 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_new_rule_any_service-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1721 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_service_group-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      678 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/add_transport_service_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     7682 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/designer_result_251.json
+-rw-r--r--   0 ploch      (502) staff       (20)    20023 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/designer_result_instruction_update_rule.json
+-rw-r--r--   0 ploch      (502) staff       (20)    19907 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/designer_results.json
+-rw-r--r--   0 ploch      (502) staff       (20)   113035 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/designer_results_multi_instructions.json
+-rw-r--r--   0 ploch      (502) staff       (20)      171 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/fully_implemented-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      217 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/fully_implemented_since_no_security-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13618 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/designer/update_rule-instruction.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.502061 pytos2-ce-2.3.13/tests/securechange/json/field/
+-rw-r--r--   0 ploch      (502) staff       (20)      117 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/approve_reject-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       91 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/checkbox-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1159 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/clone_server_policy_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       84 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/date-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      262 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/drop_down_list-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      110 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/hyperlink-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       78 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/manager-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3986 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     9895 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request_with_all_service_types.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2128 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request_with_designer_results-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21739 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_group_change-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13017 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_group_change-field.json.old
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_hyperlink-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      163 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_network_object-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      868 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_server_decommission_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      142 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_service-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      123 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_target-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      181 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_text_area-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      204 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multi_text_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/multiple_selection-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      129 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/read_only-field.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.502236 pytos2-ce-2.3.13/tests/securechange/json/field/rule_modification/
+-rw-r--r--   0 ploch      (502) staff       (20)    43082 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/rule_modification/source_mod.json
+-rw-r--r--   0 ploch      (502) staff       (20)    10726 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/rule_modification_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      119 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/text_area-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       88 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/text_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       78 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/field/time-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    34462 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/risk_results_ticket.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.507429 pytos2-ce-2.3.13/tests/securechange/json/ticket/
+-rw-r--r--   0 ploch      (502) staff       (20)    32220 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/all_fields-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5565 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/closed_group_modify-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12132 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/dynamic_assignment-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    50426 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/open_with_access_request-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    20839 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/open_with_group_modify-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)      215 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/post_bad_ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21757 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/redo.json
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/specific_workflow.json
+-rw-r--r--   0 ploch      (502) staff       (20)      153 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/ticket_not_found.json
+-rw-r--r--   0 ploch      (502) staff       (20)   346577 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/ticket_search_assigned.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5929 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/ticket_search_by_step_name.json
+-rw-r--r--   0 ploch      (502) staff       (20)  5944047 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/tickets-0-99.json
+-rw-r--r--   0 ploch      (502) staff       (20)  9501053 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/ticket/tickets-100-199.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.513246 pytos2-ce-2.3.13/tests/securechange/json/users/
+-rw-r--r--   0 ploch      (502) staff       (20)  1525217 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/users/all_users.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2103 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/users/user_45.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2095 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/users/users_by_username.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.513617 pytos2-ce-2.3.13/tests/securechange/json/verifier/
+-rw-r--r--   0 ploch      (502) staff       (20)    28476 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/json/verifier/verifier_result_199.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3617 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/object_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1196 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/risk_results_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    18093 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/ticket_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10874 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/trigger_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)      793 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securechange/verifier_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.516960 pytos2-ce-2.3.13/tests/securetrack/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)    21743 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/api_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    26361 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1592 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/device_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1726 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/domain_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)       31 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/entrypoint_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3984 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_ignored_interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7779 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_interface_customer_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7252 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6468 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_route_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6593 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_transparent_firewall_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6232 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/generic_vpn_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1351 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3842 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/join_cloud_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.474362 pytos2-ce-2.3.13/tests/securetrack/json/
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.539596 pytos2-ce-2.3.13/tests/securetrack/json/devices/
+-rw-r--r--   0 ploch      (502) staff       (20)      332 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/8.json
+-rw-r--r--   0 ploch      (502) staff       (20)      455 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/ASAv.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      241 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)      277 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)      226 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)      276 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)      263 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)      226 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)      292 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)      296 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)      295 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)      250 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)      274 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)      267 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)      275 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)      301 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)      303 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)      298 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)      305 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)      243 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      340 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)      212 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)      325 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)      248 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)      291 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)      293 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)      286 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)      287 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)      235 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)      215 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-230.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-231.json
+-rw-r--r--   0 ploch      (502) staff       (20)      259 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-232.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-233.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-234.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-235.json
+-rw-r--r--   0 ploch      (502) staff       (20)      254 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-236.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-237.json
+-rw-r--r--   0 ploch      (502) staff       (20)      213 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-239.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-240.json
+-rw-r--r--   0 ploch      (502) staff       (20)      240 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-243.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-244.json
+-rw-r--r--   0 ploch      (502) staff       (20)      275 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-245.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-246.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-348.json
+-rw-r--r--   0 ploch      (502) staff       (20)      332 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-349.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-408.json
+-rw-r--r--   0 ploch      (502) staff       (20)      249 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-411.json
+-rw-r--r--   0 ploch      (502) staff       (20)      237 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-416.json
+-rw-r--r--   0 ploch      (502) staff       (20)      229 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-552.json
+-rw-r--r--   0 ploch      (502) staff       (20)      219 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-553.json
+-rw-r--r--   0 ploch      (502) staff       (20)      256 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-554.json
+-rw-r--r--   0 ploch      (502) staff       (20)      254 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-555.json
+-rw-r--r--   0 ploch      (502) staff       (20)      291 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-556.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-557.json
+-rw-r--r--   0 ploch      (502) staff       (20)      246 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-559.json
+-rw-r--r--   0 ploch      (502) staff       (20)      211 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-561.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-562.json
+-rw-r--r--   0 ploch      (502) staff       (20)      207 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-563.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-564.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-565.json
+-rw-r--r--   0 ploch      (502) staff       (20)      262 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-566.json
+-rw-r--r--   0 ploch      (502) staff       (20)      261 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-567.json
+-rw-r--r--   0 ploch      (502) staff       (20)      286 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-568.json
+-rw-r--r--   0 ploch      (502) staff       (20)      285 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-569.json
+-rw-r--r--   0 ploch      (502) staff       (20)      289 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-570.json
+-rw-r--r--   0 ploch      (502) staff       (20)      288 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-571.json
+-rw-r--r--   0 ploch      (502) staff       (20)      260 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-572.json
+-rw-r--r--   0 ploch      (502) staff       (20)      277 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-573.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-574.json
+-rw-r--r--   0 ploch      (502) staff       (20)      268 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-575.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-576.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-577.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-579.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-580.json
+-rw-r--r--   0 ploch      (502) staff       (20)      249 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-581.json
+-rw-r--r--   0 ploch      (502) staff       (20)      243 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-582.json
+-rw-r--r--   0 ploch      (502) staff       (20)      258 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-583.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-584.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-585.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-586.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-587.json
+-rw-r--r--   0 ploch      (502) staff       (20)      283 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-588.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-589.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)      304 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-590.json
+-rw-r--r--   0 ploch      (502) staff       (20)      280 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-591.json
+-rw-r--r--   0 ploch      (502) staff       (20)      310 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-592.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-593.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-594.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-595.json
+-rw-r--r--   0 ploch      (502) staff       (20)      230 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-596.json
+-rw-r--r--   0 ploch      (502) staff       (20)      205 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-598.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)      229 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-622.json
+-rw-r--r--   0 ploch      (502) staff       (20)      440 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-637.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)      276 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)      233 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)      230 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)      253 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)      288 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)    69102 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/devices.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2508 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/devices/for-rule-test.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.539940 pytos2-ce-2.3.13/tests/securetrack/json/domains/
+-rw-r--r--   0 ploch      (502) staff       (20)      100 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/domains/domain-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1112 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/domains/domains.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.540466 pytos2-ce-2.3.13/tests/securetrack/json/generic_devices/
+-rw-r--r--   0 ploch      (502) staff       (20)      309 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_devices/generic_devices.json
+-rw-r--r--   0 ploch      (502) staff       (20)      133 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_devices/generic_devices_filtered.json
+-rw-r--r--   0 ploch      (502) staff       (20)      415 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_devices/sample_generic_device.csv
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.540658 pytos2-ce-2.3.13/tests/securetrack/json/generic_ignored_interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_ignored_interfaces/mgmt-10.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.540994 pytos2-ce-2.3.13/tests/securetrack/json/generic_interface_customers/
+-rw-r--r--   0 ploch      (502) staff       (20)      373 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interface_customers/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      166 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interface_customers/int-cust-74.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.542673 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-19.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/int-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)      777 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/mgmt-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/mgmt-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      479 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/mgmt-5.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.543799 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/
+-rw-r--r--   0 ploch      (502) staff       (20)      481 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/mgmt-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      527 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/mgmt-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/route-27.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/route-28.json
+-rw-r--r--   0 ploch      (502) staff       (20)      265 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/route-29.json
+-rw-r--r--   0 ploch      (502) staff       (20)      267 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/route-30.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.544288 pytos2-ce-2.3.13/tests/securetrack/json/generic_transparent_firewalls/
+-rw-r--r--   0 ploch      (502) staff       (20)      337 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_transparent_firewalls/data-17.json
+-rw-r--r--   0 ploch      (502) staff       (20)      333 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_transparent_firewalls/data-23.json
+-rw-r--r--   0 ploch      (502) staff       (20)      904 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_transparent_firewalls/device-9.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.545291 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/
+-rw-r--r--   0 ploch      (502) staff       (20)      469 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      417 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/device-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/vpn-17.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/vpn-22.json
+-rw-r--r--   0 ploch      (502) staff       (20)      235 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/vpn-24.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/generic_vpns/vpn-25.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.545745 pytos2-ce-2.3.13/tests/securetrack/json/interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)     3862 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/interfaces/device8-interfaces.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3195 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/interfaces/device8-objects.json
+-rw-r--r--   0 ploch      (502) staff       (20)      348 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/interfaces/device8-topology-interfaces.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.545919 pytos2-ce-2.3.13/tests/securetrack/json/join_clouds/
+-rw-r--r--   0 ploch      (502) staff       (20)       80 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/join_clouds/cloud-67.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.548406 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/
+-rw-r--r--   0 ploch      (502) staff       (20)    79537 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/157.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/174.json
+-rw-r--r--   0 ploch      (502) staff       (20)    73209 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/181.json
+-rw-r--r--   0 ploch      (502) staff       (20)    42360 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/184.json
+-rw-r--r--   0 ploch      (502) staff       (20)   103018 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      571 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json
+-rw-r--r--   0 ploch      (502) staff       (20)   119194 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/243.json
+-rw-r--r--   0 ploch      (502) staff       (20)    36452 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      585 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1649 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json
+-rw-r--r--   0 ploch      (502) staff       (20)      553 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json
+-rw-r--r--   0 ploch      (502) staff       (20)      859 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1220 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/network_objects/identity_awareness.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.548725 pytos2-ce-2.3.13/tests/securetrack/json/policies/
+-rw-r--r--   0 ploch      (502) staff       (20)      356 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/policies/157.json
+-rw-r--r--   0 ploch      (502) staff       (20)      337 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/policies/20.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.561704 pytos2-ce-2.3.13/tests/securetrack/json/revisions/
+-rw-r--r--   0 ploch      (502) staff       (20)    17051 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/1-all.json
+-rw-r--r--   0 ploch      (502) staff       (20)    15168 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/1.json
+-rw-r--r--   0 ploch      (502) staff       (20)    18723 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)    31413 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)      928 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)    31074 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5017 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)      476 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)      935 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2748 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1385 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)      931 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)      477 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1387 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)       16 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)    24971 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5479 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)    46903 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)    76878 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4644 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)    77093 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1880 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)    54424 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)    16309 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)    19380 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13012 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)    79890 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)    14883 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)    36540 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      312 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)      905 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3895 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4177 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-220.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-221.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3055 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2446 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)      616 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13412 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      609 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2109 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)      613 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)     6349 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)      979 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)    11188 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)      440 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-8-latest-revision.json
+-rw-r--r--   0 ploch      (502) staff       (20)    44184 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2140 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3293 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1491 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2136 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)      525 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/revision-2226.json
+-rw-r--r--   0 ploch      (502) staff       (20)      351 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/revisions/revision-2285.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.582640 pytos2-ce-2.3.13/tests/securetrack/json/rules/
+-rw-r--r--   0 ploch      (502) staff       (20)    71570 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-1-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)    62230 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)   543520 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)   663431 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)   109786 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)   133714 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)    34804 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)     8212 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)     7255 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)   157444 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12014 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)   194256 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)    97136 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)    55631 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)    23897 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)   141460 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)   367349 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21047 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)   162520 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)   162511 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20-with-uid.json
+-rw-r--r--   0 ploch      (502) staff       (20)   137967 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5714 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-21-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2807 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)   388533 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21127 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)    33725 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)    35869 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)    26022 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-220.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-221.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)    32311 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-5-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)    27756 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)    51831 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)    22759 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)    22802 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-7-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)    87482 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)   542053 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-8-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)   479880 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)    28029 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3282 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/kwargify-rules-test-data.json
+-rw-r--r--   0 ploch      (502) staff       (20)   127793 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/revision-2285-with-uid.json
+-rw-r--r--   0 ploch      (502) staff       (20)  8342101 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/rule_search-105-all-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)   619029 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/rule_search-105-all-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      147 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/rules/rule_search-105.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.583904 pytos2-ce-2.3.13/tests/securetrack/json/services/
+-rw-r--r--   0 ploch      (502) staff       (20)   178425 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/services/1.json
+-rw-r--r--   0 ploch      (502) staff       (20)   299824 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/services/aurora339.json
+-rw-r--r--   0 ploch      (502) staff       (20)     6477 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json
+-rw-r--r--   0 ploch      (502) staff       (20)      569 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.584073 pytos2-ce-2.3.13/tests/securetrack/json/topology/
+-rw-r--r--   0 ploch      (502) staff       (20)       31 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/topology/status.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.584846 pytos2-ce-2.3.13/tests/securetrack/json/zones/
+-rw-r--r--   0 ploch      (502) staff       (20)      250 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/zones/zone-69.json
+-rw-r--r--   0 ploch      (502) staff       (20)      256 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/zones/zone-78.json
+-rw-r--r--   0 ploch      (502) staff       (20)      693 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/zones/zone-descendants-80.json
+-rw-r--r--   0 ploch      (502) staff       (20)      397 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/zones/zone-entries-78.json
+-rw-r--r--   0 ploch      (502) staff       (20)    10385 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/json/zones/zones.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2937 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/network_object_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     5196 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/revision_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/rule_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    11536 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/service_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1624 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/securetrack/zone_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 13:08:02.585003 pytos2-ce-2.3.13/tests/utils/
+-rw-r--r--   0 ploch      (502) staff       (20)     1863 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/utils/cache_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7383 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tests/utils_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)      344 2023-05-04 13:07:17.000000 pytos2-ce-2.3.13/tox.ini
```

### Comparing `pytos2-ce-2.3.11/.gitlab-ci.yml` & `pytos2-ce-2.3.13/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/CHANGELOG.md` & `pytos2-ce-2.3.13/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,40 @@
 # Changelog
 All notable changes to this project will be documented in this file
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 
+## [2.3.13] - 2023-03-09
+- NOTES: 
+  - converted usage example to jupyter 
+  - added trigger example
+- FEATURE: 
+  - Scw.add_comment()
+  - Scw.delete_comment()
+  - Network Object Model: VMInstanceDTO
+
+## [2.3.12] - 2023-02-16
+- Add:
+  - Scw.add_comment() - Add a comment to a specific ticket, step and task
+  - Scw.delete_comment() - Remove a comment from a ticket
+- Added types to Ticket Model: 
+  - create_step
+- Added comment helpers to Ticket Model:
+  - add_comment - add comment to ticket (current step and task used by default)
+  - add_comments - add a list of comments to ticket (current step and task used by default)
+  - delete_comment - remove a comment from ticket by id
+  - delete_comments - remove a list of comments by ids
+- Added types to AccessRequest Model: 
+  - sources
+  - destinations
+  - add_target
+  - add_ar
+  - add_group_change
+
 ## [2.3.11] - 2023-02-10
 - BUGFIX: Correctly handle payloads for updated to RecordSets
 - FEATURE: Scw.add_attachment() - Add file attchment to SecureChange
 - Add Models:
   - GenericIgnoredInterface
   - GenericInterfaceCustomer
   - GenericRoute
```

### Comparing `pytos2-ce-2.3.11/LICENSE` & `pytos2-ce-2.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-closed.png` & `pytos2-ce-2.3.13/docs/assets/securechange-closed.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-step-1.png` & `pytos2-ce-2.3.13/docs/assets/securechange-step-1.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-1.png` & `pytos2-ce-2.3.13/docs/assets/securechange-step-2-edit-1.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-2.png` & `pytos2-ce-2.3.13/docs/assets/securechange-step-2-edit-2.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-step-2.png` & `pytos2-ce-2.3.13/docs/assets/securechange-step-2.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/assets/securechange-step-3.png` & `pytos2-ce-2.3.13/docs/assets/securechange-step-3.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/init.py` & `pytos2-ce-2.3.13/docs/init.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/doc/pytos2-ce.ipynb` & `pytos2-ce-2.3.13/docs/pytos2-ce.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894882404181184%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict()}, 'source': {insert: [(7, '`pytos2` CE is "*

 * *            "currently *not* yet available on [PyPI](https://pypi.org). To install, use\\n')], "*

 * *            "delete: [7]}, 'attachments': OrderedDict()}, 2: {'execution_count': None, 'metadata': "*

 * *            "{replace: OrderedDict()}, 'outputs': []}, 3: {'metadata': {replace: OrderedDict()}}, "*

 * *            "4: {'metadata': {replace: OrderedDict()}}, 5: {'execution_count': None, 'metadata': "*

 * *            "{rep […]*

```diff
@@ -15,98 +15,50 @@
                 "   * [Getting Started](#start)\n",
                 "   * [Viewing Your Config](#config)\n",
                 "   * [Secure Change](#secure-change)\n",
                 "<!--te-->\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "0587012b-525e-4914-b23c-88e14c0cbbcc",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
+            "metadata": {},
             "source": [
                 "Installation      <a class=\"anchor\" id=\"install\"></a>\n",
                 "============\n",
                 "[Git](https://git-scm.com) is a prerequisite for installation. Also, development using either\n",
                 "[`venv`](https://docs.python.org/3/library/venv.html#creating-virtual-environments)\n",
                 "or [Docker](https://docs.docker.com/get-docker/)\n",
                 "is recommended.\n",
                 "\n",
-                "`pytos2` EE is currently *not* yet available on [PyPI](https://pypi.org). To install, use\n",
+                "`pytos2` CE is currently *not* yet available on [PyPI](https://pypi.org). To install, use\n",
                 "the following [`pip`](https://pypi.org/project/pip/) command:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "id": "ff2508e5-55af-43ba-bcb1-bd89e4fe4147",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%%\n"
-                }
-            },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Found existing installation: pytos2-ce 2.3.11.dev38+g8868608.d20230110\n",
-                        "Uninstalling pytos2-ce-2.3.11.dev38+g8868608.d20230110:\n",
-                        "  Successfully uninstalled pytos2-ce-2.3.11.dev38+g8868608.d20230110\n",
-                        "Note: you may need to restart the kernel to use updated packages.\n",
-                        "Requirement already satisfied: python-dotenv in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (0.20.0)\n",
-                        "\u001b[33mWARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.\n",
-                        "You should consider upgrading via the '/Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/bin/python -m pip install --upgrade pip' command.\u001b[0m\u001b[33m\n",
-                        "\u001b[0mNote: you may need to restart the kernel to use updated packages.\n",
-                        "Processing /Users/tyler.campbell/Desktop/work/pytos2-ce\n",
-                        "  Preparing metadata (setup.py) ... \u001b[?25ldone\n",
-                        "\u001b[?25hRequirement already satisfied: requests<3 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (2.28.1)\n",
-                        "Requirement already satisfied: traversify in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (1.1.2)\n",
-                        "Requirement already satisfied: attrs<20,>=19.2 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (19.3.0)\n",
-                        "Requirement already satisfied: python-json-logger<0.2 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (0.1.11)\n",
-                        "Requirement already satisfied: netaddr<0.8 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (0.7.20)\n",
-                        "Requirement already satisfied: result==0.8.0 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (0.8.0)\n",
-                        "Requirement already satisfied: typing_extensions in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (4.3.0)\n",
-                        "Requirement already satisfied: python-dateutil<3,>=2.8 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (2.8.2)\n",
-                        "Requirement already satisfied: six>=1.5 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from python-dateutil<3,>=2.8->pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (1.16.0)\n",
-                        "Requirement already satisfied: idna<4,>=2.5 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from requests<3->pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (3.3)\n",
-                        "Requirement already satisfied: charset-normalizer<3,>=2 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from requests<3->pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (2.1.1)\n",
-                        "Requirement already satisfied: urllib3<1.27,>=1.21.1 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from requests<3->pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (1.26.12)\n",
-                        "Requirement already satisfied: certifi>=2017.4.17 in /Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/lib/python3.8/site-packages (from requests<3->pytos2-ce==2.3.11.dev41+g6cbb666.d20230111) (2022.6.15)\n",
-                        "Using legacy 'setup.py install' for pytos2-ce, since package 'wheel' is not installed.\n",
-                        "Installing collected packages: pytos2-ce\n",
-                        "  Running setup.py install for pytos2-ce ... \u001b[?25ldone\n",
-                        "\u001b[?25hSuccessfully installed pytos2-ce-2.3.11.dev41+g6cbb666.d20230111\n",
-                        "\u001b[33mWARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.\n",
-                        "You should consider upgrading via the '/Users/tyler.campbell/.pyenv/versions/3.8.13/envs/docs/bin/python -m pip install --upgrade pip' command.\u001b[0m\u001b[33m\n",
-                        "\u001b[0mNote: you may need to restart the kernel to use updated packages.\n"
-                    ]
-                }
-            ],
+            "metadata": {},
+            "outputs": [],
             "source": [
                 "# PRODUCTION INSTALL\n",
                 "# %pip install python-dotenv git+https://gitlab.com/tufinps/pytos2-ce\n",
                 "\n",
                 "# LOCAL DEVELOPMENT\n",
                 "%pip uninstall pytos2-ce -y\n",
                 "%pip install python-dotenv \n",
                 "%pip install ../../pytos2-ce"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "44cea431-c79f-474c-baed-cfc724579963",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
+            "metadata": {},
             "source": [
                 "Setup      <a class=\"anchor\" id=\"setup\"></a>\n",
                 "=====\n",
                 "`pytos2` CE recommends setting the following environment variables while using this library. They can either be set directly in the environment using a method of your choice, or you can use [python-dotenv](https://saurabh-kumar.com/python-dotenv/).\n",
                 "\n",
                 "- `HOST`: The hostname \n",
                 "- `USER`: The username \n",
@@ -114,33 +66,25 @@
                 "\n",
                 "These values can be editted in the `.env` file or overwritten in-line in the example below"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "027b4882-a96d-4109-9c77-2d237fc09e28",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
+            "metadata": {},
             "source": [
                 "Getting Started      <a class=\"anchor\" id=\"start\"></a>\n",
                 "==============="
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "id": "e2f66f34-418b-49d7-96a2-1b548e7152bd",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%%\n"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# %load init.py\n",
                 "from dotenv import dotenv_values\n",
                 "from pytos2.secureapp import Sa as SecureApp\n",
                 "from pytos2.securechange import Scw as SecureChange\n",
                 "from pytos2.securetrack import St as SecureTrack\n",
@@ -169,28 +113,18 @@
             "source": [
                 "Configuration      <a class=\"anchor\" id=\"config\"></a>\n",
                 "==================="
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "id": "d2c52e89",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "10.20.200.89\n",
-                        "r\n",
-                        "tufin123\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "print(HOST)\n",
                 "print(USER)\n",
                 "print(PASS)"
             ]
         },
         {
@@ -241,15 +175,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "88591d23",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Get Ticket by ID # 674\n",
-                "ticket = secure_change.get_ticket(674)\n",
+                "ticket = secure_change.get_ticket(993)\n",
                 "\n",
                 "print(ticket)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f143a153",
@@ -281,15 +215,15 @@
                 "tickets = secure_change.get_tickets(status)\n",
                 "\n",
                 "print(tickets)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "73addde6",
+            "id": "d4cb5045",
             "metadata": {},
             "source": [
                 "### Get Users\n",
                 "\n",
                 "```python\n",
                 "\n",
                 "```"
@@ -307,15 +241,15 @@
                 "for index, user in enumerate(users):\n",
                 "    print(f'User #{index + 1}')\n",
                 "    print(user)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "73addde6",
+            "id": "ba930218",
             "metadata": {},
             "source": [
                 "### Get User\n",
                 "\n",
                 "```python\n",
                 "    .get_user(\n",
                 "        identifier: Union[str, int], expand: bool = False\n",
@@ -326,15 +260,15 @@
                 "\n",
                 "> by default, if type is int it will search by id"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "93a28764",
+            "id": "96484f6f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Provide an integer \n",
                 "user_by_id = secure_change.get_user(1)\n",
                 "\n",
                 "print(user_by_id)"
@@ -416,26 +350,18 @@
                 "        domain_name: Optional[str] = None\n",
                 "    )\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "id": "28ac1adb",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "[]\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "tickets = secure_change.ticket_search(assigned_to='r')\n",
                 "filtered_list = list(filter(lambda ticket: ticket['id'] == 674, tickets))\n",
                 "\n",
                 "print(filtered_list)"
             ]
         },
@@ -449,26 +375,18 @@
                 "```python\n",
                 "   .get_attachment(self, file_id: Union[int, str]) -> bytes:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "id": "25c2726b",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Attachment(id=None, uid='b5672678-d9c5-46ee-87cc-d8fa7fce1a43', name='README.pdf', link='https://10.20.200.89/securechangeworkflow/api/securechange/attachments/b5672678-d9c5-46ee-87cc-d8fa7fce1a43')\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "t = secure_change.get_ticket(990)\n",
                 "\n",
                 "comment = t.comments[0]\n",
                 "attachment = comment.attachments[0]\n",
                 "attachment_content = secure_change.get_attachment(attachment.uid)\n",
                 "\n",
@@ -487,34 +405,122 @@
                 "```python\n",
                 "   .add_attachment(self, file: str) -> str:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "id": "241ce529",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "54076c01-4785-4459-b443-a4ff7543cd56\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "\n",
-                "uuid = secure_change.add_attachment(\"../../../README.pdf\")\n",
+                "uuid = secure_change.add_attachment(\"../README.pdf\")\n",
                 "\n",
                 "print(uuid)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "094f7ac5",
+            "metadata": {},
+            "source": [
+                "### Add Comment\n",
+                "\n",
+                "```python\n",
+                "   .add_comment(\n",
+                "        self,\n",
+                "        ticket_id: Union[int, str],\n",
+                "        step_id: Union[int, str],\n",
+                "        task_id: Union[int, str],\n",
+                "        comment_content: str,\n",
+                "        attachment_uuids: Optional[List[str]],\n",
+                "    ) -> str:\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2914c5a8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from pytos2.securechange.ticket import Ticket, Comment, Attachment\n",
+                "\n",
+                "ticket: Ticket = secure_change.get_ticket(990)\n",
+                "current_step = ticket.current_step\n",
+                "current_task = ticket.current_task\n",
+                "\n",
+                "uuid = secure_change.add_attachment(\"../README.pdf\")\n",
+                "comment = \"This is a new comment with an attachment\"\n",
+                "\n",
+                "secure_change.add_comment(ticket.id, current_step.id, current_task.id, comment, [uuid])\n",
+                "\n",
+                "### There is also two helpers on the Ticket ###\n",
+                "#   by default the current step and task are used if not provided #\n",
+                "\n",
+                "ticket: Ticket = secure_change.get_ticket(993)\n",
+                "\n",
+                "ticket.add_comment(comment, [uuid])\n",
+                "\n",
+                "c_one = Comment(content=\"Comment One\")\n",
+                "c_two = Comment(content=\"Comment Two\")\n",
+                "\n",
+                "ticket.add_comments([c_one, c_two])"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "da93ed45",
+            "metadata": {},
+            "source": [
+                "### Delete Comment\n",
+                "\n",
+                "```python\n",
+                "   delete_comment(self, ticket_id: Union[int, str], comment_id: Union[int, str],) -> None:\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7472f6f8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
+                "ticket: Ticket = secure_change.get_ticket(993)\n",
+                "\n",
+                "comment = ticket.comments[-1] # get last comment\n",
+                "\n",
+                "secure_change.delete_comment(ticket.id, comment.id)\n",
+                "\n",
+                "### There is also two helpers on the Ticket ###\n",
+                "\n",
+                "ticket.delete_comment(\"230\")\n",
+                "\n",
+                "ticket.delete_comments([231, 232])"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "36c50ad8",
+            "metadata": {},
+            "source": [
+                "- - -\n",
+                "- - -\n",
+                "- - -\n"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "7634916b",
             "metadata": {},
             "source": [
                 "Secure Track      <a class=\"anchor\" id=\"secure-track\"></a>\n",
                 "============="
             ]
@@ -1756,15 +1762,15 @@
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_interfaces(1)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0d0e5350",
+            "id": "1c0daf6c",
             "metadata": {},
             "source": [
                 "### Add Generic Route\n",
                 "\n",
                 "```python\n",
                 "    .add_generic_route(\n",
                 "        route: dict\n",
@@ -2006,30 +2012,30 @@
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_routes(92)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0d0e5350",
+            "id": "12f5aac1",
             "metadata": {},
             "source": [
                 "### Add Generic VPN\n",
                 "\n",
                 "```python\n",
                 "    .add_generic_vpn(\n",
                 "        vpn: dict\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4538afeb",
+            "id": "f89f64e0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vpn = {\n",
                 "    \"generic\": True,\n",
                 "    \"deviceId\": 182,\n",
                 "    \"interfaceName\": \"777\",\n",
@@ -2037,30 +2043,30 @@
                 "    \"tunnelDestIpAddr\": \"1.1.1.188\"\n",
                 "}\n",
                 "secure_track.add_generic_vpn(vpn)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5254e530",
+            "id": "8c0ff7b8",
             "metadata": {},
             "source": [
                 "### Add Generic VPNs\n",
                 "\n",
                 "```python\n",
                 "    .add_generic_vpns(\n",
                 "        vpns: List[dict]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c33a1877",
+            "id": "3779431c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vpns = [\n",
                 "    {\n",
                 "        \"generic\": True,\n",
                 "        \"deviceId\": 182,\n",
@@ -2079,78 +2085,78 @@
                 "    }\n",
                 "]\n",
                 "secure_track.add_generic_vpns(vpns)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "07fd0c3f",
+            "id": "54291567",
             "metadata": {},
             "source": [
                 "### Get Generic VPN\n",
                 "\n",
                 "```python\n",
                 "    .get_generic_vpn(\n",
                 "        int_id: Union[int, str]\n",
                 "    ) -> GenericVpn:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "58939c97",
+            "id": "ba06b356",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.get_generic_vpn(1)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e345a6ec",
+            "id": "1fde57d0",
             "metadata": {},
             "source": [
                 "### Get Generic VPNs\n",
                 "\n",
                 "```python\n",
                 "    .get_generic_vpns(\n",
                 "        device_id: Union[int, str]\n",
                 "    ) -> List[GenericVpn]:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "540260da",
+            "id": "835ad23a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.get_generic_vpns(182)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "80750118",
+            "id": "4313f707",
             "metadata": {},
             "source": [
                 "### Update Generic VPN\n",
                 "\n",
                 "```python\n",
                 "    .update_generic_vpn(\n",
                 "        vpn: dict\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "179bb108",
+            "id": "9fdcf3b8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vpn = {\n",
                 "    \"generic\": True,\n",
                 "    \"deviceId\": 182,\n",
                 "    \"interfaceName\": \"777\",\n",
@@ -2158,30 +2164,30 @@
                 "    \"tunnelDestIpAddr\": \"1.1.1.188\"\n",
                 "}\n",
                 "secure_track.update_generic_vpn(vpn)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b7c303f4",
+            "id": "a4227752",
             "metadata": {},
             "source": [
                 "### Update Generic VPNs\n",
                 "\n",
                 "```python\n",
                 "    .update_generic_vpns(\n",
                 "        vpns: List[dict]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8679a89f",
+            "id": "4ca92add",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vpns = [\n",
                 "    {\n",
                 "        \"generic\": True,\n",
                 "        \"deviceId\": 182,\n",
@@ -2200,78 +2206,78 @@
                 "    }\n",
                 "]\n",
                 "secure_track.update_generic_vpns(vpns)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2ccd81c1",
+            "id": "5f73639a",
             "metadata": {},
             "source": [
                 "### Delete Generic VPN\n",
                 "\n",
                 "```python\n",
                 "    .delete_generic_vpn(\n",
                 "        int_id: Union[int, str]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "de23a209",
+            "id": "fb4ea5c3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_vpn(3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b8d94431",
+            "id": "27711563",
             "metadata": {},
             "source": [
                 "### Delete Generic VPNs\n",
                 "\n",
                 "```python\n",
                 "    .delete_generic_vpns(\n",
                 "        mgmt_id: Union[int, str]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fc5ad789",
+            "id": "361344cd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_vpns(92)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5254e530",
+            "id": "e7addfbb",
             "metadata": {},
             "source": [
                 "### Add Generic Transparent Firewalls\n",
                 "\n",
                 "```python\n",
                 "    .add_generic_transparent_firewalls(\n",
                 "        firewalls: List[dict]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c33a1877",
+            "id": "628bb49d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "firewalls = [\n",
                 "    {\n",
                 "        \"outputL3DeviceId\": 22,\n",
                 "        \"outputL3IsGenericDevice\": False,\n",
@@ -2296,54 +2302,54 @@
                 "    }\n",
                 "]\n",
                 "secure_track.add_generic_transparent_firewalls(firewalls)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e345a6ec",
+            "id": "3317c465",
             "metadata": {},
             "source": [
                 "### Get Generic Transparent Firewalls\n",
                 "\n",
                 "```python\n",
                 "    .get_generic_transparent_firewalls(\n",
                 "        device_id: Union[int, str]\n",
                 "    ) -> List[GenericTransparentFirewall]:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "540260da",
+            "id": "f80fb854",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.get_generic_transparent_firewalls(92)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b7c303f4",
+            "id": "ce8033ee",
             "metadata": {},
             "source": [
                 "### Update Generic Transparent Firewalls\n",
                 "\n",
                 "```python\n",
                 "    .update_generic_transparent_firewalls(\n",
                 "        firewalls: List[dict]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8679a89f",
+            "id": "689cc718",
             "metadata": {},
             "outputs": [],
             "source": [
                 "firewalls = [\n",
                 "    {\n",
                 "        \"outputL3DeviceId\": 22,\n",
                 "        \"outputL3IsGenericDevice\": False,\n",
@@ -2368,54 +2374,54 @@
                 "    }\n",
                 "]\n",
                 "secure_track.update_generic_transparent_firewalls(firewalls)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2ccd81c1",
+            "id": "3a1f9e73",
             "metadata": {},
             "source": [
                 "### Delete Generic Transparent Firewalls\n",
                 "\n",
                 "```python\n",
                 "    .delete_generic_transparent_firewall(\n",
                 "        layer_2_data_id: Union[int, str]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "de23a209",
+            "id": "f555070f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_transparent_firewall(3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b8d94431",
+            "id": "71b84520",
             "metadata": {},
             "source": [
                 "### Delete Generic Transparent Firewalls\n",
                 "\n",
                 "```python\n",
                 "    .delete_generic_transparent_firewalls(\n",
                 "        device_id: Union[int, str]\n",
                 "    ) -> None:\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fc5ad789",
+            "id": "3d2a19e8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "secure_track.delete_generic_transparent_firewalls(92)"
             ]
         }
     ],
@@ -2430,16 +2436,15 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.8.13"
+            "pygments_lexer": "ipython3"
         },
         "vscode": {
             "interpreter": {
                 "hash": "7c41d00e68c286b46b1860afd24cc5d8a2454061bfe8b52d5948d3f50d434aa2"
             }
         }
     },
```

### Comparing `pytos2-ce-2.3.11/pytos2/api/__init__.py` & `pytos2-ce-2.3.13/pytos2/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/models/__init__.py` & `pytos2-ce-2.3.13/pytos2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/secureapp/api.py` & `pytos2-ce-2.3.13/pytos2/secureapp/api.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/secureapp/application_identities.py` & `pytos2-ce-2.3.13/pytos2/secureapp/application_identities.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/secureapp/entrypoint.py` & `pytos2-ce-2.3.13/pytos2/secureapp/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/api.py` & `pytos2-ce-2.3.13/pytos2/securechange/api.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/designer.py` & `pytos2-ce-2.3.13/pytos2/securechange/designer.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/designer_verifier_common.py` & `pytos2-ce-2.3.13/pytos2/securechange/designer_verifier_common.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/entrypoint.py` & `pytos2-ce-2.3.13/pytos2/securechange/entrypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -286,7 +286,48 @@
         response = self.api.session.post("attachments", files=attachment)
         if not response.ok:
             try:
                 response.raise_for_status()
             except HTTPError as e:
                 raise ValueError(f"Error Adding Attachment: {e}")
         return response.text
+
+    def add_comment(
+        self,
+        ticket_id: Union[int, str],
+        step_id: Union[int, str],
+        task_id: Union[int, str],
+        comment_content: str,
+        attachment_uuids: Optional[List[str]],
+    ) -> str:
+        def _format_attachments(uuids: List[str]) -> dict:
+            return {"attachment": [{"uid": id} for id in uuids]}
+
+        comment = {"comment": {"content": comment_content}}
+        if attachment_uuids:
+            comment["comment"]["attachments"] = _format_attachments(attachment_uuids)
+
+        response = self.api.session.post(
+            f"tickets/{ticket_id}/steps/{step_id}/tasks/{task_id}/comments",
+            json=comment,
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Comment: {e}")
+
+        return response.text
+
+    def delete_comment(
+        self,
+        ticket_id: Union[int, str],
+        comment_id: Union[int, str],
+    ) -> None:
+        response = self.api.session.delete(
+            f"tickets/{ticket_id}/comments/{comment_id}",
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Comment: {e}")
```

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/fields/__init__.py` & `pytos2-ce-2.3.13/pytos2/securechange/fields/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,16 +615,18 @@
             "targets": {Jsonable.Prop.XSI_TYPE.value: "multi_target"},
         },
         repr=False,
     )
 
     id: Optional[int] = prop(None, cmp=False, jsonify=False)
     order: Optional[str] = prop(None, jsonify=False)
-    sources: list = prop(factory=list, flatify="source", kwargify=classify_ar_object)
-    destinations: list = prop(
+    sources: List[IPNetwork] = prop(
+        factory=list, flatify="source", kwargify=classify_ar_object
+    )
+    destinations: List[IPNetwork] = prop(
         factory=list, flatify="destination", kwargify=classify_ar_object
     )
     source_domain: Optional[str] = prop(None)
     destination_domain: Optional[str] = prop(None)
     services: List[Service] = prop(
         factory=list, flatify="service", kwargify=classify_service_type
     )
@@ -695,15 +697,15 @@
 
     def add_target(
         self,
         device: Union[Device, str, int],
         policy: Union[BindingPolicy, str, None] = None,
         source_zone: Union[Zone, str, None] = None,
         destination_zone: Union[Zone, str, None] = None,
-    ):
+    ) -> Target:
         target = None
         if not isinstance(device, Device):
             _device: Device = St.default.get_device(device)
         else:
             _device = device
 
         if _device is None:
@@ -1412,15 +1414,15 @@
         None, cmp=False, repr=False, jsonify=False
     )
 
     @property
     def ars(self) -> List[AccessRequest]:
         return self.access_requests
 
-    def add_ar(self):
+    def add_ar(self) -> AccessRequest:
         if len(self.access_requests) == 1:
             ar1 = self.access_requests[0]
             if all(
                 (
                     x.at_type is AtType.ANY
                     for x in ar1.sources + ar1.destinations + ar1.services + ar1.targets
                 )
@@ -1468,15 +1470,15 @@
         }
 
     def add_group_change(
         self,
         name: Optional[str] = None,
         device: Union[None, int, str] = None,
         uid: Optional[str] = None,
-    ):
+    ) -> GroupChange:
         device_id = None
         kwargs: dict = dict(parent_field=self)
         if not uid and (not name or not device):
             raise ValueError("name and device arguments must be passed if uid is None")
         if device:
             device_obj = St.default.get_device(device)
             if device_obj is None:
```

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/fields/rule_operation.py` & `pytos2-ce-2.3.13/pytos2/securechange/fields/rule_operation.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/network_object.py` & `pytos2-ce-2.3.13/pytos2/securechange/network_object.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/risk_results.py` & `pytos2-ce-2.3.13/pytos2/securechange/risk_results.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/rule.py` & `pytos2-ce-2.3.13/pytos2/securechange/rule.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/service.py` & `pytos2-ce-2.3.13/pytos2/securechange/service.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/ticket.py` & `pytos2-ce-2.3.13/pytos2/securechange/ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -415,15 +415,15 @@
         if isinstance(step, dict):
             # extract the current_step name from the API output
             step = step.get("name")
         current_step = self.get_step(step)
         if current_step:
             self._current_step = current_step
 
-    def create_step(self, name):
+    def create_step(self, name) -> Step:
         step = Step(name=name)
         self.steps.append(step)
         return step
 
     def get_step(self, identifier: Union[int, str]) -> Optional[Step]:
         step = None
         if isinstance(identifier, int):
@@ -499,14 +499,59 @@
             return self.current_task.access_request
         return None
 
     @property
     def ar(self) -> Optional[MultiAccessRequest]:
         return self.access_request
 
+    def add_comment(
+        self,
+        comment: str,
+        attachment_uuids: List[str] = None,
+        step_id: Union[int, str] = None,
+        task_id: Union[int, str] = None,
+    ) -> str:
+        if step_id is None:
+            step_id = self.current_step.id
+
+        if task_id is None:
+            task_id = self.current_task.id
+        return Scw.add_comment(
+            Scw.default, self.id, step_id, task_id, comment, attachment_uuids
+        )
+
+    def add_comments(
+        self,
+        comments: List[Comment],
+        step_id: Union[int, str] = None,
+        task_id: Union[int, str] = None,
+    ) -> List[str]:
+        return [
+            self.add_comment(
+                comment.content,
+                [a.uid for a in comment.attachments] if comment.attachments else None,
+                step_id,
+                task_id,
+            )
+            for comment in comments
+        ]
+
+    def delete_comment(
+        self,
+        comment_id: Union[int, str] = None,
+    ):
+        Scw.delete_comment(Scw.default, self.id, comment_id)
+
+    def delete_comments(
+        self,
+        comment_ids: List[Union[int, str]],
+    ):
+        for id in comment_ids:
+            self.delete_comment(id)
+
     def post(self) -> "Ticket":
         res = Scw.default.api.session.post("tickets", json=self.post_json)
         if res.ok:
             created_url = res.headers.get("Location", "")
             tid: str = created_url.split("/")[-1]
             return Scw.default.get_ticket(int(tid))
         else:
```

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/trigger.py` & `pytos2-ce-2.3.13/pytos2/securechange/trigger.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/user.py` & `pytos2-ce-2.3.13/pytos2/securechange/user.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securechange/verifier.py` & `pytos2-ce-2.3.13/pytos2/securechange/verifier.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/api.py` & `pytos2-ce-2.3.13/pytos2/securetrack/api.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/device.py` & `pytos2-ce-2.3.13/pytos2/securetrack/device.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/entrypoint.py` & `pytos2-ce-2.3.13/pytos2/securetrack/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/generic_interface.py` & `pytos2-ce-2.3.13/pytos2/securetrack/generic_interface.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/generic_interface_customer.py` & `pytos2-ce-2.3.13/pytos2/securetrack/generic_interface_customer.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/generic_route.py` & `pytos2-ce-2.3.13/pytos2/securetrack/generic_route.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/generic_transparent_firewall.py` & `pytos2-ce-2.3.13/pytos2/securetrack/generic_transparent_firewall.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/generic_vpn.py` & `pytos2-ce-2.3.13/pytos2/securetrack/generic_vpn.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/interface.py` & `pytos2-ce-2.3.13/pytos2/securetrack/interface.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/network_object.py` & `pytos2-ce-2.3.13/pytos2/securetrack/network_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,27 @@
     VIP_NAT_INFO = "vipNatInfoDTO"
     DIP_NAT_INFO = "dipNatInfoDTO"
     CHECKPOINT_NAT_INFO = "checkpointNatInfoDTO"
     FORTIGATE_NAT_INFO = "fortigateNatInfoDTO"
 
 
 class NetworkObjectXsiType(Enum):
+    BASIC_NETWORK_OBJECT = "basicNetworkObjectDTO"
+    CLOUD_SECURITY_GROUP = "cloudSecurityGroupDTO"
     DOMAIN_NETWORK_OBJECT = "DomainNetworkObjectDTO"
     HOST_NETWORK_OBJECT = "hostNetworkObjectDTO"
     HOST_NETWORK_OBJECT_WITH_INTERFACES = "hostNetworkObjectWithInterfacesDTO"
     IDENTITY_AWARENESS = "identityAwarenessDTO"
     IDENTITY_AWARENESS_USER = "identityAwarenessUserDTO"
     NETWORK_OBJECT = "networkObjectDTO"
-    BASIC_NETWORK_OBJECT = "basicNetworkObjectDTO"
     NETWORK_OBJECT_GROUP = "networkObjectGroupDTO"
-    CLOUD_SECURITY_GROUP = "cloudSecurityGroupDTO"
     NETWORK_OBJECT_VIRTUAL_SERVER = "networkObjectVirtualServerDTO"
     RANGE_NETWORK_OBJECT = "rangeNetworkObjectDTO"
     SUBNET_NETWORK_OBJECT = "subnetNetworkObjectDTO"
+    VM_NETWORK_OBJECT = "VMInstanceDTO"
 
 
 @propify
 class NatInfo(Jsonable):
     xsi_type: Optional[NatXsiType] = prop(
         None, key=Jsonable.Prop.XSI_TYPE.value, repr=False
     )
@@ -485,25 +486,36 @@
         USERS = "users"
         NETWORKS = "networks"
 
     users: List[IdentityAwarenessUser] = prop(factory=list)
     networks: List[ObjectReference] = prop(factory=list)
 
 
+@propify
+class VMNetworkObject(NetworkObject):
+    xsi_type: NetworkObjectXsiType = prop(NetworkObjectXsiType.VM_NETWORK_OBJECT)
+    id: Optional[str] = prop(None)
+    type: NetworkObject.Type = prop(NetworkObject.Type.HOST)
+    ip: Optional[IPAddress] = prop(None)
+    interfaces: List[Interface] = prop(factory=list, flatify="interface")
+    state: Optional[str] = prop(None)
+
+
 def classify_network_object(obj):
     return (
         {
             NetworkObjectXsiType.DOMAIN_NETWORK_OBJECT.value: DomainNetworkObject,
             NetworkObjectXsiType.HOST_NETWORK_OBJECT.value: HostNetworkObject,
             NetworkObjectXsiType.HOST_NETWORK_OBJECT_WITH_INTERFACES.value: HostNetworkObjectWithInterfaces,
             NetworkObjectXsiType.IDENTITY_AWARENESS.value: IdentityAwareness,
             NetworkObjectXsiType.BASIC_NETWORK_OBJECT.value: BasicNetworkObject,
             NetworkObjectXsiType.NETWORK_OBJECT.value: NetworkObject,
             NetworkObjectXsiType.NETWORK_OBJECT_GROUP.value: NetworkObjectGroup,
             NetworkObjectXsiType.CLOUD_SECURITY_GROUP.value: CloudSecurityGroup,
             NetworkObjectXsiType.NETWORK_OBJECT_VIRTUAL_SERVER.value: NetworkObjectVirtualServer,
             NetworkObjectXsiType.RANGE_NETWORK_OBJECT.value: RangeNetworkObject,
             NetworkObjectXsiType.SUBNET_NETWORK_OBJECT.value: SubnetNetworkObject,
+            NetworkObjectXsiType.VM_NETWORK_OBJECT.value: VMNetworkObject,
         }
         .get(obj.get(Jsonable.Prop.XSI_TYPE.value), UnMapped)
         .kwargify(obj)
     )
```

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/revision.py` & `pytos2-ce-2.3.13/pytos2/securetrack/revision.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/rule.py` & `pytos2-ce-2.3.13/pytos2/securetrack/rule.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/service_object.py` & `pytos2-ce-2.3.13/pytos2/securetrack/service_object.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/securetrack/zone.py` & `pytos2-ce-2.3.13/pytos2/securetrack/zone.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/utils/__init__.py` & `pytos2-ce-2.3.13/pytos2/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2/utils/cache.py` & `pytos2-ce-2.3.13/pytos2/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/pytos2_ce.egg-info/SOURCES.txt` & `pytos2-ce-2.3.13/pytos2_ce.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 .gitignore
 .gitlab-ci.yml
+.pre-commit-config.yaml
 CHANGELOG.md
 LICENSE
 README.md
 dev-requirements.txt
 mypy.ini
 requirements.txt
 setup.py
 tox.ini
-doc/.env
-doc/Jupyter Notebook Setup.md
-doc/init.py
 doc/pytos2-ce.ipynb
-doc/assets/securechange-closed.png
-doc/assets/securechange-step-1.png
-doc/assets/securechange-step-2-edit-1.png
-doc/assets/securechange-step-2-edit-2.png
-doc/assets/securechange-step-2.png
-doc/assets/securechange-step-3.png
+docs/.env
+docs/Basic Usage.ipynb
+docs/Jupyter Notebook Setup.md
+docs/basic_trigger.py
+docs/contributing.md
+docs/init.py
+docs/pytos2-ce.ipynb
+docs/assets/securechange-closed.png
+docs/assets/securechange-step-1.png
+docs/assets/securechange-step-2-edit-1.png
+docs/assets/securechange-step-2-edit-2.png
+docs/assets/securechange-step-2.png
+docs/assets/securechange-step-3.png
 pytos2/py.typed
 pytos2/api/__init__.py
 pytos2/models/__init__.py
 pytos2/secureapp/__init__.py
 pytos2/secureapp/api.py
 pytos2/secureapp/application_identities.py
 pytos2/secureapp/entrypoint.py
```

### Comparing `pytos2-ce-2.3.11/setup.py` & `pytos2-ce-2.3.13/setup.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/api_test.py` & `pytos2-ce-2.3.13/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/secureapp/conftest.py` & `pytos2-ce-2.3.13/tests/secureapp/conftest.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/secureapp/entrypoint_test.py` & `pytos2-ce-2.3.13/tests/secureapp/entrypoint_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/secureapp/json/application_identities.json` & `pytos2-ce-2.3.13/tests/secureapp/json/application_identities.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/api_test.py` & `pytos2-ce-2.3.13/tests/securechange/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/ar_service_test.py` & `pytos2-ce-2.3.13/tests/securechange/ar_service_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/conftest.py` & `pytos2-ce-2.3.13/tests/securechange/conftest.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/designer_test.py` & `pytos2-ce-2.3.13/tests/securechange/designer_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/entrypoint_test.py` & `pytos2-ce-2.3.13/tests/securechange/entrypoint_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -95,7 +95,64 @@
             f"https://198.18.0.1/securechangeworkflow/api/securechange/attachments",
             id,
         )
 
         uuid = scw.add_attachment("tests/securechange/files/test.pdf")
         assert isinstance(uuid, str)
         assert uuid == id
+
+    @responses.activate
+    def test_add_attachment(self, scw):
+        id = "1"
+        ticket_id = 1
+        step_id = 1
+        task_id = 1
+        responses.add(
+            responses.POST,
+            f"https://198.18.0.1/securechangeworkflow/api/securechange/tickets/{ticket_id}/steps/{step_id}/tasks/{task_id}/comments",
+            id,
+        )
+
+        comment_id = scw.add_comment(
+            ticket_id,
+            step_id,
+            task_id,
+            "New Comment",
+            ["b5672678-d9c5-46ee-87cc-d8fa7fce1a43"],
+        )
+        assert isinstance(comment_id, str)
+        assert comment_id == id
+
+    @responses.activate
+    def test_delete_comment(self, scw):
+        """Delete comment by ticket and comment id"""
+        responses.add(
+            responses.DELETE,
+            f"https://198.18.0.1/securechangeworkflow/api/securechange/tickets/404/comments/404",
+            status=404,
+        )
+
+        responses.add(
+            responses.DELETE,
+            f"https://198.18.0.1/securechangeworkflow/api/securechange/tickets/1/comments/1",
+            status=200,
+        )
+
+        test_one = scw.delete_comment(1, 1)
+        test_two = scw.delete_comment(1, f"1")
+        test_three = scw.delete_comment(f"1", 1)
+        assert all([comment is None for comment in [test_one, test_two, test_three]])
+
+        with pytest.raises(ValueError) as exception:
+            scw.delete_comment(404, 404)
+        assert "Not Found" in str(exception.value)
+
+        with pytest.raises(ValueError) as exception:
+            scw.delete_comment(404, f"404")
+        assert "Not Found" in str(exception.value)
+        with pytest.raises(ValueError) as exception:
+            scw.delete_comment(f"404", 404)
+        assert "Not Found" in str(exception.value)
+
+        with pytest.raises(ValueError) as exception:
+            scw.delete_comment(f"404", f"404")
+        assert "Not Found" in str(exception.value)
```

### Comparing `pytos2-ce-2.3.11/tests/securechange/fields_test.py` & `pytos2-ce-2.3.13/tests/securechange/fields_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/all_fields-workflow.json` & `pytos2-ce-2.3.13/tests/securechange/json/all_fields-workflow.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_icmp_service_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_icmp_service_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_group_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_group_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_host_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_host_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_range_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_range_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_subnet_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_network_subnet_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_new_rule-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule_any_service-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_new_rule_any_service-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_service_group-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_service_group-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/add_transport_service_object-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/add_transport_service_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_251.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/designer_result_251.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_instruction_update_rule.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/designer_result_instruction_update_rule.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/designer_results.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results_multi_instructions.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/designer_results_multi_instructions.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/designer/update_rule-instruction.json` & `pytos2-ce-2.3.13/tests/securechange/json/designer/update_rule-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/clone_server_policy_request-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/clone_server_policy_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_all_service_types.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request_with_all_service_types.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_designer_results-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_access_request_with_designer_results-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_group_change-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json.old` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_group_change-field.json.old`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/multi_server_decommission_request-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/multi_server_decommission_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/source_mod.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/rule_modification/source_mod.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification_field-field.json` & `pytos2-ce-2.3.13/tests/securechange/json/field/rule_modification_field-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/risk_results_ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/risk_results_ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/all_fields-ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/all_fields-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/closed_group_modify-ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/closed_group_modify-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/dynamic_assignment-ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/dynamic_assignment-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_access_request-ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/open_with_access_request-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_group_modify-ticket.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/open_with_group_modify-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/redo.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/redo.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_assigned.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/ticket_search_assigned.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_by_step_name.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/ticket_search_by_step_name.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-0-99.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/tickets-0-99.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-100-199.json` & `pytos2-ce-2.3.13/tests/securechange/json/ticket/tickets-100-199.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/users/all_users.json` & `pytos2-ce-2.3.13/tests/securechange/json/users/all_users.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/users/user_45.json` & `pytos2-ce-2.3.13/tests/securechange/json/users/user_45.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/users/users_by_username.json` & `pytos2-ce-2.3.13/tests/securechange/json/users/users_by_username.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/json/verifier/verifier_result_199.json` & `pytos2-ce-2.3.13/tests/securechange/json/verifier/verifier_result_199.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/object_test.py` & `pytos2-ce-2.3.13/tests/securechange/object_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/risk_results_test.py` & `pytos2-ce-2.3.13/tests/securechange/risk_results_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/ticket_test.py` & `pytos2-ce-2.3.13/tests/securechange/ticket_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/trigger_test.py` & `pytos2-ce-2.3.13/tests/securechange/trigger_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securechange/verifier_test.py` & `pytos2-ce-2.3.13/tests/securechange/verifier_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/api_test.py` & `pytos2-ce-2.3.13/tests/securetrack/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/conftest.py` & `pytos2-ce-2.3.13/tests/securetrack/conftest.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/device_test.py` & `pytos2-ce-2.3.13/tests/securetrack/device_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/domain_test.py` & `pytos2-ce-2.3.13/tests/securetrack/domain_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_ignored_interface_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_ignored_interface_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_interface_customer_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_interface_customer_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_interface_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_interface_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_route_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_route_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_transparent_firewall_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_transparent_firewall_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/generic_vpn_test.py` & `pytos2-ce-2.3.13/tests/securetrack/generic_vpn_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/interface_test.py` & `pytos2-ce-2.3.13/tests/securetrack/interface_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/join_cloud_test.py` & `pytos2-ce-2.3.13/tests/securetrack/join_cloud_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/devices/devices.json` & `pytos2-ce-2.3.13/tests/securetrack/json/devices/devices.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/devices/for-rule-test.json` & `pytos2-ce-2.3.13/tests/securetrack/json/devices/for-rule-test.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/domains/domains.json` & `pytos2-ce-2.3.13/tests/securetrack/json/domains/domains.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/generic_interfaces/mgmt-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/mgmt-3.json` & `pytos2-ce-2.3.13/tests/securetrack/json/generic_routes/mgmt-3.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/device-9.json` & `pytos2-ce-2.3.13/tests/securetrack/json/generic_transparent_firewalls/device-9.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-interfaces.json` & `pytos2-ce-2.3.13/tests/securetrack/json/interfaces/device8-interfaces.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-objects.json` & `pytos2-ce-2.3.13/tests/securetrack/json/interfaces/device8-objects.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/157.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/174.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/181.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/184.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/243.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/243.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/5.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/identity_awareness.json` & `pytos2-ce-2.3.13/tests/securetrack/json/network_objects/identity_awareness.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/1-all.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/1-all.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-10.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-10.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-105.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-105.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-11.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-11.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-114.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-114.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-115.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-115.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-12.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-12.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-120.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-120.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-121.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-121.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-123.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-123.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-144.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-144.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-157.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-159.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-159.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-160.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-160.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-161.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-161.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-166.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-166.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-174.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-179.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-179.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-180.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-180.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-181.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-182.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-182.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-184.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-193.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-193.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-194.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-194.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-195.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-195.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-196.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-196.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-198.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-198.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-20.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-208.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-208.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-21.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-21.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-211.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-211.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-215.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-215.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-216.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-216.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-217.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-217.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-218.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-218.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-32.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-32.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-37.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-37.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-38.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-38.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-5.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-58.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-58.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-59.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-59.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-65.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-65.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-7.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-7.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-75.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-75.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-77.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-77.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-8.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-89.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-89.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-90.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-90.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-91.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-91.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-92.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/device-92.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2226.json` & `pytos2-ce-2.3.13/tests/securetrack/json/revisions/revision-2226.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1-add-documentation.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-1-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-105.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-105.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-114.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-114.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-115.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-115.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-120.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-120.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-121.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-121.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-123.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-123.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-144.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-144.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-157.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-174.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-179.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-179.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-181.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-184.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-193.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-193.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-194.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-194.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-196.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-196.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-198.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-198.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-add-documentation.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-with-uid.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20-with-uid.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-208.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-208.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-211.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-211.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-215.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-215.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-216.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-216.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-217.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-217.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-218.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-218.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-220.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-220.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5-add-documentation.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-5-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-59.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-59.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-60.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-60.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-61.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-61.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-77.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-77.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8-add-documentation.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-8-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-8.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-92.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/device-92.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/kwargify-rules-test-data.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/kwargify-rules-test-data.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/revision-2285-with-uid.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/revision-2285-with-uid.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/rule_search-105-all-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-2.json` & `pytos2-ce-2.3.13/tests/securetrack/json/rules/rule_search-105-all-2.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/services/1.json` & `pytos2-ce-2.3.13/tests/securetrack/json/services/1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/services/aurora339.json` & `pytos2-ce-2.3.13/tests/securetrack/json/services/aurora339.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json` & `pytos2-ce-2.3.13/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json` & `pytos2-ce-2.3.13/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-descendants-80.json` & `pytos2-ce-2.3.13/tests/securetrack/json/zones/zone-descendants-80.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/json/zones/zones.json` & `pytos2-ce-2.3.13/tests/securetrack/json/zones/zones.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/network_object_test.py` & `pytos2-ce-2.3.13/tests/securetrack/network_object_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/revision_test.py` & `pytos2-ce-2.3.13/tests/securetrack/revision_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/rule_test.py` & `pytos2-ce-2.3.13/tests/securetrack/rule_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/service_test.py` & `pytos2-ce-2.3.13/tests/securetrack/service_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/securetrack/zone_test.py` & `pytos2-ce-2.3.13/tests/securetrack/zone_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/utils/cache_test.py` & `pytos2-ce-2.3.13/tests/utils/cache_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.11/tests/utils_test.py` & `pytos2-ce-2.3.13/tests/utils_test.py`

 * *Files identical despite different names*

