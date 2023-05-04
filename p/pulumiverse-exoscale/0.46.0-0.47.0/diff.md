# Comparing `tmp/pulumiverse_exoscale-0.46.0.tar.gz` & `tmp/pulumiverse_exoscale-0.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.46.0.tar", last modified: Mon Feb 27 15:58:26 2023, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.47.0.tar", last modified: Thu May  4 11:43:35 2023, max compression
```

## Comparing `pulumiverse_exoscale-0.46.0.tar` & `pulumiverse_exoscale-0.47.0.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67830 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    58855 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    40776 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    50986 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    37868 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    81867 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31716 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    38660 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    39392 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 15:58:25.998010 pulumiverse_exoscale-0.46.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-27 15:58:25.000000 pulumiverse_exoscale-0.46.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48316 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35942 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39936 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.46.0/PKG-INFO` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumiverse_exoscale
-Version: 0.46.0
+Name: pulumiverse-exoscale
+Version: 0.47.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Exoscale Resource Provider
 
 The Exoscale Resource Provider lets you manage [Exoscale](https://www.exoscale.com/) resources.
 
 ## Installing
```

### Comparing `pulumiverse_exoscale-0.46.0/README.md` & `pulumiverse_exoscale-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 from .get_elastic_ip import *
 from .get_instance_pool import *
 from .get_instance_pool_list import *
 from .get_network import *
 from .get_nlb import *
 from .get_private_network import *
 from .get_security_group import *
+from .get_sks_cluster import *
+from .get_sks_cluster_list import *
+from .get_sks_nodepool import *
+from .get_sks_nodepool_list import *
 from .get_template import *
 from .iam_access_key import *
 from .instance_pool import *
 from .ip_address import *
 from .network import *
 from .nic import *
 from .nlb import *
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/instance_pool.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,1627 +4,1126 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = [
-    'ComputeInstanceNetworkInterfaceArgs',
-    'DatabaseKafkaArgs',
-    'DatabaseMysqlArgs',
-    'DatabaseOpensearchArgs',
-    'DatabaseOpensearchDashboardsArgs',
-    'DatabaseOpensearchIndexPatternArgs',
-    'DatabaseOpensearchIndexTemplateArgs',
-    'DatabasePgArgs',
-    'DatabaseRedisArgs',
-    'ElasticIPHealthcheckArgs',
-    'InstancePoolInstanceArgs',
-    'NLBServiceHealthcheckArgs',
-    'SKSClusterOidcArgs',
-    'SecurityGroupRulesEgressArgs',
-    'SecurityGroupRulesIngressArgs',
-    'GetDomainRecordFilterArgs',
-]
+__all__ = ['InstancePoolArgs', 'InstancePool']
 
 @pulumi.input_type
-class ComputeInstanceNetworkInterfaceArgs:
+class InstancePoolArgs:
     def __init__(__self__, *,
-                 network_id: pulumi.Input[str],
-                 ip_address: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] network_id: The PrivateNetwork (ID) to attach to the instance.
-        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the network interface is attached to a *managed* private network.
-        """
-        pulumi.set(__self__, "network_id", network_id)
-        if ip_address is not None:
-            pulumi.set(__self__, "ip_address", ip_address)
-
-    @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Input[str]:
-        """
-        The PrivateNetwork (ID) to attach to the instance.
-        """
-        return pulumi.get(self, "network_id")
-
-    @network_id.setter
-    def network_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network_id", value)
-
-    @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        The IPv4 address to request as static DHCP lease if the network interface is attached to a *managed* private network.
-        """
-        return pulumi.get(self, "ip_address")
-
-    @ip_address.setter
-    def ip_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip_address", value)
-
-
-@pulumi.input_type
-class DatabaseKafkaArgs:
-    def __init__(__self__, *,
-                 enable_cert_auth: Optional[pulumi.Input[bool]] = None,
-                 enable_kafka_connect: Optional[pulumi.Input[bool]] = None,
-                 enable_kafka_rest: Optional[pulumi.Input[bool]] = None,
-                 enable_sasl_auth: Optional[pulumi.Input[bool]] = None,
-                 enable_schema_registry: Optional[pulumi.Input[bool]] = None,
-                 ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 kafka_connect_settings: Optional[pulumi.Input[str]] = None,
-                 kafka_rest_settings: Optional[pulumi.Input[str]] = None,
-                 kafka_settings: Optional[pulumi.Input[str]] = None,
-                 schema_registry_settings: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[bool] enable_cert_auth: Enable certificate-based authentication method.
-        :param pulumi.Input[bool] enable_kafka_connect: Enable Kafka Connect.
-        :param pulumi.Input[bool] enable_kafka_rest: Enable Kafka REST.
-        :param pulumi.Input[bool] enable_sasl_auth: Enable SASL-based authentication method.
-        :param pulumi.Input[bool] enable_schema_registry: Enable Schema Registry.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: A list of CIDR blocks to allow incoming connections from.
-        :param pulumi.Input[str] kafka_connect_settings: Kafka Connect configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka-connect` for reference).
-        :param pulumi.Input[str] kafka_rest_settings: Kafka REST configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka-rest` for reference).
-        :param pulumi.Input[str] kafka_settings: Kafka configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka` for reference).
-        :param pulumi.Input[str] schema_registry_settings: Schema Registry configuration settings in JSON format (`exo dbaas type show kafka --settings=schema-registry` for reference)
-        :param pulumi.Input[str] version: Kafka major version (`exo dbaas type show kafka` for reference; may only be set at creation time).
-        """
-        if enable_cert_auth is not None:
-            pulumi.set(__self__, "enable_cert_auth", enable_cert_auth)
-        if enable_kafka_connect is not None:
-            pulumi.set(__self__, "enable_kafka_connect", enable_kafka_connect)
-        if enable_kafka_rest is not None:
-            pulumi.set(__self__, "enable_kafka_rest", enable_kafka_rest)
-        if enable_sasl_auth is not None:
-            pulumi.set(__self__, "enable_sasl_auth", enable_sasl_auth)
-        if enable_schema_registry is not None:
-            pulumi.set(__self__, "enable_schema_registry", enable_schema_registry)
-        if ip_filters is not None:
-            pulumi.set(__self__, "ip_filters", ip_filters)
-        if kafka_connect_settings is not None:
-            pulumi.set(__self__, "kafka_connect_settings", kafka_connect_settings)
-        if kafka_rest_settings is not None:
-            pulumi.set(__self__, "kafka_rest_settings", kafka_rest_settings)
-        if kafka_settings is not None:
-            pulumi.set(__self__, "kafka_settings", kafka_settings)
-        if schema_registry_settings is not None:
-            pulumi.set(__self__, "schema_registry_settings", schema_registry_settings)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter(name="enableCertAuth")
-    def enable_cert_auth(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable certificate-based authentication method.
-        """
-        return pulumi.get(self, "enable_cert_auth")
-
-    @enable_cert_auth.setter
-    def enable_cert_auth(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_cert_auth", value)
-
-    @property
-    @pulumi.getter(name="enableKafkaConnect")
-    def enable_kafka_connect(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable Kafka Connect.
-        """
-        return pulumi.get(self, "enable_kafka_connect")
-
-    @enable_kafka_connect.setter
-    def enable_kafka_connect(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_kafka_connect", value)
-
-    @property
-    @pulumi.getter(name="enableKafkaRest")
-    def enable_kafka_rest(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable Kafka REST.
-        """
-        return pulumi.get(self, "enable_kafka_rest")
-
-    @enable_kafka_rest.setter
-    def enable_kafka_rest(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_kafka_rest", value)
-
-    @property
-    @pulumi.getter(name="enableSaslAuth")
-    def enable_sasl_auth(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable SASL-based authentication method.
-        """
-        return pulumi.get(self, "enable_sasl_auth")
-
-    @enable_sasl_auth.setter
-    def enable_sasl_auth(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_sasl_auth", value)
-
-    @property
-    @pulumi.getter(name="enableSchemaRegistry")
-    def enable_schema_registry(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable Schema Registry.
-        """
-        return pulumi.get(self, "enable_schema_registry")
-
-    @enable_schema_registry.setter
-    def enable_schema_registry(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_schema_registry", value)
+                 size: pulumi.Input[int],
+                 template_id: pulumi.Input[str],
+                 zone: pulumi.Input[str],
+                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 deploy_target_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
+                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 instance_prefix: Optional[pulumi.Input[str]] = None,
+                 instance_type: Optional[pulumi.Input[str]] = None,
+                 instances: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]] = None,
+                 ipv6: Optional[pulumi.Input[bool]] = None,
+                 key_pair: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_offering: Optional[pulumi.Input[str]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 user_data: Optional[pulumi.Input[str]] = None,
+                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        The set of arguments for constructing a InstancePool resource.
+        :param pulumi.Input[int] size: The number of managed instances.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] description: A free-form text describing the pool.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
+        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
+        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The instance pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+               or gzip it as the provider will take care of it).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        """
+        pulumi.set(__self__, "size", size)
+        pulumi.set(__self__, "template_id", template_id)
+        pulumi.set(__self__, "zone", zone)
+        if affinity_group_ids is not None:
+            pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
+        if deploy_target_id is not None:
+            pulumi.set(__self__, "deploy_target_id", deploy_target_id)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if disk_size is not None:
+            pulumi.set(__self__, "disk_size", disk_size)
+        if elastic_ip_ids is not None:
+            pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
+        if instance_prefix is not None:
+            pulumi.set(__self__, "instance_prefix", instance_prefix)
+        if instance_type is not None:
+            pulumi.set(__self__, "instance_type", instance_type)
+        if instances is not None:
+            pulumi.set(__self__, "instances", instances)
+        if ipv6 is not None:
+            pulumi.set(__self__, "ipv6", ipv6)
+        if key_pair is not None:
+            pulumi.set(__self__, "key_pair", key_pair)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if network_ids is not None:
+            pulumi.set(__self__, "network_ids", network_ids)
+        if security_group_ids is not None:
+            pulumi.set(__self__, "security_group_ids", security_group_ids)
+        if service_offering is not None:
+            warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+            pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+        if service_offering is not None:
+            pulumi.set(__self__, "service_offering", service_offering)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if user_data is not None:
+            pulumi.set(__self__, "user_data", user_data)
+        if virtual_machines is not None:
+            warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+            pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+        if virtual_machines is not None:
+            pulumi.set(__self__, "virtual_machines", virtual_machines)
 
     @property
-    @pulumi.getter(name="ipFilters")
-    def ip_filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def size(self) -> pulumi.Input[int]:
         """
-        A list of CIDR blocks to allow incoming connections from.
+        The number of managed instances.
         """
-        return pulumi.get(self, "ip_filters")
+        return pulumi.get(self, "size")
 
-    @ip_filters.setter
-    def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ip_filters", value)
+    @size.setter
+    def size(self, value: pulumi.Input[int]):
+        pulumi.set(self, "size", value)
 
     @property
-    @pulumi.getter(name="kafkaConnectSettings")
-    def kafka_connect_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="templateId")
+    def template_id(self) -> pulumi.Input[str]:
         """
-        Kafka Connect configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka-connect` for reference).
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
         """
-        return pulumi.get(self, "kafka_connect_settings")
+        return pulumi.get(self, "template_id")
 
-    @kafka_connect_settings.setter
-    def kafka_connect_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kafka_connect_settings", value)
+    @template_id.setter
+    def template_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "template_id", value)
 
     @property
-    @pulumi.getter(name="kafkaRestSettings")
-    def kafka_rest_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def zone(self) -> pulumi.Input[str]:
         """
