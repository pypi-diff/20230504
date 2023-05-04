# Comparing `tmp/duo_client-5.0.0.tar.gz` & `tmp/duo_client-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duo_client-5.0.0.tar", last modified: Mon May  1 19:09:58 2023, max compression
+gzip compressed data, was "duo_client-5.0.1.tar", last modified: Thu May  4 20:41:22 2023, max compression
```

## Comparing `duo_client-5.0.0.tar` & `duo_client-5.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.275415 duo_client-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-01 19:09:41.000000 duo_client-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 19:09:41.000000 duo_client-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-01 19:09:58.275415 duo_client-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-01 19:09:41.000000 duo_client-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:09:41.000000 duo_client-5.0.0/apache-license-2.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.267415 duo_client-5.0.0/duo_client/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)   122004 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/auth_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/ca_certs.pem
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/https_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/duo_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/logs/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/duo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/create_integration_sso_generic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/create_user_and_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/get_billing_and_telephony_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/log_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3856 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/policies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/report_auths_by_country.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/report_users_and_phones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/examples/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/splunk/duo.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     7179 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/splunk/splunk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/trust_monitor_events.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 19:09:41.000000 duo_client-5.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 19:09:41.000000 duo_client-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 19:09:58.275415 duo_client-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 19:09:41.000000 duo_client-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.275415 duo_client-5.0.0/tests/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_administrative_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_authlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_bypass_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_desktop_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_phones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_trust_monitor_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_bypass_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_phones.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32499 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/test_https_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.032003 duo_client-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-04 20:41:08.000000 duo_client-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 20:41:08.000000 duo_client-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-04 20:41:22.032003 duo_client-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-04 20:41:08.000000 duo_client-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 20:41:08.000000 duo_client-5.0.1/apache-license-2.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/duo_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122004 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/auth_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/ca_certs.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/https_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/duo_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/logs/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-04 20:41:08.000000 duo_client-5.0.1/duo_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/duo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-04 20:41:21.000000 duo_client-5.0.1/duo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-04 20:41:22.000000 duo_client-5.0.1/duo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:41:21.000000 duo_client-5.0.1/duo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 20:41:21.000000 duo_client-5.0.1/duo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 20:41:21.000000 duo_client-5.0.1/duo_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/create_integration_sso_generic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/create_user_and_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/get_billing_and_telephony_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/log_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3856 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/policies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/report_auths_by_country.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/report_users_and_phones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/examples/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/splunk/duo.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7179 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/splunk/splunk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-05-04 20:41:08.000000 duo_client-5.0.1/examples/trust_monitor_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 20:41:08.000000 duo_client-5.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 20:41:08.000000 duo_client-5.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 20:41:22.032003 duo_client-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-04 20:41:08.000000 duo_client-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.028003 duo_client-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:22.032003 duo_client-5.0.1/tests/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_administrative_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_authlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_bypass_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_desktop_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_phones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_trust_monitor_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_bypass_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_phones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_user_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/admin/test_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33720 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/test_https_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-04 20:41:08.000000 duo_client-5.0.1/tests/util.py
```

### Comparing `duo_client-5.0.0/LICENSE` & `duo_client-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/PKG-INFO` & `duo_client-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo_client
-Version: 5.0.0
+Version: 5.0.1
 Summary: Reference client for Duo Security APIs
 Home-page: https://github.com/duosecurity/duo_client_python
 Author: Duo Security, Inc.
 Author-email: support@duosecurity.com
 License: BSD
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `duo_client-5.0.0/README.md` & `duo_client-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/apache-license-2.0.txt` & `duo_client-5.0.1/apache-license-2.0.txt`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/accounts.py` & `duo_client-5.0.1/duo_client/accounts.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/admin.py` & `duo_client-5.0.1/duo_client/admin.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/auth.py` & `duo_client-5.0.1/duo_client/auth.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/auth_v1.py` & `duo_client-5.0.1/duo_client/auth_v1.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/ca_certs.pem` & `duo_client-5.0.1/duo_client/ca_certs.pem`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/client.py` & `duo_client-5.0.1/duo_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Low level functions for generating Duo Web API calls and parsing results.
 """
 from __future__ import absolute_import
 from __future__ import print_function
 import six
 
-__version__ = '5.0.0'
+__version__ = '5.0.1'
 
 import base64
 import collections
 import datetime
 import email.utils
 import hashlib
 import hmac
@@ -581,15 +581,15 @@
             ))
         try:
             data = json.loads(data)
             if data['stat'] != 'OK':
                 raise_error('Received error response: %s' % data)
             response = data['response']
             metadata = data.get('metadata', {})
-            if not metadata and not isinstance(response, list):
+            if not metadata and isinstance(response, dict):
                 metadata = response.get('metadata', {})
 
             return (response, metadata)
         except (ValueError, KeyError, TypeError):
             raise_error('Received bad response: %s' % data)
 
     @classmethod
```

