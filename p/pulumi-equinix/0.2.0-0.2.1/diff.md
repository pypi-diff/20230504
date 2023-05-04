# Comparing `tmp/pulumi_equinix-0.2.0.tar.gz` & `tmp/pulumi_equinix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix-0.2.0.tar", last modified: Tue Apr 25 14:50:03 2023, max compression
+gzip compressed data, was "pulumi_equinix-0.2.1.tar", last modified: Thu May  4 18:38:47 2023, max compression
```

## Comparing `pulumi_equinix-0.2.0.tar` & `pulumi_equinix-0.2.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.807201 pulumi_equinix-0.2.0/pulumi_equinix/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153044 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   278947 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49961 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/service_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.815201 pulumi_equinix-0.2.0/pulumi_equinix/metal/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_plans.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    41964 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    53563 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    47745 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    28278 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    42418 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    65598 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/acl_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    92184 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_software.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/network_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.013532 pulumi_equinix-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-04 18:38:47.013532 pulumi_equinix-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.005532 pulumi_equinix-0.2.1/pulumi_equinix/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.005532 pulumi_equinix-0.2.1/pulumi_equinix/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.005532 pulumi_equinix-0.2.1/pulumi_equinix/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153044 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_service_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_service_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   278947 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49961 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/fabric/service_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.009532 pulumi_equinix-0.2.1/pulumi_equinix/metal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/get_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41964 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53563 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47745 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28278 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42418 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/metal/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.013532 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65598 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/acl_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92184 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/device_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/network_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/networkedge/ssh_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:38:47.005532 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-04 18:38:47.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/pulumi_equinix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:38:47.013532 pulumi_equinix-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 18:38:46.000000 pulumi_equinix-0.2.1/setup.py
```

### Comparing `pulumi_equinix-0.2.0/PKG-INFO` & `pulumi_equinix-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_equinix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_equinix-0.2.0/README.md` & `pulumi_equinix-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/__init__.py` & `pulumi_equinix-0.2.1/pulumi_equinix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/_enums.py` & `pulumi_equinix-0.2.1/pulumi_equinix/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/_utilities.py` & `pulumi_equinix-0.2.1/pulumi_equinix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/config/vars.py` & `pulumi_equinix-0.2.1/pulumi_equinix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/__init__.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/_enums.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/_inputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/connection.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_connection.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_port.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_ports.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profile.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profiles.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/get_service_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/outputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/fabric/service_profile.py` & `pulumi_equinix-0.2.1/pulumi_equinix/fabric/service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/__init__.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/_enums.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/_inputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/bgp_session.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/device.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/device_network_type.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/device_network_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/gateway.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device_bgp_neighbors.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_device_bgp_neighbors.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_facility.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_facility.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_gateway.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_hardware_reservation.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_hardware_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_interconnection.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_interconnection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_ip_block_ranges.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_ip_block_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_metro.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_metro.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_operating_system.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_operating_system.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_organization.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_plans.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_port.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_precreated_ip_block.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_precreated_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project_ssh_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_reserved_ip_block.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_price.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_spot_market_price.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_request.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_virtual_circuit.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vlan.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vrf.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/get_vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/interconnection.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/interconnection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/ip_attachment.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/ip_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/organization.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/organization_member.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/outputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/port.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/port_vlan_attachment.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/port_vlan_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/project.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/project_api_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/project_ssh_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/reserved_ip_block.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/spot_market_request.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/ssh_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/user_api_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/virtual_circuit.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/vlan.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/metal/vrf.py` & `pulumi_equinix-0.2.1/pulumi_equinix/metal/vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/__init__.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_enums.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_inputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/acl_template.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/acl_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/bgp.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device_link.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/device_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_account.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_platform.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_platform.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_software.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_software.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_type.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/get_device_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/network_file.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/network_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/outputs.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_key.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_user.py` & `pulumi_equinix-0.2.1/pulumi_equinix/networkedge/ssh_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix/provider.py` & `pulumi_equinix-0.2.1/pulumi_equinix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix.egg-info/PKG-INFO` & `pulumi_equinix-0.2.1/pulumi_equinix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-equinix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_equinix-0.2.0/pulumi_equinix.egg-info/SOURCES.txt` & `pulumi_equinix-0.2.1/pulumi_equinix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.2.0/setup.py` & `pulumi_equinix-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.0"
-PLUGIN_VERSION = "0.2.0"
+VERSION = "0.2.1"
+PLUGIN_VERSION = "0.2.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'equinix', PLUGIN_VERSION, '--server', 'github://api.github.com/equinix'])
         except OSError as error:
```