-        Kafka REST configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka-rest` for reference).
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        return pulumi.get(self, "kafka_rest_settings")
+        return pulumi.get(self, "zone")
 
-    @kafka_rest_settings.setter
-    def kafka_rest_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kafka_rest_settings", value)
+    @zone.setter
+    def zone(self, value: pulumi.Input[str]):
+        pulumi.set(self, "zone", value)
 
     @property
-    @pulumi.getter(name="kafkaSettings")
-    def kafka_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="affinityGroupIds")
+    def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Kafka configuration settings in JSON format (`exo dbaas type show kafka --settings=kafka` for reference).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
         """
-        return pulumi.get(self, "kafka_settings")
+        return pulumi.get(self, "affinity_group_ids")
 
-    @kafka_settings.setter
-    def kafka_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kafka_settings", value)
+    @affinity_group_ids.setter
+    def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "affinity_group_ids", value)
 
     @property
-    @pulumi.getter(name="schemaRegistrySettings")
-    def schema_registry_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="deployTargetId")
+    def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Schema Registry configuration settings in JSON format (`exo dbaas type show kafka --settings=schema-registry` for reference)
+        A deploy target ID.
         """
-        return pulumi.get(self, "schema_registry_settings")
+        return pulumi.get(self, "deploy_target_id")
 
-    @schema_registry_settings.setter
-    def schema_registry_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema_registry_settings", value)
+    @deploy_target_id.setter
+    def deploy_target_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "deploy_target_id", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
-        """
-        Kafka major version (`exo dbaas type show kafka` for reference; may only be set at creation time).
-        """
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
-
-
-@pulumi.input_type
-class DatabaseMysqlArgs:
-    def __init__(__self__, *,
-                 admin_password: Optional[pulumi.Input[str]] = None,
-                 admin_username: Optional[pulumi.Input[str]] = None,
-                 backup_schedule: Optional[pulumi.Input[str]] = None,
-                 ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 mysql_settings: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] admin_password: A custom administrator account password (may only be set at creation time).
-        :param pulumi.Input[str] admin_username: A custom administrator account username (may only be set at creation time).
-        :param pulumi.Input[str] backup_schedule: The automated backup schedule (`HH:MM`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: A list of CIDR blocks to allow incoming connections from.
-        :param pulumi.Input[str] mysql_settings: MySQL configuration settings in JSON format (`exo dbaas type show mysql --settings=mysql` for reference).
-        :param pulumi.Input[str] version: MySQL major version (`exo dbaas type show mysql` for reference; may only be set at creation time).
-        """
-        if admin_password is not None:
-            pulumi.set(__self__, "admin_password", admin_password)
-        if admin_username is not None:
-            pulumi.set(__self__, "admin_username", admin_username)
-        if backup_schedule is not None:
-            pulumi.set(__self__, "backup_schedule", backup_schedule)
-        if ip_filters is not None:
-            pulumi.set(__self__, "ip_filters", ip_filters)
-        if mysql_settings is not None:
-            pulumi.set(__self__, "mysql_settings", mysql_settings)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter(name="adminPassword")
-    def admin_password(self) -> Optional[pulumi.Input[str]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A custom administrator account password (may only be set at creation time).
+        A free-form text describing the pool.
         """
-        return pulumi.get(self, "admin_password")
+        return pulumi.get(self, "description")
 
-    @admin_password.setter
-    def admin_password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "admin_password", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="adminUsername")
-    def admin_username(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> Optional[pulumi.Input[int]]:
         """
-        A custom administrator account username (may only be set at creation time).
+        The managed instances disk size (GiB).
         """
-        return pulumi.get(self, "admin_username")
+        return pulumi.get(self, "disk_size")
 
-    @admin_username.setter
-    def admin_username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "admin_username", value)
+    @disk_size.setter
+    def disk_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "disk_size", value)
 
     @property
-    @pulumi.getter(name="backupSchedule")
-    def backup_schedule(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="elasticIpIds")
+    def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The automated backup schedule (`HH:MM`).
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
         """
-        return pulumi.get(self, "backup_schedule")
+        return pulumi.get(self, "elastic_ip_ids")
 
-    @backup_schedule.setter
-    def backup_schedule(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "backup_schedule", value)
+    @elastic_ip_ids.setter
+    def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "elastic_ip_ids", value)
 
     @property
-    @pulumi.getter(name="ipFilters")
-    def ip_filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="instancePrefix")
+    def instance_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of CIDR blocks to allow incoming connections from.
+        The string used to prefix managed instances name (default: `pool`).
         """
-        return pulumi.get(self, "ip_filters")
+        return pulumi.get(self, "instance_prefix")
 
-    @ip_filters.setter
-    def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ip_filters", value)
+    @instance_prefix.setter
+    def instance_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "instance_prefix", value)
 
     @property
-    @pulumi.getter(name="mysqlSettings")
-    def mysql_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        MySQL configuration settings in JSON format (`exo dbaas type show mysql --settings=mysql` for reference).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
-        return pulumi.get(self, "mysql_settings")
+        return pulumi.get(self, "instance_type")
 
-    @mysql_settings.setter
-    def mysql_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "mysql_settings", value)
+    @instance_type.setter
+    def instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "instance_type", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    def instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]:
         """
-        MySQL major version (`exo dbaas type show mysql` for reference; may only be set at creation time).
+        The list of managed instances. Structure is documented below.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "instances")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
-
-
-@pulumi.input_type
-class DatabaseOpensearchArgs:
-    def __init__(__self__, *,
-                 dashboards: Optional[pulumi.Input['DatabaseOpensearchDashboardsArgs']] = None,
-                 fork_from_service: Optional[pulumi.Input[str]] = None,
-                 index_patterns: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseOpensearchIndexPatternArgs']]]] = None,
-                 index_template: Optional[pulumi.Input['DatabaseOpensearchIndexTemplateArgs']] = None,
-                 ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 keep_index_refresh_interval: Optional[pulumi.Input[bool]] = None,
-                 max_index_count: Optional[pulumi.Input[int]] = None,
-                 recovery_backup_name: Optional[pulumi.Input[str]] = None,
-                 settings: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] fork_from_service: Service name
-        :param pulumi.Input[Sequence[pulumi.Input['DatabaseOpensearchIndexPatternArgs']]] index_patterns: Allows you to create glob style patterns and set a max number of indexes matching this pattern you want to keep. Creating indexes exceeding this value will cause the oldest one to get deleted. You could for example create a pattern looking like 'logs.?' and then create index logs.1, logs.2 etc, it will delete logs.1 once you create logs.6. Do note 'logs.?' does not apply to logs.10. Note: Setting max_index_count to 0 will do nothing and the pattern gets ignored.
-        :param pulumi.Input['DatabaseOpensearchIndexTemplateArgs'] index_template: Template settings for all new indexes
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: Allow incoming connections from this list of CIDR address block, e.g. `["10.20.0.0/16"]`
-        :param pulumi.Input[bool] keep_index_refresh_interval: Aiven automation resets index.refresh_interval to default value for every index to be sure that indices are always visible to search. If it doesn't fit your case, you can disable this by setting up this flag to true.
-        :param pulumi.Input[int] max_index_count: Maximum number of indexes to keep before deleting the oldest one (Minimum value is `0`)
-        :param pulumi.Input[str] version: OpenSearch major version.
-        """
-        if dashboards is not None:
-            pulumi.set(__self__, "dashboards", dashboards)
-        if fork_from_service is not None:
-            pulumi.set(__self__, "fork_from_service", fork_from_service)
-        if index_patterns is not None:
-            pulumi.set(__self__, "index_patterns", index_patterns)
-        if index_template is not None:
-            pulumi.set(__self__, "index_template", index_template)
-        if ip_filters is not None:
-            pulumi.set(__self__, "ip_filters", ip_filters)
-        if keep_index_refresh_interval is not None:
-            pulumi.set(__self__, "keep_index_refresh_interval", keep_index_refresh_interval)
-        if max_index_count is not None:
-            pulumi.set(__self__, "max_index_count", max_index_count)
-        if recovery_backup_name is not None:
-            pulumi.set(__self__, "recovery_backup_name", recovery_backup_name)
-        if settings is not None:
-            pulumi.set(__self__, "settings", settings)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
+    @instances.setter
+    def instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]):
+        pulumi.set(self, "instances", value)
 
     @property
     @pulumi.getter
-    def dashboards(self) -> Optional[pulumi.Input['DatabaseOpensearchDashboardsArgs']]:
-        return pulumi.get(self, "dashboards")
-
-    @dashboards.setter
-    def dashboards(self, value: Optional[pulumi.Input['DatabaseOpensearchDashboardsArgs']]):
-        pulumi.set(self, "dashboards", value)
-
-    @property
-    @pulumi.getter(name="forkFromService")
-    def fork_from_service(self) -> Optional[pulumi.Input[str]]:
-        """
-        Service name
-        """
-        return pulumi.get(self, "fork_from_service")
-
-    @fork_from_service.setter
-    def fork_from_service(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "fork_from_service", value)
-
-    @property
-    @pulumi.getter(name="indexPatterns")
-    def index_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseOpensearchIndexPatternArgs']]]]:
-        """
-        Allows you to create glob style patterns and set a max number of indexes matching this pattern you want to keep. Creating indexes exceeding this value will cause the oldest one to get deleted. You could for example create a pattern looking like 'logs.?' and then create index logs.1, logs.2 etc, it will delete logs.1 once you create logs.6. Do note 'logs.?' does not apply to logs.10. Note: Setting max_index_count to 0 will do nothing and the pattern gets ignored.
-        """
-        return pulumi.get(self, "index_patterns")
-
-    @index_patterns.setter
-    def index_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseOpensearchIndexPatternArgs']]]]):
-        pulumi.set(self, "index_patterns", value)
-
-    @property
-    @pulumi.getter(name="indexTemplate")
-    def index_template(self) -> Optional[pulumi.Input['DatabaseOpensearchIndexTemplateArgs']]:
-        """
-        Template settings for all new indexes
-        """
-        return pulumi.get(self, "index_template")
-
-    @index_template.setter
-    def index_template(self, value: Optional[pulumi.Input['DatabaseOpensearchIndexTemplateArgs']]):
-        pulumi.set(self, "index_template", value)
-
-    @property
-    @pulumi.getter(name="ipFilters")
-    def ip_filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Allow incoming connections from this list of CIDR address block, e.g. `["10.20.0.0/16"]`
-        """
-        return pulumi.get(self, "ip_filters")
-
-    @ip_filters.setter
-    def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ip_filters", value)
-
-    @property
-    @pulumi.getter(name="keepIndexRefreshInterval")
-    def keep_index_refresh_interval(self) -> Optional[pulumi.Input[bool]]:
+    def ipv6(self) -> Optional[pulumi.Input[bool]]:
         """
-        Aiven automation resets index.refresh_interval to default value for every index to be sure that indices are always visible to search. If it doesn't fit your case, you can disable this by setting up this flag to true.
+        Enable IPv6 on managed instances (boolean; default: `false`).
         """
-        return pulumi.get(self, "keep_index_refresh_interval")
+        return pulumi.get(self, "ipv6")
 
-    @keep_index_refresh_interval.setter
-    def keep_index_refresh_interval(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "keep_index_refresh_interval", value)
+    @ipv6.setter
+    def ipv6(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ipv6", value)
 
     @property
-    @pulumi.getter(name="maxIndexCount")
-    def max_index_count(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="keyPair")
+    def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        Maximum number of indexes to keep before deleting the oldest one (Minimum value is `0`)
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
         """
-        return pulumi.get(self, "max_index_count")
+        return pulumi.get(self, "key_pair")
 
-    @max_index_count.setter
-    def max_index_count(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "max_index_count", value)
-
-    @property
-    @pulumi.getter(name="recoveryBackupName")
-    def recovery_backup_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "recovery_backup_name")
-
-    @recovery_backup_name.setter
-    def recovery_backup_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "recovery_backup_name", value)
+    @key_pair.setter
+    def key_pair(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
-    def settings(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "settings")
-
-    @settings.setter
-    def settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "settings", value)
-
-    @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        OpenSearch major version.
+        A map of key/value labels.
         """
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
+        return pulumi.get(self, "labels")
 
-
-@pulumi.input_type
-class DatabaseOpensearchDashboardsArgs:
-    def __init__(__self__, *,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 max_old_space_size: Optional[pulumi.Input[int]] = None,
-                 request_timeout: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[bool] enabled: {Type -  schema.TypeBool, Optional -  true, Default -  true},
-        :param pulumi.Input[int] max_old_space_size: {Type -  schema.TypeInt, Optional -  true, Default -  128},
-        :param pulumi.Input[int] request_timeout: {Type -  schema.TypeInt, Optional -  true, Default -  30000},
-               `settings` -  OpenSearch-specific settings, in json. e.g.`jsonencode({thread_pool_search_size: 64})`. Use `exo x get-dbaas-settings-opensearch` to get a list of available settings.
-        """
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if max_old_space_size is not None:
-            pulumi.set(__self__, "max_old_space_size", max_old_space_size)
-        if request_timeout is not None:
-            pulumi.set(__self__, "request_timeout", request_timeout)
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
-    def enabled(self) -> Optional[pulumi.Input[bool]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        {Type -  schema.TypeBool, Optional -  true, Default -  true},
+        The instance pool name.
         """
-        return pulumi.get(self, "enabled")
+        return pulumi.get(self, "name")
 
-    @enabled.setter
-    def enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enabled", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="maxOldSpaceSize")
-    def max_old_space_size(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="networkIds")
+    def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        {Type -  schema.TypeInt, Optional -  true, Default -  128},
+        A list of [exoscale_private_network](./private_network.md) (IDs).
         """
-        return pulumi.get(self, "max_old_space_size")
+        return pulumi.get(self, "network_ids")
 
-    @max_old_space_size.setter
-    def max_old_space_size(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "max_old_space_size", value)
+    @network_ids.setter
+    def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_ids", value)
 
     @property
-    @pulumi.getter(name="requestTimeout")
-    def request_timeout(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="securityGroupIds")
+    def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        {Type -  schema.TypeInt, Optional -  true, Default -  30000},
-        `settings` -  OpenSearch-specific settings, in json. e.g.`jsonencode({thread_pool_search_size: 64})`. Use `exo x get-dbaas-settings-opensearch` to get a list of available settings.
+        A list of [exoscale_security_group](./security_groups.md) (IDs).
         """
-        return pulumi.get(self, "request_timeout")
-
-    @request_timeout.setter
-    def request_timeout(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "request_timeout", value)
+        return pulumi.get(self, "security_group_ids")
 
-
-@pulumi.input_type
-class DatabaseOpensearchIndexPatternArgs:
-    def __init__(__self__, *,
-                 max_index_count: Optional[pulumi.Input[int]] = None,
-                 pattern: Optional[pulumi.Input[str]] = None,
-                 sorting_algorithm: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[int] max_index_count: Maximum number of indexes to keep (Minimum value is `0`)
-        :param pulumi.Input[str] pattern: fnmatch pattern
-        :param pulumi.Input[str] sorting_algorithm: `alphabetical` or `creation_date`.
-        """
-        if max_index_count is not None:
-            pulumi.set(__self__, "max_index_count", max_index_count)
-        if pattern is not None:
-            pulumi.set(__self__, "pattern", pattern)
-        if sorting_algorithm is not None:
-            pulumi.set(__self__, "sorting_algorithm", sorting_algorithm)
+    @security_group_ids.setter
+    def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "security_group_ids", value)
 
     @property
-    @pulumi.getter(name="maxIndexCount")
-    def max_index_count(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="serviceOffering")
+    def service_offering(self) -> Optional[pulumi.Input[str]]:
         """
-        Maximum number of indexes to keep (Minimum value is `0`)
+        The managed instances type. Please use the `instance_type` argument instead.
         """
-        return pulumi.get(self, "max_index_count")
+        return pulumi.get(self, "service_offering")
 
-    @max_index_count.setter
-    def max_index_count(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "max_index_count", value)
+    @service_offering.setter
+    def service_offering(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_offering", value)
 
     @property
     @pulumi.getter
-    def pattern(self) -> Optional[pulumi.Input[str]]:
-        """
-        fnmatch pattern
-        """
-        return pulumi.get(self, "pattern")
-
-    @pattern.setter
-    def pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pattern", value)
-
-    @property
-    @pulumi.getter(name="sortingAlgorithm")
-    def sorting_algorithm(self) -> Optional[pulumi.Input[str]]:
-        """
-        `alphabetical` or `creation_date`.
-        """
-        return pulumi.get(self, "sorting_algorithm")
+    def state(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "state")
 
-    @sorting_algorithm.setter
-    def sorting_algorithm(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "sorting_algorithm", value)
-
-
-@pulumi.input_type
-class DatabaseOpensearchIndexTemplateArgs:
-    def __init__(__self__, *,
-                 mapping_nested_objects_limit: Optional[pulumi.Input[int]] = None,
-                 number_of_replicas: Optional[pulumi.Input[int]] = None,
-                 number_of_shards: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[int] mapping_nested_objects_limit: The maximum number of nested JSON objects that a single document can contain across all nested types. This limit helps to prevent out of memory errors when a document contains too many nested objects. (Default is 10000. Minimum value is `0`, maximum value is `100000`.)
-        :param pulumi.Input[int] number_of_replicas: The number of replicas each primary shard has. (Minimum value is `0`, maximum value is `29`)
-        :param pulumi.Input[int] number_of_shards: The number of primary shards that an index should have. (Minimum value is `1`, maximum value is `1024`.)
-        """
-        if mapping_nested_objects_limit is not None:
-            pulumi.set(__self__, "mapping_nested_objects_limit", mapping_nested_objects_limit)
-        if number_of_replicas is not None:
-            pulumi.set(__self__, "number_of_replicas", number_of_replicas)
-        if number_of_shards is not None:
-            pulumi.set(__self__, "number_of_shards", number_of_shards)
-
-    @property
-    @pulumi.getter(name="mappingNestedObjectsLimit")
-    def mapping_nested_objects_limit(self) -> Optional[pulumi.Input[int]]:
-        """
-        The maximum number of nested JSON objects that a single document can contain across all nested types. This limit helps to prevent out of memory errors when a document contains too many nested objects. (Default is 10000. Minimum value is `0`, maximum value is `100000`.)
-        """
-        return pulumi.get(self, "mapping_nested_objects_limit")
-
-    @mapping_nested_objects_limit.setter
-    def mapping_nested_objects_limit(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "mapping_nested_objects_limit", value)
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
 
     @property
-    @pulumi.getter(name="numberOfReplicas")
-    def number_of_replicas(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="userData")
+    def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        The number of replicas each primary shard has. (Minimum value is `0`, maximum value is `29`)
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+        or gzip it as the provider will take care of it).
         """
-        return pulumi.get(self, "number_of_replicas")
+        return pulumi.get(self, "user_data")
 
-    @number_of_replicas.setter
-    def number_of_replicas(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "number_of_replicas", value)
+    @user_data.setter
+    def user_data(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_data", value)
 
     @property
-    @pulumi.getter(name="numberOfShards")
-    def number_of_shards(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="virtualMachines")
+    def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The number of primary shards that an index should have. (Minimum value is `1`, maximum value is `1024`.)
+        The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
-        return pulumi.get(self, "number_of_shards")
+        return pulumi.get(self, "virtual_machines")
 
-    @number_of_shards.setter
-    def number_of_shards(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "number_of_shards", value)
+    @virtual_machines.setter
+    def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "virtual_machines", value)
 
 
 @pulumi.input_type
-class DatabasePgArgs:
+class _InstancePoolState:
     def __init__(__self__, *,
-                 admin_password: Optional[pulumi.Input[str]] = None,
-                 admin_username: Optional[pulumi.Input[str]] = None,
-                 backup_schedule: Optional[pulumi.Input[str]] = None,
-                 ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 pg_settings: Optional[pulumi.Input[str]] = None,
-                 pgbouncer_settings: Optional[pulumi.Input[str]] = None,
-                 pglookout_settings: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] admin_password: A custom administrator account password (may only be set at creation time).
-        :param pulumi.Input[str] admin_username: A custom administrator account username (may only be set at creation time).
-        :param pulumi.Input[str] backup_schedule: The automated backup schedule (`HH:MM`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: A list of CIDR blocks to allow incoming connections from.
-        :param pulumi.Input[str] pg_settings: PostgreSQL configuration settings in JSON format (`exo dbaas type show pg --settings=pg` for reference).
-        :param pulumi.Input[str] pgbouncer_settings: PgBouncer configuration settings in JSON format (`exo dbaas type show pg --settings=pgbouncer` for reference).
-        :param pulumi.Input[str] pglookout_settings: pglookout configuration settings in JSON format (`exo dbaas type show pg --settings=pglookout` for reference).
-        :param pulumi.Input[str] version: PostgreSQL major version (`exo dbaas type show pg` for reference; may only be set at creation time).
-        """
-        if admin_password is not None:
-            pulumi.set(__self__, "admin_password", admin_password)
-        if admin_username is not None:
-            pulumi.set(__self__, "admin_username", admin_username)
-        if backup_schedule is not None:
-            pulumi.set(__self__, "backup_schedule", backup_schedule)
-        if ip_filters is not None:
-            pulumi.set(__self__, "ip_filters", ip_filters)
-        if pg_settings is not None:
-            pulumi.set(__self__, "pg_settings", pg_settings)
-        if pgbouncer_settings is not None:
-            pulumi.set(__self__, "pgbouncer_settings", pgbouncer_settings)
-        if pglookout_settings is not None:
-            pulumi.set(__self__, "pglookout_settings", pglookout_settings)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter(name="adminPassword")
-    def admin_password(self) -> Optional[pulumi.Input[str]]:
-        """
-        A custom administrator account password (may only be set at creation time).
-        """
-        return pulumi.get(self, "admin_password")
-
-    @admin_password.setter
-    def admin_password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "admin_password", value)
-
-    @property
-    @pulumi.getter(name="adminUsername")
-    def admin_username(self) -> Optional[pulumi.Input[str]]:
-        """
-        A custom administrator account username (may only be set at creation time).
-        """
-        return pulumi.get(self, "admin_username")
-
-    @admin_username.setter
-    def admin_username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "admin_username", value)
-
-    @property
-    @pulumi.getter(name="backupSchedule")
-    def backup_schedule(self) -> Optional[pulumi.Input[str]]:
-        """
-        The automated backup schedule (`HH:MM`).
-        """
-        return pulumi.get(self, "backup_schedule")
-
-    @backup_schedule.setter
-    def backup_schedule(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "backup_schedule", value)
-
-    @property
-    @pulumi.getter(name="ipFilters")
-    def ip_filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of CIDR blocks to allow incoming connections from.
-        """
-        return pulumi.get(self, "ip_filters")
-
-    @ip_filters.setter
-    def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ip_filters", value)
-
-    @property
-    @pulumi.getter(name="pgSettings")
-    def pg_settings(self) -> Optional[pulumi.Input[str]]:
-        """
-        PostgreSQL configuration settings in JSON format (`exo dbaas type show pg --settings=pg` for reference).
-        """
-        return pulumi.get(self, "pg_settings")
-
-    @pg_settings.setter
-    def pg_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pg_settings", value)
-
-    @property
-    @pulumi.getter(name="pgbouncerSettings")
-    def pgbouncer_settings(self) -> Optional[pulumi.Input[str]]:
-        """
-        PgBouncer configuration settings in JSON format (`exo dbaas type show pg --settings=pgbouncer` for reference).
-        """
-        return pulumi.get(self, "pgbouncer_settings")
-
-    @pgbouncer_settings.setter
-    def pgbouncer_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pgbouncer_settings", value)
-
-    @property
-    @pulumi.getter(name="pglookoutSettings")
-    def pglookout_settings(self) -> Optional[pulumi.Input[str]]:
-        """
-        pglookout configuration settings in JSON format (`exo dbaas type show pg --settings=pglookout` for reference).
-        """
-        return pulumi.get(self, "pglookout_settings")
-
-    @pglookout_settings.setter
-    def pglookout_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pglookout_settings", value)
+                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 deploy_target_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
+                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 instance_prefix: Optional[pulumi.Input[str]] = None,
+                 instance_type: Optional[pulumi.Input[str]] = None,
+                 instances: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]] = None,
+                 ipv6: Optional[pulumi.Input[bool]] = None,
+                 key_pair: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_offering: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 template_id: Optional[pulumi.Input[str]] = None,
+                 user_data: Optional[pulumi.Input[str]] = None,
+                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 zone: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering InstancePool resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] description: A free-form text describing the pool.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
+        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
+        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The instance pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
+        :param pulumi.Input[int] size: The number of managed instances.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+               or gzip it as the provider will take care of it).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        if affinity_group_ids is not None:
+            pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
+        if deploy_target_id is not None:
+            pulumi.set(__self__, "deploy_target_id", deploy_target_id)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if disk_size is not None:
+            pulumi.set(__self__, "disk_size", disk_size)
+        if elastic_ip_ids is not None:
+            pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
+        if instance_prefix is not None:
+            pulumi.set(__self__, "instance_prefix", instance_prefix)
+        if instance_type is not None:
+            pulumi.set(__self__, "instance_type", instance_type)
+        if instances is not None:
+            pulumi.set(__self__, "instances", instances)
+        if ipv6 is not None:
+            pulumi.set(__self__, "ipv6", ipv6)
+        if key_pair is not None:
+            pulumi.set(__self__, "key_pair", key_pair)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if network_ids is not None:
+            pulumi.set(__self__, "network_ids", network_ids)
+        if security_group_ids is not None:
+            pulumi.set(__self__, "security_group_ids", security_group_ids)
+        if service_offering is not None:
+            warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+            pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+        if service_offering is not None:
+            pulumi.set(__self__, "service_offering", service_offering)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if template_id is not None:
+            pulumi.set(__self__, "template_id", template_id)
+        if user_data is not None:
+            pulumi.set(__self__, "user_data", user_data)
+        if virtual_machines is not None:
+            warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+            pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+        if virtual_machines is not None:
+            pulumi.set(__self__, "virtual_machines", virtual_machines)
+        if zone is not None:
+            pulumi.set(__self__, "zone", zone)
+
+    @property
+    @pulumi.getter(name="affinityGroupIds")
+    def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        """
+        return pulumi.get(self, "affinity_group_ids")
+
+    @affinity_group_ids.setter
+    def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "affinity_group_ids", value)
+
+    @property
+    @pulumi.getter(name="deployTargetId")
+    def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        A deploy target ID.
+        """
+        return pulumi.get(self, "deploy_target_id")
+
+    @deploy_target_id.setter
+    def deploy_target_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "deploy_target_id", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        PostgreSQL major version (`exo dbaas type show pg` for reference; may only be set at creation time).
+        A free-form text describing the pool.
         """
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
-
+        return pulumi.get(self, "description")
 
-@pulumi.input_type
-class DatabaseRedisArgs:
-    def __init__(__self__, *,
-                 ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 redis_settings: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: A list of CIDR blocks to allow incoming connections from.
-        :param pulumi.Input[str] redis_settings: Redis configuration settings in JSON format (`exo dbaas type show redis --settings=redis` for reference).
-        """
-        if ip_filters is not None:
-            pulumi.set(__self__, "ip_filters", ip_filters)
-        if redis_settings is not None:
-            pulumi.set(__self__, "redis_settings", redis_settings)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="ipFilters")
-    def ip_filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> Optional[pulumi.Input[int]]:
         """
-        A list of CIDR blocks to allow incoming connections from.
+        The managed instances disk size (GiB).
         """
-        return pulumi.get(self, "ip_filters")
+        return pulumi.get(self, "disk_size")
 
-    @ip_filters.setter
-    def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ip_filters", value)
+    @disk_size.setter
+    def disk_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "disk_size", value)
 
     @property
-    @pulumi.getter(name="redisSettings")
-    def redis_settings(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="elasticIpIds")
+    def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Redis configuration settings in JSON format (`exo dbaas type show redis --settings=redis` for reference).
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
         """
-        return pulumi.get(self, "redis_settings")
-
-    @redis_settings.setter
-    def redis_settings(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "redis_settings", value)
+        return pulumi.get(self, "elastic_ip_ids")
 
-
-@pulumi.input_type
-class ElasticIPHealthcheckArgs:
-    def __init__(__self__, *,
-                 mode: pulumi.Input[str],
-                 port: pulumi.Input[int],
-                 interval: Optional[pulumi.Input[int]] = None,
-                 strikes_fail: Optional[pulumi.Input[int]] = None,
-                 strikes_ok: Optional[pulumi.Input[int]] = None,
-                 timeout: Optional[pulumi.Input[int]] = None,
-                 tls_skip_verify: Optional[pulumi.Input[bool]] = None,
-                 tls_sni: Optional[pulumi.Input[str]] = None,
-                 uri: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] mode: The healthcheck mode (`tcp`, `http` or `https`; may only be set at creation time).
-        :param pulumi.Input[int] port: The healthcheck target port (must be between `1` and `65535`).
-        :param pulumi.Input[int] interval: The healthcheck interval (seconds; must be between `5` and `300`; default: `10`).
-        :param pulumi.Input[int] strikes_fail: The number of failed healthcheck attempts before considering the target unhealthy (must be between `1` and `20`; default: `2`).
-        :param pulumi.Input[int] strikes_ok: The number of successful healthcheck attempts before considering the target healthy (must be between `1` and `20`; default: `3`).
-        :param pulumi.Input[int] timeout: The time before considering a healthcheck probing failed (seconds; must be between `2` and `60`; default: `3`).
-        :param pulumi.Input[bool] tls_skip_verify: Disable TLS certificate verification for healthcheck in `https` mode (boolean; default: `false`).
-        :param pulumi.Input[str] tls_sni: The healthcheck server name to present with SNI in `https` mode.
-        :param pulumi.Input[str] uri: The healthcheck target URI (required in `http(s)` modes).
-        """
-        pulumi.set(__self__, "mode", mode)
-        pulumi.set(__self__, "port", port)
-        if interval is not None:
-            pulumi.set(__self__, "interval", interval)
-        if strikes_fail is not None:
-            pulumi.set(__self__, "strikes_fail", strikes_fail)
-        if strikes_ok is not None:
-            pulumi.set(__self__, "strikes_ok", strikes_ok)
-        if timeout is not None:
-            pulumi.set(__self__, "timeout", timeout)
-        if tls_skip_verify is not None:
-            pulumi.set(__self__, "tls_skip_verify", tls_skip_verify)
-        if tls_sni is not None:
-            pulumi.set(__self__, "tls_sni", tls_sni)
-        if uri is not None:
-            pulumi.set(__self__, "uri", uri)
+    @elastic_ip_ids.setter
+    def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "elastic_ip_ids", value)
 
     @property
-    @pulumi.getter
-    def mode(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="instancePrefix")
+    def instance_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck mode (`tcp`, `http` or `https`; may only be set at creation time).
+        The string used to prefix managed instances name (default: `pool`).
         """
-        return pulumi.get(self, "mode")
+        return pulumi.get(self, "instance_prefix")
 
-    @mode.setter
-    def mode(self, value: pulumi.Input[str]):
-        pulumi.set(self, "mode", value)
+    @instance_prefix.setter
+    def instance_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "instance_prefix", value)
 
     @property
-    @pulumi.getter
-    def port(self) -> pulumi.Input[int]:
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck target port (must be between `1` and `65535`).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "instance_type")
 
-    @port.setter
-    def port(self, value: pulumi.Input[int]):
-        pulumi.set(self, "port", value)
+    @instance_type.setter
+    def instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "instance_type", value)
 
     @property
     @pulumi.getter
-    def interval(self) -> Optional[pulumi.Input[int]]:
+    def instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]:
         """
-        The healthcheck interval (seconds; must be between `5` and `300`; default: `10`).
+        The list of managed instances. Structure is documented below.
         """
-        return pulumi.get(self, "interval")
+        return pulumi.get(self, "instances")
 
-    @interval.setter
-    def interval(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "interval", value)
-
-    @property
-    @pulumi.getter(name="strikesFail")
-    def strikes_fail(self) -> Optional[pulumi.Input[int]]:
-        """
-        The number of failed healthcheck attempts before considering the target unhealthy (must be between `1` and `20`; default: `2`).
-        """
-        return pulumi.get(self, "strikes_fail")
-
-    @strikes_fail.setter
-    def strikes_fail(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "strikes_fail", value)
-
-    @property
-    @pulumi.getter(name="strikesOk")
-    def strikes_ok(self) -> Optional[pulumi.Input[int]]:
-        """
-        The number of successful healthcheck attempts before considering the target healthy (must be between `1` and `20`; default: `3`).
-        """
-        return pulumi.get(self, "strikes_ok")
-
-    @strikes_ok.setter
-    def strikes_ok(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "strikes_ok", value)
+    @instances.setter
+    def instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]):
+        pulumi.set(self, "instances", value)
 
     @property
     @pulumi.getter
-    def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        The time before considering a healthcheck probing failed (seconds; must be between `2` and `60`; default: `3`).
-        """
-        return pulumi.get(self, "timeout")
-
-    @timeout.setter
-    def timeout(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "timeout", value)
-
-    @property
-    @pulumi.getter(name="tlsSkipVerify")
-    def tls_skip_verify(self) -> Optional[pulumi.Input[bool]]:
+    def ipv6(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disable TLS certificate verification for healthcheck in `https` mode (boolean; default: `false`).
+        Enable IPv6 on managed instances (boolean; default: `false`).
         """
-        return pulumi.get(self, "tls_skip_verify")
+        return pulumi.get(self, "ipv6")
 
-    @tls_skip_verify.setter
-    def tls_skip_verify(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "tls_skip_verify", value)
+    @ipv6.setter
+    def ipv6(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ipv6", value)
 
     @property
-    @pulumi.getter(name="tlsSni")
-    def tls_sni(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="keyPair")
+    def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck server name to present with SNI in `https` mode.
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
         """
-        return pulumi.get(self, "tls_sni")
+        return pulumi.get(self, "key_pair")
 
-    @tls_sni.setter
-    def tls_sni(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tls_sni", value)
+    @key_pair.setter
+    def key_pair(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
-    def uri(self) -> Optional[pulumi.Input[str]]:
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        The healthcheck target URI (required in `http(s)` modes).
+        A map of key/value labels.
         """
-        return pulumi.get(self, "uri")
+        return pulumi.get(self, "labels")
 
-    @uri.setter
-    def uri(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "uri", value)
-
-
-@pulumi.input_type
-class InstancePoolInstanceArgs:
-    def __init__(__self__, *,
-                 id: Optional[pulumi.Input[str]] = None,
-                 ipv6_address: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 public_ip_address: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] id: The compute instance ID.
-        :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address.
-        :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
-        """
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if ipv6_address is not None:
-            pulumi.set(__self__, "ipv6_address", ipv6_address)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if public_ip_address is not None:
-            pulumi.set(__self__, "public_ip_address", public_ip_address)
-
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The compute instance ID.
-        """
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "id", value)
-
-    @property
-    @pulumi.getter(name="ipv6Address")
-    def ipv6_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        The instance (main network interface) IPv6 address.
-        """
-        return pulumi.get(self, "ipv6_address")
-
-    @ipv6_address.setter
-    def ipv6_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ipv6_address", value)
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The instance pool name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="publicIpAddress")
-    def public_ip_address(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="networkIds")
+    def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The instance (main network interface) IPv4 address.
+        A list of [exoscale_private_network](./private_network.md) (IDs).
         """
-        return pulumi.get(self, "public_ip_address")
-
-    @public_ip_address.setter
-    def public_ip_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "public_ip_address", value)
+        return pulumi.get(self, "network_ids")
 
+    @network_ids.setter
+    def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "network_ids", value)
 
-@pulumi.input_type
-class NLBServiceHealthcheckArgs:
-    def __init__(__self__, *,
-                 port: pulumi.Input[int],
-                 interval: Optional[pulumi.Input[int]] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 retries: Optional[pulumi.Input[int]] = None,
-                 timeout: Optional[pulumi.Input[int]] = None,
-                 tls_sni: Optional[pulumi.Input[str]] = None,
-                 uri: Optional[pulumi.Input[str]] = None):
+    @property
+    @pulumi.getter(name="securityGroupIds")
+    def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        :param pulumi.Input[int] port: The healthcheck port.
-        :param pulumi.Input[int] interval: The healthcheck interval in seconds (default: `10`).
-        :param pulumi.Input[str] mode: The healthcheck mode (`tcp`|`http`|`https`; default: `tcp`).
-        :param pulumi.Input[int] retries: The healthcheck retries (default: `1`).
-        :param pulumi.Input[int] timeout: The healthcheck timeout (seconds; default: `5`).
-        :param pulumi.Input[str] tls_sni: The healthcheck TLS SNI server name (only if `mode` is `https`).
-        :param pulumi.Input[str] uri: The healthcheck URI (must be set only if `mode` is `http(s)`).
+        A list of [exoscale_security_group](./security_groups.md) (IDs).
         """
-        pulumi.set(__self__, "port", port)
-        if interval is not None:
-            pulumi.set(__self__, "interval", interval)
-        if mode is not None:
-            pulumi.set(__self__, "mode", mode)
-        if retries is not None:
-            pulumi.set(__self__, "retries", retries)
-        if timeout is not None:
-            pulumi.set(__self__, "timeout", timeout)
-        if tls_sni is not None:
-            pulumi.set(__self__, "tls_sni", tls_sni)
-        if uri is not None:
-            pulumi.set(__self__, "uri", uri)
+        return pulumi.get(self, "security_group_ids")
+
+    @security_group_ids.setter
+    def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "security_group_ids", value)
 
     @property
-    @pulumi.getter
-    def port(self) -> pulumi.Input[int]:
+    @pulumi.getter(name="serviceOffering")
+    def service_offering(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck port.
+        The managed instances type. Please use the `instance_type` argument instead.
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "service_offering")
 
-    @port.setter
-    def port(self, value: pulumi.Input[int]):
-        pulumi.set(self, "port", value)
+    @service_offering.setter
+    def service_offering(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_offering", value)
 
     @property
     @pulumi.getter
-    def interval(self) -> Optional[pulumi.Input[int]]:
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        The healthcheck interval in seconds (default: `10`).
+        The number of managed instances.
         """
-        return pulumi.get(self, "interval")
+        return pulumi.get(self, "size")
 
-    @interval.setter
-    def interval(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "interval", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
-    def mode(self) -> Optional[pulumi.Input[str]]:
-        """
-        The healthcheck mode (`tcp`|`http`|`https`; default: `tcp`).
-        """
-        return pulumi.get(self, "mode")
+    def state(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "state")
 
-    @mode.setter
-    def mode(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "mode", value)
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
 
     @property
-    @pulumi.getter
-    def retries(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="templateId")
+    def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck retries (default: `1`).
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
         """
-        return pulumi.get(self, "retries")
+        return pulumi.get(self, "template_id")
 
-    @retries.setter
-    def retries(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "retries", value)
+    @template_id.setter
+    def template_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "template_id", value)
 
     @property
-    @pulumi.getter
-    def timeout(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="userData")
+    def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck timeout (seconds; default: `5`).
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+        or gzip it as the provider will take care of it).
         """
-        return pulumi.get(self, "timeout")
+        return pulumi.get(self, "user_data")
 
-    @timeout.setter
-    def timeout(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "timeout", value)
+    @user_data.setter
+    def user_data(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_data", value)
 
     @property
-    @pulumi.getter(name="tlsSni")
-    def tls_sni(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="virtualMachines")
+    def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The healthcheck TLS SNI server name (only if `mode` is `https`).
+        The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
-        return pulumi.get(self, "tls_sni")
+        return pulumi.get(self, "virtual_machines")
 
-    @tls_sni.setter
-    def tls_sni(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tls_sni", value)
+    @virtual_machines.setter
+    def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "virtual_machines", value)
 
     @property
     @pulumi.getter
-    def uri(self) -> Optional[pulumi.Input[str]]:
+    def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck URI (must be set only if `mode` is `http(s)`).
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        return pulumi.get(self, "uri")
+        return pulumi.get(self, "zone")
 
-    @uri.setter
-    def uri(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "uri", value)
+    @zone.setter
+    def zone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "zone", value)
 
 
-@pulumi.input_type
-class SKSClusterOidcArgs:
-    def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
-                 issuer_url: pulumi.Input[str],
-                 groups_claim: Optional[pulumi.Input[str]] = None,
-                 groups_prefix: Optional[pulumi.Input[str]] = None,
-                 required_claim: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 username_claim: Optional[pulumi.Input[str]] = None,
-                 username_prefix: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] client_id: The OpenID client ID.
-        :param pulumi.Input[str] issuer_url: The OpenID provider URL.
-        :param pulumi.Input[str] groups_claim: An OpenID JWT claim to use as the user's group.
-        :param pulumi.Input[str] groups_prefix: An OpenID prefix prepended to group claims.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] required_claim: A map of key/value pairs that describes a required claim in the OpenID Token.
-        :param pulumi.Input[str] username_claim: An OpenID JWT claim to use as the user name.
-        :param pulumi.Input[str] username_prefix: An OpenID prefix prepended to username claims.
+class InstancePool(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 deploy_target_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
+                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 instance_prefix: Optional[pulumi.Input[str]] = None,
+                 instance_type: Optional[pulumi.Input[str]] = None,
+                 instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
+                 ipv6: Optional[pulumi.Input[bool]] = None,
+                 key_pair: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_offering: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 template_id: Optional[pulumi.Input[str]] = None,
+                 user_data: Optional[pulumi.Input[str]] = None,
+                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        ## Import
+
+        An existing instance pool may be imported by `<ID>@<zone>`
+
+        ```sh
+         $ pulumi import exoscale:index/instancePool:InstancePool \\
+        ```
+
+         exoscale_instance_pool.my_instance_pool \\
+
+         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] description: A free-form text describing the pool.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
+        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
+        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The instance pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
+        :param pulumi.Input[int] size: The number of managed instances.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+               or gzip it as the provider will take care of it).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: InstancePoolArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        ## Import
+
+        An existing instance pool may be imported by `<ID>@<zone>`
+
+        ```sh
+         $ pulumi import exoscale:index/instancePool:InstancePool \\
+        ```
+
+         exoscale_instance_pool.my_instance_pool \\
+
+         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+
+        :param str resource_name: The name of the resource.
+        :param InstancePoolArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(InstancePoolArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 deploy_target_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
+                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 instance_prefix: Optional[pulumi.Input[str]] = None,
+                 instance_type: Optional[pulumi.Input[str]] = None,
+                 instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
+                 ipv6: Optional[pulumi.Input[bool]] = None,
+                 key_pair: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 service_offering: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 template_id: Optional[pulumi.Input[str]] = None,
+                 user_data: Optional[pulumi.Input[str]] = None,
+                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = InstancePoolArgs.__new__(InstancePoolArgs)
+
+            __props__.__dict__["affinity_group_ids"] = affinity_group_ids
+            __props__.__dict__["deploy_target_id"] = deploy_target_id
+            __props__.__dict__["description"] = description
+            __props__.__dict__["disk_size"] = disk_size
+            __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
+            __props__.__dict__["instance_prefix"] = instance_prefix
+            __props__.__dict__["instance_type"] = instance_type
+            __props__.__dict__["instances"] = instances
+            __props__.__dict__["ipv6"] = ipv6
+            __props__.__dict__["key_pair"] = key_pair
+            __props__.__dict__["labels"] = labels
+            __props__.__dict__["name"] = name
+            __props__.__dict__["network_ids"] = network_ids
+            __props__.__dict__["security_group_ids"] = security_group_ids
+            if service_offering is not None and not opts.urn:
+                warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+                pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+            __props__.__dict__["service_offering"] = service_offering
+            if size is None and not opts.urn:
+                raise TypeError("Missing required property 'size'")
+            __props__.__dict__["size"] = size
+            __props__.__dict__["state"] = state
+            if template_id is None and not opts.urn:
+                raise TypeError("Missing required property 'template_id'")
+            __props__.__dict__["template_id"] = template_id
+            __props__.__dict__["user_data"] = user_data
+            if virtual_machines is not None and not opts.urn:
+                warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+                pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+            __props__.__dict__["virtual_machines"] = virtual_machines
+            if zone is None and not opts.urn:
+                raise TypeError("Missing required property 'zone'")
+            __props__.__dict__["zone"] = zone
+        super(InstancePool, __self__).__init__(
+            'exoscale:index/instancePool:InstancePool',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            deploy_target_id: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            disk_size: Optional[pulumi.Input[int]] = None,
+            elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            instance_prefix: Optional[pulumi.Input[str]] = None,
+            instance_type: Optional[pulumi.Input[str]] = None,
+            instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
+            ipv6: Optional[pulumi.Input[bool]] = None,
+            key_pair: Optional[pulumi.Input[str]] = None,
+            labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            service_offering: Optional[pulumi.Input[str]] = None,
+            size: Optional[pulumi.Input[int]] = None,
+            state: Optional[pulumi.Input[str]] = None,
+            template_id: Optional[pulumi.Input[str]] = None,
+            user_data: Optional[pulumi.Input[str]] = None,
+            virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            zone: Optional[pulumi.Input[str]] = None) -> 'InstancePool':
+        """
+        Get an existing InstancePool resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] description: A free-form text describing the pool.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
+        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
+        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The instance pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
+        :param pulumi.Input[int] size: The number of managed instances.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+               or gzip it as the provider will take care of it).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        pulumi.set(__self__, "client_id", client_id)
-        pulumi.set(__self__, "issuer_url", issuer_url)
-        if groups_claim is not None:
-            pulumi.set(__self__, "groups_claim", groups_claim)
-        if groups_prefix is not None:
-            pulumi.set(__self__, "groups_prefix", groups_prefix)
-        if required_claim is not None:
-            pulumi.set(__self__, "required_claim", required_claim)
-        if username_claim is not None:
-            pulumi.set(__self__, "username_claim", username_claim)
-        if username_prefix is not None:
-            pulumi.set(__self__, "username_prefix", username_prefix)
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-    @property
-    @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
-        """
-        The OpenID client ID.
-        """
-        return pulumi.get(self, "client_id")
+        __props__ = _InstancePoolState.__new__(_InstancePoolState)
 
-    @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "client_id", value)
+        __props__.__dict__["affinity_group_ids"] = affinity_group_ids
+        __props__.__dict__["deploy_target_id"] = deploy_target_id
+        __props__.__dict__["description"] = description
+        __props__.__dict__["disk_size"] = disk_size
+        __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
+        __props__.__dict__["instance_prefix"] = instance_prefix
+        __props__.__dict__["instance_type"] = instance_type
+        __props__.__dict__["instances"] = instances
+        __props__.__dict__["ipv6"] = ipv6
+        __props__.__dict__["key_pair"] = key_pair
+        __props__.__dict__["labels"] = labels
+        __props__.__dict__["name"] = name
+        __props__.__dict__["network_ids"] = network_ids
+        __props__.__dict__["security_group_ids"] = security_group_ids
+        __props__.__dict__["service_offering"] = service_offering
+        __props__.__dict__["size"] = size
+        __props__.__dict__["state"] = state
+        __props__.__dict__["template_id"] = template_id
+        __props__.__dict__["user_data"] = user_data
+        __props__.__dict__["virtual_machines"] = virtual_machines
+        __props__.__dict__["zone"] = zone
+        return InstancePool(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="issuerUrl")
-    def issuer_url(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="affinityGroupIds")
+    def affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The OpenID provider URL.
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
         """
-        return pulumi.get(self, "issuer_url")
-
-    @issuer_url.setter
-    def issuer_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "issuer_url", value)
+        return pulumi.get(self, "affinity_group_ids")
 
     @property
-    @pulumi.getter(name="groupsClaim")
-    def groups_claim(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="deployTargetId")
+    def deploy_target_id(self) -> pulumi.Output[Optional[str]]:
         """
-        An OpenID JWT claim to use as the user's group.
+        A deploy target ID.
         """
-        return pulumi.get(self, "groups_claim")
-
-    @groups_claim.setter
-    def groups_claim(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "groups_claim", value)
+        return pulumi.get(self, "deploy_target_id")
 
     @property
-    @pulumi.getter(name="groupsPrefix")
-    def groups_prefix(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        An OpenID prefix prepended to group claims.
+        A free-form text describing the pool.
         """
-        return pulumi.get(self, "groups_prefix")
-
-    @groups_prefix.setter
-    def groups_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "groups_prefix", value)
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="requiredClaim")
-    def required_claim(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> pulumi.Output[int]:
         """
-        A map of key/value pairs that describes a required claim in the OpenID Token.
+        The managed instances disk size (GiB).
         """
-        return pulumi.get(self, "required_claim")
-
-    @required_claim.setter
-    def required_claim(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "required_claim", value)
+        return pulumi.get(self, "disk_size")
 
     @property
-    @pulumi.getter(name="usernameClaim")
-    def username_claim(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="elasticIpIds")
+    def elastic_ip_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        An OpenID JWT claim to use as the user name.
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
         """
-        return pulumi.get(self, "username_claim")
-
-    @username_claim.setter
-    def username_claim(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username_claim", value)
+        return pulumi.get(self, "elastic_ip_ids")
 
     @property
-    @pulumi.getter(name="usernamePrefix")
-    def username_prefix(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="instancePrefix")
+    def instance_prefix(self) -> pulumi.Output[Optional[str]]:
         """
-        An OpenID prefix prepended to username claims.
+        The string used to prefix managed instances name (default: `pool`).
         """
-        return pulumi.get(self, "username_prefix")
-
-    @username_prefix.setter
-    def username_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username_prefix", value)
+        return pulumi.get(self, "instance_prefix")
 
-
-@pulumi.input_type
-class SecurityGroupRulesEgressArgs:
-    def __init__(__self__, *,
-                 cidr_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 icmp_code: Optional[pulumi.Input[int]] = None,
-                 icmp_type: Optional[pulumi.Input[int]] = None,
-                 ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 ports: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 protocol: Optional[pulumi.Input[str]] = None,
-                 user_security_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] cidr_lists: A list of (`INGRESS`) source / (`EGRESS`) destination IP subnet (in CIDR notation) to match.
-        :param pulumi.Input[str] description: A free-form text describing the block.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 type/code to match.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ports: A list of ports or port ranges (`<start_port>-<end_port>`).
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] user_security_group_lists: A list of source (for ingress)/destination (for egress) identified by a security group.
+    @property
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> pulumi.Output[str]:
         """
-        if cidr_lists is not None:
-            pulumi.set(__self__, "cidr_lists", cidr_lists)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if icmp_code is not None:
-            pulumi.set(__self__, "icmp_code", icmp_code)
-        if icmp_type is not None:
-            pulumi.set(__self__, "icmp_type", icmp_type)
-        if ids is not None:
-            pulumi.set(__self__, "ids", ids)
-        if ports is not None:
-            pulumi.set(__self__, "ports", ports)
-        if protocol is not None:
-            pulumi.set(__self__, "protocol", protocol)
-        if user_security_group_lists is not None:
-            pulumi.set(__self__, "user_security_group_lists", user_security_group_lists)
-
-    @property
-    @pulumi.getter(name="cidrLists")
-    def cidr_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of (`INGRESS`) source / (`EGRESS`) destination IP subnet (in CIDR notation) to match.
-        """
-        return pulumi.get(self, "cidr_lists")
-
-    @cidr_lists.setter
-    def cidr_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "cidr_lists", value)
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        """
+        return pulumi.get(self, "instance_type")
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def instances(self) -> pulumi.Output[Sequence['outputs.InstancePoolInstance']]:
         """
-        A free-form text describing the block.
+        The list of managed instances. Structure is documented below.
         """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="icmpCode")
-    def icmp_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "icmp_code")
-
-    @icmp_code.setter
-    def icmp_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "icmp_code", value)
+        return pulumi.get(self, "instances")
 
     @property
-    @pulumi.getter(name="icmpType")
-    def icmp_type(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def ipv6(self) -> pulumi.Output[Optional[bool]]:
         """
-        /`icmp_code` - An ICMP/ICMPv6 type/code to match.
+        Enable IPv6 on managed instances (boolean; default: `false`).
         """
-        return pulumi.get(self, "icmp_type")
-
-    @icmp_type.setter
-    def icmp_type(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "icmp_type", value)
+        return pulumi.get(self, "ipv6")
 
     @property
-    @pulumi.getter
-    def ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "ids")
-
-    @ids.setter
-    def ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ids", value)
+    @pulumi.getter(name="keyPair")
+    def key_pair(self) -> pulumi.Output[Optional[str]]:
+        """
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        """
+        return pulumi.get(self, "key_pair")
 
     @property
     @pulumi.getter
-    def ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        A list of ports or port ranges (`<start_port>-<end_port>`).
+        A map of key/value labels.
         """
-        return pulumi.get(self, "ports")
-
-    @ports.setter
-    def ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ports", value)
+        return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
-    def protocol(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Output[str]:
         """
-        The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`).
+        The instance pool name.
         """
-        return pulumi.get(self, "protocol")
-
-    @protocol.setter
-    def protocol(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "protocol", value)
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="userSecurityGroupLists")
-    def user_security_group_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="networkIds")
+    def network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of source (for ingress)/destination (for egress) identified by a security group.
-        """
-        return pulumi.get(self, "user_security_group_lists")
-
-    @user_security_group_lists.setter
-    def user_security_group_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "user_security_group_lists", value)
-
-
-@pulumi.input_type
-class SecurityGroupRulesIngressArgs:
-    def __init__(__self__, *,
-                 cidr_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 icmp_code: Optional[pulumi.Input[int]] = None,
-                 icmp_type: Optional[pulumi.Input[int]] = None,
-                 ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 ports: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 protocol: Optional[pulumi.Input[str]] = None,
-                 user_security_group_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] cidr_lists: A list of (`INGRESS`) source / (`EGRESS`) destination IP subnet (in CIDR notation) to match.
-        :param pulumi.Input[str] description: A free-form text describing the block.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 type/code to match.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ports: A list of ports or port ranges (`<start_port>-<end_port>`).
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] user_security_group_lists: A list of source (for ingress)/destination (for egress) identified by a security group.
+        A list of [exoscale_private_network](./private_network.md) (IDs).
         """
-        if cidr_lists is not None:
-            pulumi.set(__self__, "cidr_lists", cidr_lists)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if icmp_code is not None:
-            pulumi.set(__self__, "icmp_code", icmp_code)
-        if icmp_type is not None:
-            pulumi.set(__self__, "icmp_type", icmp_type)
-        if ids is not None:
-            pulumi.set(__self__, "ids", ids)
-        if ports is not None:
-            pulumi.set(__self__, "ports", ports)
-        if protocol is not None:
-            pulumi.set(__self__, "protocol", protocol)
-        if user_security_group_lists is not None:
-            pulumi.set(__self__, "user_security_group_lists", user_security_group_lists)
-
-    @property
-    @pulumi.getter(name="cidrLists")
-    def cidr_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of (`INGRESS`) source / (`EGRESS`) destination IP subnet (in CIDR notation) to match.
-        """
-        return pulumi.get(self, "cidr_lists")
-
-    @cidr_lists.setter
-    def cidr_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "cidr_lists", value)
+        return pulumi.get(self, "network_ids")
 
     @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="securityGroupIds")
