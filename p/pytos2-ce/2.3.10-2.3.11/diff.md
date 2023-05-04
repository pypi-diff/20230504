# Comparing `tmp/pytos2-ce-2.3.10.tar.gz` & `tmp/pytos2-ce-2.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytos2-ce-2.3.10.tar", last modified: Tue Dec 20 06:51:24 2022, max compression
+gzip compressed data, was "pytos2-ce-2.3.11.tar", last modified: Thu May  4 12:57:39 2023, max compression
```

## Comparing `pytos2-ce-2.3.10.tar` & `pytos2-ce-2.3.11.tar`

### file list

```diff
@@ -1,516 +1,560 @@
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.795517 pytos2-ce-2.3.10/
--rw-r--r--   0 chris.blake   (502) staff       (20)       80 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/.gitignore
--rw-r--r--   0 chris.blake   (502) staff       (20)      631 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/.gitlab-ci.yml
--rw-r--r--   0 chris.blake   (502) staff       (20)     2468 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/CHANGELOG.md
--rw-r--r--   0 chris.blake   (502) staff       (20)    10781 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/LICENSE
--rw-r--r--   0 chris.blake   (502) staff       (20)     8479 2022-12-20 06:51:24.795305 pytos2-ce-2.3.10/PKG-INFO
--rw-r--r--   0 chris.blake   (502) staff       (20)     8321 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/README.md
--rw-r--r--   0 chris.blake   (502) staff       (20)       44 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/dev-requirements.txt
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.656697 pytos2-ce-2.3.10/doc/
--rw-r--r--   0 chris.blake   (502) staff       (20)   176021 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-closed.png
--rw-r--r--   0 chris.blake   (502) staff       (20)   182801 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-step-1.png
--rw-r--r--   0 chris.blake   (502) staff       (20)   188759 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-step-2-edit-1.png
--rw-r--r--   0 chris.blake   (502) staff       (20)   181652 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-step-2-edit-2.png
--rw-r--r--   0 chris.blake   (502) staff       (20)   185275 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-step-2.png
--rw-r--r--   0 chris.blake   (502) staff       (20)   187802 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/doc/securechange-step-3.png
--rw-r--r--   0 chris.blake   (502) staff       (20)       89 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/mypy.ini
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.657022 pytos2-ce-2.3.10/pytos2/
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.657144 pytos2-ce-2.3.10/pytos2/api/
--rw-r--r--   0 chris.blake   (502) staff       (20)     4051 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/api/__init__.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.657308 pytos2-ce-2.3.10/pytos2/models/
--rw-r--r--   0 chris.blake   (502) staff       (20)     1197 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/models/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/py.typed
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.658019 pytos2-ce-2.3.10/pytos2/secureapp/
--rw-r--r--   0 chris.blake   (502) staff       (20)      112 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/secureapp/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      731 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/secureapp/api.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      713 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/secureapp/application_identities.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1799 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/secureapp/entrypoint.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.662028 pytos2-ce-2.3.10/pytos2/securechange/
--rw-r--r--   0 chris.blake   (502) staff       (20)      172 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     4017 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/api.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     8022 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/designer.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     7928 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/designer_verifier_common.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      205 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/device.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     9395 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/pytos2/securechange/entrypoint.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.662631 pytos2-ce-2.3.10/pytos2/securechange/fields/
--rw-r--r--   0 chris.blake   (502) staff       (20)    58171 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/fields/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      414 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/fields/binding.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    20741 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/fields/rule_operation.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    10020 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/network_object.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     8168 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/risk_results.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     2756 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/rule.py
--rw-r--r--   0 chris.blake   (502) staff       (20)   104439 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/service.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    22934 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/pytos2/securechange/ticket.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    13112 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/trigger.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     3309 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/user.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     4519 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securechange/verifier.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.665794 pytos2-ce-2.3.10/pytos2/securetrack/
--rw-r--r--   0 chris.blake   (502) staff       (20)       77 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    10366 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/api.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     6456 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/device.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      283 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/domain.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    61483 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/pytos2/securetrack/entrypoint.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      293 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/generic_device.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      727 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/pytos2/securetrack/generic_interface.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     3325 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/interface.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    16798 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/network_object.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      192 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/policy_browser.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     4932 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/revision.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    14094 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/rule.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     6998 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/service_object.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      237 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/topology.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     2677 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/securetrack/zone.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.666152 pytos2-ce-2.3.10/pytos2/utils/
--rw-r--r--   0 chris.blake   (502) staff       (20)    13996 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/utils/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     3127 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/pytos2/utils/cache.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.667019 pytos2-ce-2.3.10/pytos2_ce.egg-info/
--rw-r--r--   0 chris.blake   (502) staff       (20)     8479 2022-12-20 06:51:24.000000 pytos2-ce-2.3.10/pytos2_ce.egg-info/PKG-INFO
--rw-r--r--   0 chris.blake   (502) staff       (20)    22084 2022-12-20 06:51:24.000000 pytos2-ce-2.3.10/pytos2_ce.egg-info/SOURCES.txt
--rw-r--r--   0 chris.blake   (502) staff       (20)        1 2022-12-20 06:51:24.000000 pytos2-ce-2.3.10/pytos2_ce.egg-info/dependency_links.txt
--rw-r--r--   0 chris.blake   (502) staff       (20)      129 2022-12-20 06:51:24.000000 pytos2-ce-2.3.10/pytos2_ce.egg-info/requires.txt
--rw-r--r--   0 chris.blake   (502) staff       (20)        7 2022-12-20 06:51:24.000000 pytos2-ce-2.3.10/pytos2_ce.egg-info/top_level.txt
--rw-r--r--   0 chris.blake   (502) staff       (20)      106 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/requirements.txt
--rw-r--r--   0 chris.blake   (502) staff       (20)       38 2022-12-20 06:51:24.795567 pytos2-ce-2.3.10/setup.cfg
--rw-r--r--   0 chris.blake   (502) staff       (20)      812 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/setup.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.667792 pytos2-ce-2.3.10/tests/
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     4555 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/api_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.668607 pytos2-ce-2.3.10/tests/secureapp/
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/secureapp/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      914 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/secureapp/conftest.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      610 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/secureapp/entrypoint_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.668844 pytos2-ce-2.3.10/tests/secureapp/json/
--rw-r--r--   0 chris.blake   (502) staff       (20)  1337893 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/secureapp/json/application_identities.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.675696 pytos2-ce-2.3.10/tests/securechange/
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     3511 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/api_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     8758 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/ar_service_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     8399 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/conftest.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    25460 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/designer_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     3149 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securechange/entrypoint_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    28799 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/fields_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.676359 pytos2-ce-2.3.10/tests/securechange/json/
--rw-r--r--   0 chris.blake   (502) staff       (20)    35674 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/all_fields-workflow.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      201 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/application_details.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.680097 pytos2-ce-2.3.10/tests/securechange/json/designer/
--rw-r--r--   0 chris.blake   (502) staff       (20)      663 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_icmp_service_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1854 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_group_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      726 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_host_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      755 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_range_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      667 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_subnet_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     9066 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_new_rule-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     4094 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_new_rule_any_service-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1721 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_service_group-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      678 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/add_transport_service_object-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     7682 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/designer_result_251.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    20023 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/designer_result_instruction_update_rule.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    19907 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/designer_results.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   113035 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/designer_results_multi_instructions.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      171 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/fully_implemented-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      217 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/fully_implemented_since_no_security-instruction.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    13618 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/designer/update_rule-instruction.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.685230 pytos2-ce-2.3.10/tests/securechange/json/field/
--rw-r--r--   0 chris.blake   (502) staff       (20)      117 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/approve_reject-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       91 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/checkbox-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1159 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/clone_server_policy_request-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       84 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/date-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      262 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/drop_down_list-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      110 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/hyperlink-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       78 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/manager-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3986 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     9895 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request_with_all_service_types.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2128 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request_with_designer_results-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    21739 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_group_change-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    13017 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_group_change-field.json.old
--rw-r--r--   0 chris.blake   (502) staff       (20)      255 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_hyperlink-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      163 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_network_object-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      868 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_server_decommission_request-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      142 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_service-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      123 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_target-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      181 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_text_area-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      204 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multi_text_field-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/multiple_selection-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      129 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/read_only-field.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.685436 pytos2-ce-2.3.10/tests/securechange/json/field/rule_modification/
--rw-r--r--   0 chris.blake   (502) staff       (20)    43082 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/rule_modification/source_mod.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    10726 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/rule_modification_field-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      119 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/text_area-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       88 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/text_field-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       78 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/field/time-field.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    34462 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/risk_results_ticket.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.691555 pytos2-ce-2.3.10/tests/securechange/json/ticket/
--rw-r--r--   0 chris.blake   (502) staff       (20)    32220 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/all_fields-ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     5565 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/closed_group_modify-ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    12132 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/dynamic_assignment-ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    50426 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/open_with_access_request-ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    20839 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/open_with_group_modify-ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      215 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/post_bad_ticket.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    21757 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/redo.json
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/specific_workflow.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      153 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/ticket_not_found.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   346577 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/ticket_search_assigned.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     5929 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/ticket_search_by_step_name.json
--rw-r--r--   0 chris.blake   (502) staff       (20)  5944047 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/tickets-0-99.json
--rw-r--r--   0 chris.blake   (502) staff       (20)  9501053 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/ticket/tickets-100-199.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.702714 pytos2-ce-2.3.10/tests/securechange/json/users/
--rw-r--r--   0 chris.blake   (502) staff       (20)  1525217 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/users/all_users.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2103 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/users/user_45.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2095 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/users/users_by_username.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.702990 pytos2-ce-2.3.10/tests/securechange/json/verifier/
--rw-r--r--   0 chris.blake   (502) staff       (20)    28476 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/json/verifier/verifier_result_199.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3617 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/object_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1196 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/risk_results_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    18093 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/ticket_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    10875 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/trigger_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      793 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securechange/verifier_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.705533 pytos2-ce-2.3.10/tests/securetrack/
--rw-r--r--   0 chris.blake   (502) staff       (20)        0 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/__init__.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    21743 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/api_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    16281 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/conftest.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1592 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/device_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1726 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/domain_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)       31 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/entrypoint_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     7253 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/generic_interface_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1351 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/interface_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.652409 pytos2-ce-2.3.10/tests/securetrack/json/
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.731895 pytos2-ce-2.3.10/tests/securetrack/json/devices/
--rw-r--r--   0 chris.blake   (502) staff       (20)      332 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/8.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      455 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/ASAv.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      228 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      241 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-10.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      277 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-105.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      226 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-11.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      276 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-114.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      273 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-115.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      263 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-119.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      226 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-12.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      292 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-120.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      296 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-121.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      295 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-123.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      250 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-142.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      274 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-144.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      247 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-156.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      267 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-157.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      273 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-159.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      273 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-160.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      275 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-161.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      242 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-166.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      272 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-174.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      301 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-179.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      303 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-180.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      298 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-181.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      305 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-182.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      255 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-184.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      255 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-193.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      243 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-194.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      269 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-195.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      271 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-196.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      271 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-198.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      242 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-20.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      340 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-206.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      212 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-207.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      272 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-208.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      271 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-209.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      325 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-21.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      270 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-211.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      244 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-212.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      248 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-213.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      231 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-214.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      291 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-215.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      293 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-216.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      286 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-217.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      287 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-218.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      235 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-219.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      215 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-230.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      270 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-231.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      259 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-232.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-233.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-234.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-235.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      254 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-236.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      193 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-237.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      213 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-239.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      193 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-240.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      240 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-243.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      247 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-244.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      275 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-245.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      251 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-246.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      228 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-32.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      247 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-348.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      332 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-349.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      227 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-37.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      225 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-38.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      231 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-408.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      249 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-411.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      237 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-416.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      229 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-5.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      193 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-552.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      219 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-553.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      256 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-554.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      254 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-555.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      291 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-556.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      251 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-557.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      246 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-559.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      211 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-561.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      244 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-562.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      207 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-563.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      251 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-564.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      231 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-565.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      262 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-566.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      261 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-567.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      286 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-568.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      285 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-569.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      289 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-570.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      288 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-571.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      260 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-572.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      277 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-573.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      279 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-574.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      268 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-575.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      269 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-576.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      227 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-577.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      245 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-579.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      245 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-58.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      227 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-580.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      249 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-581.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      243 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-582.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      258 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-583.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      279 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-584.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      279 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-585.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-586.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-587.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      283 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-588.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-589.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-59.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      304 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-590.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      280 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-591.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      310 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-592.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      307 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-593.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      307 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-594.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      307 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-595.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      230 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-596.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      205 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-598.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      270 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-60.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      270 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-61.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      281 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-62.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      229 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-622.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      440 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-637.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      244 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-65.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      228 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-7.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      245 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-75.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      276 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-77.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      233 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-8.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      230 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-89.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      253 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-90.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      288 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-91.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      272 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/device-92.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    69102 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/devices.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2508 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/devices/for-rule-test.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.732257 pytos2-ce-2.3.10/tests/securetrack/json/domains/
--rw-r--r--   0 chris.blake   (502) staff       (20)      100 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/domains/domain-7.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1112 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/domains/domains.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.732868 pytos2-ce-2.3.10/tests/securetrack/json/generic_devices/
--rw-r--r--   0 chris.blake   (502) staff       (20)      309 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_devices/generic_devices.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      133 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_devices/generic_devices_filtered.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      415 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_devices/sample_generic_device.csv
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.735787 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/
--rw-r--r--   0 chris.blake   (502) staff       (20)      270 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      225 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-19.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      269 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-2.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      225 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-20.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      269 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-3.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      210 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/int-32.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      777 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/mgmt-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      242 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/mgmt-21.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      479 2022-12-20 06:31:03.000000 pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/mgmt-5.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.736477 pytos2-ce-2.3.10/tests/securetrack/json/interfaces/
--rw-r--r--   0 chris.blake   (502) staff       (20)     3862 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/interfaces/device8-interfaces.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3195 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/interfaces/device8-objects.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      348 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/interfaces/device8-topology-interfaces.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.739627 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/
--rw-r--r--   0 chris.blake   (502) staff       (20)    79537 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/157.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    12288 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/174.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    73209 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/181.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    42360 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/184.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   103018 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/20.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      571 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   119194 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/243.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    36452 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/5.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      585 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1649 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      553 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      859 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1220 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/network_objects/identity_awareness.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.740018 pytos2-ce-2.3.10/tests/securetrack/json/policies/
--rw-r--r--   0 chris.blake   (502) staff       (20)      356 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/policies/157.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      337 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/policies/20.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.756013 pytos2-ce-2.3.10/tests/securetrack/json/revisions/
--rw-r--r--   0 chris.blake   (502) staff       (20)    17051 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/1-all.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    15168 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    18723 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    12288 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-10.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    31413 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-105.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      928 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-11.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    31074 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-114.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     5017 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-115.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      476 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-119.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      935 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-12.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2748 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-120.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1385 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-121.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      931 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-123.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      477 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-142.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1387 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-144.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       16 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-156.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    24971 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-157.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2294 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-159.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2294 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-160.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2294 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-161.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     5479 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-166.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    46903 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-174.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    76878 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-179.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     4644 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-180.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    77093 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-181.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1880 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-182.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    54424 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-184.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    16309 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-193.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    19380 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-194.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    13012 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-195.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    79890 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-196.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    14883 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-198.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    36540 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-20.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      312 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-206.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       15 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-207.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      905 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-208.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-209.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3895 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-21.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      608 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-211.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       15 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-212.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       15 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-213.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       15 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-214.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     4177 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-215.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      608 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-216.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      608 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-217.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      608 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-218.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-219.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-220.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       15 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-221.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3055 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-32.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2446 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-37.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      616 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-38.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    13412 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-5.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      609 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-58.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2109 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-59.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-60.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-61.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-62.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      613 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-65.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     6349 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-7.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      979 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-75.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    11188 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-77.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      440 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-8-latest-revision.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    44184 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-8.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2140 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-89.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3293 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-90.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     1491 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-91.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2136 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-92.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      525 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/revision-2226.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      351 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/revisions/revision-2285.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.787696 pytos2-ce-2.3.10/tests/securetrack/json/rules/
--rw-r--r--   0 chris.blake   (502) staff       (20)    71570 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-1-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    62230 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-10.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   543520 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-105.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-11.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   663431 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-114.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   109786 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-115.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-119.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-12.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   133714 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-120.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    34804 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-121.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     8212 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-123.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-142.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     7255 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-144.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-156.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   157444 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-157.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-159.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-160.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-161.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-166.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    12014 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-174.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   194256 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-179.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-180.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    97136 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-181.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-182.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    55631 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-184.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    23897 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-193.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   141460 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-194.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-195.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   367349 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-196.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    21047 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-198.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   162520 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   162511 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20-with-uid.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   137967 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-206.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-207.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     5714 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-208.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-209.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-21-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-21.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2807 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-211.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-212.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-213.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-214.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   388533 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-215.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    21127 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-216.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    33725 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-217.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    35869 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-218.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-219.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    26022 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-220.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-221.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-32.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-37.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-38.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    32311 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-5-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    27756 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-5.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-58.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    51831 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-59.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    22759 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-60.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    22802 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-61.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-62.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-65.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-7-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-7.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-75.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    87482 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-77.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   542053 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-8-add-documentation.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   479880 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-8.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-89.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-90.json
--rw-r--r--   0 chris.blake   (502) staff       (20)       68 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-91.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    28029 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/device-92.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     3282 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/kwargify-rules-test-data.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   127793 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/revision-2285-with-uid.json
--rw-r--r--   0 chris.blake   (502) staff       (20)  8342101 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/rule_search-105-all-1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   619029 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/rule_search-105-all-2.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      147 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/rules/rule_search-105.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.793501 pytos2-ce-2.3.10/tests/securetrack/json/services/
--rw-r--r--   0 chris.blake   (502) staff       (20)   178425 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/services/1.json
--rw-r--r--   0 chris.blake   (502) staff       (20)   299824 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/services/aurora339.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     6477 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      569 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.793769 pytos2-ce-2.3.10/tests/securetrack/json/topology/
--rw-r--r--   0 chris.blake   (502) staff       (20)       31 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/topology/status.json
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.794830 pytos2-ce-2.3.10/tests/securetrack/json/zones/
--rw-r--r--   0 chris.blake   (502) staff       (20)      250 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/zones/zone-69.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      256 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/zones/zone-78.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      693 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/zones/zone-descendants-80.json
--rw-r--r--   0 chris.blake   (502) staff       (20)      397 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/zones/zone-entries-78.json
--rw-r--r--   0 chris.blake   (502) staff       (20)    10385 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/json/zones/zones.json
--rw-r--r--   0 chris.blake   (502) staff       (20)     2937 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/network_object_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     5196 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/revision_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     4932 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/rule_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)    11536 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/service_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     1624 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/securetrack/zone_test.py
-drwxr-xr-x   0 chris.blake   (502) staff       (20)        0 2022-12-20 06:51:24.795014 pytos2-ce-2.3.10/tests/utils/
--rw-r--r--   0 chris.blake   (502) staff       (20)     1863 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/utils/cache_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)     7383 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tests/utils_test.py
--rw-r--r--   0 chris.blake   (502) staff       (20)      344 2022-10-28 03:36:36.000000 pytos2-ce-2.3.10/tox.ini
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262896 pytos2-ce-2.3.11/
+-rw-r--r--   0 ploch      (502) staff       (20)       80 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/.gitignore
+-rw-r--r--   0 ploch      (502) staff       (20)      631 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/.gitlab-ci.yml
+-rw-r--r--   0 ploch      (502) staff       (20)     5628 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/CHANGELOG.md
+-rw-r--r--   0 ploch      (502) staff       (20)    10781 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/LICENSE
+-rw-r--r--   0 ploch      (502) staff       (20)     8527 2023-05-04 12:57:39.262681 pytos2-ce-2.3.11/PKG-INFO
+-rw-r--r--   0 ploch      (502) staff       (20)     8369 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/README.md
+-rw-r--r--   0 ploch      (502) staff       (20)       44 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/dev-requirements.txt
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.068799 pytos2-ce-2.3.11/doc/
+-rw-r--r--   0 ploch      (502) staff       (20)       72 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/.env
+-rw-r--r--   0 ploch      (502) staff       (20)      222 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/Jupyter Notebook Setup.md
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.071541 pytos2-ce-2.3.11/doc/assets/
+-rw-r--r--   0 ploch      (502) staff       (20)   176021 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-closed.png
+-rw-r--r--   0 ploch      (502) staff       (20)   182801 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-1.png
+-rw-r--r--   0 ploch      (502) staff       (20)   188759 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-1.png
+-rw-r--r--   0 ploch      (502) staff       (20)   181652 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-2.png
+-rw-r--r--   0 ploch      (502) staff       (20)   185275 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-2.png
+-rw-r--r--   0 ploch      (502) staff       (20)   187802 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/assets/securechange-step-3.png
+-rw-r--r--   0 ploch      (502) staff       (20)      640 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/init.py
+-rw-r--r--   0 ploch      (502) staff       (20)    58633 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/doc/pytos2-ce.ipynb
+-rw-r--r--   0 ploch      (502) staff       (20)       89 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/mypy.ini
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.071925 pytos2-ce-2.3.11/pytos2/
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.072057 pytos2-ce-2.3.11/pytos2/api/
+-rw-r--r--   0 ploch      (502) staff       (20)     4051 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/api/__init__.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.072329 pytos2-ce-2.3.11/pytos2/models/
+-rw-r--r--   0 ploch      (502) staff       (20)     1197 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/models/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/py.typed
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.073418 pytos2-ce-2.3.11/pytos2/secureapp/
+-rw-r--r--   0 ploch      (502) staff       (20)      112 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      731 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)      713 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/application_identities.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1799 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/secureapp/entrypoint.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.078412 pytos2-ce-2.3.11/pytos2/securechange/
+-rw-r--r--   0 ploch      (502) staff       (20)      172 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4015 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8022 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/designer.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7928 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/designer_verifier_common.py
+-rw-r--r--   0 ploch      (502) staff       (20)      205 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/device.py
+-rw-r--r--   0 ploch      (502) staff       (20)     9789 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/entrypoint.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.079343 pytos2-ce-2.3.11/pytos2/securechange/fields/
+-rw-r--r--   0 ploch      (502) staff       (20)    58171 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      414 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/binding.py
+-rw-r--r--   0 ploch      (502) staff       (20)    20740 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/fields/rule_operation.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10020 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/network_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8168 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/risk_results.py
+-rw-r--r--   0 ploch      (502) staff       (20)     2756 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/rule.py
+-rw-r--r--   0 ploch      (502) staff       (20)   104439 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/service.py
+-rw-r--r--   0 ploch      (502) staff       (20)    22932 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securechange/ticket.py
+-rw-r--r--   0 ploch      (502) staff       (20)    13112 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/trigger.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securechange/user.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4518 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securechange/verifier.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.085095 pytos2-ce-2.3.11/pytos2/securetrack/
+-rw-r--r--   0 ploch      (502) staff       (20)       77 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10363 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/api.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6456 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/device.py
+-rw-r--r--   0 ploch      (502) staff       (20)      283 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/domain.py
+-rw-r--r--   0 ploch      (502) staff       (20)    77507 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/entrypoint.py
+-rw-r--r--   0 ploch      (502) staff       (20)      293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_device.py
+-rw-r--r--   0 ploch      (502) staff       (20)      447 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_ignored_interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      727 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      519 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_interface_customer.py
+-rw-r--r--   0 ploch      (502) staff       (20)      620 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_route.py
+-rw-r--r--   0 ploch      (502) staff       (20)      830 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_transparent_firewall.py
+-rw-r--r--   0 ploch      (502) staff       (20)      582 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/generic_vpn.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3325 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/interface.py
+-rw-r--r--   0 ploch      (502) staff       (20)      368 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/join_cloud.py
+-rw-r--r--   0 ploch      (502) staff       (20)    16797 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/pytos2/securetrack/network_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/policy_browser.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/revision.py
+-rw-r--r--   0 ploch      (502) staff       (20)    14109 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/pytos2/securetrack/rule.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6998 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/service_object.py
+-rw-r--r--   0 ploch      (502) staff       (20)      237 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/topology.py
+-rw-r--r--   0 ploch      (502) staff       (20)     2677 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/securetrack/zone.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.085550 pytos2-ce-2.3.11/pytos2/utils/
+-rw-r--r--   0 ploch      (502) staff       (20)    13996 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/utils/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3127 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/pytos2/utils/cache.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.086537 pytos2-ce-2.3.11/pytos2_ce.egg-info/
+-rw-r--r--   0 ploch      (502) staff       (20)     8527 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/PKG-INFO
+-rw-r--r--   0 ploch      (502) staff       (20)    23801 2023-05-04 12:57:39.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 ploch      (502) staff       (20)        1 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 ploch      (502) staff       (20)      129 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/requires.txt
+-rw-r--r--   0 ploch      (502) staff       (20)        7 2023-05-04 12:57:38.000000 pytos2-ce-2.3.11/pytos2_ce.egg-info/top_level.txt
+-rw-r--r--   0 ploch      (502) staff       (20)      106 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/requirements.txt
+-rw-r--r--   0 ploch      (502) staff       (20)       38 2023-05-04 12:57:39.263069 pytos2-ce-2.3.11/setup.cfg
+-rw-r--r--   0 ploch      (502) staff       (20)      812 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/setup.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.087146 pytos2-ce-2.3.11/tests/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4555 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/api_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.087828 pytos2-ce-2.3.11/tests/secureapp/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)      914 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)      610 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/entrypoint_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.088008 pytos2-ce-2.3.11/tests/secureapp/json/
+-rw-r--r--   0 ploch      (502) staff       (20)  1337893 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/secureapp/json/application_identities.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.093084 pytos2-ce-2.3.11/tests/securechange/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3511 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/api_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8758 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/ar_service_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     8399 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)    25461 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/designer_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3575 2023-05-04 12:25:16.000000 pytos2-ce-2.3.11/tests/securechange/entrypoint_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    28797 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/fields_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.093364 pytos2-ce-2.3.11/tests/securechange/files/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/files/test.pdf
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.094334 pytos2-ce-2.3.11/tests/securechange/json/
+-rw-r--r--   0 ploch      (502) staff       (20)    35674 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/all_fields-workflow.json
+-rw-r--r--   0 ploch      (502) staff       (20)      201 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/application_details.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.099419 pytos2-ce-2.3.11/tests/securechange/json/designer/
+-rw-r--r--   0 ploch      (502) staff       (20)      663 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_icmp_service_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1854 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_group_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      726 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_host_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      755 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_range_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      667 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_subnet_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     9066 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4094 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule_any_service-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1721 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_service_group-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      678 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/add_transport_service_object-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)     7682 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_251.json
+-rw-r--r--   0 ploch      (502) staff       (20)    20023 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_instruction_update_rule.json
+-rw-r--r--   0 ploch      (502) staff       (20)    19907 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results.json
+-rw-r--r--   0 ploch      (502) staff       (20)   113035 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results_multi_instructions.json
+-rw-r--r--   0 ploch      (502) staff       (20)      171 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/fully_implemented-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)      217 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/fully_implemented_since_no_security-instruction.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13618 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/designer/update_rule-instruction.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.104958 pytos2-ce-2.3.11/tests/securechange/json/field/
+-rw-r--r--   0 ploch      (502) staff       (20)      117 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/approve_reject-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       91 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/checkbox-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1159 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/clone_server_policy_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       84 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/date-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      262 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/drop_down_list-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      110 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/hyperlink-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       78 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/manager-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3986 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)     9895 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_all_service_types.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2128 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_designer_results-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21739 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13017 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json.old
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_hyperlink-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      163 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_network_object-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      868 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_server_decommission_request-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      142 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_service-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      123 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_target-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      181 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_text_area-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      204 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multi_text_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/multiple_selection-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      129 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/read_only-field.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.105141 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/
+-rw-r--r--   0 ploch      (502) staff       (20)    43082 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/source_mod.json
+-rw-r--r--   0 ploch      (502) staff       (20)    10726 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)      119 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/text_area-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       88 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/text_field-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)       78 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/field/time-field.json
+-rw-r--r--   0 ploch      (502) staff       (20)    34462 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/risk_results_ticket.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.114620 pytos2-ce-2.3.11/tests/securechange/json/ticket/
+-rw-r--r--   0 ploch      (502) staff       (20)    32220 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/all_fields-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5565 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/closed_group_modify-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12132 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/dynamic_assignment-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    50426 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_access_request-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    20839 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_group_modify-ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)      215 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/post_bad_ticket.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21757 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/redo.json
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/specific_workflow.json
+-rw-r--r--   0 ploch      (502) staff       (20)      153 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_not_found.json
+-rw-r--r--   0 ploch      (502) staff       (20)   346577 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_assigned.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5929 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_by_step_name.json
+-rw-r--r--   0 ploch      (502) staff       (20)  5944047 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-0-99.json
+-rw-r--r--   0 ploch      (502) staff       (20)  9501053 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-100-199.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.134088 pytos2-ce-2.3.11/tests/securechange/json/users/
+-rw-r--r--   0 ploch      (502) staff       (20)  1525217 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/all_users.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2103 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/user_45.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2095 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/users/users_by_username.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.135711 pytos2-ce-2.3.11/tests/securechange/json/verifier/
+-rw-r--r--   0 ploch      (502) staff       (20)    28476 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/json/verifier/verifier_result_199.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3617 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/object_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1196 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/risk_results_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    18093 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/ticket_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    10874 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securechange/trigger_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)      793 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securechange/verifier_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.140766 pytos2-ce-2.3.11/tests/securetrack/
+-rw-r--r--   0 ploch      (502) staff       (20)        0 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/__init__.py
+-rw-r--r--   0 ploch      (502) staff       (20)    21743 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/api_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    26361 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/conftest.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1592 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/device_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1726 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/domain_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)       31 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/entrypoint_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3984 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_ignored_interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7779 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_interface_customer_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7252 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6468 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_route_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6593 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_transparent_firewall_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     6232 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/generic_vpn_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1351 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/interface_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     3842 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/join_cloud_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.064874 pytos2-ce-2.3.11/tests/securetrack/json/
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.170568 pytos2-ce-2.3.11/tests/securetrack/json/devices/
+-rw-r--r--   0 ploch      (502) staff       (20)      332 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/8.json
+-rw-r--r--   0 ploch      (502) staff       (20)      455 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/ASAv.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      241 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)      277 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)      226 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)      276 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)      263 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)      226 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)      292 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)      296 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)      295 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)      250 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)      274 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)      267 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)      273 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)      275 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)      301 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)      303 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)      298 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)      305 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)      255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)      243 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      340 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)      212 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)      271 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)      325 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)      248 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)      291 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)      293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)      286 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)      287 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)      235 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)      215 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-230.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-231.json
+-rw-r--r--   0 ploch      (502) staff       (20)      259 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-232.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-233.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-234.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-235.json
+-rw-r--r--   0 ploch      (502) staff       (20)      254 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-236.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-237.json
+-rw-r--r--   0 ploch      (502) staff       (20)      213 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-239.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-240.json
+-rw-r--r--   0 ploch      (502) staff       (20)      240 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-243.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-244.json
+-rw-r--r--   0 ploch      (502) staff       (20)      275 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-245.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-246.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)      247 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-348.json
+-rw-r--r--   0 ploch      (502) staff       (20)      332 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-349.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-408.json
+-rw-r--r--   0 ploch      (502) staff       (20)      249 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-411.json
+-rw-r--r--   0 ploch      (502) staff       (20)      237 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-416.json
+-rw-r--r--   0 ploch      (502) staff       (20)      229 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      193 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-552.json
+-rw-r--r--   0 ploch      (502) staff       (20)      219 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-553.json
+-rw-r--r--   0 ploch      (502) staff       (20)      256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-554.json
+-rw-r--r--   0 ploch      (502) staff       (20)      254 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-555.json
+-rw-r--r--   0 ploch      (502) staff       (20)      291 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-556.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-557.json
+-rw-r--r--   0 ploch      (502) staff       (20)      246 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-559.json
+-rw-r--r--   0 ploch      (502) staff       (20)      211 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-561.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-562.json
+-rw-r--r--   0 ploch      (502) staff       (20)      207 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-563.json
+-rw-r--r--   0 ploch      (502) staff       (20)      251 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-564.json
+-rw-r--r--   0 ploch      (502) staff       (20)      231 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-565.json
+-rw-r--r--   0 ploch      (502) staff       (20)      262 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-566.json
+-rw-r--r--   0 ploch      (502) staff       (20)      261 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-567.json
+-rw-r--r--   0 ploch      (502) staff       (20)      286 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-568.json
+-rw-r--r--   0 ploch      (502) staff       (20)      285 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-569.json
+-rw-r--r--   0 ploch      (502) staff       (20)      289 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-570.json
+-rw-r--r--   0 ploch      (502) staff       (20)      288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-571.json
+-rw-r--r--   0 ploch      (502) staff       (20)      260 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-572.json
+-rw-r--r--   0 ploch      (502) staff       (20)      277 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-573.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-574.json
+-rw-r--r--   0 ploch      (502) staff       (20)      268 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-575.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-576.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-577.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-579.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)      227 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-580.json
+-rw-r--r--   0 ploch      (502) staff       (20)      249 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-581.json
+-rw-r--r--   0 ploch      (502) staff       (20)      243 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-582.json
+-rw-r--r--   0 ploch      (502) staff       (20)      258 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-583.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-584.json
+-rw-r--r--   0 ploch      (502) staff       (20)      279 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-585.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-586.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-587.json
+-rw-r--r--   0 ploch      (502) staff       (20)      283 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-588.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-589.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)      304 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-590.json
+-rw-r--r--   0 ploch      (502) staff       (20)      280 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-591.json
+-rw-r--r--   0 ploch      (502) staff       (20)      310 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-592.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-593.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-594.json
+-rw-r--r--   0 ploch      (502) staff       (20)      307 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-595.json
+-rw-r--r--   0 ploch      (502) staff       (20)      230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-596.json
+-rw-r--r--   0 ploch      (502) staff       (20)      205 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-598.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)      229 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-622.json
+-rw-r--r--   0 ploch      (502) staff       (20)      440 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-637.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)      228 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)      245 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)      276 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)      233 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)      230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)      253 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)      288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)      272 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)    69102 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/devices.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2508 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/devices/for-rule-test.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.170973 pytos2-ce-2.3.11/tests/securetrack/json/domains/
+-rw-r--r--   0 ploch      (502) staff       (20)      100 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/domains/domain-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1112 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/domains/domains.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.171610 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/
+-rw-r--r--   0 ploch      (502) staff       (20)      309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/generic_devices.json
+-rw-r--r--   0 ploch      (502) staff       (20)      133 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/generic_devices_filtered.json
+-rw-r--r--   0 ploch      (502) staff       (20)      415 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_devices/sample_generic_device.csv
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.171790 pytos2-ce-2.3.11/tests/securetrack/json/generic_ignored_interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)      281 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_ignored_interfaces/mgmt-10.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.172242 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/
+-rw-r--r--   0 ploch      (502) staff       (20)      373 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      166 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interface_customers/int-cust-74.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.174434 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)      270 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-19.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      225 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      269 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/int-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)      777 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      479 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-5.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.178393 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/
+-rw-r--r--   0 ploch      (502) staff       (20)      481 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/mgmt-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      527 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/mgmt-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      242 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-27.json
+-rw-r--r--   0 ploch      (502) staff       (20)      244 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-28.json
+-rw-r--r--   0 ploch      (502) staff       (20)      265 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-29.json
+-rw-r--r--   0 ploch      (502) staff       (20)      267 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_routes/route-30.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.179241 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/
+-rw-r--r--   0 ploch      (502) staff       (20)      337 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/data-17.json
+-rw-r--r--   0 ploch      (502) staff       (20)      333 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/data-23.json
+-rw-r--r--   0 ploch      (502) staff       (20)      904 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_transparent_firewalls/device-9.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.180606 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/
+-rw-r--r--   0 ploch      (502) staff       (20)      469 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)      417 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/device-3.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-17.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-22.json
+-rw-r--r--   0 ploch      (502) staff       (20)      235 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-24.json
+-rw-r--r--   0 ploch      (502) staff       (20)      210 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/generic_vpns/vpn-25.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.181252 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/
+-rw-r--r--   0 ploch      (502) staff       (20)     3862 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-interfaces.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3195 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-objects.json
+-rw-r--r--   0 ploch      (502) staff       (20)      348 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-topology-interfaces.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.181443 pytos2-ce-2.3.11/tests/securetrack/json/join_clouds/
+-rw-r--r--   0 ploch      (502) staff       (20)       80 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/json/join_clouds/cloud-67.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.191650 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/
+-rw-r--r--   0 ploch      (502) staff       (20)    79537 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/157.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/174.json
+-rw-r--r--   0 ploch      (502) staff       (20)    73209 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/181.json
+-rw-r--r--   0 ploch      (502) staff       (20)    42360 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/184.json
+-rw-r--r--   0 ploch      (502) staff       (20)   103018 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      571 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json
+-rw-r--r--   0 ploch      (502) staff       (20)   119194 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/243.json
+-rw-r--r--   0 ploch      (502) staff       (20)    36452 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      585 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1649 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json
+-rw-r--r--   0 ploch      (502) staff       (20)      553 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json
+-rw-r--r--   0 ploch      (502) staff       (20)      859 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1220 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/network_objects/identity_awareness.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.193000 pytos2-ce-2.3.11/tests/securetrack/json/policies/
+-rw-r--r--   0 ploch      (502) staff       (20)      356 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/policies/157.json
+-rw-r--r--   0 ploch      (502) staff       (20)      337 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/policies/20.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.214947 pytos2-ce-2.3.11/tests/securetrack/json/revisions/
+-rw-r--r--   0 ploch      (502) staff       (20)    17051 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/1-all.json
+-rw-r--r--   0 ploch      (502) staff       (20)    15168 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/1.json
+-rw-r--r--   0 ploch      (502) staff       (20)    18723 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12288 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)    31413 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)      928 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)    31074 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5017 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)      476 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)      935 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2748 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1385 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)      931 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)      477 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1387 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)       16 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)    24971 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2294 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5479 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)    46903 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)    76878 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4644 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)    77093 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1880 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)    54424 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)    16309 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)    19380 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13012 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)    79890 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)    14883 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)    36540 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)      312 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)      905 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3895 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)     4177 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)      608 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-220.json
+-rw-r--r--   0 ploch      (502) staff       (20)       15 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-221.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3055 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2446 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)      616 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)    13412 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)      609 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2109 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)      311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)      613 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)     6349 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)      979 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)    11188 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)      440 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8-latest-revision.json
+-rw-r--r--   0 ploch      (502) staff       (20)    44184 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2140 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3293 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)     1491 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2136 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)      525 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2226.json
+-rw-r--r--   0 ploch      (502) staff       (20)      351 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2285.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.258669 pytos2-ce-2.3.11/tests/securetrack/json/rules/
+-rw-r--r--   0 ploch      (502) staff       (20)    71570 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)    62230 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-10.json
+-rw-r--r--   0 ploch      (502) staff       (20)   543520 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-105.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-11.json
+-rw-r--r--   0 ploch      (502) staff       (20)   663431 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-114.json
+-rw-r--r--   0 ploch      (502) staff       (20)   109786 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-115.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-119.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-12.json
+-rw-r--r--   0 ploch      (502) staff       (20)   133714 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-120.json
+-rw-r--r--   0 ploch      (502) staff       (20)    34804 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-121.json
+-rw-r--r--   0 ploch      (502) staff       (20)     8212 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-123.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-142.json
+-rw-r--r--   0 ploch      (502) staff       (20)     7255 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-144.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-156.json
+-rw-r--r--   0 ploch      (502) staff       (20)   157444 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-157.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-159.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-160.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-161.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-166.json
+-rw-r--r--   0 ploch      (502) staff       (20)    12014 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-174.json
+-rw-r--r--   0 ploch      (502) staff       (20)   194256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-179.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-180.json
+-rw-r--r--   0 ploch      (502) staff       (20)    97136 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-181.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-182.json
+-rw-r--r--   0 ploch      (502) staff       (20)    55631 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-184.json
+-rw-r--r--   0 ploch      (502) staff       (20)    23897 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-193.json
+-rw-r--r--   0 ploch      (502) staff       (20)   141460 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-194.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-195.json
+-rw-r--r--   0 ploch      (502) staff       (20)   367349 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-196.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21047 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-198.json
+-rw-r--r--   0 ploch      (502) staff       (20)   162520 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)   162511 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-with-uid.json
+-rw-r--r--   0 ploch      (502) staff       (20)   137967 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-206.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-207.json
+-rw-r--r--   0 ploch      (502) staff       (20)     5714 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-208.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-209.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-21-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-21.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2807 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-211.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-212.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-213.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-214.json
+-rw-r--r--   0 ploch      (502) staff       (20)   388533 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-215.json
+-rw-r--r--   0 ploch      (502) staff       (20)    21127 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-216.json
+-rw-r--r--   0 ploch      (502) staff       (20)    33725 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-217.json
+-rw-r--r--   0 ploch      (502) staff       (20)    35869 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-218.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-219.json
+-rw-r--r--   0 ploch      (502) staff       (20)    26022 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-220.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-221.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-32.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-37.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-38.json
+-rw-r--r--   0 ploch      (502) staff       (20)    32311 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)    27756 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-58.json
+-rw-r--r--   0 ploch      (502) staff       (20)    51831 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-59.json
+-rw-r--r--   0 ploch      (502) staff       (20)    22759 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-60.json
+-rw-r--r--   0 ploch      (502) staff       (20)    22802 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-61.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-62.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-65.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-7-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-7.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-75.json
+-rw-r--r--   0 ploch      (502) staff       (20)    87482 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-77.json
+-rw-r--r--   0 ploch      (502) staff       (20)   542053 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8-add-documentation.json
+-rw-r--r--   0 ploch      (502) staff       (20)   479880 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-89.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-90.json
+-rw-r--r--   0 ploch      (502) staff       (20)       68 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-91.json
+-rw-r--r--   0 ploch      (502) staff       (20)    28029 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/device-92.json
+-rw-r--r--   0 ploch      (502) staff       (20)     3282 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/kwargify-rules-test-data.json
+-rw-r--r--   0 ploch      (502) staff       (20)   127793 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/revision-2285-with-uid.json
+-rw-r--r--   0 ploch      (502) staff       (20)  8342101 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-1.json
+-rw-r--r--   0 ploch      (502) staff       (20)   619029 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-2.json
+-rw-r--r--   0 ploch      (502) staff       (20)      147 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.260834 pytos2-ce-2.3.11/tests/securetrack/json/services/
+-rw-r--r--   0 ploch      (502) staff       (20)   178425 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/1.json
+-rw-r--r--   0 ploch      (502) staff       (20)   299824 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/aurora339.json
+-rw-r--r--   0 ploch      (502) staff       (20)     6477 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json
+-rw-r--r--   0 ploch      (502) staff       (20)      569 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.261041 pytos2-ce-2.3.11/tests/securetrack/json/topology/
+-rw-r--r--   0 ploch      (502) staff       (20)       31 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/topology/status.json
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262025 pytos2-ce-2.3.11/tests/securetrack/json/zones/
+-rw-r--r--   0 ploch      (502) staff       (20)      250 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-69.json
+-rw-r--r--   0 ploch      (502) staff       (20)      256 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-78.json
+-rw-r--r--   0 ploch      (502) staff       (20)      693 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-descendants-80.json
+-rw-r--r--   0 ploch      (502) staff       (20)      397 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-entries-78.json
+-rw-r--r--   0 ploch      (502) staff       (20)    10385 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/json/zones/zones.json
+-rw-r--r--   0 ploch      (502) staff       (20)     2937 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/network_object_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     5196 2023-05-04 12:22:36.000000 pytos2-ce-2.3.11/tests/securetrack/revision_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     4932 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/rule_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)    11536 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/service_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     1624 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/securetrack/zone_test.py
+drwxr-xr-x   0 ploch      (502) staff       (20)        0 2023-05-04 12:57:39.262264 pytos2-ce-2.3.11/tests/utils/
+-rw-r--r--   0 ploch      (502) staff       (20)     1863 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/utils/cache_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)     7383 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tests/utils_test.py
+-rw-r--r--   0 ploch      (502) staff       (20)      344 2023-02-11 18:07:04.000000 pytos2-ce-2.3.11/tox.ini
```

### Comparing `pytos2-ce-2.3.10/.gitlab-ci.yml` & `pytos2-ce-2.3.11/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/LICENSE` & `pytos2-ce-2.3.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/PKG-INFO` & `pytos2-ce-2.3.11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: pytos2-ce
-Version: 2.3.10
-Summary: Pytos2 for tos1 tos2 and beyond
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 `pytos2` CE: Official Python Library for the [Tufin Orchestration Suite](https://tufin.com)
 ==============================================
 `pytos2` "Community Edition" (CE) is the official Python library
 for the Tufin Orchestration Suite. It is created, maintained by
 and supported by the Tufin Professional Services Solutions team (PSS). It wraps the
 [Official TOS API](https://forum.tufin.com/support/kc/latest/Content/Suite/4423.htm)
 and provides idiomatic Python-level types and features.
@@ -74,28 +67,28 @@
 scw = Scw(TOS_HOSTNAME, SCW_API_USERNAME, SCW_API_PASSWORD)
 ```
 
 #### Step 1
 The first step of the sample `Workflow` we will be using is
 enpictured here:
 
-![Example Ticket Step #1](doc/securechange-step-1.png)
+![Example Ticket Step #1](docs/assets/securechange-step-1.png)
 
 Since our `Ticket` has ID #2335, let's fetch the `Ticket` by id
 with the following:
 
 ```python
 ticket = scw.get_ticket(2335)
 # ticket = Ticket(subject='Test Ticket #355', id=2335, status=<TicketStatus.INPROGRESS: 'In Progress'>, comments=[], _current_step=Step(id=22979, name='Service Selection', redone=False, skipped=False))
 ```
 
 With that being successful, let's move on to `Step` #2.
 
 #### Step 2
-![Example Ticket Step #2](doc/securechange-step-2.png)
+![Example Ticket Step #2](docs/assets/securechange-step-2.png)
 
 Now that we have the ticket, let's copy the Hyperlink field
 "Website" from `Step` 1 to `Step` 2. (Technically, we'll be moving
 the hyperlink from the first `Task` of `Step` 1 to the first
 `Task` of `Step` 2, but since this example isn't using dynamic
 assignment, we'll assume going forward that "`Step` N" is
 referring to the first `Task` of "`Step` N"). First, let's
@@ -119,15 +112,15 @@
 *N.B.:* We are making the result of the saved `Ticket` our new
 working `Ticket`, as the prior `Ticket`-in-memory would be
 invalidated at this point (since we just saved it; `Ticket`s do not currently update in-place).
 
 If all has gone right, let's go back to SecureChange proper and
 refresh our `Ticket`'s at `Step` 2:
 
-![Example Ticket Step #2, Edit #1](doc/securechange-step-2-edit-1.png)
+![Example Ticket Step #2, Edit #1](docs/assets/securechange-step-2-edit-1.png)
 
 Excellent. Now let's also programatically fill out the "Services" and "Service Expiration" fields, and advance the `Ticket`:
 
 ```python
 services = ticket.last_task.get_field("Services")
 # services = MultipleSelection(name='Services', id=974327, xsi_type=<FieldXsiType.MULTIPLE_SELECTION: 'multiple_selection'>, selected_options=[], options=[Option(id=None, value='HTTP'), Option(id=None, value='FTP'), Option(id=None, value='SSH')])
 services.selected_options.append(services.options[0])
@@ -141,20 +134,20 @@
 ticket = ticket.advance()
 ```
 
 Double-checking with SecureChange, we indeed see that `Step` 2 has
 the corresponding fields updated, and that the `Ticket` has been
 advanced to the final step, `Step` 3:
 
-![Example Ticket Step #2, Edit #2](doc/securechange-step-2-edit-2.png)
+![Example Ticket Step #2, Edit #2](docs/assets/securechange-step-2-edit-2.png)
 
 #### Step 3
 `Step` 3 is the "Approval" step. In it, we'll accept this Service Change Request with an appropriate reason and check the "terms and conditions" checkbox programatically.
 
-![Example Ticket Step #3](doc/securechange-step-3.png)
+![Example Ticket Step #3](docs/assets/securechange-step-3.png)
 
 ```python
 approval = ticket.last_task.get_field("Approve")
 # approval = ApproveReject(name='Approve', id=974334, xsi_type=<FieldXsiType.APPROVE_REJECT: 'approve_reject'>, approved=None)
 approval.approved = True
 approval.reason = 'This service looks reasonable.'
 ```
@@ -187,15 +180,15 @@
 
 ```python
 ticket = ticket.advance()
 ```
 
 As expected, visiting that same `Ticket` in SecureChange will show both the changes we've made, and that the `Ticket` is indeed closed!:
 
-![Example Ticket, Closed](doc/securechange-closed.png)
+![Example Ticket, Closed](docs/assets/securechange-closed.png)
 
 Development
 -----------
 `pytos2` CE is under active development by the Tufin PSS team. Bug
 and feature requests can created by
 [opening a new issue](https://gitlab.com/tufinps/pytos2-ce/-/issues/new).
```

### Comparing `pytos2-ce-2.3.10/README.md` & `pytos2-ce-2.3.11/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: pytos2-ce
+Version: 2.3.11
+Summary: Pytos2 for tos1 tos2 and beyond
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 `pytos2` CE: Official Python Library for the [Tufin Orchestration Suite](https://tufin.com)
 ==============================================
 `pytos2` "Community Edition" (CE) is the official Python library
 for the Tufin Orchestration Suite. It is created, maintained by
 and supported by the Tufin Professional Services Solutions team (PSS). It wraps the
 [Official TOS API](https://forum.tufin.com/support/kc/latest/Content/Suite/4423.htm)
 and provides idiomatic Python-level types and features.
@@ -67,28 +74,28 @@
 scw = Scw(TOS_HOSTNAME, SCW_API_USERNAME, SCW_API_PASSWORD)
 ```
 
 #### Step 1
 The first step of the sample `Workflow` we will be using is
 enpictured here:
 
-![Example Ticket Step #1](doc/securechange-step-1.png)
+![Example Ticket Step #1](docs/assets/securechange-step-1.png)
 
 Since our `Ticket` has ID #2335, let's fetch the `Ticket` by id
 with the following:
 
 ```python
 ticket = scw.get_ticket(2335)
 # ticket = Ticket(subject='Test Ticket #355', id=2335, status=<TicketStatus.INPROGRESS: 'In Progress'>, comments=[], _current_step=Step(id=22979, name='Service Selection', redone=False, skipped=False))
 ```
 
 With that being successful, let's move on to `Step` #2.
 
 #### Step 2
-![Example Ticket Step #2](doc/securechange-step-2.png)
+![Example Ticket Step #2](docs/assets/securechange-step-2.png)
 
 Now that we have the ticket, let's copy the Hyperlink field
 "Website" from `Step` 1 to `Step` 2. (Technically, we'll be moving
 the hyperlink from the first `Task` of `Step` 1 to the first
 `Task` of `Step` 2, but since this example isn't using dynamic
 assignment, we'll assume going forward that "`Step` N" is
 referring to the first `Task` of "`Step` N"). First, let's
@@ -112,15 +119,15 @@
 *N.B.:* We are making the result of the saved `Ticket` our new
 working `Ticket`, as the prior `Ticket`-in-memory would be
 invalidated at this point (since we just saved it; `Ticket`s do not currently update in-place).
 
 If all has gone right, let's go back to SecureChange proper and
 refresh our `Ticket`'s at `Step` 2:
 
-![Example Ticket Step #2, Edit #1](doc/securechange-step-2-edit-1.png)
+![Example Ticket Step #2, Edit #1](docs/assets/securechange-step-2-edit-1.png)
 
 Excellent. Now let's also programatically fill out the "Services" and "Service Expiration" fields, and advance the `Ticket`:
 
 ```python
 services = ticket.last_task.get_field("Services")
 # services = MultipleSelection(name='Services', id=974327, xsi_type=<FieldXsiType.MULTIPLE_SELECTION: 'multiple_selection'>, selected_options=[], options=[Option(id=None, value='HTTP'), Option(id=None, value='FTP'), Option(id=None, value='SSH')])
 services.selected_options.append(services.options[0])
@@ -134,20 +141,20 @@
 ticket = ticket.advance()
 ```
 
 Double-checking with SecureChange, we indeed see that `Step` 2 has
 the corresponding fields updated, and that the `Ticket` has been
 advanced to the final step, `Step` 3:
 
-![Example Ticket Step #2, Edit #2](doc/securechange-step-2-edit-2.png)
+![Example Ticket Step #2, Edit #2](docs/assets/securechange-step-2-edit-2.png)
 
 #### Step 3
 `Step` 3 is the "Approval" step. In it, we'll accept this Service Change Request with an appropriate reason and check the "terms and conditions" checkbox programatically.
 
-![Example Ticket Step #3](doc/securechange-step-3.png)
+![Example Ticket Step #3](docs/assets/securechange-step-3.png)
 
 ```python
 approval = ticket.last_task.get_field("Approve")
 # approval = ApproveReject(name='Approve', id=974334, xsi_type=<FieldXsiType.APPROVE_REJECT: 'approve_reject'>, approved=None)
 approval.approved = True
 approval.reason = 'This service looks reasonable.'
 ```
@@ -180,15 +187,15 @@
 
 ```python
 ticket = ticket.advance()
 ```
 
 As expected, visiting that same `Ticket` in SecureChange will show both the changes we've made, and that the `Ticket` is indeed closed!:
 
-![Example Ticket, Closed](doc/securechange-closed.png)
+![Example Ticket, Closed](docs/assets/securechange-closed.png)
 
 Development
 -----------
 `pytos2` CE is under active development by the Tufin PSS team. Bug
 and feature requests can created by
 [opening a new issue](https://gitlab.com/tufinps/pytos2-ce/-/issues/new).
```

### Comparing `pytos2-ce-2.3.10/doc/securechange-closed.png` & `pytos2-ce-2.3.11/doc/assets/securechange-closed.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/doc/securechange-step-1.png` & `pytos2-ce-2.3.11/doc/assets/securechange-step-1.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/doc/securechange-step-2-edit-1.png` & `pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-1.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/doc/securechange-step-2-edit-2.png` & `pytos2-ce-2.3.11/doc/assets/securechange-step-2-edit-2.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/doc/securechange-step-2.png` & `pytos2-ce-2.3.11/doc/assets/securechange-step-2.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/doc/securechange-step-3.png` & `pytos2-ce-2.3.11/doc/assets/securechange-step-3.png`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/api/__init__.py` & `pytos2-ce-2.3.11/pytos2/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/models/__init__.py` & `pytos2-ce-2.3.11/pytos2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/secureapp/api.py` & `pytos2-ce-2.3.11/pytos2/secureapp/api.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/secureapp/application_identities.py` & `pytos2-ce-2.3.11/pytos2/secureapp/application_identities.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/secureapp/entrypoint.py` & `pytos2-ce-2.3.11/pytos2/secureapp/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/api.py` & `pytos2-ce-2.3.11/pytos2/securechange/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self,
         ticket_id: int,
         step_id: int,
         task_id: int,
         to_step_id: int,
         comment: str = "",
     ) -> Response:
-
         if not comment:
             comment = "Reassigned by script"
 
         body = {"redo_step_comment": {"comment": comment}}
         r = self.session.put(
             f"tickets/{ticket_id}/steps/{step_id}/tasks/{task_id}/redo/{to_step_id}",
             json=body,
@@ -58,15 +57,14 @@
         self,
         ticket_id: int,
         step_id: int,
         task_id: int,
         assignee_id: int,
         comment: str = "",
     ) -> Response:
-
         if not comment:
             comment = "Reassigned by script"
 
         body = {"reassign_task_comment": {"comment": comment}}
         r = self.session.put(
             f"tickets/{ticket_id}/steps/{step_id}/tasks/{task_id}/reassign/{assignee_id}",
             json=body,
```

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/designer.py` & `pytos2-ce-2.3.11/pytos2/securechange/designer.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/designer_verifier_common.py` & `pytos2-ce-2.3.11/pytos2/securechange/designer_verifier_common.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/entrypoint.py` & `pytos2-ce-2.3.11/pytos2/securechange/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         from pytos2.securechange.ticket import (
             TicketSearchResult,
             TicketStatus,
             Ticket,
             Task,
         )
 
-        for (k, param) in params.items():
+        for k, param in params.items():
             if isinstance(param, Enum):
                 params[k] = param.value
 
         r = self.api.session.get("tickets/search", params=params)
         if not r.ok:
             r.raise_for_status()
         else:
@@ -276,7 +276,17 @@
         response = self.api.session.get(f"attachments/{file_id}")
         if not response.ok:
             try:
                 response.raise_for_status()
             except HTTPError as e:
                 raise ValueError(f"Error Getting Attachment: {e}")
         return response.content
+
+    def add_attachment(self, file: str) -> str:
+        attachment = {"attachment": open(file, "rb")}
+        response = self.api.session.post("attachments", files=attachment)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Attachment: {e}")
+        return response.text
```

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/fields/__init__.py` & `pytos2-ce-2.3.11/pytos2/securechange/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/fields/rule_operation.py` & `pytos2-ce-2.3.11/pytos2/securechange/fields/rule_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,14 @@
             self.rule.src_networks,
             obj,
             device_id,
             CellAction.REMOVE,
         )
 
     def add_destination(self, obj: Union[str, NetworkObject], device_id):
-
         if not self.destination_modifications:
             self.destination_modifications = NetworkObjectCellModifications()
 
         return self._add_net_obj_mod(
             self.destination_modifications.network_object_cell_modifications,
             self.rule.dest_networks,
             obj,
```

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/network_object.py` & `pytos2-ce-2.3.11/pytos2/securechange/network_object.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/risk_results.py` & `pytos2-ce-2.3.11/pytos2/securechange/risk_results.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/rule.py` & `pytos2-ce-2.3.11/pytos2/securechange/rule.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/service.py` & `pytos2-ce-2.3.11/pytos2/securechange/service.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/ticket.py` & `pytos2-ce-2.3.11/pytos2/securechange/ticket.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
         self._json_override = val
 
     @property
     def current_step_index(self) -> Optional[int]:
         if not self._current_step:
             return None
 
-        for (idx, s) in enumerate(self.steps):
+        for idx, s in enumerate(self.steps):
             if s.id == self._current_step.id:
                 return idx
 
     @property
     def previous_step(self) -> Optional[Step]:
         current_step_idx = self.current_step_index
         if current_step_idx is None or current_step_idx == 0:
```

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/trigger.py` & `pytos2-ce-2.3.11/pytos2/securechange/trigger.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/user.py` & `pytos2-ce-2.3.11/pytos2/securechange/user.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securechange/verifier.py` & `pytos2-ce-2.3.11/pytos2/securechange/verifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         Binding.XsiType.NON_EXISTING_BINDING.value: NonExistingBinding,
     }
 
     if binding["@xsi.type"] in binding_types:
         cls = binding_types[binding["@xsi.type"]]
         return cls.kwargify(binding)
     else:
-
         return Binding.kwargify(binding)
 
 
 @propify
 class VerifierBinding(Jsonable):
     class ImplicitCleanupRule(Enum):
         VIOLATED = "VIOLATED"
```

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/api.py` & `pytos2-ce-2.3.11/pytos2/securetrack/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
     def post_generic_device(
         self,
         name: str,
         configuration: Union[BytesIO, str],
         update_topology: bool = False,
         customer_id: Optional[int] = None,
     ) -> Response:  # pragma: no cover
-
         if isinstance(configuration, str):
             configuration = BytesIO(configuration.encode())
         LOGGER.info(
             f"POSTing generic device {name}, domain: {customer_id}, update_topology: {update_topology}"
         )
         LOGGER.debug(f"Device config: {configuration.read()}")
         configuration.seek(0)
@@ -277,20 +276,18 @@
 
         if context:
             params["context"] = context
 
         return self.session.get("rule_search", params=params)
 
     def get_interfaces_from_device_id(self, device_id: int) -> Response:
-
         LOGGER.info(f"GETting interfaces for device id: {device_id}")
         return self.session.get(f"devices/{device_id}/interfaces")
 
     def get_bindable_objects_from_device_id(self, device_id: int) -> Response:
-
         LOGGER.info(f"GETting bindable objects for device id: {device_id}")
         return self.session.get(f"devices/{device_id}/bindable_objects")
 
     def get_topology_interfaces_from_device_id(
         self, device_id: int, is_generic: bool = 0
     ) -> Response:
         if is_generic:
```

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/device.py` & `pytos2-ce-2.3.11/pytos2/securetrack/device.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/entrypoint.py` & `pytos2-ce-2.3.11/pytos2/securetrack/entrypoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Dict, Iterable, Iterator, List, Tuple, Optional, Union
 from io import BytesIO
 import typing
 
 from requests.exceptions import HTTPError
 from requests import Response
 
+from pytos2.securetrack.generic_transparent_firewall import GenericTransparentFirewall
+
 from .api import StAPI
 from .device import Device
 from .domain import Domain
 from .network_object import classify_network_object, NetworkObject
 from .policy_browser import Emptiness
 from .revision import Revision
 from .rule import BindingPolicy, Documentation, SecurityRule
@@ -22,15 +24,20 @@
     setup_logger,
 )
 from pytos2.utils.cache import Cache
 from .service_object import classify_service_object, Service
 from .zone import Zone, ZoneReference, ZoneEntry
 from .interface import Interface, BindableObject, TopologyInterface
 from .generic_device import GenericDevice
+from .generic_ignored_interface import GenericIgnoredInterface
+from .generic_interface_customer import GenericInterfaceCustomer
 from .generic_interface import GenericInterface
+from .generic_route import GenericRoute
+from .generic_vpn import GenericVpn
+from .join_cloud import JoinCloud
 from .topology import TopologySyncStatus
 
 LOGGER = setup_logger("st_entrypoint")
 
 
 def _bool(x: bool) -> str:
     return "true" if x else "false"
@@ -389,15 +396,14 @@
     def update_domain(
         self,
         identifier: Union[int, str],
         name: Optional[str] = None,
         description: Optional[str] = None,
         address: Optional[str] = None,
     ) -> Optional[Domain]:
-
         if self._domains_cache.is_empty():
             self._prime_domains_cache()
         modify_domain = self._domains_index.get(identifier)
         res = self.api.put_domain(
             id=modify_domain.id,
             name=name or modify_domain.name,
             description=description or modify_domain.description,
@@ -1315,15 +1321,14 @@
         for policy_obj in policies:
             if policy_obj.name == policy:
                 return policy_obj
 
         raise ValueError("No matching policy found in given device.")
 
     def get_interfaces(self, device_id: int) -> List[Interface]:
-
         device_info = self.default.get_device(device_id)
 
         if device_info and device_info.vendor.name == "CHECKPOINT":
             interfaces = self.api.get_topology_interfaces_from_device_id(device_id)
             base_id = "interface"
         else:
             interfaces = self.api.get_interfaces_from_device_id(device_id)
@@ -1339,28 +1344,26 @@
         else:
             return [
                 Interface.kwargify(d)
                 for d in get_api_node(interfaces.json(), base_id, listify=True)
             ]
 
     def get_bindable_objects(self, device_id: int) -> List[BindableObject]:
-
         objects = self.api.get_bindable_objects_from_device_id(device_id)
         if objects.status_code == 404:
             raise ValueError(f"Device {device_id} not found")
         else:
             return [
                 BindableObject.kwargify(d)
                 for d in get_api_node(objects.json(), "bindable_objects", listify=True)
             ]
 
     def get_topology_interfaces(
         self, device_id: int, is_generic: Optional[int] = 0
     ) -> List[TopologyInterface]:
-
         interfaces = self.api.get_topology_interfaces_from_device_id(
             device_id, is_generic=is_generic
         )
 
         return [
             TopologyInterface.kwargify(d)
             for d in get_api_node(interfaces.json(), "interface", listify=True)
@@ -1595,7 +1598,383 @@
     def delete_generic_interfaces(self, mgmt_id: Union[int, str]) -> None:
         response = self.api.session.delete(f"topology/generic/interface/mgmt/{mgmt_id}")
         if not response.ok:
             try:
                 response.raise_for_status()
             except HTTPError as e:
                 raise ValueError(f"Error Deleting Generic Interfaces: {e}")
+
+    def add_generic_route(self, route: dict) -> None:
+        data = self._generic_body("GenericRoutes", route)
+        response = self.api.session.post("topology/generic/route", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Route: {e}")
+
+    def add_generic_routes(self, routes: List[dict]) -> None:
+        data = self._generic_body("GenericRoutes", routes)
+        response = self.api.session.post("topology/generic/route", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Routes: {e}")
+
+    def get_generic_route(self, int_id: Union[int, str]) -> GenericRoute:
+        response = self.api.session.get(f"topology/generic/route/{int_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Route: {e}")
+
+        route = get_api_node(response.json(), "GenericRoute")
+        return GenericRoute.kwargify(route)
+
+    def get_generic_routes(self, mgmt_id: Union[int, str]) -> List[GenericRoute]:
+        response = self.api.session.get(f"topology/generic/route/mgmt/{mgmt_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Routes: {e}")
+
+        return [
+            GenericRoute.kwargify(d)
+            for d in get_api_node(response.json(), "GenericRoutes", listify=True)
+        ]
+
+    def update_generic_route(self, route: dict) -> None:
+        data = self._generic_body("GenericRoutes", route)
+        response = self.api.session.put("topology/generic/route", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Route: {e}")
+
+    def update_generic_routes(self, routes: List[dict]) -> None:
+        data = self._generic_body("GenericRoutes", routes)
+        response = self.api.session.put("topology/generic/route", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Routes: {e}")
+
+    def delete_generic_route(self, int_id: Union[int, str]) -> None:
+        response = self.api.session.delete(f"topology/generic/route/{int_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Route: {e}")
+
+    def delete_generic_routes(self, mgmt_id: Union[int, str]) -> None:
+        response = self.api.session.delete(f"topology/generic/route/mgmt/{mgmt_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Routes: {e}")
+
+    def add_generic_vpn(self, vpn: dict) -> None:
+        data = self._generic_body("GenericVpns", vpn)
+        response = self.api.session.post("topology/generic/vpn", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Vpn: {e}")
+
+    def add_generic_vpns(self, vpns: List[dict]) -> None:
+        data = self._generic_body("GenericVpns", vpns)
+        response = self.api.session.post("topology/generic/vpn", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Vpns: {e}")
+
+    def get_generic_vpn(self, int_id: Union[int, str]) -> GenericVpn:
+        response = self.api.session.get(f"topology/generic/vpn/{int_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Vpn: {e}")
+
+        vpn = get_api_node(response.json(), "GenericVpn")
+        return GenericVpn.kwargify(vpn)
+
+    def get_generic_vpns(self, device_id: Union[int, str]) -> List[GenericVpn]:
+        response = self.api.session.get(f"topology/generic/vpn/device/{device_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Vpns: {e}")
+
+        return [
+            GenericVpn.kwargify(d)
+            for d in get_api_node(response.json(), "GenericVpns", listify=True)
+        ]
+
+    def update_generic_vpn(self, vpn: dict) -> None:
+        data = self._generic_body("GenericVpns", vpn)
+        response = self.api.session.put("topology/generic/vpn", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Vpn: {e}")
+
+    def update_generic_vpns(self, vpns: List[dict]) -> None:
+        data = self._generic_body("GenericVpns", vpns)
+        response = self.api.session.put("topology/generic/vpn", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Vpns: {e}")
+
+    def delete_generic_vpn(self, int_id: Union[int, str]) -> None:
+        response = self.api.session.delete(f"topology/generic/vpn/{int_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Vpn: {e}")
+
+    def delete_generic_vpns(self, device_id: Union[int, str]) -> None:
+        response = self.api.session.delete(f"topology/generic/vpn/device/{device_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Vpns: {e}")
+
+    def add_generic_transparent_firewalls(self, firewalls: List[dict]) -> None:
+        data = self._generic_body("TransparentFirewalls", firewalls)
+        response = self.api.session.post("topology/generic/transparentfw", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Transparent Firewalls: {e}")
+
+    def get_generic_transparent_firewalls(
+        self, device_id: Union[int, str]
+    ) -> List[GenericTransparentFirewall]:
+        response = self.api.session.get(
+            f"topology/generic/transparentfw/device/{device_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Transparent Firewalls: {e}")
+
+        return [
+            GenericTransparentFirewall.kwargify(d)
+            for d in get_api_node(response.json(), "TransparentFirewalls", listify=True)
+        ]
+
+    def update_generic_transparent_firewalls(self, firewalls: List[dict]) -> None:
+        data = self._generic_body("TransparentFirewalls", firewalls)
+        response = self.api.session.put("topology/generic/transparentfw", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Transparent Firewalls: {e}")
+
+    def delete_generic_transparent_firewall(
+        self, layer_2_data_id: Union[int, str]
+    ) -> None:
+        response = self.api.session.delete(
+            f"topology/generic/transparentfw/{layer_2_data_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Transparent Firewall: {e}")
+
+    def delete_generic_transparent_firewalls(self, device_id: Union[int, str]) -> None:
+        response = self.api.session.delete(
+            f"topology/generic/transparentfw/device/{device_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Transparent Firewalls: {e}")
+
+    def add_generic_ignored_interfaces(self, interfaces: List[dict]) -> None:
+        data = self._generic_body("IgnoredInterfaces", interfaces)
+        response = self.api.session.post("topology/generic/ignoredinterface", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Ignored Interfaces: {e}")
+
+    def get_generic_ignored_interfaces(
+        self, mgmt_id: Union[int, str]
+    ) -> List[GenericIgnoredInterface]:
+        response = self.api.session.get(
+            f"topology/generic/ignoredinterface/mgmt/{mgmt_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Ignored Interfaces: {e}")
+
+        return [
+            GenericIgnoredInterface.kwargify(d)
+            for d in get_api_node(response.json(), "IgnoredInterfaces", listify=True)
+        ]
+
+    def delete_generic_ignored_interfaces(self, mgmt_id: Union[int, str]) -> None:
+        response = self.api.session.delete(
+            f"topology/generic/ignoredinterface/mgmt/{mgmt_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Ignored Interfaces: {e}")
+
+    def add_generic_interface_customer(self, interface_customer: dict) -> None:
+        data = self._generic_body("InterfaceCustomerTag", interface_customer)
+        response = self.api.session.post(
+            "topology/generic/interfacecustomer", json=data
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Interface Customer Tag: {e}")
+
+    def add_generic_interface_customers(self, interface_customers: List[dict]) -> None:
+        data = self._generic_body("InterfaceCustomerTags", interface_customers)
+        response = self.api.session.post(
+            "topology/generic/interfacecustomer", json=data
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Generic Interface Customer Tags: {e}")
+
+    def get_generic_interface_customer(
+        self, int_cust_id: Union[int, str]
+    ) -> GenericInterfaceCustomer:
+        response = self.api.session.get(
+            f"topology/generic/interfacecustomer/{int_cust_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Interface Customer Tag: {e}")
+
+        interface_customer = get_api_node(response.json(), "InterfaceCustomerTag")
+        return GenericInterfaceCustomer.kwargify(interface_customer)
+
+    def get_generic_interface_customers(
+        self, device_id: Union[int, str]
+    ) -> List[GenericInterfaceCustomer]:
+        response = self.api.session.get(
+            f"topology/generic/interfacecustomer/device/{device_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Generic Interface Customer Tags: {e}")
+
+        return [
+            GenericInterfaceCustomer.kwargify(d)
+            for d in get_api_node(
+                response.json(), "InterfaceCustomerTags", listify=True
+            )
+        ]
+
+    def update_generic_interface_customer(self, interface_customer: dict) -> None:
+        data = self._generic_body("InterfaceCustomerTag", interface_customer)
+        response = self.api.session.put("topology/generic/interfacecustomer", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Interface Customer Tag: {e}")
+
+    def update_generic_interface_customers(
+        self, interface_customers: List[dict]
+    ) -> None:
+        data = self._generic_body("InterfaceCustomerTags", interface_customers)
+        response = self.api.session.put("topology/generic/interfacecustomer", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Generic Interface Customer Tag: {e}")
+
+    def delete_generic_interface_customer(self, int_cust_id: Union[int, str]) -> None:
+        response = self.api.session.delete(
+            f"topology/generic/interfacecustomer/{int_cust_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Interface Customer Tag: {e}")
+
+    def delete_generic_interface_customers(self, device_id: Union[int, str]) -> None:
+        response = self.api.session.delete(
+            f"topology/generic/interfacecustomer/device/{device_id}"
+        )
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Generic Interface Customer Tags: {e}")
+
+    def add_join_cloud(self, join_cloud: dict) -> None:
+        data = self._generic_body("JoinCloud", join_cloud)
+        response = self.api.session.post("topology/join/clouds", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Adding Join Cloud: {e}")
+
+    def get_join_cloud(self, cloud_id: Union[int, str]) -> JoinCloud:
+        response = self.api.session.get(f"topology/join/clouds/{cloud_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Getting Join Cloud: {e}")
+        return JoinCloud.kwargify(response.json())
+
+    def update_join_cloud(self, join_cloud: dict) -> None:
+        data = self._generic_body("JoinCloud", join_cloud)
+        response = self.api.session.put("topology/join/clouds", json=data)
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Updating Join Cloud: {e}")
+
+    def delete_join_cloud(self, cloud_id: Union[int, str]) -> None:
+        response = self.api.session.delete(f"topology/join/clouds/{cloud_id}")
+        if not response.ok:
+            try:
+                response.raise_for_status()
+            except HTTPError as e:
+                raise ValueError(f"Error Deleting Join Cloud: {e}")
```

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/generic_interface.py` & `pytos2-ce-2.3.11/pytos2/securetrack/generic_interface.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/interface.py` & `pytos2-ce-2.3.11/pytos2/securetrack/interface.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/network_object.py` & `pytos2-ce-2.3.11/pytos2/securetrack/network_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     NETWORK_OBJECT_VIRTUAL_SERVER = "networkObjectVirtualServerDTO"
     RANGE_NETWORK_OBJECT = "rangeNetworkObjectDTO"
     SUBNET_NETWORK_OBJECT = "subnetNetworkObjectDTO"
 
 
 @propify
 class NatInfo(Jsonable):
-
     xsi_type: Optional[NatXsiType] = prop(
         None, key=Jsonable.Prop.XSI_TYPE.value, repr=False
     )
     interface_name: Optional[str] = prop(None)
 
 
 @propify
```

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/revision.py` & `pytos2-ce-2.3.11/pytos2/securetrack/revision.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/rule.py` & `pytos2-ce-2.3.11/pytos2/securetrack/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         jsonify=lambda d: d.isoformat() if d else None,
     )
 
     ticket_cr: str = prop("", key=Prop.TICKET_CR.value)
     ticket_origin: Optional[TicketOrigin] = prop(None, key=Prop.TICKET_ORIGIN.value)
     ticket_status: str = prop("", key=Prop.TICKET_STATUS.value)
 
-    _exists_on_server: bool = prop(False)
+    _exists_on_server: bool = prop(False, jsonify=False)
 
 
 @propify
 class Violation(Jsonable):
     name: str = prop("")
     type: str = prop("")
```

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/service_object.py` & `pytos2-ce-2.3.11/pytos2/securetrack/service_object.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/securetrack/zone.py` & `pytos2-ce-2.3.11/pytos2/securetrack/zone.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/utils/__init__.py` & `pytos2-ce-2.3.11/pytos2/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2/utils/cache.py` & `pytos2-ce-2.3.11/pytos2/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/pytos2_ce.egg-info/PKG-INFO` & `pytos2-ce-2.3.11/pytos2_ce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytos2-ce
-Version: 2.3.10
+Version: 2.3.11
 Summary: Pytos2 for tos1 tos2 and beyond
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 `pytos2` CE: Official Python Library for the [Tufin Orchestration Suite](https://tufin.com)
 ==============================================
 `pytos2` "Community Edition" (CE) is the official Python library
@@ -74,28 +74,28 @@
 scw = Scw(TOS_HOSTNAME, SCW_API_USERNAME, SCW_API_PASSWORD)
 ```
 
 #### Step 1
 The first step of the sample `Workflow` we will be using is
 enpictured here:
 
-![Example Ticket Step #1](doc/securechange-step-1.png)
+![Example Ticket Step #1](docs/assets/securechange-step-1.png)
 
 Since our `Ticket` has ID #2335, let's fetch the `Ticket` by id
 with the following:
 
 ```python
 ticket = scw.get_ticket(2335)
 # ticket = Ticket(subject='Test Ticket #355', id=2335, status=<TicketStatus.INPROGRESS: 'In Progress'>, comments=[], _current_step=Step(id=22979, name='Service Selection', redone=False, skipped=False))
 ```
 
 With that being successful, let's move on to `Step` #2.
 
 #### Step 2
-![Example Ticket Step #2](doc/securechange-step-2.png)
+![Example Ticket Step #2](docs/assets/securechange-step-2.png)
 
 Now that we have the ticket, let's copy the Hyperlink field
 "Website" from `Step` 1 to `Step` 2. (Technically, we'll be moving
 the hyperlink from the first `Task` of `Step` 1 to the first
 `Task` of `Step` 2, but since this example isn't using dynamic
 assignment, we'll assume going forward that "`Step` N" is
 referring to the first `Task` of "`Step` N"). First, let's
@@ -119,15 +119,15 @@
 *N.B.:* We are making the result of the saved `Ticket` our new
 working `Ticket`, as the prior `Ticket`-in-memory would be
 invalidated at this point (since we just saved it; `Ticket`s do not currently update in-place).
 
 If all has gone right, let's go back to SecureChange proper and
 refresh our `Ticket`'s at `Step` 2:
 
-![Example Ticket Step #2, Edit #1](doc/securechange-step-2-edit-1.png)
+![Example Ticket Step #2, Edit #1](docs/assets/securechange-step-2-edit-1.png)
 
 Excellent. Now let's also programatically fill out the "Services" and "Service Expiration" fields, and advance the `Ticket`:
 
 ```python
 services = ticket.last_task.get_field("Services")
 # services = MultipleSelection(name='Services', id=974327, xsi_type=<FieldXsiType.MULTIPLE_SELECTION: 'multiple_selection'>, selected_options=[], options=[Option(id=None, value='HTTP'), Option(id=None, value='FTP'), Option(id=None, value='SSH')])
 services.selected_options.append(services.options[0])
@@ -141,20 +141,20 @@
 ticket = ticket.advance()
 ```
 
 Double-checking with SecureChange, we indeed see that `Step` 2 has
 the corresponding fields updated, and that the `Ticket` has been
 advanced to the final step, `Step` 3:
 
-![Example Ticket Step #2, Edit #2](doc/securechange-step-2-edit-2.png)
+![Example Ticket Step #2, Edit #2](docs/assets/securechange-step-2-edit-2.png)
 
 #### Step 3
 `Step` 3 is the "Approval" step. In it, we'll accept this Service Change Request with an appropriate reason and check the "terms and conditions" checkbox programatically.
 
-![Example Ticket Step #3](doc/securechange-step-3.png)
+![Example Ticket Step #3](docs/assets/securechange-step-3.png)
 
 ```python
 approval = ticket.last_task.get_field("Approve")
 # approval = ApproveReject(name='Approve', id=974334, xsi_type=<FieldXsiType.APPROVE_REJECT: 'approve_reject'>, approved=None)
 approval.approved = True
 approval.reason = 'This service looks reasonable.'
 ```
@@ -187,15 +187,15 @@
 
 ```python
 ticket = ticket.advance()
 ```
 
 As expected, visiting that same `Ticket` in SecureChange will show both the changes we've made, and that the `Ticket` is indeed closed!:
 
-![Example Ticket, Closed](doc/securechange-closed.png)
+![Example Ticket, Closed](docs/assets/securechange-closed.png)
 
 Development
 -----------
 `pytos2` CE is under active development by the Tufin PSS team. Bug
 and feature requests can created by
 [opening a new issue](https://gitlab.com/tufinps/pytos2-ce/-/issues/new).
```

### Comparing `pytos2-ce-2.3.10/pytos2_ce.egg-info/SOURCES.txt` & `pytos2-ce-2.3.11/pytos2_ce.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 LICENSE
 README.md
 dev-requirements.txt
 mypy.ini
 requirements.txt
 setup.py
 tox.ini
-doc/securechange-closed.png
-doc/securechange-step-1.png
-doc/securechange-step-2-edit-1.png
-doc/securechange-step-2-edit-2.png
-doc/securechange-step-2.png
-doc/securechange-step-3.png
+doc/.env
+doc/Jupyter Notebook Setup.md
+doc/init.py
+doc/pytos2-ce.ipynb
+doc/assets/securechange-closed.png
+doc/assets/securechange-step-1.png
+doc/assets/securechange-step-2-edit-1.png
+doc/assets/securechange-step-2-edit-2.png
+doc/assets/securechange-step-2.png
+doc/assets/securechange-step-3.png
 pytos2/py.typed
 pytos2/api/__init__.py
 pytos2/models/__init__.py
 pytos2/secureapp/__init__.py
 pytos2/secureapp/api.py
 pytos2/secureapp/application_identities.py
 pytos2/secureapp/entrypoint.py
@@ -40,16 +44,22 @@
 pytos2/securechange/fields/rule_operation.py
 pytos2/securetrack/__init__.py
 pytos2/securetrack/api.py
 pytos2/securetrack/device.py
 pytos2/securetrack/domain.py
 pytos2/securetrack/entrypoint.py
 pytos2/securetrack/generic_device.py
+pytos2/securetrack/generic_ignored_interface.py
 pytos2/securetrack/generic_interface.py
+pytos2/securetrack/generic_interface_customer.py
+pytos2/securetrack/generic_route.py
+pytos2/securetrack/generic_transparent_firewall.py
+pytos2/securetrack/generic_vpn.py
 pytos2/securetrack/interface.py
+pytos2/securetrack/join_cloud.py
 pytos2/securetrack/network_object.py
 pytos2/securetrack/policy_browser.py
 pytos2/securetrack/revision.py
 pytos2/securetrack/rule.py
 pytos2/securetrack/service_object.py
 pytos2/securetrack/topology.py
 pytos2/securetrack/zone.py
@@ -75,14 +85,15 @@
 tests/securechange/entrypoint_test.py
 tests/securechange/fields_test.py
 tests/securechange/object_test.py
 tests/securechange/risk_results_test.py
 tests/securechange/ticket_test.py
 tests/securechange/trigger_test.py
 tests/securechange/verifier_test.py
+tests/securechange/files/test.pdf
 tests/securechange/json/all_fields-workflow.json
 tests/securechange/json/application_details.json
 tests/securechange/json/risk_results_ticket.json
 tests/securechange/json/designer/add_icmp_service_object-instruction.json
 tests/securechange/json/designer/add_network_group_object-instruction.json
 tests/securechange/json/designer/add_network_host_object-instruction.json
 tests/securechange/json/designer/add_network_range_object-instruction.json
@@ -143,16 +154,22 @@
 tests/securechange/json/verifier/verifier_result_199.json
 tests/securetrack/__init__.py
 tests/securetrack/api_test.py
 tests/securetrack/conftest.py
 tests/securetrack/device_test.py
 tests/securetrack/domain_test.py
 tests/securetrack/entrypoint_test.py
+tests/securetrack/generic_ignored_interface_test.py
+tests/securetrack/generic_interface_customer_test.py
 tests/securetrack/generic_interface_test.py
+tests/securetrack/generic_route_test.py
+tests/securetrack/generic_transparent_firewall_test.py
+tests/securetrack/generic_vpn_test.py
 tests/securetrack/interface_test.py
+tests/securetrack/join_cloud_test.py
 tests/securetrack/network_object_test.py
 tests/securetrack/revision_test.py
 tests/securetrack/rule_test.py
 tests/securetrack/service_test.py
 tests/securetrack/zone_test.py
 tests/securetrack/json/devices/8.json
 tests/securetrack/json/devices/ASAv.json
@@ -286,26 +303,45 @@
 tests/securetrack/json/devices/devices.json
 tests/securetrack/json/devices/for-rule-test.json
 tests/securetrack/json/domains/domain-7.json
 tests/securetrack/json/domains/domains.json
 tests/securetrack/json/generic_devices/generic_devices.json
 tests/securetrack/json/generic_devices/generic_devices_filtered.json
 tests/securetrack/json/generic_devices/sample_generic_device.csv
+tests/securetrack/json/generic_ignored_interfaces/mgmt-10.json
+tests/securetrack/json/generic_interface_customers/device-5.json
+tests/securetrack/json/generic_interface_customers/int-cust-74.json
 tests/securetrack/json/generic_interfaces/int-1.json
 tests/securetrack/json/generic_interfaces/int-19.json
 tests/securetrack/json/generic_interfaces/int-2.json
 tests/securetrack/json/generic_interfaces/int-20.json
 tests/securetrack/json/generic_interfaces/int-3.json
 tests/securetrack/json/generic_interfaces/int-32.json
 tests/securetrack/json/generic_interfaces/mgmt-1.json
 tests/securetrack/json/generic_interfaces/mgmt-21.json
 tests/securetrack/json/generic_interfaces/mgmt-5.json
+tests/securetrack/json/generic_routes/mgmt-2.json
+tests/securetrack/json/generic_routes/mgmt-3.json
+tests/securetrack/json/generic_routes/route-27.json
+tests/securetrack/json/generic_routes/route-28.json
+tests/securetrack/json/generic_routes/route-29.json
+tests/securetrack/json/generic_routes/route-30.json
+tests/securetrack/json/generic_transparent_firewalls/data-17.json
+tests/securetrack/json/generic_transparent_firewalls/data-23.json
+tests/securetrack/json/generic_transparent_firewalls/device-9.json
+tests/securetrack/json/generic_vpns/device-1.json
+tests/securetrack/json/generic_vpns/device-3.json
+tests/securetrack/json/generic_vpns/vpn-17.json
+tests/securetrack/json/generic_vpns/vpn-22.json
+tests/securetrack/json/generic_vpns/vpn-24.json
+tests/securetrack/json/generic_vpns/vpn-25.json
 tests/securetrack/json/interfaces/device8-interfaces.json
 tests/securetrack/json/interfaces/device8-objects.json
 tests/securetrack/json/interfaces/device8-topology-interfaces.json
+tests/securetrack/json/join_clouds/cloud-67.json
 tests/securetrack/json/network_objects/157.json
 tests/securetrack/json/network_objects/174.json
 tests/securetrack/json/network_objects/181.json
 tests/securetrack/json/network_objects/184.json
 tests/securetrack/json/network_objects/20.json
 tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json
 tests/securetrack/json/network_objects/243.json
```

### Comparing `pytos2-ce-2.3.10/setup.py` & `pytos2-ce-2.3.11/setup.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/api_test.py` & `pytos2-ce-2.3.11/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/secureapp/conftest.py` & `pytos2-ce-2.3.11/tests/secureapp/conftest.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/secureapp/entrypoint_test.py` & `pytos2-ce-2.3.11/tests/secureapp/entrypoint_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/secureapp/json/application_identities.json` & `pytos2-ce-2.3.11/tests/secureapp/json/application_identities.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/api_test.py` & `pytos2-ce-2.3.11/tests/securechange/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/ar_service_test.py` & `pytos2-ce-2.3.11/tests/securechange/ar_service_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/conftest.py` & `pytos2-ce-2.3.11/tests/securechange/conftest.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/designer_test.py` & `pytos2-ce-2.3.11/tests/securechange/designer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     ICMPService,
 )
 
 from pytos2.utils import get_api_node
 
 import responses
 
+
 # need to load proper json file
 @pytest.fixture
 def load_instruction_json_by_type():
     def f(instruction_class):
         return instruction_class.kwargify(
             json.load(
                 open(
```

### Comparing `pytos2-ce-2.3.10/tests/securechange/entrypoint_test.py` & `pytos2-ce-2.3.11/tests/securechange/entrypoint_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import pytest
 import responses
 
 from . import conftest  # noqa
 
 # from pytos2.securechange.entrypoint import Scw
 from pytos2.securechange.ticket import Ticket, TicketStatus, Task, Comment, Attachment
@@ -81,7 +82,20 @@
         assert attachment.uid == "b5672678-d9c5-46ee-87cc-d8fa7fce1a43"
         responses.add(
             responses.GET,
             f"https://198.18.0.1/securechangeworkflow/api/securechange/attachments/{attachment.uid}",
         )
         attachment_content = scw.get_attachment(attachment.uid)
         assert isinstance(attachment_content, bytes)
+
+    @responses.activate
+    def test_add_attachment(self, scw):
+        id = "b5672678-d9c5-46ee-87cc-d8fa7fce1a43"
+        responses.add(
+            responses.POST,
+            f"https://198.18.0.1/securechangeworkflow/api/securechange/attachments",
+            id,
+        )
+
+        uuid = scw.add_attachment("tests/securechange/files/test.pdf")
+        assert isinstance(uuid, str)
+        assert uuid == id
```

### Comparing `pytos2-ce-2.3.10/tests/securechange/fields_test.py` & `pytos2-ce-2.3.11/tests/securechange/fields_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
     @responses.activate
     def test_add_object(self, ar1, network_objects_mock):
         dst = ar1.add_destination(name="192.168.1.82V", device=174)
         assert dst.type.value == "host"
 
     @responses.activate
     def test_add_target(self, st, ar1, mock_devices, devices_mock):
-
         policy_name = "Standard"
 
         def test_target(target: Target, target_name: str, type: Target.ObjectType):
             assert target.type.value == type.value
             assert target.name == target_name
 
         def test_policy(device: Device, target_name: str, type: Target.ObjectType):
@@ -311,15 +310,14 @@
 
     def test_jsonify(self):
         ar = AccessRequest()
         assert "sources" not in ar._json
 
     @responses.activate
     def test_target_count(self, st, ar1, mock_devices, devices_mock):
-
         policy_name = "Standard"
 
         def check_target_count(targets: List[Target]):
             assert len(targets) == len(ar1.targets)
 
         def add_targets(devices):
             targets = []
```

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/all_fields-workflow.json` & `pytos2-ce-2.3.11/tests/securechange/json/all_fields-workflow.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_icmp_service_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_icmp_service_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_group_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_group_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_host_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_host_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_range_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_range_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_network_subnet_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_network_subnet_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_new_rule-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_new_rule_any_service-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_new_rule_any_service-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_service_group-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_service_group-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/add_transport_service_object-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/add_transport_service_object-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/designer_result_251.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_251.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/designer_result_instruction_update_rule.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_result_instruction_update_rule.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/designer_results.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/designer_results_multi_instructions.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/designer_results_multi_instructions.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/designer/update_rule-instruction.json` & `pytos2-ce-2.3.11/tests/securechange/json/designer/update_rule-instruction.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/clone_server_policy_request-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/clone_server_policy_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request_with_all_service_types.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_all_service_types.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_access_request_with_designer_results-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_access_request_with_designer_results-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_group_change-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_group_change-field.json.old` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_group_change-field.json.old`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/multi_server_decommission_request-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/multi_server_decommission_request-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/rule_modification/source_mod.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification/source_mod.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/field/rule_modification_field-field.json` & `pytos2-ce-2.3.11/tests/securechange/json/field/rule_modification_field-field.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/risk_results_ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/risk_results_ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/all_fields-ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/all_fields-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/closed_group_modify-ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/closed_group_modify-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/dynamic_assignment-ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/dynamic_assignment-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/open_with_access_request-ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_access_request-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/open_with_group_modify-ticket.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/open_with_group_modify-ticket.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/redo.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/redo.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/ticket_search_assigned.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_assigned.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/ticket_search_by_step_name.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/ticket_search_by_step_name.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/tickets-0-99.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-0-99.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/ticket/tickets-100-199.json` & `pytos2-ce-2.3.11/tests/securechange/json/ticket/tickets-100-199.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/users/all_users.json` & `pytos2-ce-2.3.11/tests/securechange/json/users/all_users.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/users/user_45.json` & `pytos2-ce-2.3.11/tests/securechange/json/users/user_45.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/users/users_by_username.json` & `pytos2-ce-2.3.11/tests/securechange/json/users/users_by_username.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/json/verifier/verifier_result_199.json` & `pytos2-ce-2.3.11/tests/securechange/json/verifier/verifier_result_199.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/object_test.py` & `pytos2-ce-2.3.11/tests/securechange/object_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/risk_results_test.py` & `pytos2-ce-2.3.11/tests/securechange/risk_results_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/ticket_test.py` & `pytos2-ce-2.3.11/tests/securechange/ticket_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securechange/trigger_test.py` & `pytos2-ce-2.3.11/tests/securechange/trigger_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
         def f(ticket):
             results["ticket"] = ticket
 
         assert isinstance(results.get("ticket"), Ticket)
 
     @responses.activate
     def test_on_test(self, ticket_mock):
-
         ticket_mock.setenv("SCW_EVENT", "TEST")
         results = {}
 
         @on_test
         def f(ticket):
             results["ticket"] = ticket
```

### Comparing `pytos2-ce-2.3.10/tests/securechange/verifier_test.py` & `pytos2-ce-2.3.11/tests/securechange/verifier_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/api_test.py` & `pytos2-ce-2.3.11/tests/securetrack/api_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/device_test.py` & `pytos2-ce-2.3.11/tests/securetrack/device_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/domain_test.py` & `pytos2-ce-2.3.11/tests/securetrack/domain_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/generic_interface_test.py` & `pytos2-ce-2.3.11/tests/securetrack/generic_interface_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import responses
 
 from pytos2.securetrack.generic_interface import GenericInterface
 from pytos2.utils import get_api_node
 
 
 class TestGenericInterface:
-
     mgmt = json.load(open("tests/securetrack/json/generic_interfaces/mgmt-1.json"))
     ipv4Interfaces = mgmt["GenericInterfaces"]
 
     interface1 = json.load(open("tests/securetrack/json/generic_interfaces/int-1.json"))
     int1 = interface1["GenericInterface"]
 
     @responses.activate
```

### Comparing `pytos2-ce-2.3.10/tests/securetrack/interface_test.py` & `pytos2-ce-2.3.11/tests/securetrack/interface_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/devices/devices.json` & `pytos2-ce-2.3.11/tests/securetrack/json/devices/devices.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/devices/for-rule-test.json` & `pytos2-ce-2.3.11/tests/securetrack/json/devices/for-rule-test.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/domains/domains.json` & `pytos2-ce-2.3.11/tests/securetrack/json/domains/domains.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/generic_interfaces/mgmt-1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/generic_interfaces/mgmt-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/interfaces/device8-interfaces.json` & `pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-interfaces.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/interfaces/device8-objects.json` & `pytos2-ce-2.3.11/tests/securetrack/json/interfaces/device8-objects.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/157.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/174.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/181.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/184.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/20.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/20dcde39-b1ac-4013-adbb-81a5a705801d.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/243.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/243.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/5.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/afb2d78d-356a-4a86-805a-c80afee8e338.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b17b4120-07d4-0875-d4b2-06227767ff57.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b4e77d4c-f471-4bb2-bfff-69503bdd6669.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/b63f31eb-d8ab-410c-b526-20a48ff9dbd2.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/network_objects/identity_awareness.json` & `pytos2-ce-2.3.11/tests/securetrack/json/network_objects/identity_awareness.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/1-all.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/1-all.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-10.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-10.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-105.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-105.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-11.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-11.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-114.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-114.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-115.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-115.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-12.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-12.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-120.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-120.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-121.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-121.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-123.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-123.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-144.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-144.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-157.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-159.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-159.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-160.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-160.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-161.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-161.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-166.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-166.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-174.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-179.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-179.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-180.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-180.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-181.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-182.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-182.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-184.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-193.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-193.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-194.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-194.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-195.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-195.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-196.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-196.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-198.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-198.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-20.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-208.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-208.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-21.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-21.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-211.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-211.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-215.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-215.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-216.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-216.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-217.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-217.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-218.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-218.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-32.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-32.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-37.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-37.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-38.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-38.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-5.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-58.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-58.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-59.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-59.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-65.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-65.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-7.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-7.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-75.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-75.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-77.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-77.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-8.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-8.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-89.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-89.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-90.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-90.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-91.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-91.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/device-92.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/device-92.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/revisions/revision-2226.json` & `pytos2-ce-2.3.11/tests/securetrack/json/revisions/revision-2226.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-1-add-documentation.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-105.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-105.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-114.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-114.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-115.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-115.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-120.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-120.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-121.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-121.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-123.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-123.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-144.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-144.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-157.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-157.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-174.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-174.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-179.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-179.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-181.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-181.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-184.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-184.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-193.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-193.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-194.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-194.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-196.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-196.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-198.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-198.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20-add-documentation.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20-with-uid.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20-with-uid.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-20.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-20.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-208.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-208.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-211.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-211.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-215.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-215.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-216.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-216.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-217.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-217.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-218.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-218.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-220.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-220.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-5-add-documentation.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-5.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-5.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-59.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-59.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-60.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-60.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-61.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-61.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-77.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-77.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-8-add-documentation.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8-add-documentation.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-8.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-8.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/device-92.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/device-92.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/kwargify-rules-test-data.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/kwargify-rules-test-data.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/revision-2285-with-uid.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/revision-2285-with-uid.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/rule_search-105-all-1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/rules/rule_search-105-all-2.json` & `pytos2-ce-2.3.11/tests/securetrack/json/rules/rule_search-105-all-2.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/services/1.json` & `pytos2-ce-2.3.11/tests/securetrack/json/services/1.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/services/aurora339.json` & `pytos2-ce-2.3.11/tests/securetrack/json/services/aurora339.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json` & `pytos2-ce-2.3.11/tests/securetrack/json/services/search-3fbd8116-3801-4bee-8593-3cbf999da671.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json` & `pytos2-ce-2.3.11/tests/securetrack/json/services/search-device-1-3fbd8116-3801-4bee-8593-3cbf999da671.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/zones/zone-descendants-80.json` & `pytos2-ce-2.3.11/tests/securetrack/json/zones/zone-descendants-80.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/json/zones/zones.json` & `pytos2-ce-2.3.11/tests/securetrack/json/zones/zones.json`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/network_object_test.py` & `pytos2-ce-2.3.11/tests/securetrack/network_object_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/revision_test.py` & `pytos2-ce-2.3.11/tests/securetrack/revision_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/rule_test.py` & `pytos2-ce-2.3.11/tests/securetrack/rule_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/service_test.py` & `pytos2-ce-2.3.11/tests/securetrack/service_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/securetrack/zone_test.py` & `pytos2-ce-2.3.11/tests/securetrack/zone_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/utils/cache_test.py` & `pytos2-ce-2.3.11/tests/utils/cache_test.py`

 * *Files identical despite different names*

### Comparing `pytos2-ce-2.3.10/tests/utils_test.py` & `pytos2-ce-2.3.11/tests/utils_test.py`

 * *Files identical despite different names*