### Comparing `duo_client-5.0.0/duo_client/https_wrapper.py` & `duo_client-5.0.1/duo_client/https_wrapper.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/logs/telephony.py` & `duo_client-5.0.1/duo_client/logs/telephony.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client/util.py` & `duo_client-5.0.1/duo_client/util.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/duo_client.egg-info/PKG-INFO` & `duo_client-5.0.1/duo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo-client
-Version: 5.0.0
+Version: 5.0.1
 Summary: Reference client for Duo Security APIs
 Home-page: https://github.com/duosecurity/duo_client_python
 Author: Duo Security, Inc.
 Author-email: support@duosecurity.com
 License: BSD
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `duo_client-5.0.0/duo_client.egg-info/SOURCES.txt` & `duo_client-5.0.1/duo_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/create_integration_sso_generic.py` & `duo_client-5.0.1/examples/create_integration_sso_generic.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/create_user_and_phone.py` & `duo_client-5.0.1/examples/create_user_and_phone.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/get_billing_and_telephony_credits.py` & `duo_client-5.0.1/examples/get_billing_and_telephony_credits.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/log_examples.py` & `duo_client-5.0.1/examples/log_examples.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/policies.py` & `duo_client-5.0.1/examples/policies.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/report_auths_by_country.py` & `duo_client-5.0.1/examples/report_auths_by_country.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/report_users_and_phones.py` & `duo_client-5.0.1/examples/report_users_and_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/splunk/splunk.py` & `duo_client-5.0.1/examples/splunk/splunk.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/examples/trust_monitor_events.py` & `duo_client-5.0.1/examples/trust_monitor_events.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/setup.py` & `duo_client-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/base.py` & `duo_client-5.0.1/tests/admin/base.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_activity.py` & `duo_client-5.0.1/tests/admin/test_activity.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_administrative_units.py` & `duo_client-5.0.1/tests/admin/test_administrative_units.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_admins.py` & `duo_client-5.0.1/tests/admin/test_admins.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_authlog.py` & `duo_client-5.0.1/tests/admin/test_authlog.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_bypass_codes.py` & `duo_client-5.0.1/tests/admin/test_bypass_codes.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_desktop_tokens.py` & `duo_client-5.0.1/tests/admin/test_desktop_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_endpoints.py` & `duo_client-5.0.1/tests/admin/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_groups.py` & `duo_client-5.0.1/tests/admin/test_groups.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_integration.py` & `duo_client-5.0.1/tests/admin/test_integration.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_integrations.py` & `duo_client-5.0.1/tests/admin/test_integrations.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_logo.py` & `duo_client-5.0.1/tests/admin/test_logo.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_phones.py` & `duo_client-5.0.1/tests/admin/test_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_policies.py` & `duo_client-5.0.1/tests/admin/test_policies.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_settings.py` & `duo_client-5.0.1/tests/admin/test_settings.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_telephony.py` & `duo_client-5.0.1/tests/admin/test_telephony.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_tokens.py` & `duo_client-5.0.1/tests/admin/test_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_trust_monitor_events.py` & `duo_client-5.0.1/tests/admin/test_trust_monitor_events.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_u2f.py` & `duo_client-5.0.1/tests/admin/test_u2f.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_bypass_codes.py` & `duo_client-5.0.1/tests/admin/test_user_bypass_codes.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_groups.py` & `duo_client-5.0.1/tests/admin/test_user_groups.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_phones.py` & `duo_client-5.0.1/tests/admin/test_user_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_tokens.py` & `duo_client-5.0.1/tests/admin/test_user_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_u2f.py` & `duo_client-5.0.1/tests/admin/test_user_u2f.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_user_webauthn.py` & `duo_client-5.0.1/tests/admin/test_user_webauthn.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_users.py` & `duo_client-5.0.1/tests/admin/test_users.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/admin/test_webauthn.py` & `duo_client-5.0.1/tests/admin/test_webauthn.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/test_client.py` & `duo_client-5.0.1/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -624,14 +624,46 @@
         with self.assertRaises(RuntimeError) as e:
             self.client.parse_json_response_and_metadata(api_res, response)
 
         self.assertEqual(e.exception.status, api_res.status)
         self.assertEqual(e.exception.reason, api_res.reason)
         self.assertEqual(e.exception.data, response)
 
+    def test_response_is_a_string(self):
+        """
+        Some API requests return just a string in their response.
+        We want to make sure we handle those correctly
+        """
+        api_res = self.APIResponse(200, 'Fake reason')
+        response = {
+            'response': "just a string",
+            'stat': 'OK'
+        }
+        try:
+            self.client.parse_json_response_and_metadata(api_res, json.dumps(response))
+        except Exception:
+            self.fail("parsing raised exception for string response")
+
+    def test_response_is_a_list(self):
+        """
+        Some API requests return just a list in their response. with
+        metadata included at the top level.
+        We want to make sure we handle those correctly
+        """
+        api_res = self.APIResponse(200, "Fake reason")
+        expected_metadata = { "offset": 4 }
+        expected_response = ["multiple", "elements"]
+        response = {
+            "response": expected_response,
+            "metadata": expected_metadata,
+            "stat": "OK"
+        }
+        response, metadata = self.client.parse_json_response_and_metadata(api_res, json.dumps(response))
+        self.assertEqual(metadata, expected_metadata)
+
     def test_response_stat_isnot_OK(self):
         api_res = self.APIResponse(200, 'Fake reason')
 
         res_body = {
                 'response': {
                 'foo': 'bar'
             },
```

### Comparing `duo_client-5.0.0/tests/test_https_wrapper.py` & `duo_client-5.0.1/tests/test_https_wrapper.py`

 * *Files identical despite different names*

### Comparing `duo_client-5.0.0/tests/util.py` & `duo_client-5.0.1/tests/util.py`

 * *Files identical despite different names*