+    def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A free-form text describing the block.
+        A list of [exoscale_security_group](./security_groups.md) (IDs).
         """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+        return pulumi.get(self, "security_group_ids")
 
     @property
-    @pulumi.getter(name="icmpCode")
-    def icmp_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "icmp_code")
-
-    @icmp_code.setter
-    def icmp_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "icmp_code", value)
-
-    @property
-    @pulumi.getter(name="icmpType")
-    def icmp_type(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="serviceOffering")
+    def service_offering(self) -> pulumi.Output[str]:
         """
-        /`icmp_code` - An ICMP/ICMPv6 type/code to match.
+        The managed instances type. Please use the `instance_type` argument instead.
         """
-        return pulumi.get(self, "icmp_type")
-
-    @icmp_type.setter
-    def icmp_type(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "icmp_type", value)
+        return pulumi.get(self, "service_offering")
 
     @property
     @pulumi.getter
-    def ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "ids")
-
-    @ids.setter
-    def ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ids", value)
-
-    @property
-    @pulumi.getter
-    def ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def size(self) -> pulumi.Output[int]:
         """
-        A list of ports or port ranges (`<start_port>-<end_port>`).
+        The number of managed instances.
         """
-        return pulumi.get(self, "ports")
-
-    @ports.setter
-    def ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ports", value)
+        return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def protocol(self) -> Optional[pulumi.Input[str]]:
-        """
-        The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`).
-        """
-        return pulumi.get(self, "protocol")
-
-    @protocol.setter
-    def protocol(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "protocol", value)
+    def state(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "state")
 
     @property
-    @pulumi.getter(name="userSecurityGroupLists")
-    def user_security_group_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="templateId")
+    def template_id(self) -> pulumi.Output[str]:
         """
-        A list of source (for ingress)/destination (for egress) identified by a security group.
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
         """
-        return pulumi.get(self, "user_security_group_lists")
-
-    @user_security_group_lists.setter
-    def user_security_group_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "user_security_group_lists", value)
-
-
-@pulumi.input_type
-class GetDomainRecordFilterArgs:
-    def __init__(__self__, *,
-                 content_regex: Optional[str] = None,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 record_type: Optional[str] = None):
-        """
-        :param str content_regex: A regular expression to match the record content.
-        :param str id: The record ID to match.
-        :param str name: The domain record name to match.
-        :param str record_type: The record type to match.
-        """
-        if content_regex is not None:
-            pulumi.set(__self__, "content_regex", content_regex)
-        if id is not None:
-            pulumi.set(__self__, "id", id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if record_type is not None:
-            pulumi.set(__self__, "record_type", record_type)
+        return pulumi.get(self, "template_id")
 
     @property
-    @pulumi.getter(name="contentRegex")
-    def content_regex(self) -> Optional[str]:
+    @pulumi.getter(name="userData")
+    def user_data(self) -> pulumi.Output[Optional[str]]:
         """
-        A regular expression to match the record content.
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
+        or gzip it as the provider will take care of it).
         """
-        return pulumi.get(self, "content_regex")
-
-    @content_regex.setter
-    def content_regex(self, value: Optional[str]):
-        pulumi.set(self, "content_regex", value)
+        return pulumi.get(self, "user_data")
 
     @property
-    @pulumi.getter
-    def id(self) -> Optional[str]:
+    @pulumi.getter(name="virtualMachines")
+    def virtual_machines(self) -> pulumi.Output[Sequence[str]]:
         """
-        The record ID to match.
+        The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: Optional[str]):
-        pulumi.set(self, "id", value)
+        return pulumi.get(self, "virtual_machines")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
+    def zone(self) -> pulumi.Output[str]:
         """
-        The domain record name to match.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="recordType")
-    def record_type(self) -> Optional[str]:
-        """
-        The record type to match.
-        """
-        return pulumi.get(self, "record_type")
-
-    @record_type.setter
-    def record_type(self, value: Optional[str]):
-        pulumi.set(self, "record_type", value)
-
+        return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,30 +145,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use AntiAffinityGroup instead.
+        **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use AntiAffinityGroup instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the group.
         :param pulumi.Input[str] name: The anti-affinity group name.
         :param pulumi.Input[str] type: The type of the group (`host anti-affinity` is the only supported value).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AffinityArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use AntiAffinityGroup instead.
+        **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use AntiAffinityGroup instead.
 
         :param str resource_name: The name of the resource.
         :param AffinityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing anti-affinity group may be imported by `<ID>`console
+        An existing anti-affinity group may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/antiAffinityGroup:AntiAffinityGroup \\
         ```
 
          exoscale_anti_affinity_group.my_anti_affinity_group \\
 
