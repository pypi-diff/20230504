# Comparing `tmp/pulumi_fastly-7.4.0a1683051704.tar.gz` & `tmp/pulumi_fastly-7.4.0a1683221613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-7.4.0a1683051704.tar", last modified: Tue May  2 18:26:20 2023, max compression
+gzip compressed data, was "pulumi_fastly-7.4.0a1683221613.tar", last modified: Thu May  4 17:37:54 2023, max compression
```

## Comparing `pulumi_fastly-7.4.0a1683051704.tar` & `pulumi_fastly-7.4.0a1683221613.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   504881 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)   449591 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:26:20.732158 pulumi_fastly-7.4.0a1683051704/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-02 18:26:20.000000 pulumi_fastly-7.4.0a1683051704/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:37:54.433145 pulumi_fastly-7.4.0a1683221613/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-04 17:37:54.433145 pulumi_fastly-7.4.0a1683221613/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:37:54.429145 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   505955 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:37:54.433145 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)   450473 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:37:54.433145 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:37:54.433145 pulumi_fastly-7.4.0a1683221613/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 17:37:54.000000 pulumi_fastly-7.4.0a1683221613/setup.py
```

### Comparing `pulumi_fastly-7.4.0a1683051704/PKG-INFO` & `pulumi_fastly-7.4.0a1683221613/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 7.4.0a1683051704
+Version: 7.4.0a1683221613
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.4.0a1683051704/README.md` & `pulumi_fastly-7.4.0a1683221613/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/__init__.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/_inputs.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1814,38 +1814,41 @@
 
 
 @pulumi.input_type
 class ServiceComputeLoggingGcArgs:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
+                 project_id: pulumi.Input[str],
                  account_name: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  period: Optional[pulumi.Input[int]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
@@ -1882,14 +1885,26 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Input[str]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_id", value)
+
+    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[pulumi.Input[str]]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -7209,14 +7224,15 @@
 
 
 @pulumi.input_type
 class ServiceVclLoggingGcArgs:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
+                 project_id: pulumi.Input[str],
                  account_name: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  format: Optional[pulumi.Input[str]] = None,
                  format_version: Optional[pulumi.Input[int]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
@@ -7225,14 +7241,15 @@
                  response_condition: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
@@ -7241,14 +7258,15 @@
         :param pulumi.Input[str] response_condition: Name of a condition to apply this logging.
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
@@ -7293,14 +7311,26 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Input[str]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_id", value)
+
+    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[pulumi.Input[str]]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
```

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/_utilities.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/config/vars.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_services.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/outputs.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1636,14 +1636,16 @@
 @pulumi.output_type
 class ServiceComputeLoggingGc(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
+        elif key == "projectId":
+            suggest = "project_id"
         elif key == "accountName":
             suggest = "account_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
         elif key == "gzipLevel":
             suggest = "gzip_level"
         elif key == "messageType":
@@ -1663,38 +1665,41 @@
     def get(self, key: str, default = None) -> Any:
         ServiceComputeLoggingGc.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
+                 project_id: str,
                  account_name: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
                  period: Optional[int] = None,
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
+        :param str project_id: The ID of your Google Cloud Platform project
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
@@ -1723,14 +1728,22 @@
     def name(self) -> str:
         """
         A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[str]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -6461,14 +6474,16 @@
 @pulumi.output_type
 class ServiceVclLoggingGc(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
+        elif key == "projectId":
+            suggest = "project_id"
         elif key == "accountName":
             suggest = "account_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
         elif key == "formatVersion":
             suggest = "format_version"
         elif key == "gzipLevel":
@@ -6492,14 +6507,15 @@
     def get(self, key: str, default = None) -> Any:
         ServiceVclLoggingGc.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
+                 project_id: str,
                  account_name: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  format: Optional[str] = None,
                  format_version: Optional[int] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
@@ -6508,14 +6524,15 @@
                  response_condition: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
+        :param str project_id: The ID of your Google Cloud Platform project
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param str format: Apache-style string or VCL variables to use for log formatting
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
@@ -6524,14 +6541,15 @@
         :param str response_condition: Name of a condition to apply this logging.
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
@@ -6568,14 +6586,22 @@
     def name(self) -> str:
         """
         A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[str]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
```

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/provider.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_authorization.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_compute.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_vcl.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_activation.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly/user.py` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 7.4.0a1683051704
+Version: 7.4.0a1683221613
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.4.0a1683051704/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-7.4.0a1683221613/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683051704/setup.py` & `pulumi_fastly-7.4.0a1683221613/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "7.4.0a1683051704"
-PLUGIN_VERSION = "7.4.0-alpha.1683051704+6f973c7d"
+VERSION = "7.4.0a1683221613"
+PLUGIN_VERSION = "7.4.0-alpha.1683221613+6af9b073"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

