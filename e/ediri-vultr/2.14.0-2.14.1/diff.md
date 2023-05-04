# Comparing `tmp/ediri_vultr-2.14.0.tar.gz` & `tmp/ediri_vultr-2.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_vultr-2.14.0.tar", last modified: Sun Apr 16 11:30:48 2023, max compression
+gzip compressed data, was "ediri_vultr-2.14.1.tar", last modified: Thu May  4 12:15:31 2023, max compression
```

## Comparing `ediri_vultr-2.14.0.tar` & `ediri_vultr-2.14.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.661267 ediri_vultr-2.14.0/ediri_vultr/
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48976 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/block_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/ediri_vultr/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_block_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_iso_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/kubernetes_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    47909 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/snapshot_from_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.661267 ediri_vultr-2.14.0/ediri_vultr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.027830 ediri_vultr-2.14.1/ediri_vultr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48976 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/block_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/ediri_vultr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_block_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_iso_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/kubernetes_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47909 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/snapshot_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/ediri_vultr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/setup.py
```

### Comparing `ediri_vultr-2.14.0/PKG-INFO` & `ediri_vultr-2.14.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ediri_vultr
-Version: 2.14.0
+Version: 2.14.1
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vultr Resource Provider
 
 ![Vultr](img/logo.png)
 