@@ -122,15 +122,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AntiAffinityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing anti-affinity group may be imported by `<ID>`console
+        An existing anti-affinity group may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/antiAffinityGroup:AntiAffinityGroup \\
         ```
 
          exoscale_anti_affinity_group.my_anti_affinity_group \\
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,35 @@
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Compute resource.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
-        :param pulumi.Input[bool] ip4: Enable IPv4 on the instance (only supported value is `true`).
-        :param pulumi.Input[bool] ip6: Enable IPv6 on the instance (boolean; default: `false`).
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+               be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+               requires to reboot the instance.
+        :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
+        :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+               `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+               templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         pulumi.set(__self__, "disk_size", disk_size)
         pulumi.set(__self__, "zone", zone)
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if affinity_groups is not None:
@@ -140,51 +147,56 @@
     def affinity_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_groups", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+        be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+        requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @hostname.setter
     def hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
     def ip4(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable IPv4 on the instance (only supported value is `true`).
+        Request an IPv4 address on the default NIC
         """
         return pulumi.get(self, "ip4")
 
     @ip4.setter
     def ip4(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ip4", value)
 
     @property
     @pulumi.getter
     def ip6(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable IPv6 on the instance (boolean; default: `false`).
+        Request an IPv6 address on the default NIC
         """
         return pulumi.get(self, "ip6")
 
     @ip6.setter
     def ip6(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ip6", value)
 
@@ -200,15 +212,16 @@
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
     def keyboard(self) -> Optional[pulumi.Input[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+        `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @keyboard.setter
     def keyboard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyboard", value)
 
@@ -272,39 +285,40 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def template(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+        templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
@@ -352,35 +366,43 @@
                  username: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Compute resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
-        :param pulumi.Input[bool] ip4: Enable IPv4 on the instance (only supported value is `true`).
-        :param pulumi.Input[bool] ip6: Enable IPv6 on the instance (boolean; default: `false`).
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+               be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+               requires to reboot the instance.
+        :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
+        :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] ip6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[str] ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
-        :param pulumi.Input[str] name: (Deprecated) The instance hostname. Please use the `hostname` argument instead.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] name: The instance hostname. Please use the `hostname` argument instead.
         :param pulumi.Input[str] password: The instance initial password and/or encrypted password.
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+               templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[bool] user_data_base64: was the cloud-init configuration base64 encoded
-        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the _get_compute_template_ data source `username` attribute instead.
+        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
+               `exoscale_compute_template` data source `username` attribute instead.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if affinity_groups is not None:
             pulumi.set(__self__, "affinity_groups", affinity_groups)
         if disk_size is not None:
@@ -476,15 +498,18 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+        be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
@@ -497,39 +522,41 @@
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+        requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @hostname.setter
     def hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
     def ip4(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable IPv4 on the instance (only supported value is `true`).
+        Request an IPv4 address on the default NIC
         """
         return pulumi.get(self, "ip4")
 
     @ip4.setter
     def ip4(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ip4", value)
 
     @property
     @pulumi.getter
     def ip6(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable IPv6 on the instance (boolean; default: `false`).
+        Request an IPv6 address on the default NIC
         """
         return pulumi.get(self, "ip6")
 
     @ip6.setter
     def ip6(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ip6", value)
 
@@ -578,27 +605,28 @@
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
     def keyboard(self) -> Optional[pulumi.Input[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+        `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @keyboard.setter
     def keyboard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyboard", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        (Deprecated) The instance hostname. Please use the `hostname` argument instead.
+        The instance hostname. Please use the `hostname` argument instead.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -674,39 +702,40 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def template(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+        templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
@@ -734,15 +763,16 @@
     def user_data_base64(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "user_data_base64", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the _get_compute_template_ data source `username` attribute instead.
+        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
+        `exoscale_compute_template` data source `username` attribute instead.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
@@ -783,45 +813,56 @@
                  template_id: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance instead.
 
+        Manage Exoscale Compute Instances.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
-        :param pulumi.Input[bool] ip4: Enable IPv4 on the instance (only supported value is `true`).
-        :param pulumi.Input[bool] ip6: Enable IPv6 on the instance (boolean; default: `false`).
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+               be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+               requires to reboot the instance.
+        :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
+        :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+               `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+               templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ComputeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance instead.
 
+        Manage Exoscale Compute Instances.
+
         :param str resource_name: The name of the resource.
         :param ComputeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ComputeArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -937,35 +978,43 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
-        :param pulumi.Input[bool] ip4: Enable IPv4 on the instance (only supported value is `true`).
-        :param pulumi.Input[bool] ip6: Enable IPv6 on the instance (boolean; default: `false`).
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+               be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+               requires to reboot the instance.
+        :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
+        :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] ip6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[str] ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
-        :param pulumi.Input[str] name: (Deprecated) The instance hostname. Please use the `hostname` argument instead.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] name: The instance hostname. Please use the `hostname` argument instead.
         :param pulumi.Input[str] password: The instance initial password and/or encrypted password.
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+               templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[bool] user_data_base64: was the cloud-init configuration base64 encoded
-        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the _get_compute_template_ data source `username` attribute instead.
+        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
+               `exoscale_compute_template` data source `username` attribute instead.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeState.__new__(_ComputeState)
 
         __props__.__dict__["affinity_group_ids"] = affinity_group_ids
@@ -1021,44 +1070,49 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Output[str]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen ("-") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
+        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
+        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
+        be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter
     def gateway(self) -> pulumi.Output[str]:
         return pulumi.get(self, "gateway")
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
+        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
+        requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def ip4(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable IPv4 on the instance (only supported value is `true`).
+        Request an IPv4 address on the default NIC
         """
         return pulumi.get(self, "ip4")
 
     @property
     @pulumi.getter
     def ip6(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable IPv6 on the instance (boolean; default: `false`).
+        Request an IPv6 address on the default NIC
         """
         return pulumi.get(self, "ip6")
 
     @property
     @pulumi.getter(name="ip6Address")
     def ip6_address(self) -> pulumi.Output[str]:
         """
@@ -1087,23 +1141,24 @@
         """
         return pulumi.get(self, "key_pair")
 
     @property
     @pulumi.getter
     def keyboard(self) -> pulumi.Output[Optional[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
+        `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        (Deprecated) The instance hostname. Please use the `hostname` argument instead.
+        The instance hostname. Please use the `hostname` argument instead.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
@@ -1151,31 +1206,32 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def template(self) -> pulumi.Output[str]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
+        templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
-        The compute instance template (ID). Usage of the _get_compute_template_ data source is recommended.
+        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1191,15 +1247,16 @@
         """
         return pulumi.get(self, "user_data_base64")
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Output[str]:
         """
-        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the _get_compute_template_ data source `username` attribute instead.
+        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
+        `exoscale_compute_template` data source `username` attribute instead.
         """
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,30 +30,34 @@
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ComputeInstance resource.
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+               the instance.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+               creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+               take care of it).
         """
         pulumi.set(__self__, "template_id", template_id)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "zone", zone)
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if deploy_target_id is not None:
@@ -81,51 +85,54 @@
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Input[str]:
         """
-        The_get_compute_template_(ID) to use when creating the instance.
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+        the instance.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+        creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
@@ -153,15 +160,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of ElasticIP (IDs) to attach to the instance.
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -225,27 +232,27 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of SecurityGroup (IDs) to attach to the instance.
+        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -261,15 +268,16 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+        take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
@@ -295,34 +303,39 @@
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ComputeInstance resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+               creation time).
         :param pulumi.Input[str] created_at: The instance creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: (Deprecated) A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
+               instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+               the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+               take care of it).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
@@ -364,15 +377,16 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+        creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
@@ -412,15 +426,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of ElasticIP (IDs) to attach to the instance.
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -484,15 +498,16 @@
     def network_interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]]]):
         pulumi.set(self, "network_interfaces", value)
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Deprecated) A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
+        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
+        instead.
         """
         return pulumi.get(self, "private_network_ids")
 
     @private_network_ids.setter
     def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "private_network_ids", value)
 
@@ -520,27 +535,27 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of SecurityGroup (IDs) to attach to the instance.
+        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -556,51 +571,54 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The_get_compute_template_(ID) to use when creating the instance.
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+        the instance.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+        take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -626,53 +644,57 @@
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing compute instance may be imported by `<ID>@<zone>`console
+        An existing compute instance may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/computeInstance:ComputeInstance \\
         ```
 
          exoscale_compute_instance.my_instance \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+               creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+               the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+               take care of it).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ComputeInstanceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing compute instance may be imported by `<ID>@<zone>`console
+        An existing compute instance may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/computeInstance:ComputeInstance \\
         ```
 
          exoscale_compute_instance.my_instance \\
 
@@ -777,34 +799,39 @@
         """
         Get an existing ComputeInstance resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+               creation time).
         :param pulumi.Input[str] created_at: The instance creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: (Deprecated) A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
+               instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+               the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+               take care of it).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeInstanceState.__new__(_ComputeInstanceState)
 
         __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
         __props__.__dict__["created_at"] = created_at
@@ -828,15 +855,16 @@
         __props__.__dict__["zone"] = zone
         return ComputeInstance(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of AntiAffinityGroup (IDs) to attach to the instance (may only be set at creation time).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
+        creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
@@ -860,15 +888,15 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of ElasticIP (IDs) to attach to the instance.
+        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @property
     @pulumi.getter
     def ipv6(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -908,15 +936,16 @@
         """
         return pulumi.get(self, "network_interfaces")
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> pulumi.Output[Sequence[str]]:
         """
-        (Deprecated) A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
+        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
+        instead.
         """
         return pulumi.get(self, "private_network_ids")
 
     @property
     @pulumi.getter(name="publicIpAddress")
     def public_ip_address(self) -> pulumi.Output[str]:
         """
@@ -932,23 +961,23 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of SecurityGroup (IDs) to attach to the instance.
+        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> pulumi.Output[Optional[str]]:
         """
-        The SSHKey (name) to authorize in the instance (may only be set at creation time).
+        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -956,35 +985,38 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
-        The_get_compute_template_(ID) to use when creating the instance.
+        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
+        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
+        the instance.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> pulumi.Output[Optional[str]]:
         """
-        [cloud-init][cloud-init] configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
+        take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,25 @@
                  name: Optional[pulumi.Input[str]] = None,
                  opensearch: Optional[pulumi.Input['DatabaseOpensearchArgs']] = None,
                  pg: Optional[pulumi.Input['DatabasePgArgs']] = None,
                  redis: Optional[pulumi.Input['DatabaseRedisArgs']] = None,
                  termination_protection: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Database resource.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+               <TYPE>` - for reference).
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
-        :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments.
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+               `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
-        :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments.
         :param pulumi.Input[str] name: The name of the database service.
-        :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input['DatabasePgArgs'] pg: *pg* database service type specific arguments. Structure is documented below.
         :param pulumi.Input['DatabaseRedisArgs'] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         """
         pulumi.set(__self__, "plan", plan)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "zone", zone)
@@ -65,15 +67,16 @@
         if termination_protection is not None:
             pulumi.set(__self__, "termination_protection", termination_protection)
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Input[str]:
         """
-        The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+        <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: pulumi.Input[str]):
         pulumi.set(self, "plan", value)
 
@@ -89,39 +92,40 @@
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def kafka(self) -> Optional[pulumi.Input['DatabaseKafkaArgs']]:
         """
-        *kafka* database service type specific arguments. Structure is documented below.
+        *kafka* database service type specific arguments.
         """
         return pulumi.get(self, "kafka")
 
     @kafka.setter
     def kafka(self, value: Optional[pulumi.Input['DatabaseKafkaArgs']]):
         pulumi.set(self, "kafka", value)
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> Optional[pulumi.Input[str]]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+        `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @maintenance_dow.setter
     def maintenance_dow(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_dow", value)
 
@@ -137,15 +141,15 @@
     def maintenance_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_time", value)
 
     @property
     @pulumi.getter
     def mysql(self) -> Optional[pulumi.Input['DatabaseMysqlArgs']]:
         """
-        *mysql* database service type specific arguments. Structure is documented below.
+        *mysql* database service type specific arguments.
         """
         return pulumi.get(self, "mysql")
 
     @mysql.setter
     def mysql(self, value: Optional[pulumi.Input['DatabaseMysqlArgs']]):
         pulumi.set(self, "mysql", value)
 
@@ -161,15 +165,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input['DatabaseOpensearchArgs']]:
         """
-        *opensearch* database service type specific arguments. Structure is documented below.
+        *opensearch* database service type specific arguments.
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input['DatabaseOpensearchArgs']]):
         pulumi.set(self, "opensearch", value)
 
@@ -235,32 +239,34 @@
                  uri: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[str] ca_certificate: CA Certificate required to reach a DBaaS service through a TLS-protected connection.
         :param pulumi.Input[str] created_at: The creation date of the database service.
         :param pulumi.Input[int] disk_size: The disk size of the database service.
-        :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments.
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+               `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
-        :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments.
         :param pulumi.Input[str] name: The name of the database service.
         :param pulumi.Input[int] node_cpus: The number of CPUs of the database service.
         :param pulumi.Input[int] node_memory: The amount of memory of the database service.
         :param pulumi.Input[int] nodes: The number of nodes of the database service.
-        :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input['DatabasePgArgs'] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+               <TYPE>` - for reference).
         :param pulumi.Input['DatabaseRedisArgs'] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
         :param pulumi.Input[str] uri: The database service connection URI.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if ca_certificate is not None:
             pulumi.set(__self__, "ca_certificate", ca_certificate)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
@@ -337,27 +343,28 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter
     def kafka(self) -> Optional[pulumi.Input['DatabaseKafkaArgs']]:
         """
-        *kafka* database service type specific arguments. Structure is documented below.
+        *kafka* database service type specific arguments.
         """
         return pulumi.get(self, "kafka")
 
     @kafka.setter
     def kafka(self, value: Optional[pulumi.Input['DatabaseKafkaArgs']]):
         pulumi.set(self, "kafka", value)
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> Optional[pulumi.Input[str]]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+        `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @maintenance_dow.setter
     def maintenance_dow(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_dow", value)
 
@@ -373,15 +380,15 @@
     def maintenance_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_time", value)
 
     @property
     @pulumi.getter
     def mysql(self) -> Optional[pulumi.Input['DatabaseMysqlArgs']]:
         """
-        *mysql* database service type specific arguments. Structure is documented below.
+        *mysql* database service type specific arguments.
         """
         return pulumi.get(self, "mysql")
 
     @mysql.setter
     def mysql(self, value: Optional[pulumi.Input['DatabaseMysqlArgs']]):
         pulumi.set(self, "mysql", value)
 
@@ -433,15 +440,15 @@
     def nodes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes", value)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input['DatabaseOpensearchArgs']]:
         """
-        *opensearch* database service type specific arguments. Structure is documented below.
+        *opensearch* database service type specific arguments.
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input['DatabaseOpensearchArgs']]):
         pulumi.set(self, "opensearch", value)
 
@@ -457,15 +464,16 @@
     def pg(self, value: Optional[pulumi.Input['DatabasePgArgs']]):
         pulumi.set(self, "pg", value)
 
     @property
     @pulumi.getter
     def plan(self) -> Optional[pulumi.Input[str]]:
         """
-        The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+        <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plan", value)
 
@@ -541,15 +549,15 @@
     def uri(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uri", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -571,49 +579,51 @@
                  termination_protection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing database service may be imported by `<name>@<zone>`console
+        An existing database service may be imported by `<name>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/database:Database \\
         ```
 
          exoscale_database.my_database \\
 
          my-database@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments.
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+               `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
-        :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments.
         :param pulumi.Input[str] name: The name of the database service.
-        :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input[pulumi.InputType['DatabasePgArgs']] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+               <TYPE>` - for reference).
         :param pulumi.Input[pulumi.InputType['DatabaseRedisArgs']] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing database service may be imported by `<name>@<zone>`console
+        An existing database service may be imported by `<name>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/database:Database \\
         ```
 
          exoscale_database.my_database \\
 
@@ -721,32 +731,34 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ca_certificate: CA Certificate required to reach a DBaaS service through a TLS-protected connection.
         :param pulumi.Input[str] created_at: The creation date of the database service.
         :param pulumi.Input[int] disk_size: The disk size of the database service.
-        :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments.
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+               `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
-        :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments.
         :param pulumi.Input[str] name: The name of the database service.
         :param pulumi.Input[int] node_cpus: The number of CPUs of the database service.
         :param pulumi.Input[int] node_memory: The amount of memory of the database service.
         :param pulumi.Input[int] nodes: The number of nodes of the database service.
-        :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments. Structure is documented below.
+        :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input[pulumi.InputType['DatabasePgArgs']] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+               <TYPE>` - for reference).
         :param pulumi.Input[pulumi.InputType['DatabaseRedisArgs']] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
         :param pulumi.Input[str] uri: The database service connection URI.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatabaseState.__new__(_DatabaseState)
 
         __props__.__dict__["ca_certificate"] = ca_certificate
         __props__.__dict__["created_at"] = created_at
@@ -795,23 +807,24 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def kafka(self) -> pulumi.Output[Optional['outputs.DatabaseKafka']]:
         """
-        *kafka* database service type specific arguments. Structure is documented below.
+        *kafka* database service type specific arguments.
         """
         return pulumi.get(self, "kafka")
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> pulumi.Output[str]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
+        `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @property
     @pulumi.getter(name="maintenanceTime")
     def maintenance_time(self) -> pulumi.Output[str]:
         """
@@ -819,15 +832,15 @@
         """
         return pulumi.get(self, "maintenance_time")
 
     @property
     @pulumi.getter
     def mysql(self) -> pulumi.Output[Optional['outputs.DatabaseMysql']]:
         """
-        *mysql* database service type specific arguments. Structure is documented below.
+        *mysql* database service type specific arguments.
         """
         return pulumi.get(self, "mysql")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -859,15 +872,15 @@
         """
         return pulumi.get(self, "nodes")
 
     @property
     @pulumi.getter
     def opensearch(self) -> pulumi.Output[Optional['outputs.DatabaseOpensearch']]:
         """
-        *opensearch* database service type specific arguments. Structure is documented below.
+        *opensearch* database service type specific arguments.
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter
     def pg(self) -> pulumi.Output[Optional['outputs.DatabasePg']]:
         """
@@ -875,15 +888,16 @@
         """
         return pulumi.get(self, "pg")
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Output[str]:
         """
-        The plan of the database service (use the [Exoscale CLI][cli] - `exo dbaas type show <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
+        <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter
     def redis(self) -> pulumi.Output[Optional['outputs.DatabaseRedis']]:
         """
@@ -931,11 +945,11 @@
         """
         return pulumi.get(self, "uri")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing DNS domain may be imported by `ID`console
+        An existing DNS domain may be imported by `ID`
 
         ```sh
          $ pulumi import exoscale:index/domain:Domain \\
         ```
 
          exoscale_domain.my_domain \\
 
@@ -164,15 +164,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DomainArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing DNS domain may be imported by `ID`console
+        An existing DNS domain may be imported by `ID`
 
         ```sh
          $ pulumi import exoscale:index/domain:Domain \\
         ```
 
          exoscale_domain.my_domain \\
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
                  record_type: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  prio: Optional[pulumi.Input[int]] = None,
                  ttl: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a DomainRecord resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent Domain to attach the record to.
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
+        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+               `TXT`, `URL`).
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         pulumi.set(__self__, "content", content)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "record_type", record_type)
@@ -51,27 +52,28 @@
     def content(self, value: pulumi.Input[str]):
         pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Input[str]:
         """
-        The parent Domain to attach the record to.
+        The parent [exoscale_domain](./domain.md) to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: pulumi.Input[str]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> pulumi.Input[str]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+        `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @record_type.setter
     def record_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "record_type", value)
 
@@ -121,19 +123,20 @@
                  name: Optional[pulumi.Input[str]] = None,
                  prio: Optional[pulumi.Input[int]] = None,
                  record_type: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering DomainRecord resources.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent Domain to attach the record to.
+        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
         :param pulumi.Input[str] hostname: The record *Fully Qualified Domain Name* (FQDN). Useful for aliasing `A`/`AAAA` records with `CNAME`.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+               `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         if content is not None:
             pulumi.set(__self__, "content", content)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if hostname is not None:
@@ -159,15 +162,15 @@
     def content(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent Domain to attach the record to.
+        The parent [exoscale_domain](./domain.md) to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
@@ -207,15 +210,16 @@
     def prio(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "prio", value)
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+        `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @record_type.setter
     def record_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "record_type", value)
 
@@ -243,43 +247,44 @@
                  prio: Optional[pulumi.Input[int]] = None,
                  record_type: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing DNS domain record may be imported by `<ID>`console
+        An existing DNS domain record may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/domainRecord:DomainRecord \\
         ```
 
          exoscale_domain_record.my_host \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent Domain to attach the record to.
+        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+               `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DomainRecordArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing DNS domain record may be imported by `<ID>`console
+        An existing DNS domain record may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/domainRecord:DomainRecord \\
         ```
 
          exoscale_domain_record.my_host \\
 
@@ -349,19 +354,20 @@
         Get an existing DomainRecord resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent Domain to attach the record to.
+        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
         :param pulumi.Input[str] hostname: The record *Fully Qualified Domain Name* (FQDN). Useful for aliasing `A`/`AAAA` records with `CNAME`.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+               `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DomainRecordState.__new__(_DomainRecordState)
 
         __props__.__dict__["content"] = content
@@ -381,15 +387,15 @@
         """
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Output[str]:
         """
-        The parent Domain to attach the record to.
+        The parent [exoscale_domain](./domain.md) to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         """
@@ -413,15 +419,16 @@
         """
         return pulumi.get(self, "prio")
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> pulumi.Output[str]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
+        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
+        `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @property
     @pulumi.getter
     def ttl(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
                  address_family: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  healthcheck: Optional[pulumi.Input['ElasticIPHealthcheckArgs']] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ElasticIP resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
-        :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         """
         pulumi.set(__self__, "zone", zone)
         if address_family is not None:
             pulumi.set(__self__, "address_family", address_family)
         if description is not None:
@@ -43,15 +43,15 @@
         if reverse_dns is not None:
             pulumi.set(__self__, "reverse_dns", reverse_dns)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -79,15 +79,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def healthcheck(self) -> Optional[pulumi.Input['ElasticIPHealthcheckArgs']]:
         """
-        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         """
         return pulumi.get(self, "healthcheck")
 
     @healthcheck.setter
     def healthcheck(self, value: Optional[pulumi.Input['ElasticIPHealthcheckArgs']]):
         pulumi.set(self, "healthcheck", value)
 
@@ -128,19 +128,19 @@
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ElasticIP resources.
         :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] cidr: The Elastic IP (EIP) CIDR.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
-        :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 or IPv6 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if address_family is not None:
             pulumi.set(__self__, "address_family", address_family)
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -191,15 +191,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def healthcheck(self) -> Optional[pulumi.Input['ElasticIPHealthcheckArgs']]:
         """
-        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         """
         return pulumi.get(self, "healthcheck")
 
     @healthcheck.setter
     def healthcheck(self, value: Optional[pulumi.Input['ElasticIPHealthcheckArgs']]):
         pulumi.set(self, "healthcheck", value)
 
@@ -239,15 +239,15 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -261,53 +261,45 @@
                  description: Optional[pulumi.Input[str]] = None,
                  healthcheck: Optional[pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/).
-
-        Corresponding data source: exoscale_elastic_ip.
-
         ## Import
 
-        An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`console
+        An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/elasticIP:ElasticIP \\
         ```
 
          exoscale_elastic_ip.my_elastic_ip \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
-        :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ElasticIPArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/).
-
-        Corresponding data source: exoscale_elastic_ip.
-
         ## Import
 
-        An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`console
+        An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/elasticIP:ElasticIP \\
         ```
 
          exoscale_elastic_ip.my_elastic_ip \\
 
@@ -377,19 +369,19 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] cidr: The Elastic IP (EIP) CIDR.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
-        :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 or IPv6 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ElasticIPState.__new__(_ElasticIPState)
 
         __props__.__dict__["address_family"] = address_family
         __props__.__dict__["cidr"] = cidr
@@ -425,15 +417,15 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def healthcheck(self) -> pulumi.Output['outputs.ElasticIPHealthcheck']:
         """
-        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP. Structure is documented below:
+        Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         """
         return pulumi.get(self, "healthcheck")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
@@ -457,11 +449,11 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_affinity.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,25 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The anti-affinity group ID to match (conflicts with `name`)
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The group name to match (conflicts with `id`)
+        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetAffinityResult(GetAffinityResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,27 +31,33 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The anti-affinity group ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def instances(self) -> Sequence[str]:
         """
-        The list of attached ComputeInstance (IDs).
+        The list of attached exoscale*compute*instance (IDs).
         """
         return pulumi.get(self, "instances")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The group name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetAntiAffinityGroupResult(GetAntiAffinityGroupResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,110 +65,119 @@
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def cpu(self) -> int:
         """
-        The compute instance number of CPUs.
+        Number of cpu the Compute instance is running with
         """
         return pulumi.get(self, "cpu")
 
     @property
     @pulumi.getter
     def created(self) -> str:
         """
-        The instance creation date.
+        Date when the Compute instance was created
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> int:
         """
-        The instance disk size (GiB).
+        Size of the Compute instance disk
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The instance hostname to match.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The compute instance ID to match.
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="ip6Address")
     def ip6_address(self) -> str:
         """
-        The instance (main network interface) IPv6 address (if enabled).
+        Compute instance public ipv6 address (if ipv6 is enabled)
         """
         return pulumi.get(self, "ip6_address")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> str:
         """
-        The instance (main network interface) IPv4 address.
+        Compute instance public ipv4 address
         """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter
     def memory(self) -> int:
         """
-        The instance allocated memory.
+        Memory allocated for the Compute instance
         """
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter(name="privateNetworkIpAddresses")
     def private_network_ip_addresses(self) -> Sequence[str]:
         """
-        List of compute private IPv4 addresses (in *managed* private networks only).
+        List of Compute instance private IP addresses (in managed Private Networks only)
         """
         return pulumi.get(self, "private_network_ip_addresses")
 
     @property
     @pulumi.getter
     def size(self) -> str:
         """
-        The instance size.
+        Current size of the Compute instance
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
     def state(self) -> str:
         """
-        The current instance state.
+        State of the Compute instance
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        The instance tags to match (map of key/value).
+        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def template(self) -> str:
         """
-        The instance template.
+        Name of the template for the Compute instance
         """
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
         """
-        Exoscale Zone name.
+        Name of the availability zone for the Compute instance
         """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetComputeResult(GetComputeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,17 @@
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[Sequence[str]]:
+        """
+        The list of attached exoscale*anti*affinity_group (IDs).
+        """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> str:
         """
         The compute instance creation date.
@@ -118,21 +121,24 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Sequence[str]:
         """
-        The list of attached ElasticIP (IDs).
+        The list of attached exoscale*elastic*ip (IDs).
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The compute instance ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def ipv6(self) -> bool:
         """
         Whether IPv6 is enabled on the instance.
@@ -170,19 +176,25 @@
         The instance manager type (instance pool, SKS node pool, etc.), if any.
         """
         return pulumi.get(self, "manager_type")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The instance name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*private*network (IDs).
+        """
         return pulumi.get(self, "private_network_ids")
 
     @property
     @pulumi.getter(name="publicIpAddress")
     def public_ip_address(self) -> str:
         """
         The instance (main network interface) IPv4 address.
@@ -197,23 +209,23 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Sequence[str]:
         """
-        The list of attached SecurityGroup (IDs).
+        The list of attached exoscale*security*group (IDs).
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> str:
         """
-        The SSHKey (name) authorized on the instance.
+        The exoscale*ssh*key (name) authorized on the instance.
         """
         return pulumi.get(self, "ssh_key")
 
     @property
     @pulumi.getter
     def state(self) -> str:
         """
@@ -221,15 +233,15 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> str:
         """
-        The instance_get_compute_template_ID.
+        The instance exoscale*compute*template ID.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
@@ -237,21 +249,24 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> str:
         """
-        The instance [cloud-init][cloud-init] configuration.
+        The instance [cloud-init](http://cloudinit.readthedocs.io/en/latest/) configuration.
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetComputeInstanceResult(GetComputeInstanceResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -286,18 +301,19 @@
                          labels: Optional[Mapping[str, str]] = None,
                          name: Optional[str] = None,
                          zone: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetComputeInstanceResult:
     """
     Use this data source to access information about an existing resource.
 
+    :param Sequence[str] anti_affinity_group_ids: The list of attached exoscale*anti*affinity_group (IDs).
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param Mapping[str, str] labels: A map of key/value labels.
     :param str name: The instance name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['antiAffinityGroupIds'] = anti_affinity_group_ids
     __args__['id'] = id
     __args__['labels'] = labels
     __args__['name'] = name
     __args__['zone'] = zone
@@ -335,13 +351,14 @@
                                 labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
                                 zone: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetComputeInstanceResult]:
     """
     Use this data source to access information about an existing resource.
 
+    :param Sequence[str] anti_affinity_group_ids: The list of attached exoscale*anti*affinity_group (IDs).
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param Mapping[str, str] labels: A map of key/value labels.
     :param str name: The instance name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,294 +7,328 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetComputeInstanceListResult',
-    'AwaitableGetComputeInstanceListResult',
-    'get_compute_instance_list',
-    'get_compute_instance_list_output',
+    'GetInstancePoolResult',
+    'AwaitableGetInstancePoolResult',
+    'get_instance_pool',
+    'get_instance_pool_output',
 ]
 
 @pulumi.output_type
-class GetComputeInstanceListResult:
+class GetInstancePoolResult:
     """
-    A collection of values returned by getComputeInstanceList.
+    A collection of values returned by getInstancePool.
     """
-    def __init__(__self__, created_at=None, deploy_target_id=None, disk_size=None, id=None, instances=None, ipv6=None, ipv6_address=None, labels=None, manager_id=None, manager_type=None, name=None, public_ip_address=None, reverse_dns=None, ssh_key=None, state=None, template_id=None, type=None, user_data=None, zone=None):
-        if created_at and not isinstance(created_at, str):
-            raise TypeError("Expected argument 'created_at' to be a str")
-        pulumi.set(__self__, "created_at", created_at)
+    def __init__(__self__, affinity_group_ids=None, deploy_target_id=None, description=None, disk_size=None, elastic_ip_ids=None, id=None, instance_prefix=None, instance_type=None, instances=None, ipv6=None, key_pair=None, labels=None, name=None, network_ids=None, security_group_ids=None, size=None, state=None, template_id=None, user_data=None, zone=None):
+        if affinity_group_ids and not isinstance(affinity_group_ids, list):
+            raise TypeError("Expected argument 'affinity_group_ids' to be a list")
+        pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if deploy_target_id and not isinstance(deploy_target_id, str):
             raise TypeError("Expected argument 'deploy_target_id' to be a str")
         pulumi.set(__self__, "deploy_target_id", deploy_target_id)
+        if description and not isinstance(description, str):
+            raise TypeError("Expected argument 'description' to be a str")
+        pulumi.set(__self__, "description", description)
         if disk_size and not isinstance(disk_size, int):
             raise TypeError("Expected argument 'disk_size' to be a int")
         pulumi.set(__self__, "disk_size", disk_size)
+        if elastic_ip_ids and not isinstance(elastic_ip_ids, list):
+            raise TypeError("Expected argument 'elastic_ip_ids' to be a list")
+        pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if instance_prefix and not isinstance(instance_prefix, str):
+            raise TypeError("Expected argument 'instance_prefix' to be a str")
+        pulumi.set(__self__, "instance_prefix", instance_prefix)
+        if instance_type and not isinstance(instance_type, str):
+            raise TypeError("Expected argument 'instance_type' to be a str")
+        pulumi.set(__self__, "instance_type", instance_type)
         if instances and not isinstance(instances, list):
             raise TypeError("Expected argument 'instances' to be a list")
         pulumi.set(__self__, "instances", instances)
         if ipv6 and not isinstance(ipv6, bool):
             raise TypeError("Expected argument 'ipv6' to be a bool")
         pulumi.set(__self__, "ipv6", ipv6)
-        if ipv6_address and not isinstance(ipv6_address, str):
-            raise TypeError("Expected argument 'ipv6_address' to be a str")
-        pulumi.set(__self__, "ipv6_address", ipv6_address)
+        if key_pair and not isinstance(key_pair, str):
+            raise TypeError("Expected argument 'key_pair' to be a str")
+        pulumi.set(__self__, "key_pair", key_pair)
         if labels and not isinstance(labels, dict):
             raise TypeError("Expected argument 'labels' to be a dict")
         pulumi.set(__self__, "labels", labels)
-        if manager_id and not isinstance(manager_id, str):
-            raise TypeError("Expected argument 'manager_id' to be a str")
-        pulumi.set(__self__, "manager_id", manager_id)
-        if manager_type and not isinstance(manager_type, str):
-            raise TypeError("Expected argument 'manager_type' to be a str")
-        pulumi.set(__self__, "manager_type", manager_type)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if public_ip_address and not isinstance(public_ip_address, str):
-            raise TypeError("Expected argument 'public_ip_address' to be a str")
-        pulumi.set(__self__, "public_ip_address", public_ip_address)
-        if reverse_dns and not isinstance(reverse_dns, str):
-            raise TypeError("Expected argument 'reverse_dns' to be a str")
-        pulumi.set(__self__, "reverse_dns", reverse_dns)
-        if ssh_key and not isinstance(ssh_key, str):
-            raise TypeError("Expected argument 'ssh_key' to be a str")
-        pulumi.set(__self__, "ssh_key", ssh_key)
+        if network_ids and not isinstance(network_ids, list):
+            raise TypeError("Expected argument 'network_ids' to be a list")
+        pulumi.set(__self__, "network_ids", network_ids)
+        if security_group_ids and not isinstance(security_group_ids, list):
+            raise TypeError("Expected argument 'security_group_ids' to be a list")
+        pulumi.set(__self__, "security_group_ids", security_group_ids)
+        if size and not isinstance(size, int):
+            raise TypeError("Expected argument 'size' to be a int")
+        pulumi.set(__self__, "size", size)
         if state and not isinstance(state, str):
             raise TypeError("Expected argument 'state' to be a str")
         pulumi.set(__self__, "state", state)
         if template_id and not isinstance(template_id, str):
             raise TypeError("Expected argument 'template_id' to be a str")
         pulumi.set(__self__, "template_id", template_id)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
         if user_data and not isinstance(user_data, str):
             raise TypeError("Expected argument 'user_data' to be a str")
         pulumi.set(__self__, "user_data", user_data)
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
-        return pulumi.get(self, "created_at")
+    @pulumi.getter(name="affinityGroupIds")
+    def affinity_group_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*anti*affinity_group (IDs).
+        """
+        return pulumi.get(self, "affinity_group_ids")
 
     @property
     @pulumi.getter(name="deployTargetId")
-    def deploy_target_id(self) -> Optional[str]:
+    def deploy_target_id(self) -> str:
+        """
+        The deploy target ID.
+        """
         return pulumi.get(self, "deploy_target_id")
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The instance pool description.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="diskSize")
-    def disk_size(self) -> Optional[int]:
+    def disk_size(self) -> int:
+        """
+        The managed instances disk size.
+        """
         return pulumi.get(self, "disk_size")
 
     @property
+    @pulumi.getter(name="elasticIpIds")
+    def elastic_ip_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*elastic*ip (IDs).
+        """
+        return pulumi.get(self, "elastic_ip_ids")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The instance pool ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="instancePrefix")
+    def instance_prefix(self) -> str:
+        """
+        The string used to prefix the managed instances name.
+        """
+        return pulumi.get(self, "instance_prefix")
+
+    @property
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> str:
+        """
+        The managed instances type.
+        """
+        return pulumi.get(self, "instance_type")
+
+    @property
     @pulumi.getter
-    def instances(self) -> Sequence['outputs.GetComputeInstanceListInstanceResult']:
+    def instances(self) -> Sequence['outputs.GetInstancePoolInstanceResult']:
+        """
+        The list of managed instances. Structure is documented below.
+        """
         return pulumi.get(self, "instances")
 
     @property
     @pulumi.getter
-    def ipv6(self) -> Optional[bool]:
+    def ipv6(self) -> bool:
+        """
+        Whether IPv6 is enabled on managed instances.
+        """
         return pulumi.get(self, "ipv6")
 
     @property
-    @pulumi.getter(name="ipv6Address")
-    def ipv6_address(self) -> Optional[str]:
-        return pulumi.get(self, "ipv6_address")
+    @pulumi.getter(name="keyPair")
+    def key_pair(self) -> str:
+        """
+        The exoscale*ssh*key (name) authorized on the managed instances.
+        """
+        return pulumi.get(self, "key_pair")
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, str]]:
+        """
+        A map of key/value labels.
+        """
         return pulumi.get(self, "labels")
 
     @property
-    @pulumi.getter(name="managerId")
-    def manager_id(self) -> Optional[str]:
-        return pulumi.get(self, "manager_id")
-
-    @property
-    @pulumi.getter(name="managerType")
-    def manager_type(self) -> Optional[str]:
-        return pulumi.get(self, "manager_type")
-
-    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The pool name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="publicIpAddress")
-    def public_ip_address(self) -> Optional[str]:
-        return pulumi.get(self, "public_ip_address")
+    @pulumi.getter(name="networkIds")
+    def network_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*private*network (IDs).
+        """
+        return pulumi.get(self, "network_ids")
 
     @property