-The Vultr Resource Provider lets you manage [Vultr](https://vultr.com/) resources.
+The Vultr Resource Provider lets you manage [Vultr](https://www.vultr.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `ediri_vultr-2.14.0/README.md` & `ediri_vultr-2.14.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Vultr Resource Provider
 
 ![Vultr](img/logo.png)
 
-The Vultr Resource Provider lets you manage [Vultr](https://vultr.com/) resources.
+The Vultr Resource Provider lets you manage [Vultr](https://www.vultr.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `ediri_vultr-2.14.0/ediri_vultr/__init__.py` & `ediri_vultr-2.14.1/ediri_vultr/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/_inputs.py` & `ediri_vultr-2.14.1/ediri_vultr/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/_utilities.py` & `ediri_vultr-2.14.1/ediri_vultr/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/bare_metal_server.py` & `ediri_vultr-2.14.1/ediri_vultr/bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/block_storage.py` & `ediri_vultr-2.14.1/ediri_vultr/block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/config/vars.py` & `ediri_vultr-2.14.1/ediri_vultr/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/dns_domain.py` & `ediri_vultr-2.14.1/ediri_vultr/dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/dns_record.py` & `ediri_vultr-2.14.1/ediri_vultr/dns_record.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/firewall_group.py` & `ediri_vultr-2.14.1/ediri_vultr/firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/firewall_rule.py` & `ediri_vultr-2.14.1/ediri_vultr/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_account.py` & `ediri_vultr-2.14.1/ediri_vultr/get_account.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_application.py` & `ediri_vultr-2.14.1/ediri_vultr/get_application.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_backup.py` & `ediri_vultr-2.14.1/ediri_vultr/get_backup.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_plan.py` & `ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_server.py` & `ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_block_storage.py` & `ediri_vultr-2.14.1/ediri_vultr/get_block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_dns_domain.py` & `ediri_vultr-2.14.1/ediri_vultr/get_dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_firewall_group.py` & `ediri_vultr-2.14.1/ediri_vultr/get_firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_instance.py` & `ediri_vultr-2.14.1/ediri_vultr/get_instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_instance_ipv4.py` & `ediri_vultr-2.14.1/ediri_vultr/get_instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_iso_private.py` & `ediri_vultr-2.14.1/ediri_vultr/get_iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_iso_public.py` & `ediri_vultr-2.14.1/ediri_vultr/get_iso_public.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_kubernetes.py` & `ediri_vultr-2.14.1/ediri_vultr/get_kubernetes.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,24 @@
 ]
 
 @pulumi.output_type
 class GetKubernetesResult:
     """
     A collection of values returned by getKubernetes.
     """
-    def __init__(__self__, cluster_subnet=None, date_created=None, endpoint=None, filters=None, id=None, ip=None, kube_config=None, label=None, node_pools=None, region=None, service_subnet=None, status=None, version=None):
+    def __init__(__self__, client_certificate=None, client_key=None, cluster_ca_certificate=None, cluster_subnet=None, date_created=None, endpoint=None, filters=None, id=None, ip=None, kube_config=None, label=None, node_pools=None, region=None, service_subnet=None, status=None, version=None):
+        if client_certificate and not isinstance(client_certificate, str):
+            raise TypeError("Expected argument 'client_certificate' to be a str")
+        pulumi.set(__self__, "client_certificate", client_certificate)
+        if client_key and not isinstance(client_key, str):
+            raise TypeError("Expected argument 'client_key' to be a str")
+        pulumi.set(__self__, "client_key", client_key)
+        if cluster_ca_certificate and not isinstance(cluster_ca_certificate, str):
+            raise TypeError("Expected argument 'cluster_ca_certificate' to be a str")
+        pulumi.set(__self__, "cluster_ca_certificate", cluster_ca_certificate)
         if cluster_subnet and not isinstance(cluster_subnet, str):
             raise TypeError("Expected argument 'cluster_subnet' to be a str")
         pulumi.set(__self__, "cluster_subnet", cluster_subnet)
         if date_created and not isinstance(date_created, str):
             raise TypeError("Expected argument 'date_created' to be a str")
         pulumi.set(__self__, "date_created", date_created)
         if endpoint and not isinstance(endpoint, str):
@@ -61,14 +70,38 @@
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if version and not isinstance(version, str):
             raise TypeError("Expected argument 'version' to be a str")
         pulumi.set(__self__, "version", version)
 
     @property
+    @pulumi.getter(name="clientCertificate")
+    def client_certificate(self) -> str:
+        """
+        The base64 encoded public certificate used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_certificate")
+
+    @property
+    @pulumi.getter(name="clientKey")
+    def client_key(self) -> str:
+        """
+        The base64 encoded private key used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_key")
+
+    @property
+    @pulumi.getter(name="clusterCaCertificate")
+    def cluster_ca_certificate(self) -> str:
+        """
+        The base64 encoded public certificate for the cluster's certificate authority.
+        """
+        return pulumi.get(self, "cluster_ca_certificate")
+
+    @property
     @pulumi.getter(name="clusterSubnet")
     def cluster_subnet(self) -> str:
         """
         IP range that your pods will run on in this cluster.
         """
         return pulumi.get(self, "cluster_subnet")
 
@@ -168,14 +201,17 @@
 
 class AwaitableGetKubernetesResult(GetKubernetesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetKubernetesResult(
+            client_certificate=self.client_certificate,
+            client_key=self.client_key,
+            cluster_ca_certificate=self.cluster_ca_certificate,
             cluster_subnet=self.cluster_subnet,
             date_created=self.date_created,
             endpoint=self.endpoint,
             filters=self.filters,
             id=self.id,
             ip=self.ip,
             kube_config=self.kube_config,
@@ -211,14 +247,17 @@
     """
     __args__ = dict()
     __args__['filters'] = filters
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vultr:index/getKubernetes:getKubernetes', __args__, opts=opts, typ=GetKubernetesResult).value
 
     return AwaitableGetKubernetesResult(
+        client_certificate=__ret__.client_certificate,
+        client_key=__ret__.client_key,
+        cluster_ca_certificate=__ret__.cluster_ca_certificate,
         cluster_subnet=__ret__.cluster_subnet,
         date_created=__ret__.date_created,
         endpoint=__ret__.endpoint,
         filters=__ret__.filters,
         id=__ret__.id,
         ip=__ret__.ip,
         kube_config=__ret__.kube_config,
```

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_load_balancer.py` & `ediri_vultr-2.14.1/ediri_vultr/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_object_storage.py` & `ediri_vultr-2.14.1/ediri_vultr/get_object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_object_storage_cluster.py` & `ediri_vultr-2.14.1/ediri_vultr/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_os.py` & `ediri_vultr-2.14.1/ediri_vultr/get_os.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_plan.py` & `ediri_vultr-2.14.1/ediri_vultr/get_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_private_network.py` & `ediri_vultr-2.14.1/ediri_vultr/get_private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_region.py` & `ediri_vultr-2.14.1/ediri_vultr/get_region.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_reserved_ip.py` & `ediri_vultr-2.14.1/ediri_vultr/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv4.py` & `ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv6.py` & `ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_snapshot.py` & `ediri_vultr-2.14.1/ediri_vultr/get_snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_ssh_key.py` & `ediri_vultr-2.14.1/ediri_vultr/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_startup_script.py` & `ediri_vultr-2.14.1/ediri_vultr/get_startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_user.py` & `ediri_vultr-2.14.1/ediri_vultr/get_user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/get_vpc.py` & `ediri_vultr-2.14.1/ediri_vultr/get_vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/instance.py` & `ediri_vultr-2.14.1/ediri_vultr/instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/instance_ipv4.py` & `ediri_vultr-2.14.1/ediri_vultr/instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/iso_private.py` & `ediri_vultr-2.14.1/ediri_vultr/iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/kubernetes.py` & `ediri_vultr-2.14.1/ediri_vultr/kubernetes.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,39 +81,51 @@
     def node_pools(self, value: Optional[pulumi.Input['KubernetesNodePoolsArgs']]):
         pulumi.set(self, "node_pools", value)
 
 
 @pulumi.input_type
 class _KubernetesState:
     def __init__(__self__, *,
+                 client_certificate: Optional[pulumi.Input[str]] = None,
+                 client_key: Optional[pulumi.Input[str]] = None,
+                 cluster_ca_certificate: Optional[pulumi.Input[str]] = None,
                  cluster_subnet: Optional[pulumi.Input[str]] = None,
                  date_created: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  ip: Optional[pulumi.Input[str]] = None,
                  kube_config: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  node_pools: Optional[pulumi.Input['KubernetesNodePoolsArgs']] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  service_subnet: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Kubernetes resources.
+        :param pulumi.Input[str] client_certificate: The base64 encoded public certificate used by clients to access the cluster.
+        :param pulumi.Input[str] client_key: The base64 encoded private key used by clients to access the cluster.
+        :param pulumi.Input[str] cluster_ca_certificate: The base64 encoded public certificate for the cluster's certificate authority.
         :param pulumi.Input[str] cluster_subnet: IP range that your pods will run on in this cluster.
         :param pulumi.Input[str] date_created: Date node was created.
         :param pulumi.Input[str] endpoint: Domain for your Kubernetes clusters control plane.
         :param pulumi.Input[str] ip: IP address of VKE cluster control plane.
         :param pulumi.Input[str] kube_config: Base64 encoded Kubeconfig for this VKE cluster.
         :param pulumi.Input[str] label: The VKE clusters label.
         :param pulumi.Input['KubernetesNodePoolsArgs'] node_pools: Contains the default node pool that was deployed.
         :param pulumi.Input[str] region: The region your VKE cluster will be deployed in. Currently, supported values are `ewr` and `lax`
         :param pulumi.Input[str] service_subnet: IP range that services will run on this cluster.
         :param pulumi.Input[str] status: Status of node.
         :param pulumi.Input[str] version: The version your VKE cluster you want deployed. [See Available Version](https://www.vultr.com/api/#operation/get-kubernetes-versions)
         """
+        if client_certificate is not None:
+            pulumi.set(__self__, "client_certificate", client_certificate)
+        if client_key is not None:
+            pulumi.set(__self__, "client_key", client_key)
+        if cluster_ca_certificate is not None:
+            pulumi.set(__self__, "cluster_ca_certificate", cluster_ca_certificate)
         if cluster_subnet is not None:
             pulumi.set(__self__, "cluster_subnet", cluster_subnet)
         if date_created is not None:
             pulumi.set(__self__, "date_created", date_created)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if ip is not None:
@@ -130,14 +142,50 @@
             pulumi.set(__self__, "service_subnet", service_subnet)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
+    @pulumi.getter(name="clientCertificate")
+    def client_certificate(self) -> Optional[pulumi.Input[str]]:
+        """
+        The base64 encoded public certificate used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_certificate")
+
+    @client_certificate.setter
+    def client_certificate(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_certificate", value)
+
+    @property
+    @pulumi.getter(name="clientKey")
+    def client_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The base64 encoded private key used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_key")
+
+    @client_key.setter
+    def client_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_key", value)
+
+    @property
+    @pulumi.getter(name="clusterCaCertificate")
+    def cluster_ca_certificate(self) -> Optional[pulumi.Input[str]]:
+        """
+        The base64 encoded public certificate for the cluster's certificate authority.
+        """
+        return pulumi.get(self, "cluster_ca_certificate")
+
+    @cluster_ca_certificate.setter
+    def cluster_ca_certificate(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_ca_certificate", value)
+
+    @property
     @pulumi.getter(name="clusterSubnet")
     def cluster_subnet(self) -> Optional[pulumi.Input[str]]:
         """
         IP range that your pods will run on in this cluster.
         """
         return pulumi.get(self, "cluster_subnet")
 
@@ -417,33 +465,39 @@
             __props__.__dict__["node_pools"] = node_pools
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
             if version is None and not opts.urn:
                 raise TypeError("Missing required property 'version'")
             __props__.__dict__["version"] = version
+            __props__.__dict__["client_certificate"] = None
+            __props__.__dict__["client_key"] = None
+            __props__.__dict__["cluster_ca_certificate"] = None
             __props__.__dict__["cluster_subnet"] = None
             __props__.__dict__["date_created"] = None
             __props__.__dict__["endpoint"] = None
             __props__.__dict__["ip"] = None
             __props__.__dict__["kube_config"] = None
             __props__.__dict__["service_subnet"] = None
             __props__.__dict__["status"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["kubeConfig"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["clientCertificate", "clientKey", "clusterCaCertificate", "kubeConfig"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Kubernetes, __self__).__init__(
             'vultr:index/kubernetes:Kubernetes',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            client_certificate: Optional[pulumi.Input[str]] = None,
+            client_key: Optional[pulumi.Input[str]] = None,
+            cluster_ca_certificate: Optional[pulumi.Input[str]] = None,
             cluster_subnet: Optional[pulumi.Input[str]] = None,
             date_created: Optional[pulumi.Input[str]] = None,
             endpoint: Optional[pulumi.Input[str]] = None,
             ip: Optional[pulumi.Input[str]] = None,
             kube_config: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
             node_pools: Optional[pulumi.Input[pulumi.InputType['KubernetesNodePoolsArgs']]] = None,
@@ -454,14 +508,17 @@
         """
         Get an existing Kubernetes resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] client_certificate: The base64 encoded public certificate used by clients to access the cluster.
+        :param pulumi.Input[str] client_key: The base64 encoded private key used by clients to access the cluster.
+        :param pulumi.Input[str] cluster_ca_certificate: The base64 encoded public certificate for the cluster's certificate authority.
         :param pulumi.Input[str] cluster_subnet: IP range that your pods will run on in this cluster.
         :param pulumi.Input[str] date_created: Date node was created.
         :param pulumi.Input[str] endpoint: Domain for your Kubernetes clusters control plane.
         :param pulumi.Input[str] ip: IP address of VKE cluster control plane.
         :param pulumi.Input[str] kube_config: Base64 encoded Kubeconfig for this VKE cluster.
         :param pulumi.Input[str] label: The VKE clusters label.
         :param pulumi.Input[pulumi.InputType['KubernetesNodePoolsArgs']] node_pools: Contains the default node pool that was deployed.
@@ -470,28 +527,55 @@
         :param pulumi.Input[str] status: Status of node.
         :param pulumi.Input[str] version: The version your VKE cluster you want deployed. [See Available Version](https://www.vultr.com/api/#operation/get-kubernetes-versions)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KubernetesState.__new__(_KubernetesState)
 
+        __props__.__dict__["client_certificate"] = client_certificate
+        __props__.__dict__["client_key"] = client_key
+        __props__.__dict__["cluster_ca_certificate"] = cluster_ca_certificate
         __props__.__dict__["cluster_subnet"] = cluster_subnet
         __props__.__dict__["date_created"] = date_created
         __props__.__dict__["endpoint"] = endpoint
         __props__.__dict__["ip"] = ip
         __props__.__dict__["kube_config"] = kube_config
         __props__.__dict__["label"] = label
         __props__.__dict__["node_pools"] = node_pools
         __props__.__dict__["region"] = region
         __props__.__dict__["service_subnet"] = service_subnet
         __props__.__dict__["status"] = status
         __props__.__dict__["version"] = version
         return Kubernetes(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="clientCertificate")
+    def client_certificate(self) -> pulumi.Output[str]:
+        """
+        The base64 encoded public certificate used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_certificate")
+
+    @property
+    @pulumi.getter(name="clientKey")
+    def client_key(self) -> pulumi.Output[str]:
+        """
+        The base64 encoded private key used by clients to access the cluster.
+        """
+        return pulumi.get(self, "client_key")
+
+    @property
+    @pulumi.getter(name="clusterCaCertificate")
+    def cluster_ca_certificate(self) -> pulumi.Output[str]:
+        """
+        The base64 encoded public certificate for the cluster's certificate authority.
+        """
+        return pulumi.get(self, "cluster_ca_certificate")
+
+    @property
     @pulumi.getter(name="clusterSubnet")
     def cluster_subnet(self) -> pulumi.Output[str]:
         """
         IP range that your pods will run on in this cluster.
         """
         return pulumi.get(self, "cluster_subnet")
```

### Comparing `ediri_vultr-2.14.0/ediri_vultr/kubernetes_node_pools.py` & `ediri_vultr-2.14.1/ediri_vultr/kubernetes_node_pools.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/load_balancer.py` & `ediri_vultr-2.14.1/ediri_vultr/load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/object_storage.py` & `ediri_vultr-2.14.1/ediri_vultr/object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/outputs.py` & `ediri_vultr-2.14.1/ediri_vultr/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/private_network.py` & `ediri_vultr-2.14.1/ediri_vultr/private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/provider.py` & `ediri_vultr-2.14.1/ediri_vultr/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/reserved_ip.py` & `ediri_vultr-2.14.1/ediri_vultr/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/reverse_ipv4.py` & `ediri_vultr-2.14.1/ediri_vultr/reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/reverse_ipv6.py` & `ediri_vultr-2.14.1/ediri_vultr/reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/snapshot.py` & `ediri_vultr-2.14.1/ediri_vultr/snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/snapshot_from_url.py` & `ediri_vultr-2.14.1/ediri_vultr/snapshot_from_url.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/ssh_key.py` & `ediri_vultr-2.14.1/ediri_vultr/ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/startup_script.py` & `ediri_vultr-2.14.1/ediri_vultr/startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/user.py` & `ediri_vultr-2.14.1/ediri_vultr/user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr/vpc.py` & `ediri_vultr-2.14.1/ediri_vultr/vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/ediri_vultr.egg-info/PKG-INFO` & `ediri_vultr-2.14.1/ediri_vultr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ediri-vultr
-Version: 2.14.0
+Version: 2.14.1
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vultr Resource Provider
 
 ![Vultr](img/logo.png)
 
-The Vultr Resource Provider lets you manage [Vultr](https://vultr.com/) resources.
+The Vultr Resource Provider lets you manage [Vultr](https://www.vultr.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `ediri_vultr-2.14.0/ediri_vultr.egg-info/SOURCES.txt` & `ediri_vultr-2.14.1/ediri_vultr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.0/setup.py` & `ediri_vultr-2.14.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.14.0"
-PLUGIN_VERSION = "2.14.0"
+VERSION = "2.14.1"
+PLUGIN_VERSION = "2.14.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vultr', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-vultr'])
         except OSError as error:
```