-    @pulumi.getter(name="reverseDns")
-    def reverse_dns(self) -> Optional[str]:
-        return pulumi.get(self, "reverse_dns")
+    @pulumi.getter(name="securityGroupIds")
+    def security_group_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*security*group (IDs).
+        """
+        return pulumi.get(self, "security_group_ids")
 
     @property
-    @pulumi.getter(name="sshKey")
-    def ssh_key(self) -> Optional[str]:
-        return pulumi.get(self, "ssh_key")
+    @pulumi.getter
+    def size(self) -> int:
+        """
+        The number managed instances.
+        """
+        return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def state(self) -> Optional[str]:
+    def state(self) -> str:
+        """
+        The pool state.
+        """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
-    def template_id(self) -> Optional[str]:
+    def template_id(self) -> str:
+        """
+        The managed instances exoscale*compute*template ID.
+        """
         return pulumi.get(self, "template_id")
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="userData")
-    def user_data(self) -> Optional[str]:
+    def user_data(self) -> str:
+        """
+        [cloud-init](http://cloudinit.readthedocs.io/en/latest/) configuration.
+        """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter
-    def zone(self) -> Optional[str]:
+    def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
-class AwaitableGetComputeInstanceListResult(GetComputeInstanceListResult):
+class AwaitableGetInstancePoolResult(GetInstancePoolResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetComputeInstanceListResult(
-            created_at=self.created_at,
+        return GetInstancePoolResult(
+            affinity_group_ids=self.affinity_group_ids,
             deploy_target_id=self.deploy_target_id,
+            description=self.description,
             disk_size=self.disk_size,
+            elastic_ip_ids=self.elastic_ip_ids,
             id=self.id,
+            instance_prefix=self.instance_prefix,
+            instance_type=self.instance_type,
             instances=self.instances,
             ipv6=self.ipv6,
-            ipv6_address=self.ipv6_address,
+            key_pair=self.key_pair,
             labels=self.labels,
-            manager_id=self.manager_id,
-            manager_type=self.manager_type,
             name=self.name,
-            public_ip_address=self.public_ip_address,
-            reverse_dns=self.reverse_dns,
-            ssh_key=self.ssh_key,
+            network_ids=self.network_ids,
+            security_group_ids=self.security_group_ids,
+            size=self.size,
             state=self.state,
             template_id=self.template_id,
-            type=self.type,
             user_data=self.user_data,
             zone=self.zone)
 
 
-def get_compute_instance_list(created_at: Optional[str] = None,
-                              deploy_target_id: Optional[str] = None,
-                              disk_size: Optional[int] = None,
-                              id: Optional[str] = None,
-                              ipv6: Optional[bool] = None,
-                              ipv6_address: Optional[str] = None,
-                              labels: Optional[Mapping[str, str]] = None,
-                              manager_id: Optional[str] = None,
-                              manager_type: Optional[str] = None,
-                              name: Optional[str] = None,
-                              public_ip_address: Optional[str] = None,
-                              reverse_dns: Optional[str] = None,
-                              ssh_key: Optional[str] = None,
-                              state: Optional[str] = None,
-                              template_id: Optional[str] = None,
-                              type: Optional[str] = None,
-                              user_data: Optional[str] = None,
-                              zone: Optional[str] = None,
-                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetComputeInstanceListResult:
+def get_instance_pool(id: Optional[str] = None,
+                      labels: Optional[Mapping[str, str]] = None,
+                      name: Optional[str] = None,
+                      zone: Optional[str] = None,
+                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancePoolResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str id: The instance pool ID to match (conflicts with `name`).
+    :param Mapping[str, str] labels: A map of key/value labels.
+    :param str name: The pool name to match (conflicts with `id`).
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
-    __args__['createdAt'] = created_at
-    __args__['deployTargetId'] = deploy_target_id
-    __args__['diskSize'] = disk_size
     __args__['id'] = id
-    __args__['ipv6'] = ipv6
-    __args__['ipv6Address'] = ipv6_address
     __args__['labels'] = labels
-    __args__['managerId'] = manager_id
-    __args__['managerType'] = manager_type
     __args__['name'] = name
-    __args__['publicIpAddress'] = public_ip_address
-    __args__['reverseDns'] = reverse_dns
-    __args__['sshKey'] = ssh_key
-    __args__['state'] = state
-    __args__['templateId'] = template_id
-    __args__['type'] = type
-    __args__['userData'] = user_data
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeInstanceList:getComputeInstanceList', __args__, opts=opts, typ=GetComputeInstanceListResult).value
+    __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePool:getInstancePool', __args__, opts=opts, typ=GetInstancePoolResult).value
 
-    return AwaitableGetComputeInstanceListResult(
-        created_at=__ret__.created_at,
+    return AwaitableGetInstancePoolResult(
+        affinity_group_ids=__ret__.affinity_group_ids,
         deploy_target_id=__ret__.deploy_target_id,
+        description=__ret__.description,
         disk_size=__ret__.disk_size,
+        elastic_ip_ids=__ret__.elastic_ip_ids,
         id=__ret__.id,
+        instance_prefix=__ret__.instance_prefix,
+        instance_type=__ret__.instance_type,
         instances=__ret__.instances,
         ipv6=__ret__.ipv6,
-        ipv6_address=__ret__.ipv6_address,
+        key_pair=__ret__.key_pair,
         labels=__ret__.labels,
-        manager_id=__ret__.manager_id,
-        manager_type=__ret__.manager_type,
         name=__ret__.name,
-        public_ip_address=__ret__.public_ip_address,
-        reverse_dns=__ret__.reverse_dns,
-        ssh_key=__ret__.ssh_key,
+        network_ids=__ret__.network_ids,
+        security_group_ids=__ret__.security_group_ids,
+        size=__ret__.size,
         state=__ret__.state,
         template_id=__ret__.template_id,
-        type=__ret__.type,
         user_data=__ret__.user_data,
         zone=__ret__.zone)
 
 
-@_utilities.lift_output_func(get_compute_instance_list)
-def get_compute_instance_list_output(created_at: Optional[pulumi.Input[Optional[str]]] = None,
-                                     deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     disk_size: Optional[pulumi.Input[Optional[int]]] = None,
-                                     id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     ipv6: Optional[pulumi.Input[Optional[bool]]] = None,
-                                     ipv6_address: Optional[pulumi.Input[Optional[str]]] = None,
-                                     labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
-                                     manager_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     manager_type: Optional[pulumi.Input[Optional[str]]] = None,
-                                     name: Optional[pulumi.Input[Optional[str]]] = None,
-                                     public_ip_address: Optional[pulumi.Input[Optional[str]]] = None,
-                                     reverse_dns: Optional[pulumi.Input[Optional[str]]] = None,
-                                     ssh_key: Optional[pulumi.Input[Optional[str]]] = None,
-                                     state: Optional[pulumi.Input[Optional[str]]] = None,
-                                     template_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     type: Optional[pulumi.Input[Optional[str]]] = None,
-                                     user_data: Optional[pulumi.Input[Optional[str]]] = None,
-                                     zone: Optional[pulumi.Input[Optional[str]]] = None,
-                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetComputeInstanceListResult]:
+@_utilities.lift_output_func(get_instance_pool)
+def get_instance_pool_output(id: Optional[pulumi.Input[Optional[str]]] = None,
+                             labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
+                             name: Optional[pulumi.Input[Optional[str]]] = None,
+                             zone: Optional[pulumi.Input[str]] = None,
+                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str id: The instance pool ID to match (conflicts with `name`).
+    :param Mapping[str, str] labels: A map of key/value labels.
+    :param str name: The pool name to match (conflicts with `id`).
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,34 +37,49 @@
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
+        """
+        The EIP description to match.
+        """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The Elastic IP (EIP) ID to match.
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[str]:
+        """
+        The EIP IPv4 address to match.
+        """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        The EIP tags to match.
+        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale Zone name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetComputeIPAddressResult(GetComputeIPAddressResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,37 +37,49 @@
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def filter(self) -> Optional[str]:
+        """
+        A template category filter (default: `featured`); among: - `featured` - official Exoscale templates - `community` - community-contributed templates - `mine` - custom templates private to my organization
+        """
         return pulumi.get(self, "filter")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The compute instance template ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The template name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        Username to use to log into a compute instance based on this template
+        Username for logging into a compute instance based on this template
         """
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetComputeTemplateResult(GetComputeTemplateResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -84,18 +96,18 @@
                          id: Optional[str] = None,
                          name: Optional[str] = None,
                          zone: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetComputeTemplateResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str filter: A template category filter (default: `featured`); among:
+    :param str filter: A template category filter (default: `featured`); among: - `featured` - official Exoscale templates - `community` - community-contributed templates - `mine` - custom templates private to my organization
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['filter'] = filter
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -114,13 +126,13 @@
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
                                 zone: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetComputeTemplateResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str filter: A template category filter (default: `featured`); among:
+    :param str filter: A template category filter (default: `featured`); among: - `featured` - official Exoscale templates - `community` - community-contributed templates - `mine` - custom templates private to my organization
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        The DNS domain name to match.
+        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetDomainResult(GetDomainResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,19 +36,25 @@
         if records and not isinstance(records, list):
             raise TypeError("Expected argument 'records' to be a list")
         pulumi.set(__self__, "records", records)
 
     @property
     @pulumi.getter
     def domain(self) -> str:
+        """
+        The Domain name to match.
+        """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def filter(self) -> 'outputs.GetDomainRecordFilterResult':
+        """
+        Filter to apply when looking up domain records.
+        """
         return pulumi.get(self, "filter")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
@@ -79,15 +85,15 @@
 def get_domain_record(domain: Optional[str] = None,
                       filter: Optional[pulumi.InputType['GetDomainRecordFilterArgs']] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainRecordResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str domain: The Domain name to match.
-    :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records. Structure is documented below.
+    :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records.
     """
     __args__ = dict()
     __args__['domain'] = domain
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getDomainRecord:getDomainRecord', __args__, opts=opts, typ=GetDomainRecordResult).value
 
@@ -102,10 +108,10 @@
 def get_domain_record_output(domain: Optional[pulumi.Input[str]] = None,
                              filter: Optional[pulumi.Input[pulumi.InputType['GetDomainRecordFilterArgs']]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainRecordResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str domain: The Domain name to match.
-    :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records. Structure is documented below.
+    :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,47 +75,56 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def healthchecks(self) -> Sequence['outputs.GetElasticIPHealthcheckResult']:
         """
-        (Block) The *managed* EIP healthcheck configuration. Structure is documented below.
+        The *managed* EIP healthcheck configuration.
         """
         return pulumi.get(self, "healthchecks")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[str]:
+        """
+        The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
+        """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, str]]:
         """
-        A map of key/value labels.
+        The EIP labels to match (conflicts with `ip_address` and `id`).
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="reverseDns")
     def reverse_dns(self) -> str:
         """
         Domain name for reverse DNS record.
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exocale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetElasticIPResult(GetElasticIPResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -139,15 +148,15 @@
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetElasticIPResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
     :param Mapping[str, str] labels: The EIP labels to match (conflicts with `ip_address` and `id`).
-    :param str zone: The Exocale [Zone][zone] name.
+    :param str zone: The Exocale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['ipAddress'] = ip_address
     __args__['labels'] = labels
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -173,10 +182,10 @@
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetElasticIPResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
     :param Mapping[str, str] labels: The EIP labels to match (conflicts with `ip_address` and `id`).
-    :param str zone: The Exocale [Zone][zone] name.
+    :param str zone: The Exocale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,24 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def pools(self) -> Sequence['outputs.GetInstancePoolListPoolResult']:
         """
-        The list of exoscale_instance_pool.
+        The list of exoscale*instance*pool.
         """
         return pulumi.get(self, "pools")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetInstancePoolListResult(GetInstancePoolListResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -67,15 +70,15 @@
 
 
 def get_instance_pool_list(zone: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancePoolListResult:
     """
     Use this data source to access information about an existing resource.
 
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePoolList:getInstancePoolList', __args__, opts=opts, typ=GetInstancePoolListResult).value
 
     return AwaitableGetInstancePoolListResult(
@@ -86,10 +89,10 @@
 
 @_utilities.lift_output_func(get_instance_pool_list)
 def get_instance_pool_list_output(zone: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolListResult]:
     """
     Use this data source to access information about an existing resource.
 
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_network.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,45 +51,57 @@
         The private network description.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> str:
+        """
+        The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
         return pulumi.get(self, "end_ip")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The private network ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The network name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def netmask(self) -> str:
         """
         The network mask defining the IPv4 network allowed for static leases.
         """
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> str:
         """
-        /`end_ip` - The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        (Required) The Exoscale Zone name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetNetworkResult(GetNetworkResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -110,15 +122,15 @@
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkResult:
     """
     !> **WARNING:** This data source is **DEPRECATED** and will be removed in the next major version. Please use PrivateNetwork instead.
 
 
     :param str id: The private network ID to match (conflicts with `name`).
     :param str name: The network name to match (conflicts with `id`).
-    :param str zone: The Exoscale Zone name.
+    :param str zone: (Required) The Exoscale Zone name.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getNetwork:getNetwork', __args__, opts=opts, typ=GetNetworkResult).value
@@ -140,10 +152,10 @@
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
     """
     !> **WARNING:** This data source is **DEPRECATED** and will be removed in the next major version. Please use PrivateNetwork instead.
 
 
     :param str id: The private network ID to match (conflicts with `name`).
     :param str name: The network name to match (conflicts with `id`).
-    :param str zone: The Exoscale Zone name.
+    :param str zone: (Required) The Exoscale Zone name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_nlb.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,40 +59,49 @@
         The Network Load Balancers (NLB) description.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The Network Load Balancers (NLB) ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> str:
         """
         The NLB public IPv4 address.
         """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The NLB name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def state(self) -> str:
         """
         The current NLB state.
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetNLBResult(GetNLBResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -112,15 +121,15 @@
             zone: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNLBResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getNLB:getNLB', __args__, opts=opts, typ=GetNLBResult).value
@@ -141,10 +150,10 @@
                    zone: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNLBResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_private_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,45 +51,57 @@
         The private network description.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> str:
+        """
+        The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
         return pulumi.get(self, "end_ip")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The private network ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The network name to match (conflicts with `id`).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def netmask(self) -> str:
         """
         The network mask defining the IPv4 network allowed for static leases.
         """
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> str:
         """
-        /`end_ip` - The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetPrivateNetworkResult(GetPrivateNetworkResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -111,15 +123,15 @@
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateNetworkResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
     :param str name: The network name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['description'] = description
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -143,10 +155,10 @@
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateNetworkResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
     :param str name: The network name to match (conflicts with `id`).
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_security_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,25 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The security group ID to match (conflicts with `name`)
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The name to match (conflicts with `id`)
+        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetSecurityGroupResult(GetSecurityGroupResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,29 +45,41 @@
         Username to use to log into a compute instance based on this template
         """
         return pulumi.get(self, "default_user")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
+        """
+        The compute instance template ID to match (conflicts with `name`).
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def visibility(self) -> Optional[str]:
+        """
+        A template category filter (default: `public`); among: - `public` - official Exoscale templates - `private` - custom templates private to my organization
+        """
         return pulumi.get(self, "visibility")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
+        """
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
         return pulumi.get(self, "zone")
 
 
 class AwaitableGetTemplateResult(GetTemplateResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -86,16 +98,16 @@
                  zone: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTemplateResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
-    :param str visibility: A template category filter (default: `public`); among:
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str visibility: A template category filter (default: `public`); among: - `public` - official Exoscale templates - `private` - custom templates private to my organization
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['visibility'] = visibility
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -116,11 +128,11 @@
                         zone: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTemplateResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
-    :param str visibility: A template category filter (default: `public`); among:
-    :param str zone: The Exoscale [Zone][zone] name.
+    :param str visibility: A template category filter (default: `public`); among: - `public` - official Exoscale templates - `private` - custom templates private to my organization
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,17 @@
                  operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a IAMAccessKey resource.
         :param pulumi.Input[str] name: The IAM access key name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
+               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+               restrict the key to (`<domain>/<type>:<name>`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if operations is not None:
             pulumi.set(__self__, "operations", operations)
         if resources is not None:
@@ -58,15 +60,17 @@
     def operations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "operations", value)
 
     @property
     @pulumi.getter
     def resources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
+        A list of API
+        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+        restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "resources", value)
 
@@ -94,16 +98,18 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags_operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering IAMAccessKey resources.
         :param pulumi.Input[str] key: The IAM access key (identifier).
         :param pulumi.Input[str] name: The IAM access key name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
-        :param pulumi.Input[str] secret: (Sensitive) The key secret.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
+               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+               restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[str] secret: The key secret.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if operations is not None:
@@ -153,27 +159,29 @@
     def operations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "operations", value)
 
     @property
     @pulumi.getter
     def resources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
+        A list of API
+        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+        restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "resources", value)
 
     @property
     @pulumi.getter
     def secret(self) -> Optional[pulumi.Input[str]]:
         """
-        (Sensitive) The key secret.
+        The key secret.
         """
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
@@ -211,15 +219,17 @@
                  __props__=None):
         """
         Create a IAMAccessKey resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The IAM access key name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
+               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+               restrict the key to (`<domain>/<type>:<name>`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[IAMAccessKeyArgs] = None,
@@ -286,16 +296,18 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: The IAM access key (identifier).
         :param pulumi.Input[str] name: The IAM access key name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
-        :param pulumi.Input[str] secret: (Sensitive) The key secret.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
+               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+               restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[str] secret: The key secret.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IAMAccessKeyState.__new__(_IAMAccessKeyState)
 
         __props__.__dict__["key"] = key
@@ -331,23 +343,25 @@
         """
         return pulumi.get(self, "operations")
 
     @property
     @pulumi.getter
     def resources(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of API [resources][iam-resource] to restrict the key to (`<domain>/<type>:<name>`).
+        A list of API
+        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
+        restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[str]:
         """
-        (Sensitive) The key secret.
+        The key secret.
         """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,159 +4,134 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
-from ._inputs import *
 
-__all__ = ['InstancePoolArgs', 'InstancePool']
+__all__ = ['SKSNodepoolArgs', 'SKSNodepool']
 
 @pulumi.input_type
-class InstancePoolArgs:
+class SKSNodepoolArgs:
     def __init__(__self__, *,
+                 cluster_id: pulumi.Input[str],
+                 instance_type: pulumi.Input[str],
                  size: pulumi.Input[int],
-                 template_id: pulumi.Input[str],
                  zone: pulumi.Input[str],
-                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
-                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
-                 instance_type: Optional[pulumi.Input[str]] = None,
-                 instances: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]] = None,
-                 ipv6: Optional[pulumi.Input[bool]] = None,
-                 key_pair: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 service_offering: Optional[pulumi.Input[str]] = None,
-                 state: Optional[pulumi.Input[str]] = None,
-                 user_data: Optional[pulumi.Input[str]] = None,
-                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a InstancePool resource.
-        :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the managed instances.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        The set of arguments for constructing a SKSNodepool resource.
+        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
-        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs).
-        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
-        :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
-        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The SSHKey (name) to authorize in the managed instances.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of PrivateNetwork (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs).
-        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        :param pulumi.Input[str] name: The SKS node pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+               (`<value>:<effect>`).
         """
+        pulumi.set(__self__, "cluster_id", cluster_id)
+        pulumi.set(__self__, "instance_type", instance_type)
         pulumi.set(__self__, "size", size)
-        pulumi.set(__self__, "template_id", template_id)
         pulumi.set(__self__, "zone", zone)
-        if affinity_group_ids is not None:
-            pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
+        if anti_affinity_group_ids is not None:
+            pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
-        if elastic_ip_ids is not None:
-            pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
         if instance_prefix is not None:
             pulumi.set(__self__, "instance_prefix", instance_prefix)
-        if instance_type is not None:
-            pulumi.set(__self__, "instance_type", instance_type)
-        if instances is not None:
-            pulumi.set(__self__, "instances", instances)
-        if ipv6 is not None:
-            pulumi.set(__self__, "ipv6", ipv6)
-        if key_pair is not None:
-            pulumi.set(__self__, "key_pair", key_pair)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if network_ids is not None:
-            pulumi.set(__self__, "network_ids", network_ids)
+        if private_network_ids is not None:
+            pulumi.set(__self__, "private_network_ids", private_network_ids)
         if security_group_ids is not None:
             pulumi.set(__self__, "security_group_ids", security_group_ids)
-        if service_offering is not None:
-            warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
-            pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
-        if service_offering is not None:
-            pulumi.set(__self__, "service_offering", service_offering)
-        if state is not None:
-            pulumi.set(__self__, "state", state)
-        if user_data is not None:
-            pulumi.set(__self__, "user_data", user_data)
-        if virtual_machines is not None:
-            warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
-            pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
-        if virtual_machines is not None:
-            pulumi.set(__self__, "virtual_machines", virtual_machines)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
 
     @property
-    @pulumi.getter
-    def size(self) -> pulumi.Input[int]:
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Input[str]:
         """
-        The number of managed instances.
+        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
         """
-        return pulumi.get(self, "size")
+        return pulumi.get(self, "cluster_id")
 
-    @size.setter
-    def size(self, value: pulumi.Input[int]):
-        pulumi.set(self, "size", value)
+    @cluster_id.setter
+    def cluster_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_id", value)
 
     @property
-    @pulumi.getter(name="templateId")
-    def template_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> pulumi.Input[str]:
         """
-        The_get_compute_template_(ID) to use when creating the managed instances.
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
-        return pulumi.get(self, "template_id")
+        return pulumi.get(self, "instance_type")
 
-    @template_id.setter
-    def template_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "template_id", value)
+    @instance_type.setter
+    def instance_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "instance_type", value)
+
+    @property
+    @pulumi.getter
+    def size(self) -> pulumi.Input[int]:
+        return pulumi.get(self, "size")
+
+    @size.setter
+    def size(self, value: pulumi.Input[int]):
+        pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
-    @pulumi.getter(name="affinityGroupIds")
-    def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="antiAffinityGroupIds")
+    def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
         """
-        return pulumi.get(self, "affinity_group_ids")
+        return pulumi.get(self, "anti_affinity_group_ids")
 
-    @affinity_group_ids.setter
-    def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "affinity_group_ids", value)
+    @anti_affinity_group_ids.setter
+    def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "anti_affinity_group_ids", value)
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
         A deploy target ID.
         """
@@ -178,95 +153,35 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[int]]:
         """
-        The managed instances disk size (GiB).
+        The managed instances disk size (GiB; default: `50`).
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
-    @pulumi.getter(name="elasticIpIds")
-    def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of ElasticIP (IDs).
-        """
-        return pulumi.get(self, "elastic_ip_ids")
-
-    @elastic_ip_ids.setter
-    def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "elastic_ip_ids", value)
-
-    @property
     @pulumi.getter(name="instancePrefix")
     def instance_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        The string used to prefix managed instances name (default: `pool`).
+        The string used to prefix the managed instances name (default `pool`).
         """
         return pulumi.get(self, "instance_prefix")
 
     @instance_prefix.setter
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
-    @pulumi.getter(name="instanceType")
-    def instance_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
-        """
-        return pulumi.get(self, "instance_type")
-
-    @instance_type.setter
-    def instance_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "instance_type", value)
-
-    @property
-    @pulumi.getter
-    def instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]:
-        """
-        The list of managed instances. Structure is documented below.
-        """
-        return pulumi.get(self, "instances")
-
-    @instances.setter
-    def instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]):
-        pulumi.set(self, "instances", value)
-
-    @property
-    @pulumi.getter
-    def ipv6(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable IPv6 on managed instances (boolean; default: `false`).
-        """
-        return pulumi.get(self, "ipv6")
-
-    @ipv6.setter
-    def ipv6(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ipv6", value)
-
-    @property
-    @pulumi.getter(name="keyPair")
-    def key_pair(self) -> Optional[pulumi.Input[str]]:
-        """
-        The SSHKey (name) to authorize in the managed instances.
-        """
-        return pulumi.get(self, "key_pair")
-
-    @key_pair.setter
-    def key_pair(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key_pair", value)
-
-    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -274,199 +189,179 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance pool name.
+        The SKS node pool name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="networkIds")
-    def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="privateNetworkIds")
+    def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of PrivateNetwork (IDs).
+        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
         """
-        return pulumi.get(self, "network_ids")
+        return pulumi.get(self, "private_network_ids")
 
-    @network_ids.setter
-    def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "network_ids", value)
+    @private_network_ids.setter
+    def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "private_network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of SecurityGroup (IDs).
+        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
-    @pulumi.getter(name="serviceOffering")
-    def service_offering(self) -> Optional[pulumi.Input[str]]:
-        """
-        The managed instances type. Please use the `instance_type` argument instead.
-        """
-        return pulumi.get(self, "service_offering")
-
-    @service_offering.setter
-    def service_offering(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "service_offering", value)
-
-    @property
     @pulumi.getter
-    def state(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "state")
-
-    @state.setter
-    def state(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "state", value)
-
-    @property
-    @pulumi.getter(name="userData")
-    def user_data(self) -> Optional[pulumi.Input[str]]:
+    def taints(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+        (`<value>:<effect>`).
         """
-        return pulumi.get(self, "user_data")
+        return pulumi.get(self, "taints")
 
-    @user_data.setter
-    def user_data(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_data", value)
-
-    @property
-    @pulumi.getter(name="virtualMachines")
-    def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        """
-        return pulumi.get(self, "virtual_machines")
-
-    @virtual_machines.setter
-    def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "virtual_machines", value)
+    @taints.setter
+    def taints(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "taints", value)
 
 
 @pulumi.input_type
-class _InstancePoolState:
+class _SKSNodepoolState:
     def __init__(__self__, *,
-                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
+                 created_at: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
-                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 instance_pool_id: Optional[pulumi.Input[str]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
-                 instances: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]] = None,
-                 ipv6: Optional[pulumi.Input[bool]] = None,
-                 key_pair: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 service_offering: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  state: Optional[pulumi.Input[str]] = None,
+                 taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
-                 user_data: Optional[pulumi.Input[str]] = None,
-                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering InstancePool resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        Input properties used for looking up and filtering SKSNodepool resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
-        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs).
-        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
-        :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
-        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The SSHKey (name) to authorize in the managed instances.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
+        :param pulumi.Input[str] instance_pool_id: The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of PrivateNetwork (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs).
-        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
-        :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
-        """
-        if affinity_group_ids is not None:
-            pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
+        :param pulumi.Input[str] name: The SKS node pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] state: The current pool state.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+               (`<value>:<effect>`).
+        :param pulumi.Input[str] template_id: The managed instances template ID.
+        :param pulumi.Input[str] version: The managed instances version.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        if anti_affinity_group_ids is not None:
+            pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
-        if elastic_ip_ids is not None:
-            pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
+        if instance_pool_id is not None:
+            pulumi.set(__self__, "instance_pool_id", instance_pool_id)
         if instance_prefix is not None:
             pulumi.set(__self__, "instance_prefix", instance_prefix)
         if instance_type is not None:
             pulumi.set(__self__, "instance_type", instance_type)
-        if instances is not None:
-            pulumi.set(__self__, "instances", instances)
-        if ipv6 is not None:
-            pulumi.set(__self__, "ipv6", ipv6)
-        if key_pair is not None:
-            pulumi.set(__self__, "key_pair", key_pair)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if network_ids is not None:
-            pulumi.set(__self__, "network_ids", network_ids)
+        if private_network_ids is not None:
+            pulumi.set(__self__, "private_network_ids", private_network_ids)
         if security_group_ids is not None:
             pulumi.set(__self__, "security_group_ids", security_group_ids)
-        if service_offering is not None:
-            warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
-            pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
-        if service_offering is not None:
-            pulumi.set(__self__, "service_offering", service_offering)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if state is not None:
             pulumi.set(__self__, "state", state)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
         if template_id is not None:
             pulumi.set(__self__, "template_id", template_id)
-        if user_data is not None:
-            pulumi.set(__self__, "user_data", user_data)
-        if virtual_machines is not None:
-            warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
-            pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
-        if virtual_machines is not None:
-            pulumi.set(__self__, "virtual_machines", virtual_machines)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="affinityGroupIds")
-    def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="antiAffinityGroupIds")
+    def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        """
+        return pulumi.get(self, "anti_affinity_group_ids")
+
+    @anti_affinity_group_ids.setter
+    def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "anti_affinity_group_ids", value)
+
+    @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
         """
-        return pulumi.get(self, "affinity_group_ids")
+        return pulumi.get(self, "cluster_id")
 
-    @affinity_group_ids.setter
-    def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "affinity_group_ids", value)
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The pool creation date.
+        """
+        return pulumi.get(self, "created_at")
+
+    @created_at.setter
+    def created_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
         A deploy target ID.
         """
@@ -488,477 +383,418 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[int]]:
         """
-        The managed instances disk size (GiB).
+        The managed instances disk size (GiB; default: `50`).
         """
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
-    @pulumi.getter(name="elasticIpIds")
-    def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="instancePoolId")
+    def instance_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of ElasticIP (IDs).
+        The underlying [exoscale_instance_pool](./instance_pool.md) ID.
         """
-        return pulumi.get(self, "elastic_ip_ids")
+        return pulumi.get(self, "instance_pool_id")
 
-    @elastic_ip_ids.setter
-    def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "elastic_ip_ids", value)
+    @instance_pool_id.setter
+    def instance_pool_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "instance_pool_id", value)
 
     @property
     @pulumi.getter(name="instancePrefix")
     def instance_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        The string used to prefix managed instances name (default: `pool`).
+        The string used to prefix the managed instances name (default `pool`).
         """
         return pulumi.get(self, "instance_prefix")
 
     @instance_prefix.setter
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
     @property
     @pulumi.getter
-    def instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]:
-        """
-        The list of managed instances. Structure is documented below.
-        """
-        return pulumi.get(self, "instances")
-
-    @instances.setter
-    def instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]]]):
-        pulumi.set(self, "instances", value)
-
-    @property
-    @pulumi.getter
-    def ipv6(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable IPv6 on managed instances (boolean; default: `false`).
-        """
-        return pulumi.get(self, "ipv6")
-
-    @ipv6.setter
-    def ipv6(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ipv6", value)
-
-    @property
-    @pulumi.getter(name="keyPair")
-    def key_pair(self) -> Optional[pulumi.Input[str]]:
-        """
-        The SSHKey (name) to authorize in the managed instances.
-        """
-        return pulumi.get(self, "key_pair")
-
-    @key_pair.setter
-    def key_pair(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key_pair", value)
-
-    @property
-    @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance pool name.
+        The SKS node pool name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="networkIds")
-    def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="privateNetworkIds")
+    def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of PrivateNetwork (IDs).
+        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
         """
-        return pulumi.get(self, "network_ids")
+        return pulumi.get(self, "private_network_ids")
 
-    @network_ids.setter
-    def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "network_ids", value)
+    @private_network_ids.setter
+    def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "private_network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of SecurityGroup (IDs).
+        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
-    @pulumi.getter(name="serviceOffering")
-    def service_offering(self) -> Optional[pulumi.Input[str]]:
-        """
-        The managed instances type. Please use the `instance_type` argument instead.
-        """
-        return pulumi.get(self, "service_offering")
-
-    @service_offering.setter
-    def service_offering(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "service_offering", value)
-
-    @property
     @pulumi.getter
     def size(self) -> Optional[pulumi.Input[int]]:
-        """
-        The number of managed instances.
-        """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
+        """
+        The current pool state.
+        """
         return pulumi.get(self, "state")
 
     @state.setter
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
+    @pulumi.getter
+    def taints(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+        (`<value>:<effect>`).
+        """
+        return pulumi.get(self, "taints")
+
+    @taints.setter
+    def taints(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "taints", value)
+
+    @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The_get_compute_template_(ID) to use when creating the managed instances.
+        The managed instances template ID.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
     @property
-    @pulumi.getter(name="userData")
-    def user_data(self) -> Optional[pulumi.Input[str]]:
-        """
-        [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
-        """
-        return pulumi.get(self, "user_data")
-
-    @user_data.setter
-    def user_data(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_data", value)
-
-    @property
-    @pulumi.getter(name="virtualMachines")
-    def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[str]]:
         """
-        (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        The managed instances version.
         """
-        return pulumi.get(self, "virtual_machines")
+        return pulumi.get(self, "version")
 
-    @virtual_machines.setter
-    def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "virtual_machines", value)
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
 
-class InstancePool(pulumi.CustomResource):
+class SKSNodepool(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
-                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
-                 instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
-                 ipv6: Optional[pulumi.Input[bool]] = None,
-                 key_pair: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 service_offering: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
-                 state: Optional[pulumi.Input[str]] = None,
-                 template_id: Optional[pulumi.Input[str]] = None,
-                 user_data: Optional[pulumi.Input[str]] = None,
-                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing instance pool may be imported by `<ID>@<zone>`console
+        An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`
 
         ```sh
-         $ pulumi import exoscale:index/instancePool:InstancePool \\
+         $ pulumi import exoscale:index/sKSNodepool:SKSNodepool \\
         ```
 
-         exoscale_instance_pool.my_instance_pool \\
+         exoscale_sks_nodepool.my_sks_nodepool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
-        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs).
-        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
-        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The SSHKey (name) to authorize in the managed instances.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
+        :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of PrivateNetwork (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs).
-        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
-        :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] name: The SKS node pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+               (`<value>:<effect>`).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: InstancePoolArgs,
+                 args: SKSNodepoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing instance pool may be imported by `<ID>@<zone>`console
+        An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`
 
         ```sh
-         $ pulumi import exoscale:index/instancePool:InstancePool \\
+         $ pulumi import exoscale:index/sKSNodepool:SKSNodepool \\
         ```
 
-         exoscale_instance_pool.my_instance_pool \\
+         exoscale_sks_nodepool.my_sks_nodepool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
-        :param InstancePoolArgs args: The arguments to use to populate this resource's properties.
+        :param SKSNodepoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(InstancePoolArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SKSNodepoolArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
-                 elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
-                 instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
-                 ipv6: Optional[pulumi.Input[bool]] = None,
-                 key_pair: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 service_offering: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
-                 state: Optional[pulumi.Input[str]] = None,
-                 template_id: Optional[pulumi.Input[str]] = None,
-                 user_data: Optional[pulumi.Input[str]] = None,
-                 virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = InstancePoolArgs.__new__(InstancePoolArgs)
+            __props__ = SKSNodepoolArgs.__new__(SKSNodepoolArgs)
 
-            __props__.__dict__["affinity_group_ids"] = affinity_group_ids
+            __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
+            if cluster_id is None and not opts.urn:
+                raise TypeError("Missing required property 'cluster_id'")
+            __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["deploy_target_id"] = deploy_target_id
             __props__.__dict__["description"] = description
             __props__.__dict__["disk_size"] = disk_size
-            __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
             __props__.__dict__["instance_prefix"] = instance_prefix
+            if instance_type is None and not opts.urn:
+                raise TypeError("Missing required property 'instance_type'")
             __props__.__dict__["instance_type"] = instance_type
-            __props__.__dict__["instances"] = instances
-            __props__.__dict__["ipv6"] = ipv6
-            __props__.__dict__["key_pair"] = key_pair
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
-            __props__.__dict__["network_ids"] = network_ids
+            __props__.__dict__["private_network_ids"] = private_network_ids
             __props__.__dict__["security_group_ids"] = security_group_ids
-            if service_offering is not None and not opts.urn:
-                warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
-                pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
-            __props__.__dict__["service_offering"] = service_offering
             if size is None and not opts.urn:
                 raise TypeError("Missing required property 'size'")
             __props__.__dict__["size"] = size
-            __props__.__dict__["state"] = state
-            if template_id is None and not opts.urn:
-                raise TypeError("Missing required property 'template_id'")
-            __props__.__dict__["template_id"] = template_id
-            __props__.__dict__["user_data"] = user_data
-            if virtual_machines is not None and not opts.urn:
-                warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
-                pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
-            __props__.__dict__["virtual_machines"] = virtual_machines
+            __props__.__dict__["taints"] = taints
             if zone is None and not opts.urn:
                 raise TypeError("Missing required property 'zone'")
             __props__.__dict__["zone"] = zone
-        super(InstancePool, __self__).__init__(
-            'exoscale:index/instancePool:InstancePool',
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["instance_pool_id"] = None
+            __props__.__dict__["state"] = None
+            __props__.__dict__["template_id"] = None
+            __props__.__dict__["version"] = None
+        super(SKSNodepool, __self__).__init__(
+            'exoscale:index/sKSNodepool:SKSNodepool',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            cluster_id: Optional[pulumi.Input[str]] = None,
+            created_at: Optional[pulumi.Input[str]] = None,
             deploy_target_id: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             disk_size: Optional[pulumi.Input[int]] = None,
-            elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            instance_pool_id: Optional[pulumi.Input[str]] = None,
             instance_prefix: Optional[pulumi.Input[str]] = None,
             instance_type: Optional[pulumi.Input[str]] = None,
-            instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]]] = None,
-            ipv6: Optional[pulumi.Input[bool]] = None,
-            key_pair: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            service_offering: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[int]] = None,
             state: Optional[pulumi.Input[str]] = None,
+            taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             template_id: Optional[pulumi.Input[str]] = None,
-            user_data: Optional[pulumi.Input[str]] = None,
-            virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            zone: Optional[pulumi.Input[str]] = None) -> 'InstancePool':
+            version: Optional[pulumi.Input[str]] = None,
+            zone: Optional[pulumi.Input[str]] = None) -> 'SKSNodepool':
         """
-        Get an existing InstancePool resource's state with the given name, id, and optional extra
+        Get an existing SKSNodepool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
-        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of ElasticIP (IDs).
-        :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
-        :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The SSHKey (name) to authorize in the managed instances.
+        :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
+        :param pulumi.Input[str] instance_pool_id: The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of PrivateNetwork (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of SecurityGroup (IDs).
-        :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
-        :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The_get_compute_template_(ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] name: The SKS node pool name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] state: The current pool state.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+               (`<value>:<effect>`).
+        :param pulumi.Input[str] template_id: The managed instances template ID.
+        :param pulumi.Input[str] version: The managed instances version.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _InstancePoolState.__new__(_InstancePoolState)
+        __props__ = _SKSNodepoolState.__new__(_SKSNodepoolState)
 
-        __props__.__dict__["affinity_group_ids"] = affinity_group_ids
+        __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
+        __props__.__dict__["cluster_id"] = cluster_id
+        __props__.__dict__["created_at"] = created_at
         __props__.__dict__["deploy_target_id"] = deploy_target_id
         __props__.__dict__["description"] = description
         __props__.__dict__["disk_size"] = disk_size
-        __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
+        __props__.__dict__["instance_pool_id"] = instance_pool_id
         __props__.__dict__["instance_prefix"] = instance_prefix
         __props__.__dict__["instance_type"] = instance_type
-        __props__.__dict__["instances"] = instances
-        __props__.__dict__["ipv6"] = ipv6
-        __props__.__dict__["key_pair"] = key_pair
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
-        __props__.__dict__["network_ids"] = network_ids
+        __props__.__dict__["private_network_ids"] = private_network_ids
         __props__.__dict__["security_group_ids"] = security_group_ids
-        __props__.__dict__["service_offering"] = service_offering
         __props__.__dict__["size"] = size
         __props__.__dict__["state"] = state
+        __props__.__dict__["taints"] = taints
         __props__.__dict__["template_id"] = template_id
-        __props__.__dict__["user_data"] = user_data
-        __props__.__dict__["virtual_machines"] = virtual_machines
+        __props__.__dict__["version"] = version
         __props__.__dict__["zone"] = zone
-        return InstancePool(resource_name, opts=opts, __props__=__props__)
+        return SKSNodepool(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="affinityGroupIds")
-    def affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="antiAffinityGroupIds")
+    def anti_affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of AntiAffinityGroup (IDs; may only be set at creation time).
+        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
         """
-        return pulumi.get(self, "affinity_group_ids")
+        return pulumi.get(self, "anti_affinity_group_ids")
+
+    @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> pulumi.Output[str]:
+        """
+        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        """
+        return pulumi.get(self, "cluster_id")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[str]:
+        """
+        The pool creation date.
+        """
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> pulumi.Output[Optional[str]]:
         """
         A deploy target ID.
         """
@@ -970,146 +806,116 @@
         """
         A free-form text describing the pool.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="diskSize")
-    def disk_size(self) -> pulumi.Output[int]:
+    def disk_size(self) -> pulumi.Output[Optional[int]]:
         """
-        The managed instances disk size (GiB).
+        The managed instances disk size (GiB; default: `50`).
         """
         return pulumi.get(self, "disk_size")
 
     @property
-    @pulumi.getter(name="elasticIpIds")
-    def elastic_ip_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="instancePoolId")
+    def instance_pool_id(self) -> pulumi.Output[str]:
         """
-        A list of ElasticIP (IDs).
+        The underlying [exoscale_instance_pool](./instance_pool.md) ID.
         """
-        return pulumi.get(self, "elastic_ip_ids")
+        return pulumi.get(self, "instance_pool_id")
 
     @property
     @pulumi.getter(name="instancePrefix")
     def instance_prefix(self) -> pulumi.Output[Optional[str]]:
         """
-        The string used to prefix managed instances name (default: `pool`).
+        The string used to prefix the managed instances name (default `pool`).
         """
         return pulumi.get(self, "instance_prefix")
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> pulumi.Output[str]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI][cli] - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
+        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
     @pulumi.getter
-    def instances(self) -> pulumi.Output[Sequence['outputs.InstancePoolInstance']]:
-        """
-        The list of managed instances. Structure is documented below.
-        """
-        return pulumi.get(self, "instances")
-
-    @property
-    @pulumi.getter
-    def ipv6(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Enable IPv6 on managed instances (boolean; default: `false`).
-        """
-        return pulumi.get(self, "ipv6")
-
-    @property
-    @pulumi.getter(name="keyPair")
-    def key_pair(self) -> pulumi.Output[Optional[str]]:
-        """
-        The SSHKey (name) to authorize in the managed instances.
-        """
-        return pulumi.get(self, "key_pair")
-
-    @property
-    @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The instance pool name.
+        The SKS node pool name.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="networkIds")
-    def network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="privateNetworkIds")
+    def private_network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of PrivateNetwork (IDs).
+        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
         """
-        return pulumi.get(self, "network_ids")
+        return pulumi.get(self, "private_network_ids")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of SecurityGroup (IDs).
+        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
-    @pulumi.getter(name="serviceOffering")
-    def service_offering(self) -> pulumi.Output[str]:
-        """
-        The managed instances type. Please use the `instance_type` argument instead.
-        """
-        return pulumi.get(self, "service_offering")
-
-    @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
-        """
-        The number of managed instances.
-        """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
+        """
+        The current pool state.
+        """
         return pulumi.get(self, "state")
 
     @property
-    @pulumi.getter(name="templateId")
-    def template_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def taints(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        The_get_compute_template_(ID) to use when creating the managed instances.
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
+        (`<value>:<effect>`).
         """
-        return pulumi.get(self, "template_id")
+        return pulumi.get(self, "taints")
 
     @property
-    @pulumi.getter(name="userData")
-    def user_data(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="templateId")
+    def template_id(self) -> pulumi.Output[str]:
         """
-        [cloud-init][cloud-init] configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
+        The managed instances template ID.
         """
-        return pulumi.get(self, "user_data")
+        return pulumi.get(self, "template_id")
 
     @property
-    @pulumi.getter(name="virtualMachines")
-    def virtual_machines(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter
+    def version(self) -> pulumi.Output[str]:
         """
-        (Deprecated) The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
+        The managed instances version.
         """
-        return pulumi.get(self, "virtual_machines")
+        return pulumi.get(self, "version")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ip_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,20 @@
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
         :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthcheck_interval is not None:
             pulumi.set(__self__, "healthcheck_interval", healthcheck_interval)
         if healthcheck_mode is not None:
@@ -177,27 +179,29 @@
     def healthcheck_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_timeout", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @healthcheck_tls_skip_verify.setter
     def healthcheck_tls_skip_verify(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "healthcheck_tls_skip_verify", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @healthcheck_tls_sni.setter
     def healthcheck_tls_sni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_tls_sni", value)
 
@@ -213,15 +217,15 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -249,19 +253,21 @@
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
         :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 address.
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthcheck_interval is not None:
             pulumi.set(__self__, "healthcheck_interval", healthcheck_interval)
         if healthcheck_mode is not None:
@@ -385,27 +391,29 @@
     def healthcheck_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_timeout", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @healthcheck_tls_skip_verify.setter
     def healthcheck_tls_skip_verify(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "healthcheck_tls_skip_verify", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @healthcheck_tls_sni.setter
     def healthcheck_tls_sni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_tls_sni", value)
 
@@ -433,15 +441,15 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -486,18 +494,20 @@
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
         :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IPAddressArgs,
@@ -593,19 +603,21 @@
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
         :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 address.
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IPAddressState.__new__(_IPAddressState)
 
         __props__.__dict__["description"] = description
@@ -688,23 +700,25 @@
         """
         return pulumi.get(self, "healthcheck_timeout")
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> pulumi.Output[Optional[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
+        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> pulumi.Output[Optional[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
+        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
@@ -720,15 +734,15 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        A dictionary of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,20 @@
                  network_offering: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Network resource.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
-        :param pulumi.Input[str] start_ip: /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+               private networks.
+        :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         pulumi.set(__self__, "zone", zone)
         if display_text is not None:
             pulumi.set(__self__, "display_text", display_text)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
@@ -73,14 +75,17 @@
     @display_text.setter
     def display_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_text", value)
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        """
         return pulumi.get(self, "end_ip")
 
     @end_ip.setter
     def end_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_ip", value)
 
     @property
@@ -95,15 +100,16 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
+        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+        private networks.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
@@ -116,27 +122,27 @@
     def network_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_offering", value)
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         """
         return pulumi.get(self, "start_ip")
 
     @start_ip.setter
     def start_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_ip", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -151,18 +157,20 @@
                  network_offering: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Network resources.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
-        :param pulumi.Input[str] start_ip: /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+               private networks.
+        :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         if display_text is not None:
             pulumi.set(__self__, "display_text", display_text)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
@@ -192,14 +200,17 @@
     @display_text.setter
     def display_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_text", value)
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        """
         return pulumi.get(self, "end_ip")
 
     @end_ip.setter
     def end_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_ip", value)
 
     @property
@@ -214,15 +225,16 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
+        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+        private networks.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
@@ -235,27 +247,27 @@
     def network_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_offering", value)
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         """
         return pulumi.get(self, "start_ip")
 
     @start_ip.setter
     def start_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_ip", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -288,18 +300,20 @@
                  __props__=None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use PrivateNetwork instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
-        :param pulumi.Input[str] start_ip: /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+               private networks.
+        :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NetworkArgs,
@@ -374,18 +388,20 @@
         Get an existing Network resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
-        :param pulumi.Input[str] start_ip: /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags (key/value). To remove all tags, set `tags = {}`.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+               private networks.
+        :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         :param pulumi.Input[str] zone: The Exoscale Zone name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NetworkState.__new__(_NetworkState)
 
         __props__.__dict__["display_text"] = display_text
@@ -405,50 +421,54 @@
         A free-form text describing the network.
         """
         return pulumi.get(self, "display_text")
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> pulumi.Output[Optional[str]]:
+        """
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        """
         return pulumi.get(self, "end_ip")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The private network name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def netmask(self) -> pulumi.Output[Optional[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
+        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
+        private networks.
         """
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="networkOffering")
     def network_offering(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "network_offering")
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> pulumi.Output[Optional[str]]:
         """
-        /`end_ip` - The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
+        The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         """
         return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        A map of tags (key/value). To remove all tags, set `tags = {}`.
+        Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(__self__, *,
                  zone: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NLB resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -33,15 +33,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -96,17 +96,17 @@
         """
         Input properties used for looking up and filtering NLB resources.
         :param pulumi.Input[str] created_at: The NLB creation date.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[str] ip_address: The NLB IPv4 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the NLBService (names).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the [exoscale_nlb_service](./nlb_service.md) (names).
         :param pulumi.Input[str] state: The current NLB state.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
@@ -181,15 +181,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of the NLBService (names).
+        The list of the [exoscale_nlb_service](./nlb_service.md) (names).
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -205,15 +205,15 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -242,15 +242,15 @@
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NLBArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -331,17 +331,17 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The NLB creation date.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[str] ip_address: The NLB IPv4 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the NLBService (names).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the [exoscale_nlb_service](./nlb_service.md) (names).
         :param pulumi.Input[str] state: The current NLB state.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NLBState.__new__(_NLBState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
@@ -393,15 +393,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Sequence[str]]:
         """
-        The list of the NLBService (names).
+        The list of the [exoscale_nlb_service](./nlb_service.md) (names).
         """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -409,11 +409,11 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,20 @@
                  zone: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  strategy: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NLBService resource.
-        :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time). Structure is documented below.
-        :param pulumi.Input[str] instance_pool_id: The InstancePool (ID) to forward traffic to.
-        :param pulumi.Input[str] nlb_id: The parent NLB ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UPP) port.
+        :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time).
+        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         """
         pulumi.set(__self__, "healthchecks", healthchecks)
         pulumi.set(__self__, "instance_pool_id", instance_pool_id)
@@ -54,51 +54,51 @@
         if strategy is not None:
             pulumi.set(__self__, "strategy", strategy)
 
     @property
     @pulumi.getter
     def healthchecks(self) -> pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]:
         """
-        The service health checking configuration (may only bet set at creation time). Structure is documented below.
+        The service health checking configuration (may only bet set at creation time).
         """
         return pulumi.get(self, "healthchecks")
 
     @healthchecks.setter
     def healthchecks(self, value: pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> pulumi.Input[str]:
         """
-        The InstancePool (ID) to forward traffic to.
+        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @instance_pool_id.setter
     def instance_pool_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "instance_pool_id", value)
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> pulumi.Input[str]:
         """
-        The parent NLB ID.
+        The parent [exoscale_nlb](./nlb.md) ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @nlb_id.setter
     def nlb_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "nlb_id", value)
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Input[int]:
         """
-        The NLB service (TCP/UPP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: pulumi.Input[int]):
         pulumi.set(self, "port", value)
 
@@ -114,15 +114,15 @@
     def target_port(self, value: pulumi.Input[int]):
         pulumi.set(self, "target_port", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -188,23 +188,23 @@
                  state: Optional[pulumi.Input[str]] = None,
                  strategy: Optional[pulumi.Input[str]] = None,
                  target_port: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering NLBService resources.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
-        :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time). Structure is documented below.
-        :param pulumi.Input[str] instance_pool_id: The InstancePool (ID) to forward traffic to.
+        :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time).
+        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent NLB ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UPP) port.
+        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthchecks is not None:
             pulumi.set(__self__, "healthchecks", healthchecks)
         if instance_pool_id is not None:
             pulumi.set(__self__, "instance_pool_id", instance_pool_id)
@@ -237,27 +237,27 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def healthchecks(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]]:
         """
-        The service health checking configuration (may only bet set at creation time). Structure is documented below.
+        The service health checking configuration (may only bet set at creation time).
         """
         return pulumi.get(self, "healthchecks")
 
     @healthchecks.setter
     def healthchecks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The InstancePool (ID) to forward traffic to.
+        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @instance_pool_id.setter
     def instance_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_pool_id", value)
 
@@ -273,27 +273,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent NLB ID.
+        The parent [exoscale_nlb](./nlb.md) ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @nlb_id.setter
     def nlb_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nlb_id", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        The NLB service (TCP/UPP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -342,15 +342,15 @@
     def target_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "target_port", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -370,47 +370,47 @@
                  strategy: Optional[pulumi.Input[str]] = None,
                  target_port: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`console
+        An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/nLBService:NLBService \\
         ```
 
          exoscale_nlb_service.my_nlb_service \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time). Structure is documented below.
-        :param pulumi.Input[str] instance_pool_id: The InstancePool (ID) to forward traffic to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time).
+        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent NLB ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UPP) port.
+        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NLBServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`console
+        An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/nLBService:NLBService \\
         ```
 
          exoscale_nlb_service.my_nlb_service \\
 
@@ -498,23 +498,23 @@
         Get an existing NLBService resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time). Structure is documented below.
-        :param pulumi.Input[str] instance_pool_id: The InstancePool (ID) to forward traffic to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time).
+        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent NLB ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UPP) port.
+        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NLBServiceState.__new__(_NLBServiceState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["healthchecks"] = healthchecks
@@ -537,23 +537,23 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def healthchecks(self) -> pulumi.Output[Sequence['outputs.NLBServiceHealthcheck']]:
         """
-        The service health checking configuration (may only bet set at creation time). Structure is documented below.
+        The service health checking configuration (may only bet set at creation time).
         """
         return pulumi.get(self, "healthchecks")
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> pulumi.Output[str]:
         """
-        The InstancePool (ID) to forward traffic to.
+        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -561,23 +561,23 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> pulumi.Output[str]:
         """
-        The parent NLB ID.
+        The parent [exoscale_nlb](./nlb.md) ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[int]:
         """
-        The NLB service (TCP/UPP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def protocol(self) -> pulumi.Output[Optional[str]]:
         """
@@ -606,11 +606,11 @@
         """
         return pulumi.get(self, "target_port")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/private_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,20 @@
                  description: Optional[pulumi.Input[str]] = None,
                  end_ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  netmask: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PrivateNetwork resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
@@ -40,15 +41,15 @@
         if start_ip is not None:
             pulumi.set(__self__, "start_ip", start_ip)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -63,14 +64,17 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
         return pulumi.get(self, "end_ip")
 
     @end_ip.setter
     def end_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_ip", value)
 
     @property
@@ -85,27 +89,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IPv4 network allowed for static leases.
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         return pulumi.get(self, "start_ip")
 
     @start_ip.setter
     def start_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_ip", value)
 
@@ -118,18 +122,19 @@
                  name: Optional[pulumi.Input[str]] = None,
                  netmask: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PrivateNetwork resources.
         :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -151,14 +156,17 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
         return pulumi.get(self, "end_ip")
 
     @end_ip.setter
     def end_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_ip", value)
 
     @property
@@ -173,39 +181,39 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IPv4 network allowed for static leases.
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         return pulumi.get(self, "start_ip")
 
     @start_ip.setter
     def start_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_ip", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -221,42 +229,43 @@
                  netmask: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing private network may be imported by `<ID>@<zone>`console
+        An existing private network may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
          exoscale_private_network.my_private_network \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PrivateNetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing private network may be imported by `<ID>@<zone>`console
+        An existing private network may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
          exoscale_private_network.my_private_network \\
 
@@ -320,18 +329,19 @@
         Get an existing PrivateNetwork resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PrivateNetworkState.__new__(_PrivateNetworkState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["end_ip"] = end_ip
@@ -348,41 +358,44 @@
         A free-form text describing the network.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endIp")
     def end_ip(self) -> pulumi.Output[Optional[str]]:
+        """
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
         return pulumi.get(self, "end_ip")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The private network name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def netmask(self) -> pulumi.Output[Optional[str]]:
         """
-        The network mask defining the IPv4 network allowed for static leases.
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         """
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> pulumi.Output[Optional[str]]:
         """
-        /`end_ip` - (Required) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroup resource.
         :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR][cidr] notation.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+               notation.
         :param pulumi.Input[str] name: The security group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if external_sources is not None:
             pulumi.set(__self__, "external_sources", external_sources)
         if name is not None:
@@ -42,15 +43,16 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of external network sources, in [CIDR][cidr] notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+        notation.
         """
         return pulumi.get(self, "external_sources")
 
     @external_sources.setter
     def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_sources", value)
 
@@ -72,15 +74,16 @@
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroup resources.
         :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR][cidr] notation.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+               notation.
         :param pulumi.Input[str] name: The security group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if external_sources is not None:
             pulumi.set(__self__, "external_sources", external_sources)
         if name is not None:
@@ -98,15 +101,16 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of external network sources, in [CIDR][cidr] notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+        notation.
         """
         return pulumi.get(self, "external_sources")
 
     @external_sources.setter
     def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_sources", value)
 
@@ -131,40 +135,41 @@
                  description: Optional[pulumi.Input[str]] = None,
                  external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing security group may be imported by `<ID>`console
+        An existing security group may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
         ```
 
          exoscale_security_group.my_security_group \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR][cidr] notation.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+               notation.
         :param pulumi.Input[str] name: The security group name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SecurityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing security group may be imported by `<ID>`console
+        An existing security group may be imported by `<ID>`
 
         ```sh
          $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
         ```
 
          exoscale_security_group.my_security_group \\
 
@@ -217,15 +222,16 @@
         Get an existing SecurityGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR][cidr] notation.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+               notation.
         :param pulumi.Input[str] name: The security group name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupState.__new__(_SecurityGroupState)
 
         __props__.__dict__["description"] = description
@@ -241,15 +247,16 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of external network sources, in [CIDR][cidr] notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
+        notation.
         """
         return pulumi.get(self, "external_sources")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,23 +25,31 @@
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroupRule resource.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+               `user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] security_group_id: The parent SecurityGroup ID.
-        :param pulumi.Input[int] start_port: /`end_port` - A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
+        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+               `cidr`/`user_security_group)`).
         """
         pulumi.set(__self__, "type", type)
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
@@ -49,20 +57,26 @@
         if icmp_code is not None:
             pulumi.set(__self__, "icmp_code", icmp_code)
         if icmp_type is not None:
             pulumi.set(__self__, "icmp_type", icmp_type)
         if protocol is not None:
             pulumi.set(__self__, "protocol", protocol)
         if security_group is not None:
+            warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+            pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
+        if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
         if start_port is not None:
             pulumi.set(__self__, "start_port", start_port)
         if user_security_group is not None:
+            warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+            pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
+        if user_security_group is not None:
             pulumi.set(__self__, "user_security_group", user_security_group)
         if user_security_group_id is not None:
             pulumi.set(__self__, "user_security_group_id", user_security_group_id)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
@@ -75,15 +89,17 @@
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+        `user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
@@ -98,34 +114,40 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> Optional[pulumi.Input[int]]:
+        """
+        A `TCP`/`UDP` port range to match.
+        """
         return pulumi.get(self, "end_port")
 
     @end_port.setter
     def end_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_port", value)
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> Optional[pulumi.Input[int]]:
+        """
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        """
         return pulumi.get(self, "icmp_code")
 
     @icmp_code.setter
     def icmp_code(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_code", value)
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> Optional[pulumi.Input[int]]:
         """
-        /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @icmp_type.setter
     def icmp_type(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_type", value)
 
@@ -141,63 +163,67 @@
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
+        The parent security group name. Please use the `security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent SecurityGroup ID.
+        The parent [exoscale_security_group](./security_group.md) ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> Optional[pulumi.Input[int]]:
         """
-        /`end_port` - A `TCP`/`UDP` port range to match.
+        A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @start_port.setter
     def start_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_port", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
+        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+        `cidr`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -215,55 +241,71 @@
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroupRule resources.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+               `user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] security_group_id: The parent SecurityGroup ID.
-        :param pulumi.Input[int] start_port: /`end_port` - A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
+        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+               `cidr`/`user_security_group)`).
         """
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
             pulumi.set(__self__, "end_port", end_port)
         if icmp_code is not None:
             pulumi.set(__self__, "icmp_code", icmp_code)
         if icmp_type is not None:
             pulumi.set(__self__, "icmp_type", icmp_type)
         if protocol is not None:
             pulumi.set(__self__, "protocol", protocol)
         if security_group is not None:
+            warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+            pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
+        if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
         if start_port is not None:
             pulumi.set(__self__, "start_port", start_port)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if user_security_group is not None:
+            warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+            pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
+        if user_security_group is not None:
             pulumi.set(__self__, "user_security_group", user_security_group)
         if user_security_group_id is not None:
             pulumi.set(__self__, "user_security_group_id", user_security_group_id)
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+        `user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
@@ -278,34 +320,40 @@
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> Optional[pulumi.Input[int]]:
+        """
+        A `TCP`/`UDP` port range to match.
+        """
         return pulumi.get(self, "end_port")
 
     @end_port.setter
     def end_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_port", value)
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> Optional[pulumi.Input[int]]:
+        """
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        """
         return pulumi.get(self, "icmp_code")
 
     @icmp_code.setter
     def icmp_code(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_code", value)
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> Optional[pulumi.Input[int]]:
         """
-        /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @icmp_type.setter
     def icmp_type(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_type", value)
 
@@ -321,39 +369,40 @@
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
+        The parent security group name. Please use the `security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent SecurityGroup ID.
+        The parent [exoscale_security_group](./security_group.md) ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> Optional[pulumi.Input[int]]:
         """
-        /`end_port` - A `TCP`/`UDP` port range to match.
+        A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @start_port.setter
     def start_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_port", value)
 
@@ -369,27 +418,30 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
+        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+        `cidr`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -409,85 +461,57 @@
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
-
-        ## Usage
-
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
-
-        my_security_group = exoscale.SecurityGroup("mySecurityGroup")
-        my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
-            security_group_id=my_security_group.id,
-            type="INGRESS",
-            protocol="TCP",
-            cidr="0.0.0.0/0",
-            start_port=80,
-            end_port=80)
-        ```
-
         ## Import
 
-        An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`console
+        An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`
 
         ```sh
          $ pulumi import exoscale:index/securityGroupRule:SecurityGroupRule \\
         ```
 
          exoscale_security_group_rule.my_security_group_rule \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+               `user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] security_group_id: The parent SecurityGroup ID.
-        :param pulumi.Input[int] start_port: /`end_port` - A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
+        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+               `cidr`/`user_security_group)`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SecurityGroupRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
-
-        ## Usage
-
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
-
-        my_security_group = exoscale.SecurityGroup("mySecurityGroup")
-        my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
-            security_group_id=my_security_group.id,
-            type="INGRESS",
-            protocol="TCP",
-            cidr="0.0.0.0/0",
-            start_port=80,
-            end_port=80)
-        ```
-
         ## Import
 
-        An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`console
+        An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`
 
         ```sh
          $ pulumi import exoscale:index/securityGroupRule:SecurityGroupRule \\
         ```
 
          exoscale_security_group_rule.my_security_group_rule \\
 
@@ -531,20 +555,26 @@
 
             __props__.__dict__["cidr"] = cidr
             __props__.__dict__["description"] = description
             __props__.__dict__["end_port"] = end_port
             __props__.__dict__["icmp_code"] = icmp_code
             __props__.__dict__["icmp_type"] = icmp_type
             __props__.__dict__["protocol"] = protocol
+            if security_group is not None and not opts.urn:
+                warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+                pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
             __props__.__dict__["security_group"] = security_group
             __props__.__dict__["security_group_id"] = security_group_id
             __props__.__dict__["start_port"] = start_port
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
+            if user_security_group is not None and not opts.urn:
+                warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+                pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
             __props__.__dict__["user_security_group"] = user_security_group
             __props__.__dict__["user_security_group_id"] = user_security_group_id
         super(SecurityGroupRule, __self__).__init__(
             'exoscale:index/securityGroupRule:SecurityGroupRule',
             resource_name,
             __props__,
             opts)
@@ -568,24 +598,32 @@
         """
         Get an existing SecurityGroupRule resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+               `user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] icmp_type: /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] security_group_id: The parent SecurityGroup ID.
-        :param pulumi.Input[int] start_port: /`end_port` - A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
+        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+               `cidr`/`user_security_group)`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupRuleState.__new__(_SecurityGroupRuleState)
 
         __props__.__dict__["cidr"] = cidr
         __props__.__dict__["description"] = description
@@ -601,41 +639,49 @@
         __props__.__dict__["user_security_group_id"] = user_security_group_id
         return SecurityGroupRule(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def cidr(self) -> pulumi.Output[Optional[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation][cidr]) to match (conflicts with `user_security_group`/`user_security_group_id`).
+        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
+        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
+        `user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         A free-form text describing the security group rule.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> pulumi.Output[Optional[int]]:
+        """
+        A `TCP`/`UDP` port range to match.
+        """
         return pulumi.get(self, "end_port")
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> pulumi.Output[Optional[int]]:
+        """
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        """
         return pulumi.get(self, "icmp_code")
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> pulumi.Output[Optional[int]]:
         """
-        /`icmp_code` - An ICMP/ICMPv6 [type/code][icmp] to match.
+        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @property
     @pulumi.getter
     def protocol(self) -> pulumi.Output[Optional[str]]:
         """
@@ -643,31 +689,32 @@
         """
         return pulumi.get(self, "protocol")
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> pulumi.Output[str]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the SecurityGroup data source instead.
+        The parent security group name. Please use the `security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> pulumi.Output[str]:
         """
-        The parent SecurityGroup ID.
+        The parent [exoscale_security_group](./security_group.md) ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> pulumi.Output[Optional[int]]:
         """
-        /`end_port` - A `TCP`/`UDP` port range to match.
+        A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
@@ -675,19 +722,22 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> pulumi.Output[str]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the SecurityGroup data source instead.
+        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
+        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> pulumi.Output[Optional[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`user_security_group)`).
+        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
+        `cidr`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     def __init__(__self__, *,
                  egresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]] = None,
                  ingresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroupRules resource.
-        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]] egresses: A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
         :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         if egresses is not None:
             pulumi.set(__self__, "egresses", egresses)
         if ingresses is not None:
             pulumi.set(__self__, "ingresses", ingresses)
@@ -34,25 +35,28 @@
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
 
     @property
     @pulumi.getter
     def egresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]]:
+        """
+        A security group rule definition (can be specified multiple times).
+        """
         return pulumi.get(self, "egresses")
 
     @egresses.setter
     def egresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]]):
         pulumi.set(self, "egresses", value)
 
     @property
     @pulumi.getter
     def ingresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]:
         """
-        /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        A security group rule definition (can be specified multiple times).
         """
         return pulumi.get(self, "ingresses")
 
     @ingresses.setter
     def ingresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]):
         pulumi.set(self, "ingresses", value)
 
@@ -86,15 +90,16 @@
     def __init__(__self__, *,
                  egresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]] = None,
                  ingresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroupRules resources.
-        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]] egresses: A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
         :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         if egresses is not None:
             pulumi.set(__self__, "egresses", egresses)
         if ingresses is not None:
             pulumi.set(__self__, "ingresses", ingresses)
@@ -102,25 +107,28 @@
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
 
     @property
     @pulumi.getter
     def egresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]]:
+        """
+        A security group rule definition (can be specified multiple times).
+        """
         return pulumi.get(self, "egresses")
 
     @egresses.setter
     def egresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]]]):
         pulumi.set(self, "egresses", value)
 
     @property
     @pulumi.getter
     def ingresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]:
         """
-        /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        A security group rule definition (can be specified multiple times).
         """
         return pulumi.get(self, "ingresses")
 
     @ingresses.setter
     def ingresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]):
         pulumi.set(self, "ingresses", value)
 
@@ -160,15 +168,16 @@
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use the SecurityGroupRule instead (or refer to the ad-hoc migration guide).
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesEgressArgs']]]] egresses: A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
         :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -226,15 +235,16 @@
         """
         Get an existing SecurityGroupRules resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesEgressArgs']]]] egresses: A security group rule definition (can be specified multiple times).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
         :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupRulesState.__new__(_SecurityGroupRulesState)
 
@@ -243,21 +253,24 @@
         __props__.__dict__["security_group"] = security_group
         __props__.__dict__["security_group_id"] = security_group_id
         return SecurityGroupRules(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def egresses(self) -> pulumi.Output[Optional[Sequence['outputs.SecurityGroupRulesEgress']]]:
+        """
+        A security group rule definition (can be specified multiple times).
+        """
         return pulumi.get(self, "egresses")
 
     @property
     @pulumi.getter
     def ingresses(self) -> pulumi.Output[Optional[Sequence['outputs.SecurityGroupRulesIngress']]]:
         """
-        /`egress` - (Block) A security group rule definition (can be specified multiple times).
+        A security group rule definition (can be specified multiple times).
         """
         return pulumi.get(self, "ingresses")
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,28 @@
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oidc: Optional[pulumi.Input['SKSClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SKSCluster resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
-        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+               control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+               (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+               documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+               reference; may only be set at creation time).
         """
         pulumi.set(__self__, "zone", zone)
         if addons is not None:
             warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
             pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
         if addons is not None:
             pulumi.set(__self__, "addons", addons)
@@ -68,15 +72,15 @@
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -89,15 +93,15 @@
     def addons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "addons", value)
 
     @property
     @pulumi.getter(name="autoUpgrade")
     def auto_upgrade(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        Enable automatic upgrading of the control plane version.
         """
         return pulumi.get(self, "auto_upgrade")
 
     @auto_upgrade.setter
     def auto_upgrade(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_upgrade", value)
 
@@ -122,15 +126,16 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+        control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
@@ -146,15 +151,16 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+        (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "metrics_server", value)
 
@@ -170,15 +176,16 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['SKSClusterOidcArgs']]:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+        documented below.
         """
         return pulumi.get(self, "oidc")
 
     @oidc.setter
     def oidc(self, value: Optional[pulumi.Input['SKSClusterOidcArgs']]):
         pulumi.set(self, "oidc", value)
 
@@ -194,15 +201,16 @@
     def service_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_level", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+        reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
@@ -227,31 +235,36 @@
                  oidc: Optional[pulumi.Input['SKSClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SKSCluster resources.
-        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
-        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
+               `metrics-server`).
+        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+               control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+               (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of SKSNodepool (IDs) attached to the cluster.
-        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
+        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+               documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] state: The cluster state.
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+               reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if addons is not None:
             warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
             pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
         if addons is not None:
             pulumi.set(__self__, "addons", addons)
         if aggregation_ca is not None:
@@ -300,27 +313,28 @@
     def addons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "addons", value)
 
     @property
     @pulumi.getter(name="aggregationCa")
     def aggregation_ca(self) -> Optional[pulumi.Input[str]]:
         """
-        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
+        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
+        `metrics-server`).
         """
         return pulumi.get(self, "aggregation_ca")
 
     @aggregation_ca.setter
     def aggregation_ca(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aggregation_ca", value)
 
     @property
     @pulumi.getter(name="autoUpgrade")
     def auto_upgrade(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        Enable automatic upgrading of the control plane version.
         """
         return pulumi.get(self, "auto_upgrade")
 
     @auto_upgrade.setter
     def auto_upgrade(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_upgrade", value)
 
@@ -381,15 +395,16 @@
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+        control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
@@ -417,15 +432,16 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+        (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "metrics_server", value)
 
@@ -441,27 +457,28 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def nodepools(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of SKSNodepool (IDs) attached to the cluster.
+        The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
         """
         return pulumi.get(self, "nodepools")
 
     @nodepools.setter
     def nodepools(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "nodepools", value)
 
     @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['SKSClusterOidcArgs']]:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+        documented below.
         """
         return pulumi.get(self, "oidc")
 
     @oidc.setter
     def oidc(self, value: Optional[pulumi.Input['SKSClusterOidcArgs']]):
         pulumi.set(self, "oidc", value)
 
@@ -489,27 +506,28 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+        reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -531,47 +549,51 @@
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing SKS cluster may be imported by `<ID>@<zone>`console
+        An existing SKS cluster may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/sKSCluster:SKSCluster \\
         ```
 
          exoscale_sks_cluster.my_sks_cluster \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+               control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+               (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+               documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+               reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SKSClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing SKS cluster may be imported by `<ID>@<zone>`console
+        An existing SKS cluster may be imported by `<ID>@<zone>`
 
         ```sh
          $ pulumi import exoscale:index/sKSCluster:SKSCluster \\
         ```
 
          exoscale_sks_cluster.my_sks_cluster \\
 
@@ -669,31 +691,36 @@
         """
         Get an existing SKSCluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
-        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
+               `metrics-server`).
+        :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+               control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+               (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of SKSNodepool (IDs) attached to the cluster.
-        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
+        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+               documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] state: The cluster state.
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone][zone] name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+               reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SKSClusterState.__new__(_SKSClusterState)
 
         __props__.__dict__["addons"] = addons
         __props__.__dict__["aggregation_ca"] = aggregation_ca
@@ -721,23 +748,24 @@
     def addons(self) -> pulumi.Output[Sequence[str]]:
         return pulumi.get(self, "addons")
 
     @property
     @pulumi.getter(name="aggregationCa")
     def aggregation_ca(self) -> pulumi.Output[str]:
         """
-        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
+        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
+        `metrics-server`).
         """
         return pulumi.get(self, "aggregation_ca")
 
     @property
     @pulumi.getter(name="autoUpgrade")
     def auto_upgrade(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable automatic upgrading of the control plane version (boolean; default: `false`).
+        Enable automatic upgrading of the control plane version.
         """
         return pulumi.get(self, "auto_upgrade")
 
     @property
     @pulumi.getter
     def cni(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "cni")
@@ -774,15 +802,16 @@
         """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> pulumi.Output[Optional[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager][ccm] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
+        control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
     @pulumi.getter(name="kubeletCa")
     def kubelet_ca(self) -> pulumi.Output[str]:
         """
@@ -798,15 +827,16 @@
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> pulumi.Output[Optional[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server][ms] in the control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
+        (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -814,23 +844,24 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def nodepools(self) -> pulumi.Output[Sequence[str]]:
         """
-        The list of SKSNodepool (IDs) attached to the cluster.
+        The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
         """
         return pulumi.get(self, "nodepools")
 
     @property
     @pulumi.getter
     def oidc(self) -> pulumi.Output['outputs.SKSClusterOidc']:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
+        documented below.
         """
         return pulumi.get(self, "oidc")
 
     @property
     @pulumi.getter(name="serviceLevel")
     def service_level(self) -> pulumi.Output[Optional[str]]:
         """
@@ -846,19 +877,20 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
+        reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone][zone] name.
+        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
-        An existing SSH key may be imported as a resource by `<name>`console
+        An existing SSH key may be imported as a resource by `<name>`
 
         ```sh
          $ pulumi import exoscale:index/sSHKey:SSHKey \\
         ```
 
          exoscale_ssh_key.my_ssh_key \\
 
@@ -138,15 +138,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SSHKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        An existing SSH key may be imported as a resource by `<name>`console
+        An existing SSH key may be imported as a resource by `<name>`
 
         ```sh
          $ pulumi import exoscale:index/sSHKey:SSHKey \\
         ```
 
          exoscale_ssh_key.my_ssh_key \\
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 class SSHKeypairArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SSHKeypair resource.
         :param pulumi.Input[str] name: The SSH keypair name.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+               *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
 
     @property
@@ -38,15 +39,16 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+        *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -59,15 +61,16 @@
                  private_key: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SSHKeypair resources.
         :param pulumi.Input[str] fingerprint: The SSH keypair unique identifier.
         :param pulumi.Input[str] name: The SSH keypair name.
         :param pulumi.Input[str] private_key: The SSH *private* key generated if no public key was provided.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+               *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         if fingerprint is not None:
             pulumi.set(__self__, "fingerprint", fingerprint)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_key is not None:
             pulumi.set(__self__, "private_key", private_key)
@@ -110,15 +113,16 @@
     def private_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_key", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+        *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -132,15 +136,16 @@
                  public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a SSHKeypair resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The SSH keypair name.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+               *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SSHKeypairArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -198,15 +203,16 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] fingerprint: The SSH keypair unique identifier.
         :param pulumi.Input[str] name: The SSH keypair name.
         :param pulumi.Input[str] private_key: The SSH *private* key generated if no public key was provided.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+               *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SSHKeypairState.__new__(_SSHKeypairState)
 
         __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["name"] = name
@@ -238,11 +244,12 @@
         """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> pulumi.Output[Optional[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
+        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
+        *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.47.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumiverse-exoscale
-Version: 0.46.0
+Name: pulumiverse_exoscale
+Version: 0.47.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Exoscale Resource Provider
 
 The Exoscale Resource Provider lets you manage [Exoscale](https://www.exoscale.com/) resources.
 
 ## Installing
```

### Comparing `pulumiverse_exoscale-0.46.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 pulumiverse_exoscale/get_elastic_ip.py
 pulumiverse_exoscale/get_instance_pool.py
 pulumiverse_exoscale/get_instance_pool_list.py
 pulumiverse_exoscale/get_network.py
 pulumiverse_exoscale/get_nlb.py
 pulumiverse_exoscale/get_private_network.py
 pulumiverse_exoscale/get_security_group.py
+pulumiverse_exoscale/get_sks_cluster.py
+pulumiverse_exoscale/get_sks_cluster_list.py
+pulumiverse_exoscale/get_sks_nodepool.py
+pulumiverse_exoscale/get_sks_nodepool_list.py
 pulumiverse_exoscale/get_template.py
 pulumiverse_exoscale/iam_access_key.py
 pulumiverse_exoscale/instance_pool.py
 pulumiverse_exoscale/ip_address.py
 pulumiverse_exoscale/network.py
 pulumiverse_exoscale/nic.py
 pulumiverse_exoscale/nlb.py
```

### Comparing `pulumiverse_exoscale-0.46.0/setup.py` & `pulumiverse_exoscale-0.47.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.46.0"
-PLUGIN_VERSION = "0.46.0"
+VERSION = "0.47.0"
+PLUGIN_VERSION = "0.47.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'exoscale', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-exoscale'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "exoscale Pulumi Package - Development Version"
 
 
 setup(name='pulumiverse_exoscale',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing exoscale cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

