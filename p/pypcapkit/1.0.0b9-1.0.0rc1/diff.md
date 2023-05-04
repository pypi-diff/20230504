# Comparing `tmp/pypcapkit-1.0.0b9.tar.gz` & `tmp/pypcapkit-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypcapkit-1.0.0b9.tar", last modified: Fri Apr 21 17:37:52 2023, max compression
+gzip compressed data, was "pypcapkit-1.0.0rc1.tar", last modified: Thu May  4 06:22:14 2023, max compression
```

## Comparing `pypcapkit-1.0.0b9.tar` & `pypcapkit-1.0.0rc1.tar`

### file list

```diff
@@ -1,511 +1,527 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.497974 pypcapkit-1.0.0b9/pcapkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.497974 pypcapkit-1.0.0b9/pcapkit/const/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.497974 pypcapkit-1.0.0b9/pcapkit/const/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/arp/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/arp/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.497974 pypcapkit-1.0.0b9/pcapkit/const/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ftp/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ftp/return_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.501974 pypcapkit-1.0.0b9/pcapkit/const/hip/
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/di.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/ecdsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/ecdsa_low_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/eddsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/esp_transform_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/hi_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/hit_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/nat_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/notify_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/registration_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/hip/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.501974 pypcapkit-1.0.0b9/pcapkit/const/http/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/http/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.501974 pypcapkit-1.0.0b9/pcapkit/const/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/classification_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/option_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/option_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/protection_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_rel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_thr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv4/ts_flag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.505974 pypcapkit-1.0.0b9/pcapkit/const/ipv6/
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/extension_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/option_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/seed_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/smf_dpd_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipv6/tagger_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.505974 pypcapkit-1.0.0b9/pcapkit/const/ipx/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipx/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ipx/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.505974 pypcapkit-1.0.0b9/pcapkit/const/l2tp/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/l2tp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/l2tp/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.509974 pypcapkit-1.0.0b9/pcapkit/const/mh/
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/ack_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/ani_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/auth_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/binding_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/binding_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/binding_update_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/dhcp_support_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/dns_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/dsmip6_tls_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/dsmipv6_home_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/enumerating_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/fb_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/fb_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/fb_indication_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/fb_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/flow_id_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/flow_id_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/handoff_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/handover_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/handover_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/handover_initiate_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/handover_initiate_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/home_address_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/lma_mag_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/mn_group_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/mn_id_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/operator_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/qos_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/revocation_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/revocation_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/traffic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/upa_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/mh/upn_reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.509974 pypcapkit-1.0.0b9/pcapkit/const/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ospf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ospf/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/ospf/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.509974 pypcapkit-1.0.0b9/pcapkit/const/pcapng/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/pcapng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/pcapng/block_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.509974 pypcapkit-1.0.0b9/pcapkit/const/reg/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/reg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27235 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/reg/ethertype.py
--rw-r--r--   0 runner    (1001) docker     (123)    37259 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/reg/linktype.py
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/reg/transtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.509974 pypcapkit-1.0.0b9/pcapkit/const/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/tcp/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/tcp/mp_tcp_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/tcp/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/const/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/const/vlan/priority_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/corekit/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/corekit/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/fields/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/infoclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/multidict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/protochain.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/corekit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/dumpkit/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/dumpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/dumpkit/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/dumpkit/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/dumpkit/pcap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/foundation/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.513974 pypcapkit-1.0.0b9/pcapkit/foundation/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/dpkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/pyshark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/engines/scapy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.517974 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.517974 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/reassembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24943 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.517974 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.517974 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/data/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/traceflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.521975 pypcapkit-1.0.0b9/pcapkit/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/interface/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/interface/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.521975 pypcapkit-1.0.0b9/pcapkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.521975 pypcapkit-1.0.0b9/pcapkit/protocols/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.521975 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/dhcpv6.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/imap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/nntp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/onc_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/rip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/rtp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/sip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/smtp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/telnet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/NotImplemented/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    49224 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/application/httpv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/application/
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/application/httpv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)    28229 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.525975 pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.529975 pypcapkit-1.0.0b9/pcapkit/protocols/internet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.529975 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/esp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/icmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/icmpv6.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/igmp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/shim6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)   209999 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    76152 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/internet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipsec.py
--rw-r--r--   0 runner    (1001) docker     (123)    70654 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    76974 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29634 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.529975 pypcapkit-1.0.0b9/pcapkit/protocols/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/eapol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/fddi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/isdn.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/ndp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/NotImplemented/ppp.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/rarp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    42030 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/httpv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/httpv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.533975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ah.py
--rw-r--r--   0 runner    (1001) docker     (123)    42307 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/hip.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/hopopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6_frag.py
--rw-r--r--   0 runner    (1001) docker     (123)    21454 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/mh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/l2tp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcapng.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/transport/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/protocols/transport/NotImplemented/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/NotImplemented/dccp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/NotImplemented/rsvp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/NotImplemented/sctp.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113820 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/protocols/transport/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.537975 pypcapkit-1.0.0b9/pcapkit/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/toolkit/default.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/toolkit/dpkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/toolkit/pyshark.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/toolkit/scapy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.541975 pypcapkit-1.0.0b9/pcapkit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.541975 pypcapkit-1.0.0b9/pcapkit/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.541975 pypcapkit-1.0.0b9/pcapkit/vendor/arp/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/arp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/arp/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/arp/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.541975 pypcapkit-1.0.0b9/pcapkit/vendor/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ftp/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ftp/return_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.541975 pypcapkit-1.0.0b9/pcapkit/vendor/hip/
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/di.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/ecdsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/ecdsa_low_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/eddsa_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/esp_transform_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/hi_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/hit_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/nat_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/notify_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/registration_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/hip/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.545975 pypcapkit-1.0.0b9/pcapkit/vendor/http/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/http/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.545975 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/classification_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/option_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/option_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/protection_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_del.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_ecn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_pre.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_rel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_thr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/ts_flag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.545975 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/extension_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/option_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/qs_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/router_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/seed_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/smf_dpd_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/tagger_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.545975 pypcapkit-1.0.0b9/pcapkit/vendor/ipx/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipx/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ipx/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.549975 pypcapkit-1.0.0b9/pcapkit/vendor/l2tp/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/l2tp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/l2tp/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/mh/
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/ack_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/ani_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/auth_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_update_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/dhcp_support_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/dns_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/dsmip6_tls_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/dsmipv6_home_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/enumerating_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_indication_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/flow_id_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/flow_id_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/handoff_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_ack_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_ack_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_initiate_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_initiate_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/home_address_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/lma_mag_suboption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/mn_group_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/mn_id_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/operator_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/qos_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/revocation_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/revocation_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/traffic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/upa_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/mh/upn_reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ospf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ospf/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/ospf/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/pcapng/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/pcapng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/pcapng/block_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/reg/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/reg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/reg/ethertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/reg/linktype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/reg/transtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/tcp/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/tcp/mp_tcp_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/tcp/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pcapkit/vendor/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pcapkit/vendor/vlan/priority_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/pypcapkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 17:37:52.000000 pypcapkit-1.0.0b9/pypcapkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:37:52.553975 pypcapkit-1.0.0b9/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 17:37:36.000000 pypcapkit-1.0.0b9/util/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/arp/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.471485 pypcapkit-1.0.0rc1/pcapkit/const/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ftp/return_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.475485 pypcapkit-1.0.0rc1/pcapkit/const/hip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_low_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/eddsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/esp_transform_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/hi_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/hit_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/nat_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/notify_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/registration_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/hip/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.479485 pypcapkit-1.0.0rc1/pcapkit/const/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/http/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.479485 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/classification_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/protection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_rel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_thr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv4/ts_flag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/extension_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/seed_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipv6/tagger_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/ipx/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ipx/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.483485 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/l2tp/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.491485 pypcapkit-1.0.0rc1/pcapkit/const/mh/
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/ack_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/ani_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/auth_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_update_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dhcp_support_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dns_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmipv6_home_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/enumerating_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_indication_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handoff_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/home_address_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/lma_mag_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_id_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/operator_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/qos_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/traffic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/upa_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/mh/upn_reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.491485 pypcapkit-1.0.0rc1/pcapkit/const/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/ospf/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/block_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/hash_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/secrets_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/pcapng/verdict_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25954 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/ethertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/linktype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/reg/transtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/mp_tcp_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/tcp/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.495485 pypcapkit-1.0.0rc1/pcapkit/const/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/const/vlan/priority_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/corekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/fields/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/infoclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/protochain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/corekit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/dumpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/dumpkit/pcap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.499485 pypcapkit-1.0.0rc1/pcapkit/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/dpkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/engines/scapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27578 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/reassembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.503486 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/traceflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/interface/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.507485 pypcapkit-1.0.0rc1/pcapkit/protocols/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dhcpv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/imap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/nntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/onc_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/rip.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/rtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/sip.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/smtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/NotImplemented/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49557 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.511485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28229 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.515485 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.519486 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.519486 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/esp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/icmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/icmpv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/igmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/shim6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76152 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/internet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76974 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29634 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.523486 pypcapkit-1.0.0rc1/pcapkit/protocols/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/eapol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/fddi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/isdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/ndp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/NotImplemented/ppp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/rarp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237556 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.527485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42392 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hopopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_frag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/mh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.531485 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/l2tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62017 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.535486 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/dccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/rsvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/NotImplemented/sctp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113821 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/protocols/transport/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/dpkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pcapng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/toolkit/scapy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.539486 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/arp/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.543485 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/return_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.547485 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_low_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/eddsa_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/esp_transform_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hi_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hit_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/nat_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/notify_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/hip/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.547485 pypcapkit-1.0.0rc1/pcapkit/vendor/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/http/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/classification_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/protection_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_ecn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_rel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_thr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/ts_flag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/extension_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/qs_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/router_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/seed_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/smf_dpd_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/tagger_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.551486 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.559486 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ack_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ani_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/auth_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_update_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dhcp_support_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dns_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmip6_tls_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmipv6_home_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/enumerating_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_indication_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handoff_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/home_address_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/lma_mag_suboption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_group_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_id_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/operator_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/qos_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/traffic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upa_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upn_reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/block_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/hash_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/secrets_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/verdict_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/ethertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/linktype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/reg/transtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/mp_tcp_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.563485 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/priority_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/pypcapkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16319 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 06:22:14.000000 pypcapkit-1.0.0rc1/pypcapkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:22:14.567486 pypcapkit-1.0.0rc1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-04 06:21:58.000000 pypcapkit-1.0.0rc1/util/bump_version.py
```

### Comparing `pypcapkit-1.0.0b9/LICENSE` & `pypcapkit-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/PKG-INFO` & `pypcapkit-1.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypcapkit
-Version: 1.0.0b9
+Version: 1.0.0rc1
 Summary: PyPCAPKit: comprehensive network packet analysis library
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
-Maintainer-email: Jarry Shaw <jarryshaw@icloud.com>
+Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: documentation, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: repository, https://github.com/JarryShaw/PyPCAPKit
 Project-URL: changelog, https://github.com/JarryShaw/PyPCAPKit/releases
 Keywords: network,pcap,packet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pypcapkit-1.0.0b9/README.rst` & `pypcapkit-1.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,8 +109,8 @@
     'TCP', 'UDP',                                           # Transport Layer
 
     'FTP', 'FTP_DATA',                                      # Application Layer
     'HTTP',
 ]
 
 #: version number
-__version__ = '1.0.0b9'
+__version__ = '1.0.0rc1'
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/__main__.py` & `pypcapkit-1.0.0rc1/pcapkit/__main__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/all.py` & `pypcapkit-1.0.0rc1/pcapkit/all.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     'NumberField', 'Int32Field', 'UInt32Field',             # numeric protocol fields
     'Int16Field', 'UInt16Field', 'Int64Field', 'UInt64Field',
     'Int8Field', 'UInt8Field', 'EnumField',
     'BytesField', 'StringField', 'BitField',                # text protocol fields
     'PaddingField',
     'ConditionalField', 'PayloadField', 'SchemaField',      # misc protocol fields
     'ForwardMatchField', 'NoValueField',
-    'IPv4Field', 'IPv6Field',                               # IP address protocol fields
+    'IPv4AddressField', 'IPv6AddressField',                 # IP address protocol fields
+    'IPv4InterfaceField', 'IPv6InterfaceField',
     'ListField', 'OptionField',                             # container protocol fields
 
     # pcapkit.dumpkit
     'PCAPIO',                                               # PCAP Dumper
     'NotImplementedIO',                                     # Simulated I/O
 
     # pcapkit.foundation
@@ -74,20 +75,22 @@
 
     # pcapkit.foundation.reassembly
     'IPv4_Reassembly', 'IPv6_Reassembly',                   # IP Reassembly
     'TCP_Reassembly',                                       # TCP Reassembly
 
     # pcapkit.foundation.registry
     'register_protocol',
-    'register_linktype', 'register_pcap',
+    'register_linktype', 'register_pcap', 'register_pcapng',
     'register_ethertype', 'register_transtype',
     'register_port', 'register_tcp_port', 'register_udp_port',
     'register_output',
     'register_extractor_dumper', 'register_extractor_engine',
     'register_traceflow',
+    'register_pcapng_block', 'register_pcapng_option', 'register_pcapng_secrets',
+    'register_pcapng_record',
     'register_hopopt', 'register_ipv6_opts', 'register_ipv6_route',
     'register_ipv4', 'register_hip',
     'register_tcp', 'register_mptcp',
     'register_http',
 
     # pcapkit.interface
     'extract', 'reassemble', 'trace',                       # Interface Functions
@@ -109,15 +112,16 @@
     'FTP', 'FTP_DATA',                                      # Application Layer
     'HTTP',
     'Schema', 'schema',                                     # Protocol Schema
     'Data', 'data',                                         # Protocol Data
 
     # pcapkit.toolkit
     'ipv4_reassembly', 'ipv6_reassembly', 'tcp_reassembly', 'tcp_traceflow',
-                                                            # default engine
+    'pcapng_ipv4_reassembly', 'pcapng_ipv6_reassembly', 'pcapng_tcp_reassembly', 'pcapng_tcp_traceflow',
+    'pcapng_block2frame',                                   # default engine
     'dpkt_ipv6_hdr_len', 'dpkt_packet2chain', 'dpkt_packet2dict',
     'dpkt_ipv4_reassembly', 'dpkt_ipv6_reassembly', 'dpkt_tcp_reassembly', 'dpkt_tcp_traceflow',
                                                             # DPKT engine
     'pyshark_packet2dict', 'pyshark_tcp_traceflow',         # PyShark engine
     'scapy_packet2chain', 'scapy_packet2dict',
     'scapy_ipv4_reassembly', 'scapy_ipv6_reassembly', 'scapy_tcp_reassembly', 'scapy_tcp_traceflow',
                                                             # Scapy engine
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,9 +70,11 @@
     # OSPF
     'OSPF_Authentication', 'OSPF_Packet',
     # TCP
     'TCP_Checksum', 'TCP_Option',
     # VLAN
     'VLAN_PriorityLevel',
     # PCAPNG
-    'PCAPNG_BlockType',
+    'PCAPNG_BlockType', 'PCAPNG_OptionType', 'PCAPNG_HashAlgorithm',
+    'PCAPNG_VerdictType', 'PCAPNG_RecordType', 'PCAPNG_SecretsType',
+    'PCAPNG_FilterType',
 ]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/arp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/arp/hardware.py` & `pypcapkit-1.0.0rc1/pcapkit/const/arp/hardware.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,29 +155,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Hardware(key)
         if key not in Hardware._member_map_:  # pylint: disable=no-member
-            extend_enum(Hardware, key, default)
+            return extend_enum(Hardware, key, default)
         return Hardware[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Hardware':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 39 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 258 <= value <= 65534:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/arp/operation.py` & `pypcapkit-1.0.0rc1/pcapkit/const/arp/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,25 +108,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Operation(key)
         if key not in Operation._member_map_:  # pylint: disable=no-member
-            extend_enum(Operation, key, default)
+            return extend_enum(Operation, key, default)
         return Operation[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Operation':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 26 <= value <= 65534:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ftp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ftp/command.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ftp/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,36 @@
 
 __all__ = ['Command']
 
 
 class Command(StrEnum):
     """[Command] FTP Command"""
 
+    if TYPE_CHECKING:
+        #: Feature of command.
+        feat: 'Optional[str]'
+        #: Description of command.
+        desc: 'Optional[str]'
+        #: Type of command.
+        type: 'Optional[tuple[str, ...]]'
+        #: Conformance of command.
+        conf: 'Optional[str]'
+        #: Note of command.
+        note: 'Optional[tuple[str, ...]]'
+
     def __new__(cls, name: 'str', feat: 'Optional[str]' = None, desc: 'Optional[str]' = None,
                 type: 'Optional[tuple[str, ...]]' = None, conf: 'Optional[str]' = None,
                 note: 'Optional[tuple[str, ...]]' = None) -> 'Type[Command]':
         obj = str.__new__(cls, name)
         obj._value_ = name
 
-        #: Feature of command.
         obj.feat = feat
-        #: Description of command.
         obj.desc = desc
-        #: Type of command.
         obj.type = type
-        #: Conformance of command.
         obj.conf = conf
-        #: Note of command.
         obj.note = note
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s.%s>" % (self.__class__.__name__, self._name_)
 
@@ -232,20 +239,19 @@
         Args:
             key: Key to get enum item.
             default: Default value if not found.
 
         :meta private:
         """
         if key not in Command._member_map_:  # pylint: disable=no-member
-            extend_enum(Command, key.upper(), default if default is not None else key)
+            return extend_enum(Command, key.upper(), default if default is not None else key)
         return Command[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'str') -> 'Command':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
-        extend_enum(cls, value.upper(), value)
-        return cls(value)
+        return extend_enum(cls, value.upper(), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ftp/return_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ftp/return_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,29 @@
     '5': 'File system',
 }  # type: dict[str, str]
 
 
 class ReturnCode(IntEnum):
     """[ReturnCode] FTP Server Return Code"""
 
+    if TYPE_CHECKING:
+        #: Description of the return code.
+        description: 'Optional[str]'
+        #: Response kind.
+        kind: 'str'
+        #: Grouping information.
+        group: 'str'
+
     def __new__(cls, value: 'int', description: 'Optional[str]' = None) -> 'Type[ReturnCode]':
         obj = int.__new__(cls, value)
         obj._value_ = value
 
         code = str(value)
-        #: Description of the return code.
         obj.description = description
-        #: Response kind.
         obj.kind = KIND.get(str(value)[0], 'Reserved')
-        #: Grouping information.
         obj.group = INFO.get(str(value)[1], 'Reserved')
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s [%s]>" % (self.__class__.__name__, self._value_)
 
@@ -251,22 +256,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ReturnCode(key)
         if key not in ReturnCode._member_map_:  # pylint: disable=no-member
-            extend_enum(ReturnCode, key, default)
+            return extend_enum(ReturnCode, key, default)
         return ReturnCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ReturnCode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 100 <= value <= 659):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'CODE_%s' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'CODE_%s' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/certificate.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,25 +54,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Certificate(key)
         if key not in Certificate._member_map_:  # pylint: disable=no-member
-            extend_enum(Certificate, key, default)
+            return extend_enum(Certificate, key, default)
         return Certificate[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Certificate':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 9 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/cipher.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/cipher.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Cipher(key)
         if key not in Cipher._member_map_:  # pylint: disable=no-member
-            extend_enum(Cipher, key, default)
+            return extend_enum(Cipher, key, default)
         return Cipher[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Cipher':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 5 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/di.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/di.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,25 +36,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return DITypes(key)
         if key not in DITypes._member_map_:  # pylint: disable=no-member
-            extend_enum(DITypes, key, default)
+            return extend_enum(DITypes, key, default)
         return DITypes[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'DITypes':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 15):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 15:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/ecdsa_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_curve.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,25 +36,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ECDSACurve(key)
         if key not in ECDSACurve._member_map_:  # pylint: disable=no-member
-            extend_enum(ECDSACurve, key, default)
+            return extend_enum(ECDSACurve, key, default)
         return ECDSACurve[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ECDSACurve':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/ecdsa_low_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/ecdsa_low_curve.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,25 +33,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ECDSALowCurve(key)
         if key not in ECDSALowCurve._member_map_:  # pylint: disable=no-member
-            extend_enum(ECDSALowCurve, key, default)
+            return extend_enum(ECDSALowCurve, key, default)
         return ECDSALowCurve[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ECDSALowCurve':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 2 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/eddsa_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/eddsa_curve.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,25 +42,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return EdDSACurve(key)
         if key not in EdDSACurve._member_map_:  # pylint: disable=no-member
-            extend_enum(EdDSACurve, key, default)
+            return extend_enum(EdDSACurve, key, default)
         return EdDSACurve[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'EdDSACurve':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 5 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/esp_transform_suite.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/esp_transform_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ESPTransformSuite(key)
         if key not in ESPTransformSuite._member_map_:  # pylint: disable=no-member
-            extend_enum(ESPTransformSuite, key, default)
+            return extend_enum(ESPTransformSuite, key, default)
         return ESPTransformSuite[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ESPTransformSuite':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 16 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/group.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Group(key)
         if key not in Group._member_map_:  # pylint: disable=no-member
-            extend_enum(Group, key, default)
+            return extend_enum(Group, key, default)
         return Group[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Group':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 12 <= value <= 255:
             # Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/hi_algorithm.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/hi_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,29 +60,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return HIAlgorithm(key)
         if key not in HIAlgorithm._member_map_:  # pylint: disable=no-member
-            extend_enum(HIAlgorithm, key, default)
+            return extend_enum(HIAlgorithm, key, default)
         return HIAlgorithm[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'HIAlgorithm':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 10 <= value <= 12:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 14 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/hit_suite.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/hit_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,25 +45,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return HITSuite(key)
         if key not in HITSuite._member_map_:  # pylint: disable=no-member
-            extend_enum(HITSuite, key, default)
+            return extend_enum(HITSuite, key, default)
         return HITSuite[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'HITSuite':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 15):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 6 <= value <= 15:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/nat_traversal.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/nat_traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,25 +39,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return NATTraversal(key)
         if key not in NATTraversal._member_map_:  # pylint: disable=no-member
-            extend_enum(NATTraversal, key, default)
+            return extend_enum(NATTraversal, key, default)
         return NATTraversal[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'NATTraversal':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 4 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/notify_message.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/notify_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -141,73 +141,60 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return NotifyMessage(key)
         if key not in NotifyMessage._member_map_:  # pylint: disable=no-member
-            extend_enum(NotifyMessage, key, default)
+            return extend_enum(NotifyMessage, key, default)
         return NotifyMessage[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'NotifyMessage':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 2 <= value <= 6:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 8 <= value <= 13:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 21 <= value <= 23:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 29 <= value <= 31:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 33 <= value <= 39:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 52 <= value <= 59:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 65 <= value <= 69:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 71 <= value <= 89:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 91 <= value <= 99:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 101 <= value <= 8191:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 8192 <= value <= 16383:
             #: Reserved for Private Use [:rfc:`7401`]
-            extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
         if 16386 <= value <= 40959:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 40960 <= value <= 65535:
             #: Reserved for Private Use [:rfc:`7401`]
-            extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/packet.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,33 +60,30 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Packet(key)
         if key not in Packet._member_map_:  # pylint: disable=no-member
-            extend_enum(Packet, key, default)
+            return extend_enum(Packet, key, default)
         return Packet[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Packet':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 127):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 5 <= value <= 15:
             # Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 21 <= value <= 31:
             # Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 33 <= value <= 127:
             # Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/parameter.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/parameter.py`

 * *Files 26% similar despite different names*

```diff
@@ -213,213 +213,165 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Parameter(key)
         if key not in Parameter._member_map_:  # pylint: disable=no-member
-            extend_enum(Parameter, key, default)
+            return extend_enum(Parameter, key, default)
         return Parameter[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Parameter':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0 <= value <= 64:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 66 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 130 <= value <= 192:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 194 <= value <= 256:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 258 <= value <= 320:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 322 <= value <= 384:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 386 <= value <= 448:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 450 <= value <= 510:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 514 <= value <= 576:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 580 <= value <= 607:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 611 <= value <= 640:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 642 <= value <= 704:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 706 <= value <= 714:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 716 <= value <= 767:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 769 <= value <= 831:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 833 <= value <= 896:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 898 <= value <= 929:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 937 <= value <= 949:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 951 <= value <= 960:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 962 <= value <= 2048:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 2050 <= value <= 4094:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4096 <= value <= 4480:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4482 <= value <= 4544:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4546 <= value <= 4576:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4578 <= value <= 4579:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4581 <= value <= 4591:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4593 <= value <= 4600:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4602 <= value <= 4649:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4651 <= value <= 4659:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4661 <= value <= 4679:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4681 <= value <= 4699:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4701 <= value <= 4709:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 4711 <= value <= 7679:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 7681 <= value <= 32767:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 32768 <= value <= 49151:
             #: Reserved [:rfc:`7401`]
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         if 49152 <= value <= 61504:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 61506 <= value <= 61568:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 61570 <= value <= 61632:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 61634 <= value <= 61696:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 61698 <= value <= 63660:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 63662 <= value <= 63424:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 63426 <= value <= 63997:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 63999 <= value <= 64001:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 64003 <= value <= 64010:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 64012 <= value <= 64016:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 64018 <= value <= 65497:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 65503 <= value <= 65519:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 65521 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/registration.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,29 +42,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Registration(key)
         if key not in Registration._member_map_:  # pylint: disable=no-member
-            extend_enum(Registration, key, default)
+            return extend_enum(Registration, key, default)
         return Registration[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Registration':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 5 <= value <= 200:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 201 <= value <= 255:
             #: Reserved for Private Use [:rfc:`8003`]
-            extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/registration_failure.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/registration_failure.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,29 +58,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return RegistrationFailure(key)
         if key not in RegistrationFailure._member_map_:  # pylint: disable=no-member
-            extend_enum(RegistrationFailure, key, default)
+            return extend_enum(RegistrationFailure, key, default)
         return RegistrationFailure[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'RegistrationFailure':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 10 <= value <= 200:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 201 <= value <= 255:
             #: Reserved for Private Use [:rfc:`8003`]
-            extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Private_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/suite.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/suite.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,25 +48,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Suite(key)
         if key not in Suite._member_map_:  # pylint: disable=no-member
-            extend_enum(Suite, key, default)
+            return extend_enum(Suite, key, default)
         return Suite[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Suite':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 7 <= value <= 65535:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/hip/transport.py` & `pypcapkit-1.0.0rc1/pcapkit/const/hip/transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Transport(key)
         if key not in Transport._member_map_:  # pylint: disable=no-member
-            extend_enum(Transport, key, default)
+            return extend_enum(Transport, key, default)
         return Transport[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Transport':
         """Lookup function used when value is not found.
 
         Args:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/error_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/error_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ErrorCode(key)
         if key not in ErrorCode._member_map_:  # pylint: disable=no-member
-            extend_enum(ErrorCode, key, default)
+            return extend_enum(ErrorCode, key, default)
         return ErrorCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ErrorCode':
         """Lookup function used when value is not found.
 
         Args:
@@ -87,10 +87,9 @@
 
         """
         if not (isinstance(value, int) and 0x00000000 <= value <= 0xFFFFFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x0000000E <= value <= 0xFFFFFFFF:
             #: Unassigned
             temp = hex(value)[2:].upper().zfill(8)
-            extend_enum(cls, 'Unassigned_0x%s' % (temp[:4]+'_'+temp[4:]), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % (temp[:4]+'_'+temp[4:]), value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/frame.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Frame(key)
         if key not in Frame._member_map_:  # pylint: disable=no-member
-            extend_enum(Frame, key, default)
+            return extend_enum(Frame, key, default)
         return Frame[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Frame':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x00 <= value <= 0xFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x0D <= value <= 0x0F:
             #: ``Unassigned``
-            extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
         if 0x11 <= value <= 0xFF:
             #: ``Unassigned``
-            extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/method.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,26 @@
     from typing import Optional, Type
 
 __all__ = ['Method']
 
 class Method(StrEnum):
     """[Method] HTTP Method"""
 
+    if TYPE_CHECKING:
+        #: Safe method.
+        safe: 'bool'
+        #: Idempotent method.
+        idempotent: 'bool'
+
     def __new__(cls, value: 'str', safe: 'bool' = False,
                 idempotent: 'bool' = False) -> 'Type[Method]':
         obj = str.__new__(cls)
         obj._value_ = value
 
-        #: Safe method.
         obj.safe = safe
-        #: Idempotent method.
         obj.idempotent = idempotent
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s.%s>" % (self.__class__.__name__, self._value_)
 
@@ -162,20 +166,19 @@
         Args:
             key: Key to get enum item.
             default: Default value if not found.
 
         :meta private:
         """
         if key not in Method._member_map_:  # pylint: disable=no-member
-            extend_enum(Method, key.upper(), default if default is not None else key)
+            return extend_enum(Method, key.upper(), default if default is not None else key)
         return Method[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'str') -> 'Method':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
-        extend_enum(cls, value.upper(), value)
-        return cls(value)
+        return extend_enum(cls, value.upper(), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/setting.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/setting.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,33 +67,30 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Setting(key)
         if key not in Setting._member_map_:  # pylint: disable=no-member
-            extend_enum(Setting, key, default)
+            return extend_enum(Setting, key, default)
         return Setting[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Setting':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x0000 <= value <= 0xFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x000A <= value <= 0x000F:
             #: ``Unassigned``
-            extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x0011 <= value <= 0x4D43:
             #: ``Unassigned``
-            extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x4D45 <= value <= 0xFFFF:
             #: ``Unassigned``
-            extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/http/status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/http/status_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 
 __all__ = ['StatusCode']
 
 
 class StatusCode(IntEnum):
     """[StatusCode] HTTP Status Code"""
 
+    if TYPE_CHECKING:
+        #: Status message.
+        message: 'str'
+
     def __new__(cls, value: 'int', message: 'str' = '') -> 'Type[StatusCode]':
         obj = int.__new__(cls, value)
         obj._value_ = value
 
-        #: Status message.
         obj.message = message
 
         return obj
 
     #: Continue [:rfc:`9110#section-15.2.1`]
     CONTINUE = 100, 'Continue'
 
@@ -285,8 +288,7 @@
             #: Unassigned
             extend_enum(cls, 'Unassigned_%d' % value, value)
             return cls(value)
         if 512 <= value <= 599:
             #: Unassigned
             extend_enum(cls, 'Unassigned_%d' % value, value)
             return cls(value)
-        return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/classification_level.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/classification_level.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,23 +43,23 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ClassificationLevel(key)
         if key not in ClassificationLevel._member_map_:  # pylint: disable=no-member
-            extend_enum(ClassificationLevel, key, default)
+            return extend_enum(ClassificationLevel, key, default)
         return ClassificationLevel[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ClassificationLevel':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b00000000 <= value <= 0b11111111):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         temp = bin(value)[2:].upper().zfill(8)
-        extend_enum(cls, 'Unassigned_0b%s' % (temp[:4]+'_'+temp[4:]), value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_0b%s' % (temp[:4]+'_'+temp[4:]), value)
+        return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/option_class.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,22 +35,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return OptionClass(key)
         if key not in OptionClass._member_map_:  # pylint: disable=no-member
-            extend_enum(OptionClass, key, default)
+            return extend_enum(OptionClass, key, default)
         return OptionClass[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'OptionClass':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 3):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/option_number.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/option_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,22 +117,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return OptionNumber(key)
         if key not in OptionNumber._member_map_:  # pylint: disable=no-member
-            extend_enum(OptionNumber, key, default)
+            return extend_enum(OptionNumber, key, default)
         return OptionNumber[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'OptionNumber':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/protection_authority.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/protection_authority.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ProtectionAuthority(key)
         if key not in ProtectionAuthority._member_map_:  # pylint: disable=no-member
-            extend_enum(ProtectionAuthority, key, default)
+            return extend_enum(ProtectionAuthority, key, default)
         return ProtectionAuthority[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ProtectionAuthority':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and value >= 0):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/qs_function.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/qs_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return QSFunction(key)
         if key not in QSFunction._member_map_:  # pylint: disable=no-member
-            extend_enum(QSFunction, key, default)
+            return extend_enum(QSFunction, key, default)
         return QSFunction[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'QSFunction':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 8):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/router_alert.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/router_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,29 +225,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return RouterAlert(key)
         if key not in RouterAlert._member_map_:  # pylint: disable=no-member
-            extend_enum(RouterAlert, key, default)
+            return extend_enum(RouterAlert, key, default)
         return RouterAlert[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'RouterAlert':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 66 <= value <= 65502:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 65503 <= value <= 65534:
             #: Reserved for experimental use [:rfc:`5350`]
-            extend_enum(cls, 'Reserved for experimental use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved for experimental use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_del.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_del.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ToSDelay(key)
         if key not in ToSDelay._member_map_:  # pylint: disable=no-member
-            extend_enum(ToSDelay, key, default)
+            return extend_enum(ToSDelay, key, default)
         return ToSDelay[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ToSDelay':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_ecn.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_ecn.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,22 +35,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ToSECN(key)
         if key not in ToSECN._member_map_:  # pylint: disable=no-member
-            extend_enum(ToSECN, key, default)
+            return extend_enum(ToSECN, key, default)
         return ToSECN[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ToSECN':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b00 <= value <= 0b11):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_pre.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_pre.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ToSPrecedence(key)
         if key not in ToSPrecedence._member_map_:  # pylint: disable=no-member
-            extend_enum(ToSPrecedence, key, default)
+            return extend_enum(ToSPrecedence, key, default)
         return ToSPrecedence[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ToSPrecedence':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b000 <= value <= 0b111):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_rel.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_rel.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ToSReliability(key)
         if key not in ToSReliability._member_map_:  # pylint: disable=no-member
-            extend_enum(ToSReliability, key, default)
+            return extend_enum(ToSReliability, key, default)
         return ToSReliability[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ToSReliability':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/tos_thr.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/tos_thr.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ToSThroughput(key)
         if key not in ToSThroughput._member_map_:  # pylint: disable=no-member
-            extend_enum(ToSThroughput, key, default)
+            return extend_enum(ToSThroughput, key, default)
         return ToSThroughput[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ToSThroughput':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv4/ts_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv4/ts_flag.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,22 +33,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return TSFlag(key)
         if key not in TSFlag._member_map_:  # pylint: disable=no-member
-            extend_enum(TSFlag, key, default)
+            return extend_enum(TSFlag, key, default)
         return TSFlag[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'TSFlag':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b0000 <= value <= 0b1111):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/extension_header.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/extension_header.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/option.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Option(key)
         if key not in Option._member_map_:  # pylint: disable=no-member
-            extend_enum(Option, key, default)
+            return extend_enum(Option, key, default)
         return Option[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Option':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x00 <= value <= 0xFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/option_action.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/option_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return OptionAction(key)
         if key not in OptionAction._member_map_:  # pylint: disable=no-member
-            extend_enum(OptionAction, key, default)
+            return extend_enum(OptionAction, key, default)
         return OptionAction[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'OptionAction':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 3):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/qs_function.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/qs_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return QSFunction(key)
         if key not in QSFunction._member_map_:  # pylint: disable=no-member
-            extend_enum(QSFunction, key, default)
+            return extend_enum(QSFunction, key, default)
         return QSFunction[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'QSFunction':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 8):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/router_alert.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/router_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,29 +240,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return RouterAlert(key)
         if key not in RouterAlert._member_map_:  # pylint: disable=no-member
-            extend_enum(RouterAlert, key, default)
+            return extend_enum(RouterAlert, key, default)
         return RouterAlert[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'RouterAlert':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 70 <= value <= 65502:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 65503 <= value <= 65534:
             #: Reserved for experimental use [:rfc:`5350`]
-            extend_enum(cls, 'Reserved for experimental use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved for experimental use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/routing.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/routing.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,25 +59,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Routing(key)
         if key not in Routing._member_map_:  # pylint: disable=no-member
-            extend_enum(Routing, key, default)
+            return extend_enum(Routing, key, default)
         return Routing[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Routing':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 7 <= value <= 252:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/seed_id.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/seed_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,22 +35,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return SeedID(key)
         if key not in SeedID._member_map_:  # pylint: disable=no-member
-            extend_enum(SeedID, key, default)
+            return extend_enum(SeedID, key, default)
         return SeedID[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'SeedID':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b00 <= value <= 0b11):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/smf_dpd_mode.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/smf_dpd_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return SMFDPDMode(key)
         if key not in SMFDPDMode._member_map_:  # pylint: disable=no-member
-            extend_enum(SMFDPDMode, key, default)
+            return extend_enum(SMFDPDMode, key, default)
         return SMFDPDMode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'SMFDPDMode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipv6/tagger_id.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipv6/tagger_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,25 +39,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return TaggerID(key)
         if key not in TaggerID._member_map_:  # pylint: disable=no-member
-            extend_enum(TaggerID, key, default)
+            return extend_enum(TaggerID, key, default)
         return TaggerID[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'TaggerID':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 7):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 4 <= value <= 7:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipx/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipx/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipx/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipx/packet.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,22 +49,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Packet(key)
         if key not in Packet._member_map_:  # pylint: disable=no-member
-            extend_enum(Packet, key, default)
+            return extend_enum(Packet, key, default)
         return Packet[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Packet':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ipx/socket.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ipx/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,41 +69,36 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Socket(key)
         if key not in Socket._member_map_:  # pylint: disable=no-member
-            extend_enum(Socket, key, default)
+            return extend_enum(Socket, key, default)
         return Socket[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Socket':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x0000 <= value <= 0xFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x0001 <= value <= 0x0BB8:
             #: Registered by Xerox
-            extend_enum(cls, 'Registered by Xerox_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Registered by Xerox_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x0020 <= value <= 0x003F:
             #: Experimental
-            extend_enum(cls, 'Experimental_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Experimental_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x0BB9 <= value <= 0xFFFF:
             #: Dynamically Assigned
-            extend_enum(cls, 'Dynamically Assigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Dynamically Assigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x4000 <= value <= 0x4FFF:
             #: Dynamically Assigned Socket Numbers
-            extend_enum(cls, 'Dynamically Assigned Socket Numbers_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Dynamically Assigned Socket Numbers_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8000 <= value <= 0xFFFF:
             #: Statically Assigned Socket Numbers
-            extend_enum(cls, 'Statically Assigned Socket Numbers_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Statically Assigned Socket Numbers_0x%s' % hex(value)[2:].upper().zfill(4), value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/l2tp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/l2tp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/l2tp/type.py` & `pypcapkit-1.0.0rc1/pcapkit/const/l2tp/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Type(key)
         if key not in Type._member_map_:  # pylint: disable=no-member
-            extend_enum(Type, key, default)
+            return extend_enum(Type, key, default)
         return Type[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Type':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/access_type.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/access_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,25 +69,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return AccessType(key)
         if key not in AccessType._member_map_:  # pylint: disable=no-member
-            extend_enum(AccessType, key, default)
+            return extend_enum(AccessType, key, default)
         return AccessType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'AccessType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 14 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/ack_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/ack_status_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ACKStatusCode(key)
         if key not in ACKStatusCode._member_map_:  # pylint: disable=no-member
-            extend_enum(ACKStatusCode, key, default)
+            return extend_enum(ACKStatusCode, key, default)
         return ACKStatusCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ACKStatusCode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 133 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/ani_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/ani_suboption.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return ANISuboption(key)
         if key not in ANISuboption._member_map_:  # pylint: disable=no-member
-            extend_enum(ANISuboption, key, default)
+            return extend_enum(ANISuboption, key, default)
         return ANISuboption[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'ANISuboption':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 7 <= value <= 254:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/auth_subtype.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/auth_subtype.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return AuthSubtype(key)
         if key not in AuthSubtype._member_map_:  # pylint: disable=no-member
-            extend_enum(AuthSubtype, key, default)
+            return extend_enum(AuthSubtype, key, default)
         return AuthSubtype[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'AuthSubtype':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/binding_ack_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/binding_revocation.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_revocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return BindingRevocation(key)
         if key not in BindingRevocation._member_map_:  # pylint: disable=no-member
-            extend_enum(BindingRevocation, key, default)
+            return extend_enum(BindingRevocation, key, default)
         return BindingRevocation[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'BindingRevocation':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/binding_update_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/binding_update_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/dhcp_support_mode.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/dhcp_support_mode.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,22 +33,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return DHCPSupportMode(key)
         if key not in DHCPSupportMode._member_map_:  # pylint: disable=no-member
-            extend_enum(DHCPSupportMode, key, default)
+            return extend_enum(DHCPSupportMode, key, default)
         return DHCPSupportMode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'DHCPSupportMode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 1):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/dns_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/dns_status_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return DNSStatusCode(key)
         if key not in DNSStatusCode._member_map_:  # pylint: disable=no-member
-            extend_enum(DNSStatusCode, key, default)
+            return extend_enum(DNSStatusCode, key, default)
         return DNSStatusCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'DNSStatusCode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 131 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/dsmip6_tls_packet.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmip6_tls_packet.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,29 +36,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return DSMIP6TLSPacket(key)
         if key not in DSMIP6TLSPacket._member_map_:  # pylint: disable=no-member
-            extend_enum(DSMIP6TLSPacket, key, default)
+            return extend_enum(DSMIP6TLSPacket, key, default)
         return DSMIP6TLSPacket[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'DSMIP6TLSPacket':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 15):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 2 <= value <= 7:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 9 <= value <= 15:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/dsmipv6_home_address.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/dsmipv6_home_address.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,29 +48,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return DSMIPv6HomeAddress(key)
         if key not in DSMIPv6HomeAddress._member_map_:  # pylint: disable=no-member
-            extend_enum(DSMIPv6HomeAddress, key, default)
+            return extend_enum(DSMIPv6HomeAddress, key, default)
         return DSMIPv6HomeAddress[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'DSMIPv6HomeAddress':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 134 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/enumerating_algorithm.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/enumerating_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return EnumeratingAlgorithm(key)
         if key not in EnumeratingAlgorithm._member_map_:  # pylint: disable=no-member
-            extend_enum(EnumeratingAlgorithm, key, default)
+            return extend_enum(EnumeratingAlgorithm, key, default)
         return EnumeratingAlgorithm[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'EnumeratingAlgorithm':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/fb_ack_status.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_ack_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,29 +36,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowBindingACKStatus(key)
         if key not in FlowBindingACKStatus._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowBindingACKStatus, key, default)
+            return extend_enum(FlowBindingACKStatus, key, default)
         return FlowBindingACKStatus[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowBindingACKStatus':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 130 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/fb_action.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_action.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,29 +45,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowBindingAction(key)
         if key not in FlowBindingAction._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowBindingAction, key, default)
+            return extend_enum(FlowBindingAction, key, default)
         return FlowBindingAction[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowBindingAction':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0 <= value <= 10:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 17 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/fb_indication_trigger.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_indication_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowBindingIndicationTrigger(key)
         if key not in FlowBindingIndicationTrigger._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowBindingIndicationTrigger, key, default)
+            return extend_enum(FlowBindingIndicationTrigger, key, default)
         return FlowBindingIndicationTrigger[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowBindingIndicationTrigger':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 4 <= value <= 249:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 250 <= value <= 255:
             #: Reserved for Testing Purposes Only [:rfc:`7109`]
-            extend_enum(cls, 'Reserved_for_Testing_Purposes_Only_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Testing_Purposes_Only_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/fb_type.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/fb_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,25 +36,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowBindingType(key)
         if key not in FlowBindingType._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowBindingType, key, default)
+            return extend_enum(FlowBindingType, key, default)
         return FlowBindingType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowBindingType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/flow_id_status.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,33 +48,30 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowIDStatus(key)
         if key not in FlowIDStatus._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowIDStatus, key, default)
+            return extend_enum(FlowIDStatus, key, default)
         return FlowIDStatus[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowIDStatus':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned; available for success codes
-            extend_enum(cls, 'Unassigned_available_for_success_codes_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_available_for_success_codes_%d' % value, value)
         if 134 <= value <= 250:
             #: Unassigned; available for reject codes
-            extend_enum(cls, 'Unassigned_available_for_reject_codes_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_available_for_reject_codes_%d' % value, value)
         if 251 <= value <= 255:
             #: Reserved for Experimental Use [:rfc:`6089`]
-            extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/flow_id_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/flow_id_suboption.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,29 +45,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return FlowIDSuboption(key)
         if key not in FlowIDSuboption._member_map_:  # pylint: disable=no-member
-            extend_enum(FlowIDSuboption, key, default)
+            return extend_enum(FlowIDSuboption, key, default)
         return FlowIDSuboption[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'FlowIDSuboption':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 6 <= value <= 250:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 251 <= value <= 255:
             #: Reserved for Experimental Use [:rfc:`6089`]
-            extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/handoff_type.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/handoff_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,25 +48,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return HandoffType(key)
         if key not in HandoffType._member_map_:  # pylint: disable=no-member
-            extend_enum(HandoffType, key, default)
+            return extend_enum(HandoffType, key, default)
         return HandoffType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'HandoffType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 7 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/handover_ack_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/handover_ack_status.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_ack_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,29 +66,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return HandoverACKStatus(key)
         if key not in HandoverACKStatus._member_map_:  # pylint: disable=no-member
-            extend_enum(HandoverACKStatus, key, default)
+            return extend_enum(HandoverACKStatus, key, default)
         return HandoverACKStatus[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'HandoverACKStatus':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 7 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 133 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/handover_initiate_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/handover_initiate_status.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/handover_initiate_status.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/home_address_reply.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/home_address_reply.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return HomeAddressReply(key)
         if key not in HomeAddressReply._member_map_:  # pylint: disable=no-member
-            extend_enum(HomeAddressReply, key, default)
+            return extend_enum(HomeAddressReply, key, default)
         return HomeAddressReply[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'HomeAddressReply':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 133 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/lma_mag_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/lma_mag_suboption.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return LMAControlledMAGSuboption(key)
         if key not in LMAControlledMAGSuboption._member_map_:  # pylint: disable=no-member
-            extend_enum(LMAControlledMAGSuboption, key, default)
+            return extend_enum(LMAControlledMAGSuboption, key, default)
         return LMAControlledMAGSuboption[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'LMAControlledMAGSuboption':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/mn_group_id.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ospf/packet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,consider-using-f-string
-"""Mobile Node Group Identifier Type Registry
-================================================
+"""OSPF Packet Types
+=======================
 
-.. module:: pcapkit.const.mh.mn_group_id
+.. module:: pcapkit.const.ospf.packet
 
-This module contains the constant enumeration for **Mobile Node Group Identifier Type Registry**,
-which is automatically generated from :class:`pcapkit.vendor.mh.mn_group_id.MNGroupID`.
+This module contains the constant enumeration for **OSPF Packet Types**,
+which is automatically generated from :class:`pcapkit.vendor.ospf.packet.Packet`.
 
 """
 
 from aenum import IntEnum, extend_enum
 
-__all__ = ['MNGroupID']
+__all__ = ['Packet']
 
 
-class MNGroupID(IntEnum):
-    """[MNGroupID] Mobile Node Group Identifier Type Registry"""
+class Packet(IntEnum):
+    """[Packet] OSPF Packet Types"""
 
-    #: Reserved [:rfc:`6602`]
+    #: Reserved
     Reserved_0 = 0
 
-    #: Bulk Binding Update Group [:rfc:`6602`]
-    Bulk_Binding_Update_Group = 1
+    #: Hello [:rfc:`2328`]
+    Hello = 1
 
-    #: Reserved [:rfc:`6602`]
-    Reserved_255 = 255
+    #: Database Description [:rfc:`2328`]
+    Database_Description = 2
+
+    #: Link State Request [:rfc:`2328`]
+    Link_State_Request = 3
+
+    #: Link State Update [:rfc:`2328`]
+    Link_State_Update = 4
+
+    #: Link State Ack [:rfc:`2328`]
+    Link_State_Ack = 5
 
     @staticmethod
-    def get(key: 'int | str', default: 'int' = -1) -> 'MNGroupID':
+    def get(key: 'int | str', default: 'int' = -1) -> 'Packet':
         """Backport support for original codes.
 
         Args:
             key: Key to get enum item.
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
-            return MNGroupID(key)
-        if key not in MNGroupID._member_map_:  # pylint: disable=no-member
-            extend_enum(MNGroupID, key, default)
-        return MNGroupID[key]  # type: ignore[misc]
+            return Packet(key)
+        if key not in Packet._member_map_:  # pylint: disable=no-member
+            return extend_enum(Packet, key, default)
+        return Packet[key]  # type: ignore[misc]
 
     @classmethod
-    def _missing_(cls, value: 'int') -> 'MNGroupID':
+    def _missing_(cls, value: 'int') -> 'Packet':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
-        if not (isinstance(value, int) and 0 <= value <= 255):
+        if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        if 2 <= value <= 254:
+        if 6 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
+        if 128 <= value <= 255:
+            #: Reserved
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/mn_id_subtype.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/mn_id_subtype.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,29 +51,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return MNIDSubtype(key)
         if key not in MNIDSubtype._member_map_:  # pylint: disable=no-member
-            extend_enum(MNIDSubtype, key, default)
+            return extend_enum(MNIDSubtype, key, default)
         return MNIDSubtype[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'MNIDSubtype':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 9 <= value <= 15:
             #: Reserved [:rfc:`8371`]
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         if 16 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/operator_id.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/operator_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,25 +40,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return OperatorID(key)
         if key not in OperatorID._member_map_:  # pylint: disable=no-member
-            extend_enum(OperatorID, key, default)
+            return extend_enum(OperatorID, key, default)
         return OperatorID[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'OperatorID':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 254:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/option.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,22 +240,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Option(key)
         if key not in Option._member_map_:  # pylint: disable=no-member
-            extend_enum(Option, key, default)
+            return extend_enum(Option, key, default)
         return Option[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Option':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,22 +99,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Packet(key)
         if key not in Packet._member_map_:  # pylint: disable=no-member
-            extend_enum(Packet, key, default)
+            return extend_enum(Packet, key, default)
         return Packet[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Packet':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/qos_attribute.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/qos_attribute.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,25 +66,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return QoSAttribute(key)
         if key not in QoSAttribute._member_map_:  # pylint: disable=no-member
-            extend_enum(QoSAttribute, key, default)
+            return extend_enum(QoSAttribute, key, default)
         return QoSAttribute[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'QoSAttribute':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 12 <= value <= 254:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/revocation_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_status_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,29 +39,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return RevocationStatusCode(key)
         if key not in RevocationStatusCode._member_map_:  # pylint: disable=no-member
-            extend_enum(RevocationStatusCode, key, default)
+            return extend_enum(RevocationStatusCode, key, default)
         return RevocationStatusCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'RevocationStatusCode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 131 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/revocation_trigger.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/revocation_trigger.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,33 +57,30 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return RevocationTrigger(key)
         if key not in RevocationTrigger._member_map_:  # pylint: disable=no-member
-            extend_enum(RevocationTrigger, key, default)
+            return extend_enum(RevocationTrigger, key, default)
         return RevocationTrigger[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'RevocationTrigger':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 8 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 130 <= value <= 249:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 250 <= value <= 255:
             #: Reserved for Testing Purposes Only [:rfc:`5846`]
-            extend_enum(cls, 'Reserved_for_Testing_Purposes_Only_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Testing_Purposes_Only_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/status_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,31 +39,29 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return StatusCode(key)
         if key not in StatusCode._member_map_:  # pylint: disable=no-member
-            extend_enum(StatusCode, key, default)
+            return extend_enum(StatusCode, key, default)
         return StatusCode[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'StatusCode':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 131 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         #: Unspecified in the IANA registry
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
+        return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/traffic_selector.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/traffic_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,29 +36,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return TrafficSelector(key)
         if key not in TrafficSelector._member_map_:  # pylint: disable=no-member
-            extend_enum(TrafficSelector, key, default)
+            return extend_enum(TrafficSelector, key, default)
         return TrafficSelector[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'TrafficSelector':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 3 <= value <= 250:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 251 <= value <= 255:
             #: Reserved for Experimental Use [:rfc:`6089`]
-            extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_for_Experimental_Use_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/upa_status.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/upa_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,29 +45,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return UpdateNotificationACKStatus(key)
         if key not in UpdateNotificationACKStatus._member_map_:  # pylint: disable=no-member
-            extend_enum(UpdateNotificationACKStatus, key, default)
+            return extend_enum(UpdateNotificationACKStatus, key, default)
         return UpdateNotificationACKStatus[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'UpdateNotificationACKStatus':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 1 <= value <= 127:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 133 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/mh/upn_reason.py` & `pypcapkit-1.0.0rc1/pcapkit/const/mh/upn_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,24 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return UpdateNotificationReason(key)
         if key not in UpdateNotificationReason._member_map_:  # pylint: disable=no-member
-            extend_enum(UpdateNotificationReason, key, default)
+            return extend_enum(UpdateNotificationReason, key, default)
         return UpdateNotificationReason[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'UpdateNotificationReason':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 9 <= value <= 254:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ospf/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ospf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/ospf/authentication.py` & `pypcapkit-1.0.0rc1/pcapkit/const/ospf/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,29 +39,27 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Authentication(key)
         if key not in Authentication._member_map_:  # pylint: disable=no-member
-            extend_enum(Authentication, key, default)
+            return extend_enum(Authentication, key, default)
         return Authentication[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Authentication':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 65535):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 4 <= value <= 255:
             #: Unassigned
-            extend_enum(cls, 'Unassigned_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Unassigned_%d' % value, value)
         if 256 <= value <= 65535:
             #: Deprecated [:rfc:`6549`]
-            extend_enum(cls, 'Deprecated_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Deprecated_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/pcapng/block_type.py` & `pypcapkit-1.0.0rc1/pcapkit/const/pcapng/block_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,41 +117,36 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return BlockType(key)
         if key not in BlockType._member_map_:  # pylint: disable=no-member
-            extend_enum(BlockType, key, default)
+            return extend_enum(BlockType, key, default)
         return BlockType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'BlockType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 0xFFFFFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x0a0d0a00 <= value <= 0x0a0d0aff:
-           #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
-            extend_enum(cls, 'Reserved_%08x' % value, value)
-            return cls(value)
+            #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
+            return extend_enum(cls, 'Reserved_%08x' % value, value)
         if 0x000a0d0a <= value <= 0xff0a0d0a:
-           #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
-            extend_enum(cls, 'Reserved_%08x' % value, value)
-            return cls(value)
+            #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
+            return extend_enum(cls, 'Reserved_%08x' % value, value)
         if 0x000a0d0d <= value <= 0xff0a0d0d:
-           #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
-            extend_enum(cls, 'Reserved_%08x' % value, value)
-            return cls(value)
+            #: Reserved. Used to detect trace files corrupted because of file transfers using the HTTP protocol in text mode.
+            return extend_enum(cls, 'Reserved_%08x' % value, value)
         if 0x0d0d0a00 <= value <= 0x0d0d0aff:
-           #: Reserved. Used to detect trace files corrupted because of file transfers using the FTP protocol in text mode.
-            extend_enum(cls, 'Reserved_%08x' % value, value)
-            return cls(value)
+            #: Reserved. Used to detect trace files corrupted because of file transfers using the FTP protocol in text mode.
+            return extend_enum(cls, 'Reserved_%08x' % value, value)
         if 0x80000000 <= value <= 0xffffffff:
-           #: Reserved for local use.
-            extend_enum(cls, 'Reserved_%08x' % value, value)
-            return cls(value)
+            #: Reserved for local use.
+            return extend_enum(cls, 'Reserved_%08x' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/reg/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/reg/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/reg/ethertype.py` & `pypcapkit-1.0.0rc1/pcapkit/const/reg/ethertype.py`

 * *Files 15% similar despite different names*

```diff
@@ -519,245 +519,189 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return EtherType(key)
         if key not in EtherType._member_map_:  # pylint: disable=no-member
-            extend_enum(EtherType, key, default)
+            return extend_enum(EtherType, key, default)
         return EtherType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'EtherType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x0000 <= value <= 0xFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 0x0000 <= value <= 0x05DC:
             #: IEEE802.3 Length Field [Neil Sembower]
-            extend_enum(cls, 'IEEE802_3_Length_Field_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'IEEE802_3_Length_Field_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x0101 <= value <= 0x01FF:
             #: Experimental [Neil Sembower]
-            extend_enum(cls, 'Experimental_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Experimental_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x0888 <= value <= 0x088A:
             #: Xyplex [Neil Sembower]
-            extend_enum(cls, 'Xyplex_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Xyplex_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x1001 <= value <= 0x100F:
             #: Berkeley Trailer encap/IP [Neil Sembower]
-            extend_enum(cls, 'Berkeley_Trailer_encap_IP_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Berkeley_Trailer_encap_IP_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x6008 <= value <= 0x6009:
             #: DEC Unassigned [Neil Sembower]
-            extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x6010 <= value <= 0x6014:
             #: 3Com Corporation [Neil Sembower]
-            extend_enum(cls, 'EtherType_3Com_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'EtherType_3Com_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x7020 <= value <= 0x7029:
             #: LRT [Neil Sembower]
-            extend_enum(cls, 'LRT_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'LRT_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8039 <= value <= 0x803C:
             #: DEC Unassigned [Neil Sembower]
-            extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8040 <= value <= 0x8042:
             #: DEC Unassigned [Neil Sembower]
-            extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'DEC_Unassigned_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x806E <= value <= 0x8077:
             #: Landmark Graphics Corp. [Neil Sembower]
-            extend_enum(cls, 'Landmark_Graphics_Corp_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Landmark_Graphics_Corp_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x807D <= value <= 0x807F:
             #: Vitalink Communications [Neil Sembower]
-            extend_enum(cls, 'Vitalink_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Vitalink_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8081 <= value <= 0x8083:
             #: Counterpoint Computers [Neil Sembower]
-            extend_enum(cls, 'Counterpoint_Computers_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Counterpoint_Computers_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x809C <= value <= 0x809E:
             #: Datability [Neil Sembower]
-            extend_enum(cls, 'Datability_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Datability_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80A4 <= value <= 0x80B3:
             #: Siemens Gammasonics Inc. [Neil Sembower]
-            extend_enum(cls, 'Siemens_Gammasonics_Inc_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Siemens_Gammasonics_Inc_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80C0 <= value <= 0x80C3:
             #: DCA Data Exchange Cluster [Neil Sembower]
-            extend_enum(cls, 'DCA_Data_Exchange_Cluster_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'DCA_Data_Exchange_Cluster_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80C8 <= value <= 0x80CC:
             #: Intergraph Corporation [Neil Sembower]
-            extend_enum(cls, 'Intergraph_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Intergraph_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80CD <= value <= 0x80CE:
             #: Harris Corporation [Neil Sembower]
-            extend_enum(cls, 'Harris_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Harris_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80CF <= value <= 0x80D2:
             #: Taylor Instrument [Neil Sembower]
-            extend_enum(cls, 'Taylor_Instrument_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Taylor_Instrument_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80D3 <= value <= 0x80D4:
             #: Rosemount Corporation [Neil Sembower]
-            extend_enum(cls, 'Rosemount_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Rosemount_Corporation_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80DE <= value <= 0x80DF:
             #: Integrated Solutions TRFS [Neil Sembower]
-            extend_enum(cls, 'Integrated_Solutions_TRFS_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Integrated_Solutions_TRFS_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80E0 <= value <= 0x80E3:
             #: Allen-Bradley [Neil Sembower]
-            extend_enum(cls, 'Allen_Bradley_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Allen_Bradley_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80E4 <= value <= 0x80F0:
             #: Datability [Neil Sembower]
-            extend_enum(cls, 'Datability_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Datability_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x80F4 <= value <= 0x80F5:
             #: Kinetics [Neil Sembower]
-            extend_enum(cls, 'Kinetics_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Kinetics_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8101 <= value <= 0x8103:
             #: Wellfleet Communications [Neil Sembower]
-            extend_enum(cls, 'Wellfleet_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Wellfleet_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8107 <= value <= 0x8109:
             #: Symbolics Private [Neil Sembower]
-            extend_enum(cls, 'Symbolics_Private_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Symbolics_Private_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8132 <= value <= 0x8136:
             #: Bridge Communications [Neil Sembower]
-            extend_enum(cls, 'Bridge_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Bridge_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8137 <= value <= 0x8138:
             #: Novell, Inc. [Neil Sembower]
-            extend_enum(cls, 'Novell_Inc_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Novell_Inc_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8139 <= value <= 0x813D:
             #: KTI [Neil Sembower]
-            extend_enum(cls, 'KTI_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'KTI_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8151 <= value <= 0x8153:
             #: Qualcomm [Neil Sembower]
-            extend_enum(cls, 'Qualcomm_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Qualcomm_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x815C <= value <= 0x815E:
             #: Computer Protocol Pty Ltd [Neil Sembower]
-            extend_enum(cls, 'Computer_Protocol_Pty_Ltd_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Computer_Protocol_Pty_Ltd_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8164 <= value <= 0x8166:
             #: Charles River Data System [Neil Sembower]
-            extend_enum(cls, 'Charles_River_Data_System_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Charles_River_Data_System_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8184 <= value <= 0x818C:
             #: Silicon Graphics prop. [Neil Sembower]
-            extend_enum(cls, 'Silicon_Graphics_prop_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Silicon_Graphics_prop_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x819A <= value <= 0x81A3:
             #: Qualcomm [Neil Sembower]
-            extend_enum(cls, 'Qualcomm_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Qualcomm_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81A5 <= value <= 0x81AE:
             #: RAD Network Devices [Neil Sembower]
-            extend_enum(cls, 'RAD_Network_Devices_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'RAD_Network_Devices_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81B7 <= value <= 0x81B9:
             #: Xyplex [Neil Sembower]
-            extend_enum(cls, 'Xyplex_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Xyplex_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81CC <= value <= 0x81D5:
             #: Apricot Computers [Neil Sembower]
-            extend_enum(cls, 'Apricot_Computers_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Apricot_Computers_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81D6 <= value <= 0x81DD:
             #: Artisoft [Neil Sembower]
-            extend_enum(cls, 'Artisoft_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Artisoft_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81E6 <= value <= 0x81EF:
             #: Polygon [Neil Sembower]
-            extend_enum(cls, 'Polygon_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Polygon_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81F0 <= value <= 0x81F2:
             #: Comsat Labs [Neil Sembower]
-            extend_enum(cls, 'Comsat_Labs_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Comsat_Labs_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81F3 <= value <= 0x81F5:
             #: SAIC [Neil Sembower]
-            extend_enum(cls, 'SAIC_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'SAIC_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x81F6 <= value <= 0x81F8:
             #: VG Analytical [Neil Sembower]
-            extend_enum(cls, 'VG_Analytical_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'VG_Analytical_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8203 <= value <= 0x8205:
             #: Quantum Software [Neil Sembower]
-            extend_enum(cls, 'Quantum_Software_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Quantum_Software_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8221 <= value <= 0x8222:
             #: Ascom Banking Systems [Neil Sembower]
-            extend_enum(cls, 'Ascom_Banking_Systems_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Ascom_Banking_Systems_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x823E <= value <= 0x8240:
             #: Advanced Encryption Syste [Neil Sembower]
-            extend_enum(cls, 'Advanced_Encryption_Syste_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Advanced_Encryption_Syste_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x827F <= value <= 0x8282:
             #: Athena Programming [Neil Sembower]
-            extend_enum(cls, 'Athena_Programming_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Athena_Programming_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8263 <= value <= 0x826A:
             #: Charles River Data System [Neil Sembower]
-            extend_enum(cls, 'Charles_River_Data_System_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Charles_River_Data_System_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x829A <= value <= 0x829B:
             #: Inst Ind Info Tech [Neil Sembower]
-            extend_enum(cls, 'Inst_Ind_Info_Tech_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Inst_Ind_Info_Tech_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x829C <= value <= 0x82AB:
             #: Taurus Controls [Neil Sembower]
-            extend_enum(cls, 'Taurus_Controls_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Taurus_Controls_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x82AC <= value <= 0x8693:
             #: Walker Richer & Quinn [Neil Sembower]
-            extend_enum(cls, 'Walker_Richer_Quinn_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Walker_Richer_Quinn_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8694 <= value <= 0x869D:
             #: Idea Courier [Neil Sembower]
-            extend_enum(cls, 'Idea_Courier_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Idea_Courier_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x869E <= value <= 0x86A1:
             #: Computer Network Tech [Neil Sembower]
-            extend_enum(cls, 'Computer_Network_Tech_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Computer_Network_Tech_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x86A3 <= value <= 0x86AC:
             #: Gateway Communications [Neil Sembower]
-            extend_enum(cls, 'Gateway_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Gateway_Communications_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x86E0 <= value <= 0x86EF:
             #: Landis & Gyr Powers [Neil Sembower]
-            extend_enum(cls, 'Landis_Gyr_Powers_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Landis_Gyr_Powers_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8700 <= value <= 0x8710:
             #: Motorola [Neil Sembower]
-            extend_enum(cls, 'Motorola_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Motorola_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0x8A96 <= value <= 0x8A97:
             #: Invisible Software [Neil Sembower]
-            extend_enum(cls, 'Invisible_Software_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'Invisible_Software_0x%s' % hex(value)[2:].upper().zfill(4), value)
         if 0xFF00 <= value <= 0xFF0F:
             #: ISC Bunker Ramo [Neil Sembower]
-            extend_enum(cls, 'ISC_Bunker_Ramo_0x%s' % hex(value)[2:].upper().zfill(4), value)
-            return cls(value)
+            return extend_enum(cls, 'ISC_Bunker_Ramo_0x%s' % hex(value)[2:].upper().zfill(4), value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/reg/linktype.py` & `pypcapkit-1.0.0rc1/pcapkit/const/reg/linktype.py`

 * *Files 0% similar despite different names*

```diff
@@ -904,22 +904,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return LinkType(key)
         if key not in LinkType._member_map_:  # pylint: disable=no-member
-            extend_enum(LinkType, key, default)
+            return extend_enum(LinkType, key, default)
         return LinkType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'LinkType':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0x00000000 <= value <= 0xFFFFFFFF):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/reg/transtype.py` & `pypcapkit-1.0.0rc1/pcapkit/const/reg/transtype.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return TransType(key)
         if key not in TransType._member_map_:  # pylint: disable=no-member
-            extend_enum(TransType, key, default)
+            return extend_enum(TransType, key, default)
         return TransType[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'TransType':
         """Lookup function used when value is not found.
 
         Args:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/tcp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/tcp/checksum.py` & `pypcapkit-1.0.0rc1/pcapkit/const/tcp/checksum.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Checksum(key)
         if key not in Checksum._member_map_:  # pylint: disable=no-member
-            extend_enum(Checksum, key, default)
+            return extend_enum(Checksum, key, default)
         return Checksum[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Checksum':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/tcp/mp_tcp_option.py` & `pypcapkit-1.0.0rc1/pcapkit/const/tcp/mp_tcp_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,22 +43,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return MPTCPOption(key)
         if key not in MPTCPOption._member_map_:  # pylint: disable=no-member
-            extend_enum(MPTCPOption, key, default)
+            return extend_enum(MPTCPOption, key, default)
         return MPTCPOption[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'MPTCPOption':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned_%d' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned_%d' % value, value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/tcp/option.py` & `pypcapkit-1.0.0rc1/pcapkit/const/tcp/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,37 +167,33 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return Option(key)
         if key not in Option._member_map_:  # pylint: disable=no-member
-            extend_enum(Option, key, default)
+            return extend_enum(Option, key, default)
         return Option[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'Option':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0 <= value <= 255):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         if 35 <= value <= 68:
             #: Reserved
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         if 71 <= value <= 75:
             #: Reserved
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         if 79 <= value <= 171:
             #: Reserved
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         if 175 <= value <= 252:
             #: Reserved
-            extend_enum(cls, 'Reserved_%d' % value, value)
-            return cls(value)
+            return extend_enum(cls, 'Reserved_%d' % value, value)
         return super()._missing_(value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/vlan/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/const/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/const/vlan/priority_level.py` & `pypcapkit-1.0.0rc1/pcapkit/const/vlan/priority_level.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,22 +51,21 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return PriorityLevel(key)
         if key not in PriorityLevel._member_map_:  # pylint: disable=no-member
-            extend_enum(PriorityLevel, key, default)
+            return extend_enum(PriorityLevel, key, default)
         return PriorityLevel[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> 'PriorityLevel':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not (isinstance(value, int) and 0b000 <= value <= 0b111):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'Unassigned [0b%s]' % bin(value)[2:].zfill(3), value)
-        return cls(value)
+        return extend_enum(cls, 'Unassigned [0b%s]' % bin(value)[2:].zfill(3), value)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,9 +43,10 @@
     'PaddingField',
 
     'ConditionalField', 'PayloadField', 'SchemaField',
     'ForwardMatchField', 'NoValueField',
 
     'ListField', 'OptionField',
 
-    'IPv4Field', 'IPv6Field',
+    'IPv4AddressField', 'IPv6AddressField',
+    'IPv4InterfaceField', 'IPv6InterfaceField',
 ]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 descriptive of the structure of protocol headers.
 
 """
 
 from pcapkit.corekit.fields.field import Field
 
 from pcapkit.corekit.fields.collections import ListField, OptionField
-from pcapkit.corekit.fields.ipaddress import IPv4Field, IPv6Field
+from pcapkit.corekit.fields.ipaddress import (IPv4AddressField, IPv4InterfaceField,
+                                              IPv6AddressField, IPv6InterfaceField)
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, NoValueField,
                                          PayloadField, SchemaField)
 from pcapkit.corekit.fields.numbers import (EnumField, Int8Field, Int16Field, Int32Field,
                                             Int64Field, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field, UInt64Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField, StringField
 
@@ -35,9 +36,10 @@
     'PaddingField',
 
     'ConditionalField', 'PayloadField', 'SchemaField',
     'ForwardMatchField', 'NoValueField',
 
     'ListField', 'OptionField',
 
-    'IPv4Field', 'IPv6Field',
+    'IPv4AddressField', 'IPv6AddressField',
+    'IPv4InterfaceField', 'IPv6InterfaceField',
 ]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/collections.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 if TYPE_CHECKING:
     from collections import defaultdict
     from enum import IntEnum as StdlibEnum
     from typing import IO, Any, Callable, Optional, Type
 
     from aenum import IntEnum as AenumEnum
+    from typing_extensions import Self
 
     from pcapkit.protocols.schema.schema import Schema
 
 _TL = TypeVar('_TL', 'Schema', '_Field', 'bytes')
 
 
 class ListField(_Field[List[_TL]]):
@@ -38,32 +39,37 @@
 
     This field is used to represent a list of fields, as in the case of lists of
     constrant-length-field items in a protocol.
 
     """
 
     @property
+    def length(self) -> 'int':
+        """Field size."""
+        return self._length
+
+    @property
     def optional(self) -> 'bool':
         """Field is optional."""
         return True
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]' = lambda _: -1,
                  item_type: 'Optional[_Field]' = None,
-                 callback: 'Callable[[ListField, dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         self._name = '<list>'
         self._callback = callback
         self._item_type = item_type
 
         self._length_callback = None
         if not isinstance(length, int):
             self._length_callback, length = length, -1
         self._length = length
         self._template = '0s'
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'ListField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             Updated field instance.
@@ -116,28 +122,28 @@
             buffer: Field buffer.
             packet: Packet data.
 
         Returns:
             Unpacked field value.
 
         """
-        length = self.length
+        length = self._length
         if isinstance(buffer, bytes):
             file = io.BytesIO(buffer)  # type: IO[bytes]
         else:
             file = buffer
 
         if self._item_type is None:
             return file.read(length)
 
         from pcapkit.corekit.fields.misc import SchemaField
         is_schema = isinstance(self._item_type, SchemaField)
 
         temp = []  # type: list[_TL]
-        while length:
+        while length > 0:
             field = self._item_type(packet)
 
             if is_schema:
                 data = cast('SchemaField', self._item_type).unpack(file, packet)
 
                 length -= len(data)
                 if length < 0:
@@ -190,23 +196,29 @@
         return self._registry
 
     @property
     def eool(self) -> 'int | StdlibEnum | AenumEnum':
         """EOOL option."""
         return self._eool
 
+    @property
+    def option_padding(self) -> 'int':
+        """Length option padding data."""
+        return self._option_padding
+
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]' = lambda _: -1,
                  base_schema: 'Optional[Type[Schema]]' = None,
                  type_name: 'str' = 'type',
                  registry: 'Optional[defaultdict[int | StdlibEnum | AenumEnum, Type[Schema]]]' = None,
                  eool: 'Optional[int | StdlibEnum | AenumEnum]' = None,
-                 callback: 'Callable[[ListField, dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         super().__init__(length, None, callback)
         self._name = '<option>'
         self._eool = eool
+        self._option_padding = 0
 
         if base_schema is None:
             raise FieldValueError('Field <option> has no base schema.')
         self._base_schema = base_schema
 
         if not hasattr(self._base_schema, type_name):
             raise FieldValueError(f'Field <option> has no type field "{type_name}".')
@@ -222,42 +234,49 @@
         Args:
             buffer: Field buffer.
             packet: Packet data.
 
         Returns:
             Unpacked field value.
 
+        Important:
+            If the option list ended before the specified size limit,
+            set :attr:`self.option_padding <OptionField.option_padding>` as the remaining length to
+            the ``packet`` argument such that the next fields can be
+            aware of such informations.
+
         """
-        length = self.length
+        length = self._length
         if isinstance(buffer, bytes):
             file = io.BytesIO(buffer)  # type: IO[bytes]
         else:
             file = buffer
 
         # make a copy of the ``packet`` dict so that we can include
         # parsed option schema in the ``packet`` dict
         new_packet = packet.copy()
         new_packet[self.name] = OrderedMultiDict()
 
         temp = []  # type: list[Schema]
-        while length:
+        while length > 0:
             # unpack option type using base schema
-            meta = self._base_schema.unpack(file, length, packet)  # type: ignore[call-arg,misc]
+            meta = self._base_schema.unpack(file, length, packet)  # type: ignore[call-arg,misc,var-annotated]
             code = cast('int', meta[self._type_name])
             schema = self._registry[code]
 
             # rewind to the beginning of the option
             file.seek(-len(meta), io.SEEK_CUR)
 
             # unpack option using option schema
-            data = schema.unpack(file, length, packet)  # type: ignore[call-arg,misc]
+            data = schema.unpack(file, length, packet)  # type: ignore[call-arg,misc,var-annotated]
             new_packet[self.name].add(code, data)
             temp.append(data)
 
             # update length
             length -= len(data)
 
             # check for EOOL
             if code == self._eool:
-                packet['__option_padding__'] = length
                 break
+
+        self._option_padding = length
         return temp
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/field.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pcapkit.utilities.exceptions import NoDefaultValue
 
 __all__ = ['Field']
 
 if TYPE_CHECKING:
     from typing import IO, Any, Callable, Optional
 
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Self
 
 _T = TypeVar('_T')
 
 
 @final
 class NoValueType:
     """Default value for fields."""
@@ -29,20 +29,29 @@
 
 
 #: NoValueType: Default value for :attr:`_Field.default`.
 NoValue = NoValueType()
 
 
 class _Field(Generic[_T], metaclass=abc.ABCMeta):
-    """Internal base class for protocol fields."""
+    """Internal base class for protocol fields.
+
+    Important:
+        A negative value of :attr:`~_Field.length` indicates that the field
+        is variable-length (i.e., length unspecified) and thus
+        :meth:`~_Field.pack` should be considerate of the template format
+        and the actual value provided for packing.
+
+    """
 
     if TYPE_CHECKING:
         _name: 'str'
         _default: '_T | NoValueType'
         _template: 'str'
+        _callback: 'Callable[[Self, dict[str, Any]], None]'
 
     @property
     def name(self) -> 'str':
         """Field name."""
         return self._name
 
     @name.setter
@@ -76,30 +85,30 @@
         return struct.calcsize(self.template)
 
     @property
     def optional(self) -> 'bool':
         """Field is optional."""
         return False
 
-    def __call__(self, packet: 'dict[str, Any]') -> '_Field':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Arguments:
             packet: Packet data.
 
         Returns:
             Updated field instance.
 
         Notes:
             This method will return a new instance of :class:`_Field` instead of
             updating the current instance.
 
         """
         new_self = copy.copy(self)
-        new_self._callback(new_self, packet)  # type: ignore[attr-defined]
+        new_self._callback(new_self, packet)
         return new_self
 
     def __repr__(self) -> 'str':
         if not self.name.isidentifier():
             return f'<{self.__class__.__name__}>'
         return f'<{self.__class__.__name__} {self.name}>'
 
@@ -181,32 +190,27 @@
         _template: 'str'
 
     @property
     def template(self) -> 'str':
         """Field template."""
         return self._template
 
-    @property
-    def length(self) -> 'int':
-        """Field size."""
-        return struct.calcsize(self.template)
-
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]',
                  default: '_T | NoValueType' = NoValue,
-                 callback: 'Callable[[Field[_T], dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         self._name = '<unknown>'
         self._default = default
         self._callback = callback
 
         self._length_callback = None
         if not isinstance(length, int):
-            self._length_callback, length = length, 0
+            self._length_callback, length = length, -1
         self._length = length
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'Field':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             New instance of :class:`Field`.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/misc.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,27 +13,31 @@
     'SwitchField', 'ForwardMatchField',
     'NoValueField',
 ]
 
 if TYPE_CHECKING:
     from typing import IO, Any, Callable, Optional, Type
 
+    from typing_extensions import Self
+
     from pcapkit.corekit.fields.field import NoValueType
     from pcapkit.protocols.protocol import Protocol
     from pcapkit.protocols.schema.schema import Schema
 
 _TC = TypeVar('_TC')
 _TS = TypeVar('_TS', bound='Schema')
 _TP = TypeVar('_TP', bound='Protocol')
 _TN = TypeVar('_TN', bound='NoValueType')
 
 
 class NoValueField(_Field[_TN]):
     """Schema field for no value type (or :obj:`None`)."""
 
+    _default = NoValue
+
     @property
     def template(self) -> 'str':
         """Field template."""
         return '0s'
 
     @property
     def length(self) -> 'int':
@@ -124,15 +128,15 @@
         return self._field
 
     def __init__(self, field: '_Field[_TC]',  # pylint: disable=super-init-not-called
                  condition: 'Callable[[dict[str, Any]], bool]') -> 'None':
         self._field = field  # type: _Field[_TC]
         self._condition = condition
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'ConditionalField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Arguments:
             packet: Packet data.
 
         Returns:
             Updated field instance.
@@ -140,15 +144,15 @@
         Notes:
             This method will return a new instance of :class:`ConditionalField`
             instead of updating the current instance.
 
         """
         new_self = copy.copy(self)
         if new_self._condition(packet):
-            new_self._field(packet)
+            new_self._field = new_self._field(packet)
         return new_self
 
     def pre_process(self, value: '_TC', packet: 'dict[str, Any]') -> 'Any':  # pylint: disable=unused-argument
         """Process field value before construction (packing).
 
         Arguments:
             value: Field value.
@@ -264,27 +268,27 @@
             from pcapkit.protocols import __proto__  # pylint: disable=import-outside-top-level
             protocol = cast('Type[_TP]', __proto__.get(protocol))
         self._protocol = protocol
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]' = lambda _: -1,
                  default: '_TP | NoValueType | bytes' = NoValue,
                  protocol: 'Optional[Type[_TP]]' = None,
-                 callback: 'Callable[[PayloadField[_TP], dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         self._name = '<payload>'
         self._default = default  # type: ignore[assignment]
         self._protocol = protocol  # type: ignore[assignment]
         self._callback = callback
 
         self._length_callback = None
         if not isinstance(length, int):
-            self._length_callback, length = length, 0
+            self._length_callback, length = length, -1
         self._length = length
-        self._template = f'{self._length}s' if self._length else '1024s'  # use a reasonable default
+        self._template = f'{self._length}s' if self._length >= 0 else '1024s'  # use a reasonable default
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'PayloadField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             Updated field instance.
@@ -341,27 +345,74 @@
                 return cast('_TP', buffer)
             return cast('_TP', buffer.read())
 
         if isinstance(buffer, bytes):
             file = io.BytesIO(buffer)  # type: IO[bytes]
         else:
             file = buffer
-        return self._protocol(file, self.length)  # type: ignore[abstract]
+
+        length = self._length if self._length > 0 else None
+        return self._protocol(file, length)  # type: ignore[abstract]
 
 
 class SwitchField(_Field[_TC]):
-    """Conditional type-switching field for protocol schema."""
+    """Conditional type-switching field for protocol schema.
+
+    Args:
+        selector: Callable function to select field type, which should accept
+            the current packet as its only argument and return a field instance.
+
+    """
+
+    @property
+    def name(self) -> 'str':
+        """Field name."""
+        return self._field.name
+
+    @name.setter
+    def name(self, value: 'str') -> 'None':
+        """Set field name."""
+        self._field.name = value
+
+    @property
+    def default(self) -> '_TC | NoValueType':
+        """Field default value."""
+        return self._field.default
+
+    @default.setter
+    def default(self, value: '_TC | NoValueType') -> 'None':
+        """Set field default value."""
+        self._field.default = value
+
+    @default.deleter
+    def default(self) -> 'None':
+        """Delete field default value."""
+        self._field.default = NoValue
+
+    @property
+    def template(self) -> 'str':
+        """Field template."""
+        return self._field.template
+
+    @property
+    def length(self) -> 'int':
+        """Field size."""
+        return self._field.length
 
     @property
     def optional(self) -> 'bool':
         """Field is optional."""
         return True
 
-    def __init__(self, length: 'int | Callable[[dict[str, Any]], int]' = lambda _: -1,
-                 selector: 'Callable[[dict[str, Any]], _Field[_TC]]' = lambda _: NoValueField()) -> 'None':  # type: ignore[assignment,return-value]
+    @property
+    def field(self) -> '_Field[_TC]':
+        """Field instance."""
+        return self._field
+
+    def __init__(self, selector: 'Callable[[dict[str, Any]], _Field[_TC]]' = lambda _: NoValueField()) -> 'None':  # type: ignore[assignment,return-value]
         self._name = '<switch>'
         self._field = cast('_Field[_TC]', NoValueField())
         self._selector = selector
 
     def __call__(self, packet: 'dict[str, Any]') -> 'SwitchField[_TC]':
         """Call field.
 
@@ -373,16 +424,16 @@
 
         Notes:
             This method will return a new instance of :class:`SwitchField`
             instead of updating the current instance.
 
         """
         new_self = copy.copy(self)
-        new_self._field = self._selector(packet)
-        new_self._template = new_self._field.template
+        new_self._field = new_self._selector(packet)(packet)
+        new_self._field.name = self.name
         return new_self
 
     def pre_process(self, value: '_TC', packet: 'dict[str, Any]') -> 'Any':  # pylint: disable=unused-argument
         """Process field value before construction (packing).
 
         Arguments:
             value: Field value.
@@ -439,48 +490,69 @@
         """
         if self._field is None:
             return None  # type: ignore[unreachable]
         return self._field.unpack(buffer, packet)
 
 
 class SchemaField(_Field[_TS]):
-    """Schema field for protocol schema."""
+    """Schema field for protocol schema.
+
+    Args:
+        length: Field size (in bytes); if a callable is given, it should return
+            an integer value and accept the current packet as its only argument.
+        schema: Field schema.
+        default: Default value for field.
+        packet: Optional packet data for unpacking and/or packing purposes.
+        callback: Callback function to process field value, which should accept
+            the current field and the current packet as its arguments.
+
+    """
+
+    @property
+    def length(self) -> 'int':
+        """Field size."""
+        return self._length  # type: ignore[has-type]
 
     @property
     def optional(self) -> 'bool':
         """Field is optional."""
         return True
 
     @property
     def schema(self) -> 'Type[_TS]':
         """Field schema."""
         return self._schema
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]' = lambda _: -1,
                  schema: 'Optional[Type[_TS]]' = None,
                  default: '_TS | NoValueType | bytes' = NoValue,
-                 callback: 'Callable[[SchemaField[_TS], dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 packet: 'Optional[dict[str, Any]]' = None,
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         self._name = '<schema>'
         self._callback = callback
 
+        if packet is None:
+            packet = {}
+        self._packet = packet
+
         if schema is None:
             raise FieldError('Schema field must have a schema.')
         self._schema = schema
 
         if isinstance(default, bytes):
             default = cast('_TS', schema.unpack(default))  # type: ignore[call-arg,misc]
         self._default = default
 
         self._length_callback = None
         if not isinstance(length, int):
-            self._length_callback, length = length, 0
+            self._length_callback, length = length, -1
         self._length = length
-        self._template = f'{self._length}s' if self._length else '1024s'  # use a reasonable default
+        self._template = f'{self._length}s' if self._length >= 0 else '1024s'  # use a reasonable default
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'SchemaField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             New field instance.
@@ -490,53 +562,71 @@
             instead of updating the current instance.
 
         """
         new_self = copy.copy(self)
         new_self._callback(new_self, packet)
         if new_self._length_callback is not None:
             new_self._length = new_self._length_callback(packet)
-            new_self._template = f'{new_self._length}s'
+            new_self._template = f'{new_self._length}s' if self._length >= 0 else '1024s'  # use a reasonable default
         return new_self
 
     def pack(self, value: 'Optional[_TS | bytes]', packet: 'dict[str, Any]') -> 'bytes':
         """Pack field value into :obj:`bytes`.
 
         Args:
             value: Field value.
             packet: Packet data.
 
         Returns:
             Packed field value.
 
+        Notes:
+            We will use ``packet`` as a ``__packet__`` key in the packet context
+            passed to the underlying :class:`~pcapkit.protocols.schema.schema.Schema`
+            for packing purposes.
+
         """
         if value is None:
             if self._default is NoValue:
                 raise NoDefaultValue(f'Field {self.name} has no default value.')
             value = cast('_TS', self._default)
 
         if isinstance(value, bytes):
             return value
-        return value.pack(packet)
+
+        packet.update(self._packet)
+        return value.pack({
+            '__packet__': packet,
+        })
 
     def unpack(self, buffer: 'bytes | IO[bytes]', packet: 'dict[str, Any]') -> '_TS':
         """Unpack field value from :obj:`bytes`.
 
         Args:
             buffer: Field buffer.
             packet: Packet data.
 
         Returns:
             Unpacked field value.
 
+        Notes:
+            We will use ``packet`` as a ``__packet__`` key in the packet context
+            passed to the underlying :class:`~pcapkit.protocols.schema.schema.Schema`
+            for unpacking purposes.
+
         """
         if isinstance(buffer, bytes):
             file = io.BytesIO(buffer)  # type: IO[bytes]
         else:
             file = buffer
-        return cast('_TS', self._schema.unpack(file, self.length, packet))  # type: ignore[call-arg,misc]
+
+        packet.update(self._packet)
+        return cast('_TS', self._schema.unpack(file, self.length, {  # type: ignore[call-arg,misc]
+            '__packet__': packet,
+        }))
 
 
 class ForwardMatchField(_Field[_TC]):
     """Schema field for non-capturing forward matching.
 
     Args:
         field: Field to forward match.
@@ -588,14 +678,32 @@
         """Field instance."""
         return self._field
 
     def __init__(self, field: '_Field[_TC]') -> 'None':
         self._name = '<forward_match>'
         self._field = field
 
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
+        """Update field attributes.
+
+        Arguments:
+            packet: Packet data.
+
+        Returns:
+            Updated field instance.
+
+        Notes:
+            This method will return a new instance of :class:`ConditionalField`
+            instead of updating the current instance.
+
+        """
+        new_self = copy.copy(self)
+        new_self._field = new_self._field(packet)
+        return new_self
+
     def pack(self, value: 'Optional[_TC]', packet: 'dict[str, Any]') -> 'bytes':
         """Pack field value into :obj:`bytes`.
 
         Args:
             value: Field value.
             packet: Packet data.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/numbers.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/numbers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """numerical field class"""
 
-import copy
 import enum
+import math
 from typing import TYPE_CHECKING, Generic, TypeVar, cast
 
 import aenum
 
 from pcapkit.corekit.fields.field import Field, NoValue
 from pcapkit.utilities.exceptions import IntError
 
@@ -20,15 +20,15 @@
 ]
 
 if TYPE_CHECKING:
     from enum import IntEnum as StdlibEnum
     from typing import Any, Callable, Optional, Type
 
     from aenum import IntEnum as AenumEnum
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Self
 
     from pcapkit.corekit.fields.field import NoValueType
 
 _T = TypeVar('_T', bound='int')
 
 
 class NumberField(Field[int], Generic[_T]):
@@ -55,53 +55,57 @@
         """Field bit length."""
         return self._bit_length
 
     def __init__(self, length: 'Optional[int | Callable[[dict[str, Any]], int]]' = None,
                  default: 'int | NoValueType' = NoValue, signed: 'bool' = False,
                  byteorder: 'Literal["little", "big"]' = 'big',
                  bit_length: 'Optional[int]' = None,
-                 callback: 'Callable[[NumberField[_T], dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         if length is None:
             if self.__length__ is None:
                 raise IntError(f'Field has no length.')
             length = self.__length__
-        super().__init__(length, default, callback)  # type: ignore[arg-type]
+        super().__init__(length, default, callback)
 
-        if bit_length is None:
-            bit_length = self._length * 8
-        self._bit_length = bit_length
-        self._bit_mask = (1 << bit_length) - 1
+        if bit_length is not None:
+            self._bit_length = bit_length
+            self._bit_mask = (1 << bit_length) - 1
+        else:
+            self._bit_length, self._bit_mask = -1, -1
 
         self._signed = signed if self.__signed__ is None else self.__signed__
         self._byteorder = byteorder
         self._need_process = False
 
         endian = '>' if byteorder == 'big' else '<'
         if self.__template__ is not None:
             struct_fmt = self.__template__
         else:
             struct_fmt = self.build_template(self._length, signed)
         self._template = f'{endian}{struct_fmt}'
 
-    def __call__(self, packet: 'dict[str, Any]') -> 'NumberField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             New instance of :class:`NumberField`.
 
         Notes:
             This method will return a new instance of :class:`NumberField` instead of
             updating the current instance.
 
         """
-        new_self = copy.copy(self)
-        new_self._callback(new_self, packet)
+        new_self = super().__call__(packet)
+
+        if new_self._bit_length < 0:
+            new_self._bit_length = new_self._length * 8
+            new_self._bit_mask = (1 << new_self._bit_length) - 1
 
         endian = '>' if new_self._byteorder == 'big' else '<'
         struct_fmt = new_self.build_template(new_self._length, new_self._signed)
 
         new_self._template = f'{endian}{struct_fmt}'
         return new_self
 
@@ -139,14 +143,23 @@
         Returns:
             Processed field value.
 
         """
         value = value & self._bit_mask
         if not self._need_process:
             return value
+
+        if self._length < 0:
+            self._length = math.ceil(value.bit_length() // 8)
+
+            endian = '>' if self._byteorder == 'big' else '<'
+            struct_fmt = self.build_template(self._length, self._signed)
+
+            self._template = f'{endian}{struct_fmt}'
+
         return value.to_bytes(
             self._length, self._byteorder, signed=self._signed
         )
 
     def post_process(self, value: 'int | bytes', packet: 'dict[str, Any]') -> 'int':  # pylint: disable=unused-argument
         """Process field value after parsing (unpacked).
 
@@ -334,16 +347,16 @@
     """
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]',
                  default: 'StdlibEnum | AenumEnum | NoValueType' = NoValue, signed: 'bool' = False,
                  byteorder: 'Literal["little", "big"]' = 'big',
                  bit_length: 'Optional[int]' = None,
                  namespace: 'Optional[Type[StdlibEnum] | Type[AenumEnum]]' = None,
-                 callback: 'Callable[[EnumField, dict[str, Any]], None]' = lambda *_: None) -> 'None':
-        super().__init__(length, default, signed, byteorder, bit_length, callback)  # type: ignore[arg-type]
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
+        super().__init__(length, default, signed, byteorder, bit_length, callback)
 
         self._namespace = namespace
 
     def post_process(self, value: 'int | bytes', packet: 'dict[str, Any]') -> 'StdlibEnum | AenumEnum':
         """Process field value after parsing (unpacked).
 
         Args:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/fields/strings.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/fields/strings.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'BitField',
     'PaddingField',
 ]
 
 if TYPE_CHECKING:
     from typing import Callable, Optional, Tuple
 
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Self
 
     from pcapkit.corekit.fields.field import NoValueType
 
     NamespaceEntry = Tuple[int, int]
 
 _T = TypeVar('_T', 'str', 'bytes', 'dict[str, Any]')
 
@@ -38,34 +38,34 @@
         callback: Callback function to be called upon
             :meth:`self.__call__ <pcapkit.corekit.fields.field._Field.__call__>`.
 
     """
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]',
                  default: '_T | NoValueType' = NoValue,
-                 callback: 'Callable[[_TextField[_T], dict[str, Any]], None]' = lambda *_: None) -> 'None':
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
         super().__init__(length, default, callback)  # type: ignore[arg-type]
 
-        self._template = f'{self._length}s'
+        self._template = f'{self._length}s' if self._length >= 0 else '1024s'  # reasonable default
 
-    def __call__(self, packet: 'dict[str, Any]') -> '_TextField':
+    def __call__(self, packet: 'dict[str, Any]') -> 'Self':
         """Update field attributes.
 
         Args:
             packet: Packet data.
 
         Returns:
             New instance of :class:`_TextField`.
 
         Notes:
             This method will return a new instance of :class:`_TextField` instead of
             updating the current instance.
 
         """
-        new_self = cast('_TextField', super().__call__(packet))
+        new_self = super().__call__(packet)
         new_self._template = f'{new_self._length}s'
         return new_self
 
 
 class BytesField(_TextField[bytes]):
     """Bytes value for protocol fields.
 
@@ -74,14 +74,30 @@
             an integer value and accept the current packet as its only argument.
         default: Field default value, if any.
         callback: Callback function to be called upon
             :meth:`self.__call__ <pcapkit.corekit.fields.field._Field.__call__>`.
 
     """
 
+    def pre_process(self, value: 'bytes', packet: 'dict[str, Any]') -> 'bytes':  # pylint: disable=unused-argument
+        """Process field value before construction (packing).
+
+        Arguments:
+            value: Field value.
+            packet: Packet data.
+
+        Returns:
+            Processed field value.
+
+        """
+        if self._length < 0:
+            self._length = len(value)
+            self._template = f'{self._length}s'
+        return value
+
 
 class StringField(_TextField[str]):
     r"""String value for protocol fields.
 
     Args:
         length: Field size (in bytes); if a callable is given, it should return
             an integer value and accept the current packet as its only argument.
@@ -105,16 +121,16 @@
 
     """
 
     def __init__(self, length: 'int | Callable[[dict[str, Any]], int]',
                  default: 'str | NoValueType' = NoValue, encoding: 'Optional[str]' = None,
                  errors: 'Literal["strict", "ignore", "replace"]' = 'strict',
                  unquote: 'bool' = False,
-                 callback: 'Callable[[StringField, dict[str, Any]], None]' = lambda *_: None) -> 'None':
-        super().__init__(length, default, callback)  # type: ignore[arg-type]
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
+        super().__init__(length, default, callback)
 
         self._encoding = encoding
         self._errors = errors
         self._unquote = unquote
 
     def pre_process(self, value: 'str', packet: 'dict[str, Any]') -> 'bytes':  # pylint: disable=unused-argument
         """Process field value before construction (packing).
@@ -125,14 +141,18 @@
 
         Returns:
             Processed field value.
 
         """
         if self._unquote:
             value = urllib_parse.quote(value, encoding=self._encoding or 'utf-8', errors=self._errors)
+
+        if self._length < 0:
+            self._length = len(value)
+            self._template = f'{self._length}s'
         return value.encode(self._encoding or 'utf-8', self._errors)
 
     def post_process(self, value: 'bytes', packet: 'dict[str, Any]') -> 'str':  # pylint: disable=unused-argument
         """Process field value after parsing (unpacked).
 
         Arguments:
             value: Field value.
@@ -156,29 +176,28 @@
         return ret
 
 
 class BitField(_TextField[Dict[str, Any]]):
     """Bit value for protocol fields.
 
     Args:
-        length: Field size (in bytes); if a callable is given, it should return
-            an integer value and accept the current packet as its only argument.
+        length: Field size (in bytes).
         default: Field default value, if any.
         namespace: Field namespace (a dict mapping field name to a tuple of start index,
             and length of the subfield).
         callback: Callback function to be called upon
             :meth:`self.__call__ <pcapkit.corekit.fields.field._Field.__call__>`.
 
     """
 
-    def __init__(self, length: 'int | Callable[[dict[str, Any]], int]',
+    def __init__(self, length: 'int',
                  default: 'dict[str, Any] | NoValueType' = NoValue,
                  namespace: 'Optional[dict[str, NamespaceEntry]]' = None,
-                 callback: 'Callable[[BitField, dict[str, Any]], None]' = lambda *_: None) -> 'None':
-        super().__init__(length, default, callback)  # type: ignore[arg-type]
+                 callback: 'Callable[[Self, dict[str, Any]], None]' = lambda *_: None) -> 'None':
+        super().__init__(length, default, callback)
 
         self._namespace = namespace or {}
 
     def pre_process(self, value: 'dict[str, Any]', packet: 'dict[str, Any]') -> 'bytes':  # pylint: disable=unused-argument
         """Process field value before construction (packing).
 
         Arguments:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/infoclass.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/infoclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from pcapkit.utilities.compat import Mapping
 from pcapkit.utilities.exceptions import UnsupportedCall
 
 if TYPE_CHECKING:
     from typing import Any, Iterable, Iterator, NoReturn, Optional
 
+    from typing_extensions import Self
+
 __all__ = ['Info']
 
 VT = TypeVar('VT')
 
 
 class Info(Mapping[str, VT], Generic[VT]):
     """Turn dictionaries into :obj:`object` like instances.
@@ -54,15 +56,15 @@
         __builtin__: 'set[str]'
 
     #: List of additional built-in names.
     __additional__: 'list[str]' = []
     #: List of names to be excluded from :obj:`dict` conversion.
     __excluded__: 'list[str]' = []
 
-    def __new__(cls, *args: 'VT', **kwargs: 'VT') -> 'Info':  # pylint: disable=unused-argument
+    def __new__(cls, *args: 'VT', **kwargs: 'VT') -> 'Self':  # pylint: disable=unused-argument
         """Create a new instance.
 
         The class will try to automatically generate ``__init__`` method with
         the same signature as specified in class variables' type annotations,
         which is inspired by :pep:`557` (:mod:`dataclasses`).
 
         Args:
@@ -112,21 +114,23 @@
             if args_:
                 # NOTE: The following code is to make the ``__init__`` method work.
                 # It is inspired from the :func:`dataclasses._create_fn` function.
                 init_ = (
                     f'def __create_fn__():\n'
                     f'    def __init__(self, {", ".join(args_)}):\n'
                     f'        self.__update__({", ".join(dict_)})\n'
+                    f'        self.__post_init__()\n'
                     f'    return __init__\n'
                 )
             else:
                 init_ = (
                     'def __create_fn__():\n'
                     '    def __init__(self, dict_=None, **kwargs):\n'
                     '        self.__update__(dict_, **kwargs)\n'
+                    '        self.__post_init__()\n'
                     '    return __init__\n'
                 )
 
             ns = {}  # type: dict[str, Any]
             exec(init_, None, ns)  # pylint: disable=exec-used # nosec
             cls.__init__ = ns['__create_fn__']()
             cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
@@ -137,14 +141,17 @@
         # here under ``self`` to avoid them being considered as class variables
         # and thus being shared by all instances.
         super().__setattr__(self, '__map__', {})
         super().__setattr__(self, '__map_reverse__', {})
 
         return self
 
+    def __post_init__(self) -> 'None':
+        """Customisation method to be called after initialisation."""
+
     def __update__(self, dict_: 'Optional[Mapping[str, VT] | Iterable[tuple[str, VT]]]' = None,
                    **kwargs: 'VT') -> 'None':
         # NOTE: Keys with the same names as the class's builtin methods will be
         # renamed with the class name prefixed as mangled class variables
         # implicitly and internally. Such mapping information will be stored
         # within: attr: `__map__` attribute.
 
@@ -220,15 +227,15 @@
         raise UnsupportedCall("can't set attribute")
 
     def __delattr__(self, name: 'str') -> 'NoReturn':
         raise UnsupportedCall("can't delete attribute")
 
     @classmethod
     def from_dict(cls, dict_: 'Optional[Mapping[str, VT] | Iterable[tuple[str, VT]]]' = None,
-                  **kwargs: 'VT') -> 'Info[VT]':
+                  **kwargs: 'VT') -> 'Self':
         r"""Create a new instance.
 
         * If ``dict_`` is present and has a ``.keys()`` method, then does:
           ``for k in dict_: self[k] = dict_[k]``.
         * If ``dict_`` is present and has no ``.keys()`` method, then does:
           ``for k, v in dict_: self[k] = v``.
         * If ``dict_`` is not present, then does:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/multidict.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/multidict.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         for key, value in mapping.items():
             if isinstance(value, (tuple, list)):
                 for v in value:
                     yield key, v
             else:
                 yield key, value
     else:
-        yield from mapping
+        yield from mapping  # type: ignore[misc]
 
 
 ###############################################################################
 # Data structures
 ###############################################################################
 
 
@@ -176,15 +176,15 @@
             KeyError: if the key does not exist.
 
         """
         if key in self:
             lst = dict.__getitem__(self, key)
             if len(lst) > 0:
                 return lst[0]
-        raise MissingKeyError(key)
+        raise MissingKeyError(key, quiet=True)
 
     def __setitem__(self, key: '_KT', value: '_VT') -> 'None':
         """Like :meth:`add` but removes an existing key first.
 
         Args:
             key: The key for the value.
             value: The value to set.
@@ -507,15 +507,15 @@
         dict.clear(self)
         for key, value in values:
             self.add(key, value)
 
     def __getitem__(self, key: '_KT') -> '_VT':
         if key in self:
             return dict.__getitem__(self, key)[0].value
-        raise MissingKeyError(key)
+        raise MissingKeyError(key, quiet=True)
 
     def __setitem__(self, key: '_KT', value: '_VT') -> 'None':
         self.poplist(key)
         self.add(key, value)
 
     def __delitem__(self, key: '_KT') -> 'None':
         self.pop(key)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/corekit/protochain.py` & `pypcapkit-1.0.0rc1/pcapkit/corekit/protochain.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from pcapkit.utilities.compat import cached_property
 from pcapkit.utilities.exceptions import IndexNotFound
 
 if TYPE_CHECKING:
     from typing import Iterator, Optional, Type
 
+    from typing_extensions import Self
+
     from pcapkit.protocols.protocol import Protocol
 
 __all__ = ['ProtoChain']
 
 
 class ProtoChain(collections.abc.Sequence):
     """Protocols chain."""
@@ -49,15 +51,15 @@
         return self.__str__()
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
     @classmethod
-    def from_list(cls, data: 'list[Protocol | Type[Protocol]]') -> 'ProtoChain':
+    def from_list(cls, data: 'list[Protocol | Type[Protocol]]') -> 'Self':
         """Create a protocol chain from a list.
 
         Args:
             data: Protocol chain list.
 
         """
         from pcapkit.protocols.protocol import Protocol  # pylint: disable=import-outside-toplevel
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/dumpkit/null.py` & `pypcapkit-1.0.0rc1/pcapkit/dumpkit/null.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/dumpkit/pcap.py` & `pypcapkit-1.0.0rc1/pcapkit/dumpkit/pcap.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 __all__ = [
     'Extractor',
     'IPv4_Reassembly', 'IPv6_Reassembly', 'TCP_Reassembly',
     'TCP_TraceFlow',
 
     'register_protocol',
 
-    'register_linktype', 'register_pcap',
+    'register_linktype', 'register_pcap', 'register_pcapng',
     'register_ethertype', 'register_transtype',
     'register_port', 'register_tcp_port', 'register_udp_port',
 
     'register_output',
     'register_extractor_dumper', 'register_extractor_engine',
     'register_traceflow',
 
+    'register_pcapng_block', 'register_pcapng_option', 'register_pcapng_secrets',
+    'register_pcapng_record',
     'register_hopopt', 'register_ipv6_opts', 'register_ipv6_route',
     'register_ipv4', 'register_hip',
     'register_tcp', 'register_mptcp',
     'register_http',
 ]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/dpkt.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/dpkt.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 .. _DPKT: https://dpkt.readthedocs.io
 
 """
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.reg.linktype import LinkType as Enum_LinkType
 from pcapkit.foundation.engines.engine import Engine
-from pcapkit.utilities.exceptions import stacklevel
+from pcapkit.utilities.exceptions import FormatError, stacklevel
 from pcapkit.utilities.warnings import AttributeWarning, DPKTWarning, warn
 
 __all__ = ['DPKT']
 
 if TYPE_CHECKING:
-    from typing import Iterator
+    from typing import Optional, Type, Union
 
     from dpkt.dpkt import Packet as DPKTPacket
+    from dpkt.pcap import Reader as PCAPReader
+    from dpkt.pcapng import Reader as PCAPNGReader
 
     from pcapkit.foundation.extraction import Extractor
 
+    Reader = Union[PCAPReader, PCAPNGReader]
+
 
 class DPKT(Engine['DPKTPacket']):
     """DPKT engine support.
 
     Args:
         extractor: :class:`~pcapkit.foundation.extraction.Extractor` instance.
 
@@ -53,15 +57,15 @@
     # Data models.
     ##########################################################################
 
     def __init__(self, extractor: 'Extractor') -> 'None':
         import dpkt  # isort:skip
 
         self._expkg = dpkt
-        self._extmp = cast('Iterator[tuple[float, DPKTPacket]]', None)
+        self._extmp = cast('Reader', None)
 
         super().__init__(extractor)
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
@@ -72,15 +76,22 @@
         :attr:`self._extmp <Extractor._extmp>` as an iterator from :class:`dpkt.pcap.Reader`.
 
         Warns:
             AttributeWarning: If :attr:`self._exlyr <Extractor._exlyr>` and/or
                 :attr:`self._exptl <Extractor._exptl>` is provided as the DPKT
                 engine currently does not support such operations.
 
+        Raises:
+            FormatError: If the file format is not supported, i.e., not a PCAP
+                file.
+
         """
+        from pcapkit.foundation.engines.pcap import PCAP
+        from pcapkit.foundation.engines.pcapng import PCAPNG
+
         ext = self._extractor
         dpkt = self._expkg
 
         if ext._exlyr != 'none' or ext._exptl != 'null':
             warn("'Extractor(engine=dpkt)' does not support protocol and layer threshold; "
                  f"'layer={ext._exlyr}' and 'protocol={ext._exptl}' ignored",
                  AttributeWarning, stacklevel=stacklevel())
@@ -88,44 +99,23 @@
         # setup verbose handler
         if ext._flag_v:
             from pcapkit.toolkit.dpkt import packet2chain  # isort:skip
             ext._vfunc = lambda e, f: print(
                 f'Frame {e._frnum:>3d}: {packet2chain(f)}'  # pylint: disable=protected-access
             )  # pylint: disable=logging-fstring-interpolation
 
-        # extract global header
-        ext.record_header()
-
-        if ext._dlink == Enum_LinkType.ETHERNET:
-            pkg = dpkt.ethernet.Ethernet
-        elif ext._dlink.value == Enum_LinkType.IPV4:
-            pkg = dpkt.ip.IP
-        elif ext._dlink.value == Enum_LinkType.IPV6:
-            pkg = dpkt.ip6.IP6
+        if ext.magic_number in PCAP.MAGIC_NUMBER:
+            reader = dpkt.pcap.Reader(ext._ifile)
+        elif ext.magic_number in PCAPNG.MAGIC_NUMBER:
+            reader = dpkt.pcapng.Reader(ext._ifile)
         else:
-            warn('unrecognised link layer protocol; all analysis functions ignored',
-                 DPKTWarning, stacklevel=stacklevel())
-
-            class RawPacket(dpkt.dpkt.Packet):  # type: ignore[name-defined]
-                """Raw packet."""
-
-                def __len__(ext) -> 'int':
-                    return len(ext.data)
-
-                def __bytes__(ext) -> 'bytes':
-                    return ext.data
-
-                def unpack(ext, buf: 'bytes') -> 'None':
-                    ext.data = buf
-
-            pkg = RawPacket
+            raise FormatError(f'unsupported file format: {ext.magic_number!r}')
 
         # extract & analyse file
-        self._expkg = pkg
-        self._extmp = iter(dpkt.pcap.Reader(ext._ifile))
+        self._extmp = reader
 
     def read_frame(self) -> 'DPKTPacket':
         """Read frames with DPKT engine.
 
         Returns:
             dpkt.dpkt.Packet: Parsed frame instance.
 
@@ -133,31 +123,37 @@
             Please refer to :meth:`_default_read_frame` for more operational information.
 
         """
         from pcapkit.toolkit.dpkt import (ipv4_reassembly, ipv6_reassembly, packet2dict,
                                           tcp_reassembly, tcp_traceflow)
         ext = self._extractor
 
+        reader = self._extmp
+        linktype = Enum_LinkType.get(reader.datalink())
+
         # fetch DPKT packet
-        timestamp, pkt = cast('tuple[float, bytes]', next(self._extmp))
-        packet = self._expkg(pkt)  # type: DPKTPacket
+        timestamp, pkt = cast('tuple[float, bytes]', next(reader))
+        protocol = self._get_protocol(linktype)
+        packet = protocol(pkt)  # type: DPKTPacket
 
         # verbose output
         ext._frnum += 1
         ext._vfunc(ext, packet)
 
         # write plist
         frnum = f'Frame {ext._frnum}'
         if not ext._flag_q:
-            info = packet2dict(packet, timestamp, data_link=ext._dlink)
+            info = packet2dict(packet, timestamp, data_link=linktype)
             if ext._flag_f:
                 ofile = ext._ofile(f'{ext._ofnm}/{frnum}.{ext._fext}')
                 ofile(info, name=frnum)
             else:
                 ext._ofile(info, name=frnum)
+                ofile = ext._ofile
+            ext._offmt = ofile.kind
 
         # record fragments
         if ext._flag_r:
             if ext._ipv4:
                 data_ipv4 = ipv4_reassembly(packet, count=ext._frnum)
                 if data_ipv4 is not None:
                     ext._reasm.ipv4(data_ipv4)
@@ -169,19 +165,61 @@
                 data_tcp = tcp_reassembly(packet, count=ext._frnum)
                 if data_tcp is not None:
                     ext._reasm.tcp(data_tcp)
 
         # trace flows
         if ext._flag_t:
             if ext._tcp:
-                data_tf_tcp = tcp_traceflow(packet, timestamp, data_link=ext._dlink, count=ext._frnum)
+                data_tf_tcp = tcp_traceflow(packet, timestamp, data_link=linktype, count=ext._frnum)
                 if data_tf_tcp is not None:
                     ext._trace.tcp(data_tf_tcp)
 
         # record frames
         if ext._flag_d:
             # setattr(packet, 'packet2dict', packet2dict)
             # setattr(packet, 'packet2chain', packet2chain)
             ext._frame.append(packet)
 
         # return frame record
         return packet
+
+    ##########################################################################
+    # Utilities.
+    ##########################################################################
+
+    def _get_protocol(self, linktype: 'Optional[Enum_LinkType]' = None) -> 'Type[DPKTPacket]':
+        """Returns the protocol for parsing the current packet.
+
+        Args:
+            linktype: Link type code.
+
+        """
+        dpkt = self._expkg
+        reader = self._extmp
+
+        if linktype is None:
+            linktype = Enum_LinkType.get(reader.datalink())
+
+        if linktype == Enum_LinkType.ETHERNET:
+            pkg = dpkt.ethernet.Ethernet
+        elif linktype.value == Enum_LinkType.IPV4:
+            pkg = dpkt.ip.IP
+        elif linktype.value == Enum_LinkType.IPV6:
+            pkg = dpkt.ip6.IP6
+        else:
+            warn('unrecognised link layer protocol; all analysis functions ignored',
+                 DPKTWarning, stacklevel=stacklevel())
+
+            class RawPacket(dpkt.dpkt.Packet):  # type: ignore[name-defined]
+                """Raw packet."""
+
+                def __len__(ext) -> 'int':
+                    return len(ext.data)
+
+                def __bytes__(ext) -> 'bytes':
+                    return ext.data
+
+                def unpack(ext, buf: 'bytes') -> 'None':
+                    ext.data = buf
+
+            pkg = RawPacket
+        return pkg
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/engine.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/engine.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/pcap.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pcap.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,45 @@
 
 .. module:: pcapkit.foundation.engines.pcap
 
 This module contains the implementation for PCAP file extraction
 support, as is used by :class:`pcapkit.foundation.extraction.Extractor`.
 
 """
+from typing import TYPE_CHECKING
+
 from pcapkit.foundation.engines.engine import Engine
 from pcapkit.protocols.misc.pcap.frame import Frame
 from pcapkit.protocols.misc.pcap.header import Header
 
 __all__ = ['PCAP']
 
+if TYPE_CHECKING:
+    from pcapkit.const.reg.linktype import LinkType as Enum_LinkType
+    from pcapkit.corekit.version import VersionInfo
+
 
 class PCAP(Engine[Frame]):
     """PCAP file extraction support.
 
     Args:
         extractor: :class:`~pcapkit.foundation.extraction.Extractor` instance.
 
     """
 
+    if TYPE_CHECKING:
+        #: Global header.
+        _gbhdr: 'Header'
+        #: Version info.
+        _vinfo: 'VersionInfo'
+        #: Data link layer protocol.
+        _dlink: 'Enum_LinkType'
+        #: Nanosecond flag.
+        _nnsec: 'bool'
+
     MAGIC_NUMBER = (
         b'\xa1\xb2\x3c\x4d',
         b'\xa1\xb2\xc3\xd4',
         b'\x4d\x3c\xb2\xa1',
         b'\xd4\xc3\xb2\xa1',
     )
 
@@ -40,60 +56,68 @@
         return 'PCAP'
 
     @classmethod
     def module(cls) -> 'str':
         """Engine module name."""
         return 'pcapkit.foundation.engine.pcap'
 
+    @property
+    def header(self) -> 'Header':
+        """Global header."""
+        return self._gbhdr
+
+    @property
+    def version(self) -> 'VersionInfo':
+        """Version of input PCAP file."""
+        return self._vinfo
+
+    @property
+    def dlink(self) -> 'Enum_LinkType':
+        """Data link layer protocol."""
+        return self._dlink
+
     ##########################################################################
     # Methods.
     ##########################################################################
 
     def run(self) -> 'None':
         """Start extraction.
 
         This method is the entry point for PCAP file extraction. It will start
         the extraction process by parsing the PCAP global header and then halt
         the extraction process until the :meth:`self.extractor._read_frame <Extractor._read_frame>` method
         is called.
 
         The method will parse the PCAP global header and save the parsed result
-        as :attr:`self.extractor._gbhdr <Extractor._gbhdr>`. Information such as
-        PCAP version, data link layer protocol type, nanosecond flag and byteorder
-        will also be save the current :class:`Extractor` instance.
-
-        If TCP flow tracing is enabled, the nanosecond flag and byteorder will
-        be used for the output PCAP file of the traced TCP flows.
+        as :attr:`self._gbhdr <_gbhdr>`. Information such as PCAP version, data
+        link layer protocol type, nanosecond flag and byteorder will also be
+        save the current :class:`PCAP` engine instance.
 
         For output, the method will dump the parsed PCAP global header under
         the name of ``Global Header``.
 
         """
         # pylint: disable=attribute-defined-outside-init,protected-access
         ext = self._extractor
 
-        ext._gbhdr = Header(ext._ifile)
-        ext._vinfo = ext._gbhdr.version
-        ext._dlink = ext._gbhdr.protocol
-        ext._nnsec = ext._gbhdr.nanosecond
-
-        if ext._flag_t:
-            ext._trace._endian = ext._gbhdr.byteorder
-            ext._trace._nnsecd = ext._gbhdr.nanosecond
+        self._gbhdr = Header(ext._ifile)
+        self._vinfo = self._gbhdr.version
+        self._dlink = self._gbhdr.protocol
+        self._nnsec = self._gbhdr.nanosecond
 
         if ext._flag_q:
             return
 
         if ext._flag_f:
             ofile = ext._ofile(f'{ext._ofnm}/Global Header.{ext._fext}')
-            ofile(ext._gbhdr.info.to_dict(), name='Global Header')
+            ofile(self._gbhdr.info.to_dict(), name='Global Header')
         else:
-            ext._ofile(ext._gbhdr.info.to_dict(), name='Global Header')
+            ext._ofile(self._gbhdr.info.to_dict(), name='Global Header')
             ofile = ext._ofile
-        ext._type = ofile.kind
+        ext._offmt = ofile.kind
 
     def read_frame(self) -> 'Frame':
         """Read frames.
 
         This method performs following operations:
 
         - extract frames and each layer of packets;
@@ -103,21 +127,21 @@
         - trace TCP flows if any;
         - record frame :class:`~pcapkit.corekit.infoclass.Info` object to frame storage.
 
         Returns:
             Parsed frame instance.
 
         """
-        from pcapkit.toolkit.default import (ipv4_reassembly, ipv6_reassembly, tcp_reassembly,
-                                             tcp_traceflow)
+        from pcapkit.toolkit.pcap import (ipv4_reassembly, ipv6_reassembly, tcp_reassembly,
+                                          tcp_traceflow)
         ext = self._extractor
 
         # read frame header
-        frame = Frame(ext._ifile, num=ext._frnum+1, header=ext._gbhdr.info,
-                      layer=ext._exlyr, protocol=ext._exptl, nanosecond=ext._nnsec)
+        frame = Frame(ext._ifile, num=ext._frnum+1, header=self._gbhdr.info,
+                      layer=ext._exlyr, protocol=ext._exptl, nanosecond=self._nnsec)
         ext._frnum += 1
 
         # verbose output
         ext._vfunc(ext, frame)
 
         # write plist
         frnum = f'Frame {ext._frnum}'
@@ -142,15 +166,15 @@
                 data_tcp = tcp_reassembly(frame)
                 if data_tcp is not None:
                     ext._reasm.tcp(data_tcp)
 
         # trace flows
         if ext._flag_t:
             if ext._tcp:
-                data_tf_tcp = tcp_traceflow(frame, data_link=ext._dlink)
+                data_tf_tcp = tcp_traceflow(frame, data_link=self._dlink)
                 if data_tf_tcp is not None:
                     ext._trace.tcp(data_tf_tcp)
 
         # record frames
         if ext._flag_d:
             ext._frame.append(frame)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/pyshark.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/pyshark.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 This module contains the implementation for `PyShark`_ engine
 support, as is used by :class:`pcapkit.foundation.extraction.Extractor`.
 
 .. _PyShark: https://kiminewt.github.io/pyshark
 
 """
-#import os
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.foundation.engines.engine import Engine
 from pcapkit.foundation.reassembly import ReassemblyManager
 from pcapkit.utilities.exceptions import stacklevel
 from pcapkit.utilities.warnings import AttributeWarning, warn
 
@@ -97,18 +96,14 @@
 
         # setup verbose handler
         if ext._flag_v:
             ext._vfunc = lambda e, f: print(
                 f'Frame {e._frnum:>3d}: {f.frame_info.protocols}'  # pylint: disable=protected-access
             )  # pylint: disable=logging-fstring-interpolation
 
-        # extract global header
-        #ext.record_header()
-        #ext._ifile.seek(0, os.SEEK_SET)
-
         # extract & analyse file
         self._extmp = self._expkg.FileCapture(ext._ifnm, keep_packets=False)
 
     def read_frame(self) -> 'PySharkPacket':
         """Read frames with PyShark engine.
 
         Returns:
@@ -133,14 +128,16 @@
         if not ext._flag_q:
             info = packet2dict(packet)
             if ext._flag_f:
                 ofile = ext._ofile(f'{ext._ofnm}/{frnum}.{ext._fext}')
                 ofile(info, name=frnum)
             else:
                 ext._ofile(info, name=frnum)
+                ofile = ext._ofile
+            ext._offmt = ofile.kind
 
         # trace flows
         if ext._flag_t:
             if ext._tcp:
                 data_tf_tcp = tcp_traceflow(packet)
                 if data_tf_tcp is not None:
                     ext._trace.tcp(data_tf_tcp)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/engines/scapy.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/engines/scapy.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,14 @@
         # setup verbose handler
         if ext._flag_v:
             from pcapkit.toolkit.scapy import packet2chain  # isort:skip
             ext._vfunc = lambda e, f: print(
                 f'Frame {e._frnum:>3d}: {packet2chain(f)}'  # pylint: disable=protected-access
             )  # pylint: disable=logging-fstring-interpolation
 
-        # extract global header
-        ext.record_header()
-
         # extract & analyse file
         self._extmp = iter(self._expkg.sniff(offline=ext._ifnm))
 
     def read_frame(self) -> 'ScapyPacket':
         """Read frames with Scapy engine.
 
         Returns:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/extraction.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,131 +16,126 @@
 
 import collections
 import importlib
 import os
 import sys
 from typing import TYPE_CHECKING, Generic, TypeVar, cast
 
-from pcapkit.const.reg.linktype import LinkType as Enum_LinkType
-from pcapkit.dumpkit.common import _append_fallback as dumpkit_append_fallback
-from pcapkit.dumpkit.common import default as dumpkit_default
-from pcapkit.dumpkit.common import object_hook as dumpkit_object_hook
+from pcapkit.dumpkit.common import make_dumper
 from pcapkit.foundation.engines.pcap import PCAP as PCAP_Engine
+from pcapkit.foundation.engines.pcapng import PCAPNG as PCAPNG_Engine
 from pcapkit.foundation.reassembly import ReassemblyManager
 from pcapkit.foundation.traceflow import TraceFlowManager
-from pcapkit.protocols.misc.pcap.frame import Frame
-from pcapkit.protocols.misc.pcap.header import Header
 from pcapkit.utilities.exceptions import (CallableError, FileNotFound, FormatError, IterableError,
                                           UnsupportedCall, stacklevel)
 from pcapkit.utilities.warnings import EngineWarning, FormatWarning, warn
 
 if TYPE_CHECKING:
     from types import ModuleType, TracebackType
     from typing import IO, Any, Callable, DefaultDict, Optional, Type, Union
 
     from dictdumper.dumper import Dumper
     from dpkt.dpkt import Packet as DPKTPacket
     from pyshark.packet.packet import Packet as PySharkPacket
     from scapy.packet import Packet as ScapyPacket
     from typing_extensions import Literal
 
-    from pcapkit.corekit.version import VersionInfo
     from pcapkit.foundation.engines.engine import Engine
     from pcapkit.foundation.reassembly.data import ReassemblyData
     from pcapkit.foundation.traceflow.data import TraceFlowData
+    from pcapkit.protocols.misc.pcap.frame import Frame
+    from pcapkit.protocols.misc.pcapng import PCAPNG
     from pcapkit.protocols.protocol import Protocol
 
     Formats = Literal['pcap', 'json', 'tree', 'plist']
     Engines = Literal['default', 'pcapkit', 'dpkt', 'scapy', 'pyshark']
     Layers = Literal['link', 'internet', 'transport', 'application', 'none']
 
+    Packet = Union[Frame, PCAPNG, ScapyPacket, DPKTPacket, PySharkPacket]
+
     Protocols = Union[str, Protocol, Type[Protocol]]
-    VerboseHandler = Callable[['Extractor', Union[Frame, ScapyPacket, DPKTPacket, PySharkPacket]], Any]
+    VerboseHandler = Callable[['Extractor', Packet], Any]
 
 __all__ = ['Extractor']
 
 P = TypeVar('P')
 
 
 class Extractor(Generic[P]):
     """Extractor for PCAP files.
 
     Notes:
         For supported engines, please refer to
         :meth:`~pcapkit.foundation.extraction.Extractor.run`.
 
     """
-    #: Input file name.
-    _ifnm: 'str'
-    #: Output file name.
-    _ofnm: 'Optional[str]'
-    #: Output file extension.
-    _fext: 'Optional[str]'
-
-    #: Auto extract flag.
-    _flag_a: 'bool'
-    #: Store data flag.
-    _flag_d: 'bool'
-    #: EOF flag.
-    _flag_e: 'bool'
-    #: Split file flag.
-    _flag_f: 'bool'
-    #: No output file.
-    _flag_q: 'bool'
-    #: Trace flag.
-    _flag_t: 'bool'
-    #: Verbose flag.
-    _flag_v: 'bool'
-
-    #: Verbose callback function.
-    #_vfunc: 'VerboseHandler'
-
-    #: Frame number.
-    _frnum: 'int'
-    #: Frame records.
-    _frame: 'list[Frame | ScapyPacket | DPKTPacket]'
-
-    #: Frame record for reassembly.
-    _reasm: 'ReassemblyManager'
-    #: Flow tracer.
-    _trace: 'TraceFlowManager'
-
-    #: IPv4 reassembly flag.
-    _ipv4: 'bool'
-    #: IPv6 reassembly flag.
-    _ipv6: 'bool'
-    #: TCP reassembly flag.
-    _tcp: 'bool'
-
-    #: Extract til protocol.
-    _exptl: 'Protocols'
-    #: Extract til layer.
-    _exlyr: 'Layers'
-    #: Extraction engine name.
-    _exnam: 'Engines'
-    #: Extraction engine instance.
-    _exeng: 'Engine[P]'
-
-    #: Input file object.
-    _ifile: 'IO[bytes]'
-    #: Output file object.
-    _ofile: 'Dumper | Type[Dumper]'
-
-    #: Magic number.
-    _magic: 'bytes'
-    #: Global header.
-    _gbhdr: 'Header'
-    #: Version info.
-    _vinfo: 'VersionInfo'
-    #: Data link layer protocol.
-    _dlink: 'Enum_LinkType'
-    #: Nanosecond flag.
-    _nnsec: 'bool'
-    #: Output format.
-    _type: 'Formats'
+    if TYPE_CHECKING:
+        #: Input file name.
+        _ifnm: 'str'
+        #: Output file name.
+        _ofnm: 'Optional[str]'
+        #: Output file extension.
+        _fext: 'Optional[str]'
+
+        #: Auto extract flag.
+        _flag_a: 'bool'
+        #: Store data flag.
+        _flag_d: 'bool'
+        #: EOF flag.
+        _flag_e: 'bool'
+        #: Split file flag.
+        _flag_f: 'bool'
+        #: No output file.
+        _flag_q: 'bool'
+        #: Trace flag.
+        _flag_t: 'bool'
+        #: Verbose flag.
+        _flag_v: 'bool'
+
+        #: Verbose callback function.
+        #_vfunc: 'VerboseHandler'
+
+        #: Frame number.
+        _frnum: 'int'
+        #: Frame records.
+        _frame: 'list[Packet]'
+
+        #: Frame record for reassembly.
+        _reasm: 'ReassemblyManager'
+        #: Flow tracer.
+        _trace: 'TraceFlowManager'
+
+        #: IPv4 reassembly flag.
+        _ipv4: 'bool'
+        #: IPv6 reassembly flag.
+        _ipv6: 'bool'
+        #: TCP reassembly flag.
+        _tcp: 'bool'
+
+        #: Extract til protocol.
+        _exptl: 'Protocols'
+        #: Extract til layer.
+        _exlyr: 'Layers'
+        #: Extraction engine name.
+        _exnam: 'Engines'
+        #: Extraction engine instance.
+        _exeng: 'Engine[P]'
+
+        #: Input file object.
+        _ifile: 'IO[bytes]'
+        #: Output file object.
+        _ofile: 'Dumper | Type[Dumper]'
+
+        #: Magic number.
+        _magic: 'bytes'
+        #: Output format.
+        _offmt: 'Formats'
+
+    #: List of potential PCAP file extentions.
+    PCAP_EXT = ['.pcap', '.cap', '.pcapng']
 
     ##########################################################################
     # Defaults.
     ##########################################################################
 
     #: DefaultDict[str, tuple[str, str, str | None]]: Format dumper mapping for
     #: writing output files. The values should be a tuple representing the
@@ -158,37 +153,24 @@
             'txt': ('dictdumper', 'Tree', '.txt'),
         },
     )  # type: DefaultDict[str, tuple[str, str, str | None]]
 
     #: dict[str, tuple[str, str]]: Engine mapping for extracting frames.
     #: The values should be a tuple representing the module name and class name.
     __engine__ = {
-        'scapy': ('pcapkit.foundation.engine.scapy', 'Scapy'),
-        'dpkt': ('pcapkit.foundation.engine.dpkt', 'DPKT'),
-        'pyshark': ('pcapkit.foundation.engine.pyshark', 'PyShark'),
+        'scapy': ('pcapkit.foundation.engines.scapy', 'Scapy'),
+        'dpkt': ('pcapkit.foundation.engines.dpkt', 'DPKT'),
+        'pyshark': ('pcapkit.foundation.engines.pyshark', 'PyShark'),
     }  # type: dict[str, tuple[str, str]]
 
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
-    def info(self) -> 'VersionInfo':
-        """Version of input PCAP file.
-
-        Raises:
-            UnsupportedCall: If :attr:`self._exnam <pcapkit.foundation.extraction.Extractor._exnam>`
-                is ``'scapy'`` or ``'pyshark'``, as such engines does not reserve such information.
-
-        """
-        if self._exnam in ('scapy', 'pyshark'):
-            raise UnsupportedCall(f"'Extractor(engine={self._exnam})' object has no attribute 'info'")
-        return self._vinfo
-
-    @property
     def length(self) -> 'int':
         """Frame number (of current extracted frame or all)."""
         return self._frnum
 
     @property
     def format(self) -> 'Formats':
         """Format of output file.
@@ -196,15 +178,15 @@
         Raises:
             UnsupportedCall: If :attr:`self._flag_q <pcapkit.foundation.extraction.Extractor._flag_q>`
                 is set as :data:`True`, as output is disabled by initialisation parameter.
 
         """
         if self._flag_q:
             raise UnsupportedCall("'Extractor(nofile=True)' object has no attribute 'format'")
-        return self._type
+        return self._offmt
 
     @property
     def input(self) -> 'str':
         """Name of input PCAP file."""
         return self._ifnm
 
     @property
@@ -217,20 +199,15 @@
 
         """
         if self._flag_q:
             raise UnsupportedCall("'Extractor(nofile=True)' object has no attribute 'format'")
         return cast('str', self._ofnm)
 
     @property
-    def header(self) -> 'Header':
-        """Global header."""
-        return self._gbhdr
-
-    @property
-    def frame(self) -> 'tuple[Frame, ...]':
+    def frame(self) -> 'tuple[Packet, ...]':
         """Extracted frames.
 
         Raises:
             UnsupportedCall: If :attr:`self._flag_d <pcapkit.foundation.extraction.Extractor._flag_d>`
                 is :data:`True`, as storing frame data is disabled.
 
         """
@@ -263,14 +240,19 @@
         return data
 
     @property
     def engine(self) -> 'Engine':
         """PCAP extraction engine."""
         return self._exeng
 
+    @property
+    def magic_number(self) -> 'bytes':
+        """Magic number of input PCAP file."""
+        return self._magic
+
     ##########################################################################
     # Methods.
     ##########################################################################
 
     @classmethod
     def register_dumper(cls, format: 'str', module: 'str', class_: 'str', ext: 'str') -> 'None':
         r"""Register a new dumper class.
@@ -342,15 +324,22 @@
             self._exnam = 'default'  # using default/pcapkit engine
 
         if self._exnam not in ('default', 'pcapkit'):
             warn(f'unsupported extraction engine: {self._exnam}; '
                  'using default engine instead', EngineWarning, stacklevel=stacklevel())
             self._exnam = 'default'  # using default/pcapkit engine
 
-        self._exeng = cast('Engine[P]', PCAP_Engine(self))
+        if self._magic in PCAP_Engine.MAGIC_NUMBER:
+            self._exeng = cast('Engine[P]', PCAP_Engine(self))
+        elif self._magic in PCAPNG_Engine.MAGIC_NUMBER:
+            self._exeng = cast('Engine[P]', PCAPNG_Engine(self))
+        else:
+            raise FormatError(f'unknown file format: {self._magic!r}')
+
+        # start engine
         self._exeng.run()
 
         # start iteration
         self.record_frames()
 
     @staticmethod
     def import_test(engine: 'str', *, name: 'Optional[str]' = None) -> 'Optional[ModuleType]':
@@ -417,15 +406,15 @@
 
         Raises:
             FileNotFound: If input file does not exists.
             FormatError: If output format not provided and cannot be presumpted.
 
         """
         if extension:  # pylint: disable=else-if-used
-            ifnm = fin if os.path.splitext(fin)[1] == '.pcap' else f'{fin}.pcap'
+            ifnm = fin if os.path.splitext(fin)[1] in cls.PCAP_EXT else f'{fin}.pcap'
         else:
             ifnm = fin
 
         if not os.path.isfile(ifnm):
             raise FileNotFound(2, 'No such file or directory', ifnm)
 
         if nofile:
@@ -445,35 +434,46 @@
             elif extension:
                 ofnm = fout if os.path.splitext(fout)[1] == ext else f'{fout}{ext}'
             else:
                 ofnm = fout
 
         return ifnm, ofnm, fmt, ext, files
 
-    def record_header(self) -> 'None':
+    def record_header(self) -> 'Engine':
         """Read global header.
 
         The method will parse the PCAP global header and save the parsed result
-        as :attr:`self._gbhdr <Extractor._gbhdr>`. Information such as PCAP version,
-        data link layer protocol type, nanosecond flag and byteorder will also be
-        save the current :class:`Extractor` instance.
+        to its extraction context. Information such as PCAP version, data link
+        layer protocol type, nanosecond flag and byteorder will also be save
+        the current :class:`~pcapkit.foundation.engins.engine.Engine` instance
+        as well.
 
         If TCP flow tracing is enabled, the nanosecond flag and byteorder will
         be used for the output PCAP file of the traced TCP flows.
 
         For output, the method will dump the parsed PCAP global header under
         the name of ``Global Header``.
 
         """
         # pylint: disable=attribute-defined-outside-init,protected-access
         if self._magic in PCAP_Engine.MAGIC_NUMBER:
-            PCAP_Engine(self).run()
+            engine = PCAP_Engine(self)
+            engine.run()
+
             self._ifile.seek(0, os.SEEK_SET)
-            return
-        raise FormatError(f'unknown PCAP file format: {self._magic!r}')
+            return engine
+
+        if self._magic in PCAPNG_Engine.MAGIC_NUMBER:
+            engine = PCAPNG_Engine(self)  # type: ignore[assignment]
+            engine.run()
+
+            self._ifile.seek(0, os.SEEK_SET)
+            return engine
+
+        raise FormatError(f'unknown file format: {self._magic!r}')
 
     def record_frames(self) -> 'None':
         """Read packet frames.
 
         The method calls :meth:`self._exeng.read_frame <pcapkit.foundation.engine.engine.Engin.read_frame>`
         to parse each frame from the input PCAP file; and
         performs cleanup by calling :meth:`self._exeng.close <pcapkit.foundation.engine.engine.Engin.close>`
@@ -621,23 +621,17 @@
         self._ifile = open(ifnm, 'rb')  # input file # pylint: disable=unspecified-encoding,consider-using-with
         if not self._flag_q:
             module, class_, ext = self.__output__[fmt]
             if ext is None:
                 warn(f'Unsupported output format: {fmt}; disabled file output feature',
                      FormatWarning, stacklevel=stacklevel())
             output = getattr(importlib.import_module(module), class_)  # type: Type[Dumper]
+            dumper = make_dumper(output)
 
-            class DictDumper(output):  # type: ignore[valid-type,misc]
-                """Customised :class:`~dictdumper.dumper.Dumper` object."""
-
-                object_hook = dumpkit_object_hook
-                default = dumpkit_default
-                _append_fallback = dumpkit_append_fallback
-
-            self._ofile = DictDumper if self._flag_f else DictDumper(ofnm)  # output file
+            self._ofile = dumper if self._flag_f else dumper(ofnm)  # output file
 
         self._magic = self._ifile.read(4)  # magic number
         self._ifile.seek(0, os.SEEK_SET)
 
         self.run()    # start extraction
 
     def __iter__(self) -> 'Extractor':
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from pcapkit.foundation.reassembly.data.ip import Buffer as IP_Buffer
 from pcapkit.foundation.reassembly.data.ip import BufferID as IP_BufferID
 from pcapkit.foundation.reassembly.data.ip import Datagram as IP_Datagram
 from pcapkit.foundation.reassembly.data.ip import DatagramID as IP_DatagramID
 from pcapkit.foundation.reassembly.data.ip import Packet as IP_Packet
 
 # TCP reassembly
-from pcapkit.foundation.reassembly.data.tcp import Packet as TCP_Packet
-from pcapkit.foundation.reassembly.data.tcp import Datagram as TCP_Datagram
-from pcapkit.foundation.reassembly.data.tcp import DatagramID as TCP_DatagramID
 from pcapkit.foundation.reassembly.data.tcp import Buffer as TCP_Buffer
 from pcapkit.foundation.reassembly.data.tcp import BufferID as TCP_BufferID
+from pcapkit.foundation.reassembly.data.tcp import Datagram as TCP_Datagram
+from pcapkit.foundation.reassembly.data.tcp import DatagramID as TCP_DatagramID
 from pcapkit.foundation.reassembly.data.tcp import Fragment as TCP_Fragment
 from pcapkit.foundation.reassembly.data.tcp import HoleDiscriptor as TCP_HoleDiscriptor
+from pcapkit.foundation.reassembly.data.tcp import Packet as TCP_Packet
 
 __all__ = [
     'IP_Packet', 'IP_DatagramID', 'IP_Datagram', 'IP_Buffer',
     'IP_BufferID',
 
     'TCP_Packet', 'TCP_DatagramID', 'TCP_Datagram', 'TCP_Buffer',
     'TCP_Fragment', 'TCP_HoleDiscriptor', 'TCP_BufferID',
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/ip.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/ip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/data/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/data/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ip.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ipv4.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv4.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/ipv6.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/ipv6.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/reassembly.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/reassembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import abc
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 if TYPE_CHECKING:
     from typing import Any, Optional, Type
 
+    from typing_extensions import Self
+
     from pcapkit.corekit.infoclass import Info
     from pcapkit.protocols.protocol import Protocol
 
 __all__ = ['Reassembly']
 
 # packet
 PT = TypeVar('PT', bound='Info')
@@ -178,15 +180,15 @@
         for packet in packets:
             self.reassembly(packet)
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Reassembly[PT, DT, IT, BT]':  # pylint: disable=unused-argument
+    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Self':  # pylint: disable=unused-argument
         self = super().__new__(cls)
 
         # NOTE: Assign this attribute after ``__new__`` to avoid shared memory
         # reference between instances.
         self.__cached__ = {}
 
         return self
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/reassembly/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/reassembly/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/registry.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from pcapkit.protocols.internet.hopopt import HOPOPT
 from pcapkit.protocols.internet.internet import Internet
 from pcapkit.protocols.internet.ipv4 import IPv4
 from pcapkit.protocols.internet.ipv6_opts import IPv6_Opts
 from pcapkit.protocols.internet.ipv6_route import IPv6_Route
 from pcapkit.protocols.link.link import Link
 from pcapkit.protocols.misc.pcap.frame import Frame
+from pcapkit.protocols.misc.pcapng import PCAPNG
 from pcapkit.protocols.protocol import Protocol
 from pcapkit.protocols.transport.tcp import TCP
 from pcapkit.protocols.transport.udp import UDP
 from pcapkit.utilities.exceptions import RegistryError
 from pcapkit.utilities.logging import logger
 
 if TYPE_CHECKING:
@@ -38,14 +39,18 @@
     from typing_extensions import Literal
 
     from pcapkit.const.hip.parameter import Parameter as HIP_Parameter
     from pcapkit.const.http.frame import Frame as HTTP_Frame
     from pcapkit.const.ipv4.option_number import OptionNumber as IPv4_OptionNumber
     from pcapkit.const.ipv6.option import Option as IPv6_Option
     from pcapkit.const.ipv6.routing import Routing as IPv6_Routing
+    from pcapkit.const.pcapng.block_type import BlockType as PCAPNG_BlockType
+    from pcapkit.const.pcapng.option_type import OptionType as PCAPNG_OptionType
+    from pcapkit.const.pcapng.record_type import RecordType as PCAPNG_RecordType
+    from pcapkit.const.pcapng.secrets_type import SecretsType as PCAPNG_SecretsType
     from pcapkit.const.reg.ethertype import EtherType
     from pcapkit.const.reg.linktype import LinkType
     from pcapkit.const.reg.transtype import TransType
     from pcapkit.const.tcp.mp_tcp_option import MPTCPOption as TCP_MPTCPOption
     from pcapkit.const.tcp.option import Option as TCP_Option
     from pcapkit.protocols.application.httpv2 import FrameConstructor as HTTP_FrameConstructor
     from pcapkit.protocols.application.httpv2 import FrameParser as HTTP_FrameParser
@@ -56,38 +61,48 @@
     from pcapkit.protocols.internet.ipv4 import OptionConstructor as IPv4_OptionConstructor
     from pcapkit.protocols.internet.ipv4 import OptionParser as IPv4_OptionParser
     from pcapkit.protocols.internet.ipv6_opts import \
         OptionConstructor as IPv6_Opts_OptionConstructor
     from pcapkit.protocols.internet.ipv6_opts import OptionParser as IPv6_Opts_OptionParser
     from pcapkit.protocols.internet.ipv6_route import TypeConstructor as IPv6_Route_TypeConstructor
     from pcapkit.protocols.internet.ipv6_route import TypeParser as IPv6_Route_TypeParser
+    from pcapkit.protocols.misc.pcapng import BlockConstructor as PCAPNG_BlockConstructor
+    from pcapkit.protocols.misc.pcapng import BlockParser as PCAPNG_BlockParser
+    from pcapkit.protocols.misc.pcapng import OptionConstructor as PCAPNG_OptionConstructor
+    from pcapkit.protocols.misc.pcapng import OptionParser as PCAPNG_OptionParser
+    from pcapkit.protocols.misc.pcapng import RecordConstructor as PCAPNG_RecordConstructor
+    from pcapkit.protocols.misc.pcapng import RecordParser as PCAPNG_RecordParser
+    from pcapkit.protocols.misc.pcapng import SecretsConstructor as PCAPNG_SecretsConstructor
+    from pcapkit.protocols.misc.pcapng import SecretsParser as PCAPNG_SecretsParser
     from pcapkit.protocols.transport.tcp import MPOptionConstructor as TCP_MPOptionConstructor
     from pcapkit.protocols.transport.tcp import MPOptionParser as TCP_MPOptionParser
     from pcapkit.protocols.transport.tcp import OptionConstructor as TCP_OptionConstructor
     from pcapkit.protocols.transport.tcp import OptionParser as TCP_OptionParser
 
 __all__ = [
     'register_protocol',
 
-    'register_linktype', 'register_pcap',
+    'register_linktype', 'register_pcap', 'register_pcapng',
     'register_ethertype', 'register_transtype',
     'register_port', 'register_tcp_port', 'register_udp_port',
 
     'register_output',
     'register_extractor_dumper', 'register_extractor_engine',
     'register_traceflow',
 
+    'register_pcapng_block', 'register_pcapng_option', 'register_pcapng_secrets',
+    'register_pcapng_record',
     'register_hopopt', 'register_ipv6_opts', 'register_ipv6_route',
     'register_ipv4', 'register_hip',
     'register_tcp', 'register_mptcp',
     'register_http',
 ]
 
 ###############################################################################
-# pcapkit.protocols.Protocol.__proto__
+# pcapkit.protocols.Protocol
 ###############################################################################
 
 
 def register_protocol(protocol: 'Type[Protocol]') -> 'None':
     """Registered protocol class.
 
     The protocol class must be a subclass of
@@ -102,15 +117,15 @@
         raise RegistryError('protocol must be a Protocol subclass')
 
     protocol_registry[protocol.__name__.upper()] = protocol
     logger.info('registered protocol: %s', protocol.__name__)
 
 
 ###############################################################################
-# pcapkit.foundation.extraction.Extractor.__output__
+# pcapkit.foundation.extraction.Extractor
 ###############################################################################
 
 
 def register_extractor_dumper(format: 'str', module: 'str', class_: 'str', ext: 'str') -> 'None':  # pylint: disable=redefined-builtin
     r"""Registered a new dumper class.
 
     Notes:
@@ -131,19 +146,14 @@
     if not issubclass(dumper, Dumper):
         raise RegistryError('dumper must be a Dumper subclass')
 
     Extractor.register_dumper(format, module, class_, ext)
     logger.info('registered extractor output dumper: %s', format)
 
 
-###############################################################################
-# pcapkit.foundation.extraction.Extractor.__engine__
-###############################################################################
-
-
 def register_extractor_engine(engine: 'str', module: 'str', class_: 'str') -> 'None':  # pylint: disable=redefined-builtin
     r"""Registered a new engine class.
 
     Notes:
         The full qualified class name of the new engine class
         should be as ``{module}.{class_}``.
 
@@ -161,15 +171,15 @@
         raise RegistryError('engine must be a Engine subclass')
 
     Extractor.register_engine(engine, module, class_)
     logger.info('registered extractor engine: %s', engine)
 
 
 ###############################################################################
-# pcapkit.foundation.traceflow.TraceFlow.__output__
+# pcapkit.foundation.traceflow.TraceFlow
 ###############################################################################
 
 
 def register_traceflow(format: 'str', module: 'str', class_: 'str', ext: 'str') -> 'None':  # pylint: disable=redefined-builtin
     r"""Registered a new dumper class.
 
     Notes:
@@ -191,15 +201,15 @@
         raise RegistryError('dumper must be a Dumper subclass')
 
     TraceFlow.register(format, module, class_, ext)
     logger.info('registered traceflow output: %s', format)
 
 
 ###############################################################################
-# pcapkit.protocols.application.httpv2.HTTPv2.__frame__
+# pcapkit.protocols.application.httpv2.HTTPv2
 ###############################################################################
 
 
 def register_http(code: 'HTTP_Frame', meth: 'str | tuple[HTTP_FrameParser, HTTP_FrameConstructor]') -> 'None':
     """Registered a frame parser.
 
     The function will register the given frame parser to the
@@ -239,15 +249,15 @@
         raise RegistryError('method must be a valid HIP parameter parser function')
 
     HIP.register_parameter(code, meth)
     logger.info('registered HIP parameter parser: %s', code.name)
 
 
 ###############################################################################
-# pcapkit.protocols.internet.hopopt.HOPOPT.__option__
+# pcapkit.protocols.internet.hopopt.HOPOPT
 ###############################################################################
 
 
 def register_hopopt(code: 'IPv6_Option', meth: 'str | tuple[HOPOPT_OptionParser, HOPOPT_OptionConstructor]') -> 'None':
     """Register an option parser.
 
     The function will register the given option parser to the
@@ -263,15 +273,15 @@
         raise RegistryError('method must be a valid HOPOPT option parser function')
 
     HOPOPT.register_option(code, meth)
     logger.info('registered HOPOPT option parser: %s', code.name)
 
 
 ###############################################################################
-# pcapkit.protocols.internet.internet.Internet.__proto__
+# pcapkit.protocols.internet.internet.Internet
 ###############################################################################
 
 
 def register_transtype(code: 'TransType', module: str, class_: str) -> 'None':
     r"""Register a new protocol class.
 
     Notes:
@@ -319,15 +329,15 @@
         raise RegistryError('method must be a valid IPv4 option parser function')
 
     IPv4.register_option(code, meth)
     logger.info('registered IPv4 option parser: %s', code.name)
 
 
 ###############################################################################
-# pcapkit.protocols.internet.ipv6_opts.IPv6_Opts.__option__
+# pcapkit.protocols.internet.ipv6_opts.IPv6_Opts
 ###############################################################################
 
 
 def register_ipv6_opts(code: 'IPv6_Option', meth: 'str | tuple[IPv6_Opts_OptionParser, IPv6_Opts_OptionConstructor]') -> 'None':
     """Register an option parser.
 
     The function will register the given option parser to the
@@ -343,15 +353,15 @@
         raise RegistryError('method must be a valid IPv6-Opts option parser function')
 
     IPv6_Opts.register_option(code, meth)
     logger.info('registered IPv6_Opts option parser: %s', code.name)
 
 
 ###############################################################################
-# pcapkit.protocols.internet.ipv6_route.IPv6_Route.__routing__
+# pcapkit.protocols.internet.ipv6_route.IPv6_Route
 ###############################################################################
 
 
 def register_ipv6_route(code: 'IPv6_Routing', meth: 'str | tuple[IPv6_Route_TypeParser, IPv6_Route_TypeConstructor]') -> 'None':
     r"""Register an routing data parser.
 
     The function will register the given routing data parser to the
@@ -367,15 +377,15 @@
         raise RegistryError('method must be a valid IPv6-Route routing data parser function')
 
     IPv6_Route.register_routing(code, meth)
     logger.info('registered IPv6_Route routing data parser: %s', code.name)
 
 
 ###############################################################################
-# pcapkit.protocols.link.link.Link.__proto__
+# pcapkit.protocols.link.link.Link
 ###############################################################################
 
 
 def register_ethertype(code: 'EtherType', module: str, class_: str) -> 'None':
     r"""Register a new protocol class.
 
     Notes:
@@ -399,15 +409,15 @@
     logger.info('registered ethertype protocol: %s', code.name)
 
     # register protocol to protocol registry
     register_protocol(protocol)
 
 
 ###############################################################################
-# pcapkit.protocols.misc.pcap.frame.Frame.__proto__
+# pcapkit.protocols.misc.pcap.frame.Frame
 ###############################################################################
 
 
 def register_pcap(code: 'LinkType', module: str, class_: str) -> 'None':
     r"""Register a new protocol class.
 
     Notes:
@@ -424,22 +434,131 @@
 
     """
     protocol = getattr(importlib.import_module(module), class_)
     if not issubclass(protocol, Protocol):
         raise RegistryError('protocol must be a Protocol subclass')
 
     Frame.register(code, module, class_)
-    logger.info('registered PCAP frame protocol: %s', code.name)
+    logger.info('registered PCAP linktype protocol: %s', code.name)
 
     # register protocol to protocol registry
     register_protocol(protocol)
 
 
 ###############################################################################
-# pcapkit.protocols.transport.tcp.TCP.__option__
+# pcapkit.protocols.misc.pcapng.PCAPNG
+###############################################################################
+
+
+def register_pcapng(code: 'LinkType', module: str, class_: str) -> 'None':
+    r"""Register a new protocol class.
+
+    Notes:
+        The full qualified class name of the new protocol class
+        should be as ``{module}.{class_}``.
+
+    The function will register the given protocol class to the
+    :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__proto__` registry.
+
+    Arguments:
+        code: protocol code as in :class:`~pcapkit.const.reg.linktype.LinkType`
+        module: module name
+        class\_: class name
+
+    """
+    protocol = getattr(importlib.import_module(module), class_)
+    if not issubclass(protocol, Protocol):
+        raise RegistryError('protocol must be a Protocol subclass')
+
+    PCAPNG.register(code, module, class_)
+    logger.info('registered PCAP-NG linktype protocol: %s', code.name)
+
+    # register protocol to protocol registry
+    register_protocol(protocol)
+
+
+def register_pcapng_block(code: 'PCAPNG_BlockType', meth: 'str | tuple[PCAPNG_BlockParser, PCAPNG_BlockConstructor]') -> 'None':
+    """Registered a block parser.
+
+    The function will register the given block parser to the
+    :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__block__` registry.
+
+    Args:
+        code: :class:`HTTP/2 <pcapkit.protocols.misc.pcapng.PCAPNG>` block type
+            code as in :class:`~pcapkit.const.pcapng.block_type.BlockType`.
+        meth: Method name or callable to parse and/or construct the block.
+
+    """
+    if isinstance(meth, str) and not hasattr(PCAPNG, f'_read_block_{meth}'):
+        raise RegistryError('method must be a block parser function')
+
+    PCAPNG.register_block(code, meth)
+    logger.info('registered PCAP-NG block parser: %s', code.name)
+
+
+def register_pcapng_option(code: 'PCAPNG_OptionType', meth: 'str | tuple[PCAPNG_OptionParser, PCAPNG_OptionConstructor]') -> 'None':
+    """Registered a option parser.
+
+    The function will register the given option parser to the
+    :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__option__` registry.
+
+    Args:
+        code: :class:`PCAPNG <pcapkit.protocols.misc.pcapng.PCAPNG>` option type
+            code as in :class:`~pcapkit.const.pcapng.option_type.OptionType`.
+        meth: Method name or callable to parse and/or construct the option.
+
+    """
+    if isinstance(meth, str) and not hasattr(PCAPNG, f'_read_option_{meth}'):
+        raise RegistryError('method must be a option parser function')
+
+    PCAPNG.register_option(code, meth)
+    logger.info('registered PCAP-NG option parser: %s', code.name)
+
+
+def register_pcapng_record(code: 'PCAPNG_RecordType', meth: 'str | tuple[PCAPNG_RecordParser, PCAPNG_RecordConstructor]') -> 'None':
+    """Registered a name resolution record parser.
+
+    The function will register the given name resolution record parser to the
+    :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__record__` registry.
+
+    Args:
+        code: :class:`PCAPNG <pcapkit.protocols.misc.pcapng.PCAPNG>` name
+            resolution record type code as in :class:`~pcapkit.const.pcapng.record_type.RecordType`.
+        meth: Method name or callable to parse and/or construct the name
+            resolution record.
+
+    """
+    if isinstance(meth, str) and not hasattr(PCAPNG, f'_read_record_{meth}'):
+        raise RegistryError('method must be a name resolution record parser function')
+
+    PCAPNG.register_record(code, meth)
+    logger.info('registered PCAP-NG name resolution record parser: %s', code.name)
+
+
+def register_pcapng_secrets(code: 'PCAPNG_SecretsType', meth: 'str | tuple[PCAPNG_SecretsParser, PCAPNG_SecretsConstructor]') -> 'None':
+    """Registered a decryption secrets parser.
+
+    The function will register the given decryption secrets parser to the
+    :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__secrets__` registry.
+
+    Args:
+        code: :class:`PCAPNG <pcapkit.protocols.misc.pcapng.PCAPNG>` decryption
+            secrets type code as in :class:`~pcapkit.const.pcapng.secrets_type.SecretsType`.
+        meth: Method name or callable to parse and/or construct the decryption secrets.
+
+    """
+    if isinstance(meth, str) and not hasattr(PCAPNG, f'_read_secrets_{meth}'):
+        raise RegistryError('method must be a decryption secrets parser function')
+
+    PCAPNG.register_secrets(code, meth)
+    logger.info('registered PCAP-NG decryption secrets parser: %s', code.name)
+
+
+###############################################################################
+# pcapkit.protocols.transport.tcp.TCP
 ###############################################################################
 
 
 def register_tcp(code: 'TCP_Option', meth: 'str | tuple[TCP_OptionParser, TCP_OptionConstructor]') -> 'None':
     """Register an option parser.
 
     The function will register the given option parser to the
@@ -454,19 +573,14 @@
     if isinstance(meth, str) and not hasattr(TCP, f'_read_mode_{meth}'):
         raise RegistryError('method must be a TCP option parser function')
 
     TCP.register_option(code, meth)
     logger.info('registered TCP option parser: %s', code.name)
 
 
-###############################################################################
-# pcapkit.protocols.transport.tcp.TCP.__mp_option__
-###############################################################################
-
-
 def register_mptcp(code: 'TCP_MPTCPOption', meth: 'str | tuple[TCP_MPOptionParser, TCP_MPOptionConstructor]') -> 'None':
     """Register an MPTCP option parser.
 
     The function will register the given option parser to the
     :data:`pcapkit.protocols.transport.tcp.TCP.__mp_option__` registry.
 
     Args:
@@ -478,19 +592,14 @@
     if isinstance(meth, str) and not hasattr(TCP, f'_read_mptcp_{meth}'):
         raise RegistryError('method must be a MPTCP option parser function')
 
     TCP.register_mp_option(code, meth)
     logger.info('registered MPTCP option parser: %s', code.name)
 
 
-###############################################################################
-# pcapkit.protocols.transport.tcp.TCP.__proto__
-###############################################################################
-
-
 def register_tcp_port(code: 'int', module: str, class_: str) -> 'None':
     r"""Register a new protocol class.
 
     Notes:
         The full qualified class name of the new protocol class
         should be as ``{module}.{class_}``.
 
@@ -511,15 +620,15 @@
     logger.info('registered TCP port: %s', code)
 
     # register protocol to protocol registry
     register_protocol(protocol)
 
 
 ###############################################################################
-# pcapkit.protocols.transport.udp.UDP.__proto__
+# pcapkit.protocols.transport.udp.UDP
 ###############################################################################
 
 
 def register_udp_port(code: 'int', module: str, class_: str) -> 'None':
     r"""Register a new protocol class.
 
     Notes:
@@ -586,30 +695,35 @@
     r"""Register a new protocol class.
 
     Notes:
         The full qualified class name of the new protocol class
         should be as ``{module}.{class_}``.
 
     The function will register the given protocol class to the
-    :data:`pcapkit.protocols.misc.pcap.frame.Frame.__proto__` registry.
+    following registries:
+
+    - :data:`pcapkit.protocols.misc.pcap.frame.Frame.__proto__`
+    - :data:`pcapkit.protocols.misc.pcapng.PCAPNG.__proto__`
 
     See Also:
         * :func:`pcapkit.foundation.registry.register_pcap`
+        * :func:`pcapkit.foundation.registry.register_pcapng`
 
     Arguments:
         code: protocol code as in :class:`~pcapkit.const.reg.linktype.LinkType`
         module: module name
         class\_: class name
 
     """
     protocol = getattr(importlib.import_module(module), class_)
     if not issubclass(protocol, Protocol):
         raise RegistryError('protocol must be a Protocol subclass')
 
     Frame.register(code, module, class_)
+    PCAPNG.register(code, module, class_)
     logger.info('registered linktype protocol: %s', code.name)
 
     # register protocol to protocol registry
     register_protocol(protocol)
 
 
 def register_port(proto: 'Literal["tcp", "udp"]', code: 'int', module: str, class_: str) -> 'None':
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/data/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/data/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/data/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/foundation/traceflow/traceflow.py` & `pypcapkit-1.0.0rc1/pcapkit/foundation/traceflow/traceflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 import collections
 import importlib
 import os
 import sys
 from typing import TYPE_CHECKING, Generic, TypeVar, overload
 
 from pcapkit.corekit.infoclass import Info
-from pcapkit.dumpkit.common import _append_fallback as dumpkit_append_fallback
-from pcapkit.dumpkit.common import default as dumpkit_default
-from pcapkit.dumpkit.common import object_hook as dumpkit_object_hook
+from pcapkit.dumpkit.common import make_dumper
 from pcapkit.utilities.exceptions import FileExists, stacklevel
 from pcapkit.utilities.warnings import FileWarning, FormatWarning, warn
 
 __all__ = ['TraceFlow']
 
 if TYPE_CHECKING:
     from typing import Any, DefaultDict, Optional, Type
 
     from dictdumper.dumper import Dumper
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Self
 
     from pcapkit.protocols.protocol import Protocol
 
 BufferID = TypeVar('BufferID')
 Buffer = TypeVar('Buffer', bound='Info')
 Index = TypeVar('Index', bound='Info')
 Packet = TypeVar('Packet', bound='Info')
@@ -146,23 +144,15 @@
         try:
             os.makedirs(fout, exist_ok=True)
         except FileExistsError as error:
             if ext is None:
                 warn(error.strerror, FileWarning, stacklevel=stacklevel())
             else:
                 raise FileExists(*error.args).with_traceback(error.__traceback__)
-
-        class DictDumper(output):  # type: ignore[valid-type,misc]
-            """Customised :class:`~dictdumper.dumper.Dumper` object."""
-
-            object_hook = dumpkit_object_hook
-            default = dumpkit_default
-            _append_fallback = dumpkit_append_fallback
-
-        return DictDumper, ext
+        return make_dumper(output), ext
 
     @abc.abstractmethod
     def dump(self, packet: 'Packet') -> 'None':
         """Dump frame to output files.
 
         Arguments:
             packet: a flow packet (:term:`trace.tcp.packet`)
@@ -199,15 +189,15 @@
 
         """
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'TraceFlow':  # pylint: disable=unused-argument
+    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Self':  # pylint: disable=unused-argument
         self = super().__new__(cls)
 
         # NOTE: Assign this attribute after ``__new__`` to avoid shared memory
         # reference between instances.
         self.__cached__ = {}
 
         return self
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/interface/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/interface/core.py` & `pypcapkit-1.0.0rc1/pcapkit/interface/core.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/interface/misc.py` & `pypcapkit-1.0.0rc1/pcapkit/interface/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pcapkit.utilities.warnings import EngineWarning, warn
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from typing_extensions import Literal
 
-    from pcapkit.protocols.misc.pcap.frame import Frame
+    from pcapkit.foundation.extraction import Packet
 
     ByteOrder = Literal['little', 'big']
     Formats = Literal['pcap', 'json', 'tree', 'plist']
     Engines = Literal['default', 'pcapkit', 'dpkt', 'scapy', 'pyshark']
 
 __all__ = ['follow_tcp_stream']
 
@@ -38,20 +38,20 @@
 
 class Stream(Info):
     """Data model for TCP streams."""
 
     #: Output filename.
     filename: 'Optional[str]'
     #: Packet list.
-    packets: 'tuple[Frame, ...]'
+    packets: 'tuple[Packet, ...]'
     #: TCP conversation.
     conversations: 'tuple[bytes | tuple[bytes, ...], ...]'
 
     if TYPE_CHECKING:
-        def __init__(self, filename: 'Optional[str]', packets: 'tuple[Frame, ...]', conversations: 'tuple[bytes | tuple[bytes, ...], ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long
+        def __init__(self, filename: 'Optional[str]', packets: 'tuple[Packet, ...]', conversations: 'tuple[bytes | tuple[bytes, ...], ...]') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements,line-too-long
 
 
 def follow_tcp_stream(fin: 'Optional[str]' = None, verbose: 'bool' = False,              # Extrator options
                       extension: 'bool' = True, engine: 'Optional[Engines]' = None,
                       fout: 'Optional[str]' = None, format: 'Optional[Formats]' = None,  # TraceFlow options # pylint: disable=redefined-builtin
                       byteorder: 'ByteOrder' = sys.byteorder, nanosecond: 'bool' = False) -> 'tuple[Stream, ...]':
     """Follow TCP streams.
@@ -82,25 +82,25 @@
                            strict=False, trace=True, trace_fout=fout, trace_format=format,
                            trace_byteorder=byteorder, trace_nanosecond=nanosecond)  # type: ignore[var-annotated]
 
     fallback = False
     if extraction.engine == 'dpkt':  # type: ignore[comparison-overlap]
         from pcapkit.toolkit.dpkt import tcp_reassembly  # pylint: disable=import-outside-toplevel
     elif extraction.engine == 'scapy':  # type: ignore[comparison-overlap]
-        from pcapkit.toolkit.scapy import tcp_reassembly  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+        from pcapkit.toolkit.scapy import tcp_reassembly  # isort: skip # pylint: disable=import-outside-toplevel
     else:
-        from pcapkit.toolkit.default import tcp_reassembly  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+        from pcapkit.toolkit.pcap import tcp_reassembly  # type: ignore[assignment] # isort: skip # pylint: disable=import-outside-toplevel
         fallback = True
 
     streams = []  # type: list[Stream]
     frames = extraction.frame
     for stream in extraction.trace.tcp:
         reassembly = TCP_Reassembly(strict=False)
 
-        packets = []  # type: list[Frame]
+        packets = []  # type: list[Packet]
         for index in stream.index:
             frame = frames[index-1]
             packets.append(frame)
 
             if fallback:
                 data = tcp_reassembly(frame)
             else:
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/application.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/application.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/ftp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/ftp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/http.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/http.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/httpv1.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv1.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/application/httpv2.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/application/httpv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,21 @@
              flags: 'Flags' = 0,  # type: ignore[assignment]
              sid: 'int' = 0,
              frame: 'bytes | Data_HTTP | Schema_FrameType | dict[str, Any]' = b'',
              **kwargs: 'Any') -> 'Schema_HTTP':
         """Make (construct) packet data.
 
         Args:
+            type: Type of HTTP/2 frame.
+            type_default: Default frame type.
+            type_namespace: Namespace of frame type.
+            type_reversed: Whether to reverse the namespace.
+            flags: Flags of HTTP/2 frame.
+            sid: Stream ID of HTTP/2 frame.
+            frame: Frame data of HTTP/2 frame.
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Constructed packet data.
 
         """
         type_val = self._make_index(type, type_default, namespace=type_namespace,  # type: ignore[call-overload]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/application/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/application/ftp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/ftp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/application/httpv1.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv1.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/application/httpv2.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/application/httpv2.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ah.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ah.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/hip.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/hopopt.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/hopopt.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv4.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv4.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_frag.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_frag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_opts.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_opts.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipv6_route.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipv6_route.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/ipx.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/ipx.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/internet/mh.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/internet/mh.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/arp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/arp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/ethernet.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ethernet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/l2tp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/l2tp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/ospf.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/ospf.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/link/vlan.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/link/vlan.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/null.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/null.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""data modules for no-payload packet"""
+"""data models for no-payload packet"""
 
 from pcapkit.protocols.data.data import Data
 
 __all__ = ['NoPayload']
 
 
 class NoPayload(Data):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/frame.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""data modules for frame header of PCAP file"""
+"""data models for frame header of PCAP file"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from datetime import datetime
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/misc/pcap/header.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/misc/pcap/header.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""data modules for global header of PCAP file"""
+"""data models for global header of PCAP file"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.protocols.data.data import Data
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/data/transport/udp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/data/transport/udp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/NotImplemented/esp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/NotImplemented/esp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ah.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ah.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/hip.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hip.py`

 * *Files 0% similar despite different names*

```diff
@@ -3429,15 +3429,15 @@
         """
         if param is not None:
             cipher_id = param.cipher
             iv = param.iv
             data = param.data
         else:
             cipher_id = self._make_index(cipher, cipher_default, namespace=cipher_namespace,  # type: ignore[call-overload]
-                                      reversed=cipher_reversed, pack=False)
+                                         reversed=cipher_reversed, pack=False)
 
         if cipher_id in (Enum_Cipher.AES_128_CBC, Enum_Cipher.AES_256_CBC):
             if iv is None:
                 raise ProtocolError(f'HIPv{version}: [ParamNo {code}] IV is required for AES cipher')
             if len(iv) != 16:
                 raise ProtocolError(f'HIPv{version}: [ParamNo {code}] IV length must be 16 bytes for AES cipher')
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/hopopt.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/hopopt.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/internet.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/internet.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,17 +160,23 @@
             packet: packet info (passed from :meth:`self.unpack <pcapkit.protocols.protocol.Protocol.unpack>`)
             version: IP version
             ipv6_exthdr: protocol chain of IPv6 extension headers
 
         Returns:
             Current protocol with next layer extracted.
 
+        Notes:
+            We added a new key ``__next_type__`` to ``dict_`` to store the
+            next layer protocol type, and a new key ``__next_name__`` to
+            store the next layer protocol name. These two keys will **NOT**
+            be included when :meth:`Info.to_dict <pcapkit.corekit.infoclass.Info.to_dict>` is called.
+
         """
         next_ = cast('Protocol',  # type: ignore[redundant-cast]
-                     self._import_next_layer(proto, length, packet=packet, version=version))  # type: ignore[call-arg,arg-type,misc]
+                     self._import_next_layer(proto, length, packet=packet, version=version))  # type: ignore[arg-type,misc,call-arg]
         info, chain = next_.info, next_.protochain
 
         # make next layer protocol name
         layer = next_.info_name
         # proto = next_.__class__.__name__
 
         # write info and protocol chain into dict
@@ -209,17 +215,17 @@
             protocol: 'Type[Protocol]'
 
         file_ = self.__header__.get_payload()
         if length is None:
             length = len(file_)
 
         if length == 0:
-            from pcapkit.protocols.misc.null import NoPayload as protocol  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+            from pcapkit.protocols.misc.null import NoPayload as protocol  # isort: skip # pylint: disable=import-outside-toplevel
         elif self._sigterm:
-            from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+            from pcapkit.protocols.misc.raw import Raw as protocol  # isort: skip # pylint: disable=import-outside-toplevel
         else:
             module, name = self.__proto__[proto]
             protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
 
         next_ = protocol(file_, length, version=version, extension=extension,  # type: ignore[abstract]
                          alias=proto, packet=packet, layer=self._exlayer, protocol=self._exproto)
         return next_
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ip.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ip.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipsec.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipsec.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv4.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv4.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         return self._exthdr
 
     ##########################################################################
     # Methods.
     ##########################################################################
 
     def read(self, length: 'Optional[int]' = None, *,
-             packet: 'Optional[dict[str, Any]]' = None, **kwargs: 'Any') -> 'Data_IPv6':  # pylint: disable=unused-argument
+             __packet__: 'Optional[dict[str, Any]]' = None, **kwargs: 'Any') -> 'Data_IPv6':  # pylint: disable=unused-argument
         """Read Internet Protocol version 6 (IPv6).
 
         Structure of IPv6 header [:rfc:`2460`]:
 
         .. code-block:: text
 
             0                   1                   2                   3
@@ -125,15 +125,15 @@
            |                                                               |
            +                                                               +
            |                                                               |
            +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 
         Args:
             length: Length of packet data.
-            packet: Optional packet data.
+            __packet__: Optional packet data.
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Parsed packet data.
 
         """
         if length is None:
@@ -148,22 +148,22 @@
             'next': schema.next,
             'limit': schema.limit,
             'src': schema.src,
             'dst': schema.dst,
         })  # type: Data_IPv6
 
         # update packet info
-        if packet is None:
-            packet = {}
-        packet.update({
+        if __packet__ is None:
+            __packet__ = {}
+        __packet__.update({
             'src': ipv6.src,
             'dst': ipv6.dst,
         })
 
-        return self._decode_next_layer(ipv6, schema.next, ipv6.payload, packet=packet)  # pylint: disable=no-member
+        return self._decode_next_layer(ipv6, schema.next, ipv6.payload, packet=__packet__)  # pylint: disable=no-member
 
     def make(self,
              traffic_class: 'int' = 0,
              flow_label: 'int' = 0,
              next: 'Enum_TransType | StdlibEnum | AenumEnum | str | int' = Enum_TransType.UDP,
              next_default: 'Optional[int]' = None,
              next_namespace: 'Optional[dict[str, int] | dict[int, str] | Type[StdlibEnum] | Type[AenumEnum]]' = None,  # pylint: disable=line-too-long
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_frag.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_frag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_opts.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_opts.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipv6_route.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipv6_route.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/ipx.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/ipx.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/internet/mh.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/internet/mh.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/arp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/arp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/ethernet.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/ethernet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/l2tp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/l2tp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/link.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/link.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/ospf.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/ospf.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/rarp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/rarp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/link/vlan.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/link/vlan.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/null.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/null.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/frame.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,21 @@
 from typing import TYPE_CHECKING, cast, overload
 
 from pcapkit.const.reg.linktype import LinkType as Enum_LinkType
 from pcapkit.protocols.data.misc.pcap.frame import Frame as Data_Frame
 from pcapkit.protocols.data.misc.pcap.frame import FrameInfo as Data_FrameInfo
 from pcapkit.protocols.protocol import Protocol
 from pcapkit.protocols.schema.misc.pcap.frame import Frame as Schema_Frame
-from pcapkit.utilities.exceptions import UnsupportedCall
-from pcapkit.utilities.warnings import RegistryWarning, warn
+from pcapkit.utilities.exceptions import UnsupportedCall, stacklevel
+from pcapkit.utilities.warnings import ProtocolWarning, RegistryWarning, warn
 
 if TYPE_CHECKING:
+    from datetime import datetime as dt_type
     from decimal import Decimal
-    from typing import IO, Any, Optional, Type
+    from typing import IO, Any, DefaultDict, Optional, Type
 
     from typing_extensions import Literal
 
     from pcapkit.protocols.data.misc.pcap.header import Header as Data_Header
     from pcapkit.protocols.schema.schema import Schema
 
 __all__ = ['Frame']
@@ -74,26 +75,26 @@
 
     """
 
     ##########################################################################
     # Defaults.
     ##########################################################################
 
-    #: DefaultDict[int, tuple[str, str]]: Protocol index mapping for decoding next layer,
-    #: c.f. :meth:`self._decode_next_layer <pcapkit.protocols.protocol.Protocol._decode_next_layer>`
+    #: DefaultDict[Enum_LinkType, tuple[str, str]]: Protocol index mapping for
+    #: decoding next layer, c.f. :meth:`self._decode_next_layer <pcapkit.protocols.protocol.Protocol._decode_next_layer>`
     #: & :meth:`self._import_next_layer <pcapkit.protocols.protocol.Protocol._import_next_layer>`.
     #: The values should be a tuple representing the module name and class name.
     __proto__ = collections.defaultdict(
         lambda: ('pcapkit.protocols.misc.raw', 'Raw'),
         {
             Enum_LinkType.ETHERNET: ('pcapkit.protocols.link', 'Ethernet'),
             Enum_LinkType.IPV4:     ('pcapkit.protocols.internet', 'IPv4'),
             Enum_LinkType.IPV6:     ('pcapkit.protocols.internet', 'IPv6'),
         },
-    )
+    )  # type: DefaultDict[Enum_LinkType | int, tuple[str, str]]
 
     ##########################################################################
     # Properties.
     ##########################################################################
 
     @property
     def name(self) -> 'str':
@@ -143,14 +144,56 @@
 
         Raises:
             IndexNotFound: if ``name`` is not present
 
         """
         return self._protos.index(name)
 
+    def pack(self, **kwargs: 'Any') -> 'bytes':
+        """Pack (construct) packet data.
+
+        Args:
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Constructed packet data.
+
+        Notes:
+            We used a special keyword argument ``__packet__`` to pass the
+            global packet data to underlying methods. This is useful when
+            the packet data is not available in the current instance.
+
+        """
+        self.__header__ = self.make(**kwargs)
+        packet = kwargs.get('__packet__', {})  # packet data
+        packet['byteorder'] = self._ghdr.magic_number.byteorder
+        return self.__header__.pack(packet)
+
+    def unpack(self, length: 'Optional[int]' = None, **kwargs: 'Any') -> 'Data_Frame':
+        """Unpack (parse) packet data.
+
+        Args:
+            length: Length of packet data.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            Parsed packet data.
+
+        Notes:
+            We used a special keyword argument ``__packet__`` to pass the
+            global packet data to underlying methods. This is useful when
+            the packet data is not available in the current instance.
+
+        """
+        if cast('Optional[Schema_Frame]', self.__header__) is None:
+            packet = kwargs.get('__packet__', {})  # packet data
+            packet['bytesorder'] = self._ghdr.magic_number.byteorder
+            self.__header__ = cast('Schema_Frame', self.__schema__.unpack(self._file, length, packet))  # type: ignore[call-arg,misc]
+        return self.read(length, **kwargs)
+
     def read(self, length: 'Optional[int]' = None, *, _read: 'bool' = True, **kwargs: 'Any') -> 'Data_Frame':
         r"""Read each block after global header.
 
         Args:
             length: Length of data to be read.
             \_read: If the class is called in a parsing scenario.
             **kwargs: Arbitrary keyword arguments.
@@ -162,19 +205,26 @@
         schema = self.__header__
 
         _tsss = schema.ts_sec
         _tsus = schema.ts_usec
         _ilen = schema.incl_len
         _olen = schema.orig_len
 
-        if self._nsec:
-            _epch = _tsss + decimal.Decimal(_tsus) / 1_000_000_000
-        else:
-            _epch = _tsss + decimal.Decimal(_tsus) / 1_000_000
-        _time = datetime.datetime.fromtimestamp(float(_epch))
+        with decimal.localcontext(prec=64):
+            if self._nsec:
+                _epch = _tsss + decimal.Decimal(_tsus) / 1_000_000_000
+            else:
+                _epch = _tsss + decimal.Decimal(_tsus) / 1_000_000
+        _irat = _epch.as_integer_ratio()
+
+        try:
+            _time = datetime.datetime.fromtimestamp(_irat[0] / _irat[1])
+        except ValueError:
+            warn(f'PCAP: invalid timestamp: {_epch}', ProtocolWarning, stacklevel=stacklevel())
+            _time = datetime.datetime.fromtimestamp(0, datetime.timezone.utc)
 
         frame = Data_Frame(
             frame_info=Data_FrameInfo(
                 ts_sec=_tsss,
                 ts_usec=_tsus,
                 incl_len=_ilen,
                 orig_len=_olen,
@@ -186,29 +236,34 @@
             cap_len=_olen,
         )
 
         if not _read:
             # move backward to the beginning of the packet
             self._file.seek(0, io.SEEK_SET)
         else:
-            # NOTE: We create a copy of the frame packet data here for parsing
-            # scenarios to keep the original packet data intact.
+            # NOTE: We create a copy of the frame data here for parsing
+            # scenarios to keep the original frame data intact.
+            seek_cur = self._file.tell()
 
-            #: bytes: Raw packet data.
-            self._data = schema.packet
-            #: io.BytesIO: Source packet stream.
-            self._file = io.BytesIO(self._data)
+            # move backward to the beginning of the frame
+            self._file.seek(-self.length, io.SEEK_CUR)
+
+            #: bytes: Raw frame data.
+            self._data = self._read_fileng(self.length + _ilen)
 
-            # move forward to the beginning of frame's first packet
-            self._file.seek(self.length, io.SEEK_CUR)
+            # move backward to the beginning of frame's payload
+            self._file.seek(seek_cur, io.SEEK_SET)
+
+            #: io.BytesIO: Source data stream.
+            self._file = io.BytesIO(self._data)
 
         return self._decode_next_layer(frame, self._ghdr.network, frame.len)
 
     def make(self,
-             timestamp: 'Optional[float | Decimal]' = None,
+             timestamp: 'Optional[float | Decimal | int | dt_type]' = None,
              ts_sec: 'Optional[int]' = None,
              ts_usec: 'Optional[int]' = None,
              incl_len: 'Optional[int]' = None,
              orig_len: 'Optional[int]' = None,
              packet: 'bytes | Protocol | Schema' = b'',
              nanosecond: 'bool' = False,
              **kwargs: 'Any') -> 'Schema_Frame':
@@ -336,41 +391,44 @@
             'ts_src': data.frame_info.ts_sec,
             'ts_usec': data.frame_info.ts_usec,
             'incl_len': data.frame_info.incl_len,
             'orig_len': data.frame_info.orig_len,
             'packet': cls._make_payload(data),
         }
 
-    def _make_timestamp(self, timestamp: 'Optional[float | Decimal]' = None, ts_sec: 'Optional[int]' = None,
+    def _make_timestamp(self, timestamp: 'Optional[float | Decimal | dt_type | int]' = None, ts_sec: 'Optional[int]' = None,
                         ts_usec: 'Optional[int]' = None, nanosecond: 'bool' = False) -> 'tuple[int, int]':
         """Make timestamp.
 
         Args:
             timestamp: UNIX-Epoch timestamp
             ts_sec: timestamp seconds
             ts_usec: timestamp microseconds
             nanosecond: nanosecond-resolution file flag
 
         Returns:
             Second and microsecond/nanosecond value of timestamp.
 
         """
-        if timestamp is None:
-            if py37 and nanosecond:
-                timestamp = decimal.Decimal(time.time_ns()) / 1_000_000_000
+        with decimal.localcontext(prec=64):
+            if timestamp is None:
+                if py37 and nanosecond:
+                    timestamp = decimal.Decimal(time.time_ns()) / 1_000_000_000
+                else:
+                    timestamp = decimal.Decimal(time.time())
             else:
-                timestamp = decimal.Decimal(time.time())
-        else:
-            timestamp = decimal.Decimal(timestamp)
+                if isinstance(timestamp, datetime.datetime):
+                    timestamp = timestamp.timestamp()
+                timestamp = decimal.Decimal(timestamp)
 
         if ts_sec is None:
             ts_sec = int(timestamp)
 
         if ts_usec is None:
-            ts_usec = int(timestamp - ts_sec) * (1_000_000_000 if nanosecond else 1_000_000)
+            ts_usec = int((timestamp - ts_sec) * (1_000_000_000 if nanosecond else 1_000_000))
 
         return ts_sec, ts_usec
 
     def _decode_next_layer(self, dict_: 'Data_Frame', proto: 'Optional[int]' = None,
                            length: 'Optional[int]' = None, *, packet: 'Optional[dict[str, Any]]' = None) -> 'Data_Frame':  # pylint: disable=arguments-differ
         r"""Decode next layer protocol.
 
@@ -379,25 +437,34 @@
             proto: next layer protocol index
             length: valid (*non-padding*) length
             packet: packet info (passed from :meth:`self.unpack <pcapkit.protocols.protocol.Protocol.unpack>`)
 
         Returns:
             Current protocol with packet extracted.
 
+        Notes:
+            We added a new key ``__next_type__`` to ``dict_`` to store the
+            next layer protocol type, and a new key ``__next_name__`` to
+            store the next layer protocol name. These two keys will **NOT**
+            be included when :meth:`Info.to_dict <pcapkit.corekit.infoclass.Info.to_dict>` is called.
+
+            We also added a new key ``protocols`` to ``dict_`` to store the
+            protocol chain of the current packet (frame).
+
         """
         next_ = cast('Protocol', self._import_next_layer(proto, length, packet=packet))  # type: ignore[misc,call-arg,redundant-cast]
         info, chain = next_.info, next_.protochain
 
         # make next layer protocol name
         layer = next_.info_name
         # proto = next_.__class__.__name__
 
         # write info and protocol chain into dict
         dict_.__update__({
             layer: info,
-            'protocols': chain.chain,
+            'protocols': chain.chain if chain else '',
             '__next_type__': type(next_),
             '__next_name__': layer,
         })
         self._next = next_  # pylint: disable=attribute-defined-outside-init
         self._protos = chain  # pylint: disable=attribute-defined-outside-init
         return dict_
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/pcap/header.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/pcap/header.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/misc/raw.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/misc/raw.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/protocol.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,31 +226,42 @@
 
         Args:
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Constructed packet data.
 
+        Notes:
+            We used a special keyword argument ``__packet__`` to pass the
+            global packet data to underlying methods. This is useful when
+            the packet data is not available in the current instance.
+
         """
         self.__header__ = self.make(**kwargs)
-        return self.__header__.pack()
+        packet = kwargs.get('__packet__', {})  # packet data
+        return self.__header__.pack(packet)
 
     def unpack(self, length: 'Optional[int]' = None, **kwargs: 'Any') -> 'PT':
         """Unpack (parse) packet data.
 
         Args:
             length: Length of packet data.
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Parsed packet data.
 
+        Notes:
+            We used a special keyword argument ``__packet__`` to pass the
+            global packet data to underlying methods. This is useful when
+            the packet data is not available in the current instance.
+
         """
         if cast('Optional[ST]', self.__header__) is None:
-            packet = kwargs.get('packet', {})  # packet data
+            packet = kwargs.get('__packet__', {})  # packet data
             self.__header__ = cast('ST', self.__schema__.unpack(self._file, length, packet))  # type: ignore[call-arg,misc]
         return self.read(length, **kwargs)
 
     @staticmethod
     def decode(byte: bytes, *, encoding: 'Optional[str]' = None,
                errors: 'Literal["strict", "ignore", "replace"]' = 'strict') -> 'str':
         """Decode :obj:`bytes` into :obj:`str`.
@@ -361,17 +372,17 @@
         protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
 
         payload_io = io.BytesIO(payload)
         try:
             report = protocol(payload_io, len(payload), **kwargs)  # type: ignore[abstract]
         except Exception as exc:
             if isinstance(exc, StructError) and exc.eof:  # pylint: disable=no-member
-                from pcapkit.protocols.misc.null import NoPayload as protocol  # type: ignore[no-redef] # pylint: disable=import-outside-toplevel # isort: skip
+                from pcapkit.protocols.misc.null import NoPayload as protocol  # pylint: disable=import-outside-toplevel # isort: skip
             else:
-                from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[no-redef] # pylint: disable=import-outside-toplevel # isort: skip
+                from pcapkit.protocols.misc.raw import Raw as protocol  # pylint: disable=import-outside-toplevel # isort: skip
             # error = traceback.format_exc(limit=1).strip().rsplit(os.linesep, maxsplit=1)[-1]
 
             # log error
             #logger.error(str(exc), exc_info=exc, stack_info=DEVMODE, stacklevel=stacklevel())
 
             report = protocol(payload_io, len(payload), **kwargs)  # type: ignore[abstract]
         return report
@@ -392,15 +403,15 @@
         """
         protocol = getattr(importlib.import_module(module), class_)
         if not issubclass(protocol, Protocol):
             raise RegistryError('protocol must be a Protocol subclass')
         cls.__proto__[code] = (module, class_)
 
     @classmethod
-    def from_schema(cls, schema: 'ST | dict[str, Any]') -> 'Self':  # type: ignore[valid-type]
+    def from_schema(cls, schema: 'ST | dict[str, Any]') -> 'Self':
         """Create protocol instance from schema.
 
         Args:
             schema: Protocol schema.
 
         Returns:
             Protocol instance.
@@ -414,15 +425,15 @@
 
         # initialize protocol instance
         self.__init__(bytes(schema), len(schema))  # type: ignore[misc]
 
         return self
 
     @classmethod
-    def from_data(cls, data: 'PT | dict[str, Any]') -> 'Self':  # type: ignore[valid-type]
+    def from_data(cls, data: 'PT | dict[str, Any]') -> 'Self':
         """Create protocol instance from data.
 
         Args:
             data: Protocol data.
 
         Returns:
             Protocol instance.
@@ -439,15 +450,15 @@
 
         return self
 
     ##########################################################################
     # Data models.
     ##########################################################################
 
-    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Protocol[PT, ST]':  # pylint: disable=unused-argument
+    def __new__(cls, *args: 'Any', **kwargs: 'Any') -> 'Self':  # pylint: disable=unused-argument
         self = super().__new__(cls)
 
         # NOTE: Assign this attribute after ``__new__`` to avoid shared memory
         # reference between instances.
         self.__cached__ = {}
         self.__header__ = None  # type: ignore[assignment]
 
@@ -729,14 +740,26 @@
         """Return the hash value for :attr:`self._data <pcapkit.protocols.protocol.Protocol._data>`."""
         return hash(self._data)
 
     ##########################################################################
     # Utilities.
     ##########################################################################
 
+    def _get_payload(self) -> 'bytes':
+        """Get payload of :attr:`self.__header__ <Protocol.__header__>`.
+
+        Returns:
+            Payload of :attr:`self.__header__ <Protocol.__header__>` as :obj:`bytes`.
+
+        See Also:
+            This is a wrapper function for :meth:`pcapkit.protocols.schema.Schema.get_payload`.
+
+        """
+        return self.__header__.get_payload()
+
     def _read_protos(self, size: int) -> 'Optional[StdlibEnum | AenumEnum]':  # pylint: disable=unused-argument
         """Read next layer protocol type.
 
         * If *succeed*, returns the enum of next layer protocol.
         * If *fail*, returns :obj:`None`.
 
         Arguments:
@@ -1007,14 +1030,20 @@
         """
         return data.to_dict()
 
     @classmethod
     def _make_payload(cls, data: 'Data') -> 'Protocol':
         """Create payload from ``data`` for protocol construction.
 
+        This method uses ``__next_type__`` and ``__next_name__`` to
+        determine the payload type and name. If either of them is
+        :data:`None`, a :class:`~pcapkit.protocols.misc.null.NoPayload`
+        instance will be returned. Otherwise, the payload will be
+        constructed by :meth:`Protocol.from_data <pcapkit.protocols.protocol.Protocol.from_data>`.
+
         Args:
             data: protocol data
 
         Returns:
             Payload for protocol construction.
 
         """
@@ -1041,14 +1070,20 @@
             proto: next layer protocol index
             length: valid (*non-padding*) length
             packet: packet info (passed from :meth:`unpack`)
 
         Returns:
             Current protocol with next layer extracted.
 
+        Notes:
+            We added a new key ``__next_type__`` to ``dict_`` to store the
+            next layer protocol type, and a new key ``__next_name__`` to
+            store the next layer protocol name. These two keys will **NOT**
+            be included when :meth:`Info.to_dict <pcapkit.corekit.infoclass.Info.to_dict>` is called.
+
         """
         next_ = cast('Protocol', self._import_next_layer(proto, length, packet=packet))  # type: ignore[misc,call-arg,redundant-cast]
         info, chain = next_.info, next_.protochain
 
         # make next layer protocol name
         layer = next_.info_name
         # proto = next_.__class__.__name__
@@ -1076,22 +1111,22 @@
         Returns:
             Instance of next layer.
 
         """
         if TYPE_CHECKING:
             protocol: 'Type[Protocol]'
 
-        file_ = self.__header__.get_payload()
+        file_ = self._get_payload()
         if length is None:
             length = len(file_)
 
         if length == 0:
-            from pcapkit.protocols.misc.null import NoPayload as protocol  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+            from pcapkit.protocols.misc.null import NoPayload as protocol  # isort: skip # pylint: disable=import-outside-toplevel
         elif self._sigterm:
-            from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+            from pcapkit.protocols.misc.raw import Raw as protocol  # isort: skip # pylint: disable=import-outside-toplevel
         else:
             module, name = self.__proto__[proto]
             protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
 
         next_ = protocol(file_, length, alias=proto, packet=packet,
                          layer=self._exlayer, protocol=self._exproto)  # type: ignore[abstract]
         return next_
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/application/httpv2.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/application/httpv2.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'FrameType',
     'UnassignedFrame', 'DataFrame', 'HeadersFrame', 'PriorityFrame',
     'RSTStreamFrame', 'SettingsFrame', 'PushPromiseFrame', 'PingFrame',
     'GoawayFrame', 'WindowUpdateFrame', 'ContinuationFrame',
 ]
 
 if TYPE_CHECKING:
-    from typing import IO, Any, Optional
+    from typing import Any, Optional
 
     from pcapkit.corekit.fields.field import _Field as Field
 
 if SPHINX_TYPE_CHECKING:
     from typing_extensions import TypedDict
 
     class FrameFlags(TypedDict):
@@ -75,34 +75,34 @@
         Returns a :class:`~pcapkit.corekit.fields.misc.SchemaField` wrapped
         :class:`~pcapkit.protocols.schema.application.httpv2.FrameType`
         instance.
 
     """
     type = cast('Enum_Frame', pkt['type'])
     if type == Enum_Frame.DATA:
-        return SchemaField(schema=DataFrame)
+        return SchemaField(length=pkt['__length__'], schema=DataFrame)
     if type == Enum_Frame.HEADERS:
-        return SchemaField(schema=HeadersFrame)
+        return SchemaField(length=pkt['__length__'], schema=HeadersFrame)
     if type == Enum_Frame.PRIORITY:
-        return SchemaField(schema=PriorityFrame)
+        return SchemaField(length=pkt['__length__'], schema=PriorityFrame)
     if type == Enum_Frame.RST_STREAM:
-        return SchemaField(schema=RSTStreamFrame)
+        return SchemaField(length=pkt['__length__'], schema=RSTStreamFrame)
     if type == Enum_Frame.SETTINGS:
-        return SchemaField(schema=SettingsFrame)
+        return SchemaField(length=pkt['__length__'], schema=SettingsFrame)
     if type == Enum_Frame.PUSH_PROMISE:
-        return SchemaField(schema=PushPromiseFrame)
+        return SchemaField(length=pkt['__length__'], schema=PushPromiseFrame)
     if type == Enum_Frame.PING:
-        return SchemaField(schema=PingFrame)
+        return SchemaField(length=pkt['__length__'], schema=PingFrame)
     if type == Enum_Frame.GOAWAY:
-        return SchemaField(schema=GoawayFrame)
+        return SchemaField(length=pkt['__length__'], schema=GoawayFrame)
     if type == Enum_Frame.WINDOW_UPDATE:
-        return SchemaField(schema=WindowUpdateFrame)
+        return SchemaField(length=pkt['__length__'], schema=WindowUpdateFrame)
     if type == Enum_Frame.CONTINUATION:
-        return SchemaField(schema=ContinuationFrame)
-    return SchemaField(schema=UnassignedFrame)
+        return SchemaField(length=pkt['__length__'], schema=ContinuationFrame)
+    return SchemaField(length=pkt['__length__'], schema=UnassignedFrame)
 
 
 class HTTP(Schema):
     """Header schema for HTTP/2 packet."""
 
     #: Length.
     length: 'int' = NumberField(length=3, signed=False)
@@ -121,15 +121,14 @@
     })
     #: Stream identifier.
     stream: 'StreamID' = BitField(length=4, namespace={
         'sid': (1, 31),
     })
     #: Frame payload.
     frame: 'FrameType' = SwitchField(
-        length=lambda pkt: pkt['__length__'],
         selector=http_frame_selector,
     )
 
     if TYPE_CHECKING:
         def __init__(self, length: 'int', type: 'Enum_Frame', flags: 'FrameFlags', stream: 'StreamID', frame: 'FrameType | bytes') -> 'None': ...
 
 
@@ -138,38 +137,34 @@
 
     if TYPE_CHECKING:
         __flags__: 'Flags'
 
     class Flags(enum.IntFlag):
         """Flags enumeration for HTTP/2 frames."""
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
             schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
         flags = 0
         for key, val in filter(lambda kv: kv[0].startswith('BIT_'),
-                               cls.Flags.__members__.items()):
+                               self.Flags.__members__.items()):
             name = key.lower()
             if packet['flags'][name]:
                 flags |= val
 
-        schema.__flags__ = flags
-        return schema
+        self.__flags__ = flags
+        return self
 
 
 class UnassignedFrame(FrameType):
     """Header schema for unassigned HTTP/2 frame payload."""
 
     #: Frame payload.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ah.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ah.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/hip.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hip.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pcapkit.const.hip.parameter import Parameter as Enum_Parameter
 from pcapkit.const.hip.registration import Registration as Enum_Registration
 from pcapkit.const.hip.registration_failure import RegistrationFailure as Enum_RegistrationFailure
 from pcapkit.const.hip.suite import Suite as Enum_Suite
 from pcapkit.const.hip.transport import Transport as Enum_Transport
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import ListField, OptionField
-from pcapkit.corekit.fields.ipaddress import IPv6Field
+from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import ConditionalField, PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
@@ -56,15 +56,15 @@
     'EchoRequestUnsignedParameter', 'EchoResponseUnsignedParameter', 'RelayFromParameter',
     'RelayToParameter', 'RouteViaParameter', 'FromParameter',
     'RVSHMACParameter', 'RelayHMACParameter',
 ]
 
 if TYPE_CHECKING:
     from ipaddress import IPv6Address
-    from typing import IO, Any, Optional
+    from typing import Any, Optional
 
     from pcapkit.corekit.fields.field import _Field as Field
     from pcapkit.protocols.data.internet.hip import EncryptedParameter as Data_EncryptedParameter
     from pcapkit.protocols.data.internet.hip import HIPCipherParameter as Data_HIPCipherParameter
     from pcapkit.protocols.protocol import Protocol
 
 if SPHINX_TYPE_CHECKING:
@@ -126,15 +126,15 @@
           returns an :class:`~pcapkit.corekit.fields.ipaddress.IPv6Field` instance.
         * If ``kind`` is ``1`` and ``size`` is ``20``,
           returns a :class:`~pcapkit.corekit.fields.misc.SchemaField` wrapped
           :class:`~pcapkit.protocols.schema.internet.hip.LocatorData` instance.
 
     """
     if pkt['type'] == 0 and pkt['len'] == 4:
-        return IPv6Field()
+        return IPv6AddressField()
     if pkt['type'] == 1 and pkt['len'] == 5:
         return SchemaField(
             length=20,
             schema=LocatorData,
         )
     raise FieldValueError('invalid locator type or length')
 
@@ -154,19 +154,19 @@
           :class:`~pcapkit.protocols.schema.internet.hip.ECDSALowCurveHostIdentity` instance.
         * If ``algorithm`` is ``13`` (EdDSA), returns a
           :class:`~pcapkit.corekit.fields.misc.SchemaField` wrapped
           :class:`~pcapkit.protocols.schema.internet.hip.EdDSACurveHostIdentity` instance.
 
     """
     if pkt['algorithm'] == Enum_HIAlgorithm.ECDSA:
-        return SchemaField(schema=ECDSACurveHostIdentity)
+        return SchemaField(length=pkt['hi_len'], schema=ECDSACurveHostIdentity)
     if pkt['algorithm'] == Enum_HIAlgorithm.ECDSA_LOW:
-        return SchemaField(schema=ECDSALowCurveHostIdentity)
+        return SchemaField(length=pkt['hi_len'], schema=ECDSALowCurveHostIdentity)
     if pkt['algorithm'] == Enum_HIAlgorithm.EdDSA:
-        return SchemaField(schema=EdDSACurveHostIdentity)
+        return SchemaField(length=pkt['hi_len'], schema=EdDSACurveHostIdentity)
     return BytesField(length=pkt['hi_len'])
 
 
 class Parameter(Schema):
     """Base schema for HIP parameters."""
 
     #: Parameter type.
@@ -235,15 +235,14 @@
         namespace={
             'preferred': (7, 1),
         },
     )
     lifetime: 'int' = UInt32Field()
     #: Locator value.
     value: 'IPv6Address | LocatorData' = SwitchField(
-        length=lambda pkt: pkt['len'] * 4,
         selector=locator_value_selector,
     )
 
     if TYPE_CHECKING:
         def __init__(self, traffic: 'int', type: 'int', len: 'int', flags: 'LocatorFlags',
                      lifetime: 'int', value: 'bytes | LocatorData') -> 'None': ...
 
@@ -265,15 +264,15 @@
 
 class LocatorData(Schema):
     """Header schema for HIP locator data."""
 
     #: SPI.
     spi: 'int' = UInt32Field()
     #: Locator.
-    ip: 'IPv6Address' = IPv6Field()
+    ip: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, spi: 'int', ip: 'IPv6Address | int | bytes | str') -> 'None': ...
 
 
 class PuzzleParameter(Parameter):
     """Header schema for HIP ``PUZZLE`` parameters."""
@@ -447,66 +446,66 @@
     data: 'bytes' = BytesField(
         length=lambda pkt: pkt['len'] - (16 if pkt.get('iv') else 0),
     )
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     @classmethod
-    def pre_process(cls, packet: 'dict[str, Any]') -> 'None':
+    def pre_unpack(cls, packet: 'dict[str, Any]') -> 'None':
         """Prepare ``packet`` data for unpacking process.
 
         Args:
             packet: packet data
 
         """
-        cipher_list = cast('list[Data_HIPCipherParameter]',
-                           packet['options'].getlist(Enum_Parameter.HIP_CIPHER))
-        if cipher_list:
-            warn(f'HIPv{packet["ver"]["version"]}: [ParamNo {Enum_Parameter.ENCRYPTED}] '
-                 'missing HIP_CIPHER parameter', ProtocolWarning)
-            # raise ProtocolError(f'HIPv{version}: [ParamNo {schema.type}] invalid format')
-
-            cipher_id = Enum_Cipher(0xffff)
-        else:
-            cipher_ids = []  # type: list[Enum_Cipher]
-            for cipher in cipher_list:
-                cipher_ids.extend(cipher.cipher_id)
-
-            encrypted_list = cast('list[Data_EncryptedParameter]',
-                                  packet['options'].getlist(Enum_Parameter.ENCRYPTED))
-            encrypted_index = len(encrypted_list)
-
-            if encrypted_index >= len(cipher_ids):
-                warn(f'HIPv{packet["ver"]["version"]}: [ParamNo {Enum_Parameter.ENCRYPTED}] '
-                     'too many ENCRYPTED parameters', ProtocolWarning)
+        if 'options' in packet:
+            cipher_list = cast('list[Data_HIPCipherParameter]',
+                            packet['options'].getlist(Enum_Parameter.HIP_CIPHER))
+            if cipher_list:
+                warn(f'HIP: [ParamNo {Enum_Parameter.ENCRYPTED}] '
+                    'missing HIP_CIPHER parameter', ProtocolWarning)
                 # raise ProtocolError(f'HIPv{version}: [ParamNo {schema.type}] invalid format')
 
-                cipher_id = Enum_Cipher(0xfffe)
+                cipher_id = Enum_Cipher(0xffff)
             else:
-                cipher_id = cipher_ids[encrypted_index]
+                cipher_ids = []  # type: list[Enum_Cipher]
+                for cipher in cipher_list:
+                    cipher_ids.extend(cipher.cipher_id)
+
+                encrypted_list = cast('list[Data_EncryptedParameter]',
+                                    packet['options'].getlist(Enum_Parameter.ENCRYPTED))
+                encrypted_index = len(encrypted_list)
+
+                if encrypted_index >= len(cipher_ids):
+                    warn(f'HIP: [ParamNo {Enum_Parameter.ENCRYPTED}] '
+                        'too many ENCRYPTED parameters', ProtocolWarning)
+                    # raise ProtocolError(f'HIPv{version}: [ParamNo {schema.type}] invalid format')
+
+                    cipher_id = Enum_Cipher(0xfffe)
+                else:
+                    cipher_id = cipher_ids[encrypted_index]
+        else:
+            warn(f'HIP: [ParamNo {Enum_Parameter.ENCRYPTED}] '
+                 'missing HIP_CIPHER parameter', ProtocolWarning)
+            cipher_id = Enum_Cipher(0xffff)
 
         packet['__cipher__'] = cipher_id
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        schema.cipher = packet['__cipher__']
-        return schema
+        self.cipher = packet['__cipher__']
+        return self
 
     if TYPE_CHECKING:
         #: Cipher ID.
         cipher: 'Enum_Cipher'
 
         def __init__(self, type: 'Enum_Parameter', len: 'int', cipher: 'Enum_Cipher',
                      iv: 'Optional[bytes]', data: 'bytes') -> 'None': ...
@@ -524,17 +523,15 @@
             'type': (0, 4),
             'len': (4, 12),
         },
     )
     #: Algorithm type.
     algorithm: 'Enum_HIAlgorithm' = EnumField(length=2, namespace=Enum_HIAlgorithm)
     #: Host ID.
-    hi: 'bytes | HostIdentity' = SwitchField(
-        length=lambda pkt: pkt['hi_len'],
-        selector=host_id_hi_selector)
+    hi: 'bytes | HostIdentity' = SwitchField(selector=host_id_hi_selector)
     #: Domain ID.
     di: 'bytes' = BytesField(length=lambda pkt: pkt['di_data']['len'])
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', hi_len: 'int', di_data: 'DIData',
@@ -723,15 +720,15 @@
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
     #: Address.
-    address: 'IPv6Address' = IPv6Field()
+    address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'IPv6Address | bytes | int | str') -> 'None': ...
 
 
 class EchoResponseSignedParameter(Parameter):
     """Header schema for HIP ``ECHO_RESPONSE_SIGNED`` parameters."""
@@ -855,15 +852,15 @@
             'must_follow': (1, 1),
     })
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: HIT addresses.
     hit: 'list[IPv6Address]' = ListField(
         length=lambda pkt: pkt['len'] - 4,
-        item_type=IPv6Field(),
+        item_type=IPv6AddressField(),
     )
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', flags: 'RouteFlags', hit: 'list[str | int | bytes | IPv6Address]') -> 'None': ...
 
@@ -967,15 +964,15 @@
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
     #: Address.
-    address: 'IPv6Address' = IPv6Field()
+    address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
 class RelayToParameter(Parameter):
     """Header schema for HIP ``RELAY_TO`` parameters."""
@@ -983,15 +980,15 @@
     #: Port.
     port: 'int' = UInt16Field()
     #: Protocol.
     protocol: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=1)
     #: Address.
-    address: 'IPv6Address' = IPv6Field()
+    address: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', port: 'int', protocol: 'Enum_TransType', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
 class OverlayTTLParameter(Parameter):
     """Header schema for HIP ``OVERLAY_TTL`` parameters."""
@@ -1016,28 +1013,28 @@
         'must_follow': (1, 1),
     })
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=2)
     #: HIT addresses.
     hit: 'list[IPv6Address]' = ListField(
         length=lambda pkt: pkt['len'] - 4,
-        item_type=IPv6Field(),
+        item_type=IPv6AddressField(),
     )
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', flags: 'RouteFlags', hit: 'list[str | bytes | int | IPv6Address]') -> 'None': ...
 
 
 class FromParameter(Parameter):
     """Header schema for HIP ``FROM`` parameters."""
 
     #: Address.
-    address: 'IPv6Address' = IPv6Field()
+    address: 'IPv6Address' = IPv6AddressField()
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', address: 'str | bytes | int | IPv6Address') -> 'None': ...
 
 
@@ -1055,15 +1052,15 @@
 
 class ViaRVSParameter(Parameter):
     """Header schema for HIP ``VIA_RVS`` parameters."""
 
     #: Address.
     address: 'list[IPv6Address]' = ListField(
         length=lambda pkt: pkt['len'],
-        item_type=IPv6Field(),
+        item_type=IPv6AddressField(),
     )
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: (8 - (pkt['len'] % 8)) % 8)
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Parameter', len: 'int', address: 'list[str | bytes | int | IPv6Address]') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/hopopt.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/hopopt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
 """header schema for hop-by-hop options"""
 
 import collections
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING
 
 from pcapkit.const.ipv6.option import Option as Enum_Option
 from pcapkit.const.ipv6.qs_function import QSFunction as Enum_QSFunction
 from pcapkit.const.ipv6.router_alert import RouterAlert as Enum_RouterAlert
 from pcapkit.const.ipv6.seed_id import SeedID as Enum_SeedID
 from pcapkit.const.ipv6.smf_dpd_mode import SMFDPDMode as Enum_SMFDPDMode
 from pcapkit.const.ipv6.tagger_id import TaggerID as Enum_TaggerID
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import OptionField
 from pcapkit.corekit.fields.field import NoValue
-from pcapkit.corekit.fields.ipaddress import IPv4Field, IPv6Field
+from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, NoValueField,
                                          PayloadField, SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.exceptions import FieldValueError
@@ -34,15 +34,15 @@
     'QuickStartReportOption', 'RPLOption', 'MPLOption', 'ILNPOption',
     'LineIdentificationOption', 'JumboPayloadOption', 'HomeAddressOption',
     'IPDFFOption',
 ]
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address, IPv6Address
-    from typing import IO, Any, Optional
+    from typing import Any, Optional
 
     from pcapkit.corekit.fields.field import _Field as Field
     from pcapkit.protocols.protocol import Protocol
 
 if SPHINX_TYPE_CHECKING:
     from typing_extensions import TypedDict
 
@@ -154,17 +154,17 @@
         * If ``mode`` is ``1``, returns a :class:`~pcapkit.corekit.fields.misc.SchemaField`
           wrapped :class:`~pcapkit.protocols.schema.internet.hopopt.SMFHashBasedDPDOption`
           instance.
 
     """
     mode = Enum_SMFDPDMode.get(pkt['test']['mode'])
     if mode == Enum_SMFDPDMode.I_DPD:
-        return SchemaField(schema=SMFIdentificationBasedDPDOption)
+        return SchemaField(length=pkt['test']['len'], schema=SMFIdentificationBasedDPDOption)
     if mode == Enum_SMFDPDMode.H_DPD:
-        return SchemaField(schema=SMFHashBasedDPDOption)
+        return SchemaField(length=pkt['test']['len'], schema=SMFHashBasedDPDOption)
     raise FieldValueError(f'HOPOPT: invalid SMF DPD mode: {mode}')
 
 
 def smf_i_dpd_tid_selector(pkt: 'dict[str, Any]') -> 'Field':
     """Selector function for :attr:`SMFIdentificationBasedDPDOption.tid` field.
 
     Args:
@@ -189,19 +189,19 @@
     if tid_type == Enum_TaggerID.NULL:
         if tid_len != 0:
             raise FieldValueError(f'HOPOPT: invalid TaggerID length: {tid_len}')
         return NoValueField()
     if tid_type == Enum_TaggerID.IPv4:
         if tid_len != 3:
             raise FieldValueError(f'HOPOPT: invalid TaggerID length: {tid_len}')
-        return IPv4Field()
+        return IPv4AddressField()
     if tid_type == Enum_TaggerID.IPv6:
         if tid_len != 15:
             raise FieldValueError(f'HOPOPT: invalid TaggerID length: {tid_len}')
-        return IPv6Field()
+        return IPv6AddressField()
     return BytesField(length=tid_len + 1)
 
 
 def quick_start_data_selector(pkt: 'dict[str, Any]') -> 'Field':
     """Selector function for :attr:`_QuickStartOption.data` field.
 
     Args:
@@ -216,53 +216,45 @@
           instance.
 
     """
     func = Enum_QSFunction.get(pkt['flags']['func'])
     pkt['flags']['func'] = func
 
     if func == Enum_QSFunction.Quick_Start_Request:
-        return SchemaField(schema=QuickStartRequestOption)
+        return SchemaField(length=5, schema=QuickStartRequestOption)
     if func == Enum_QSFunction.Report_of_Approved_Rate:
-        return SchemaField(schema=QuickStartReportOption)
+        return SchemaField(length=5, schema=QuickStartReportOption)
     raise FieldValueError(f'HOPOPT: invalid QS function: {func}')
 
 
 class Option(Schema):
     """Header schema for HOPOPT options."""
 
     #: Option type.
     type: 'Enum_Option' = EnumField(length=1, namespace=Enum_Option)
     #: Option length (conditional in case of ``Pad1`` option).
     len: 'int' = ConditionalField(
         UInt8Field(default=0),
         lambda pkt: pkt['type'] != Enum_Option.Pad1,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('Option', schema)
-
         # for Pad1 option, length is always 0
-        if schema.type == Enum_Option.Pad1:
-            schema.len = 0
-        return schema
+        if self.type == Enum_Option.Pad1:
+            self.len = 0
+        return self
 
 
 class UnassignedOption(Option):
     """Header schema for HOPOPT unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
@@ -331,83 +323,97 @@
     #: SMF DPD mode.
     test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=3, namespace={
         'len': (1, 8),
         'mode': (16, 1),
     }))
     #: SMF DPD data.
     data: 'SMFIdentificationBasedDPDOption | SMFHashBasedDPDOption' = SwitchField(
-        length=lambda pkt: pkt['test']['len'],
         selector=smf_dpd_data_selector,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFDPDOption':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('_SMFDPDOption', schema)
-
-        ret = schema.data
-        ret.mode = Enum_SMFDPDMode.get(schema.test['mode'])
+        ret = self.data
         return ret
 
 
 class SMFDPDOption(Option):
     """Header schema for HOPOPT simplified multicast forwarding duplicate packet
     detection (``SMF_DPD``) options."""
 
     if TYPE_CHECKING:
         mode: 'Enum_SMFDPDMode'
 
 
 class SMFIdentificationBasedDPDOption(SMFDPDOption):
     """Header schema for HOPOPT SMF identification-based DPD options."""
 
-    test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=1, namespace={
-        'mode': (0, 1),
-    }))
     #: TaggerID information.
     info: 'TaggerIDInfo' = BitField(length=1, namespace={
         'mode': (0, 1),
         'type': (1, 3),
         'len': (4, 4),
     })
     #: TaggerID.
     tid: 'bytes | IPv4Address | IPv6Address' = ConditionalField(
-        SwitchField(length=lambda pkt: pkt['info']['len'] + 1,
-                    selector=smf_i_dpd_tid_selector),
+        SwitchField(selector=smf_i_dpd_tid_selector),
         lambda pkt: pkt['info']['type'] != 0,
     )
     #: Identifier.
     id: 'bytes' = BytesField(length=lambda pkt: pkt['len'] - (
         1 if pkt['info']['type'] == 0 else (pkt['info']['len'] + 2)
     ))
 
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
+        """Revise ``schema`` data after unpacking process.
+
+        Args:
+            packet: Unpacked data.
+
+        Returns:
+            Revised schema.
+
+        """
+        ret = super().post_process(packet)  # type: SMFIdentificationBasedDPDOption
+        ret.mode = Enum_SMFDPDMode.I_DPD
+        return ret
+
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', info: 'TaggerIDInfo',
                      tid: 'Optional[bytes]', id: 'bytes') -> 'None': ...
 
 
 class SMFHashBasedDPDOption(SMFDPDOption):
     """Header schema for HOPOPT SMF hash-based DPD options."""
 
     #: Hash assist value (HAV).
     hav: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
+        """Revise ``schema`` data after unpacking process.
+
+        Args:
+            packet: Unpacked data.
+
+        Returns:
+            Revised schema.
+
+        """
+        ret = super().post_process(packet)  # type: SMFIdentificationBasedDPDOption
+        ret.mode = Enum_SMFDPDMode.H_DPD
+        return ret
+
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', hav: 'bytes') -> 'None': ...
 
 
 class PDMOption(Option):
     """Header schema for HOPOPT performance and diagnostic metrics (PDM) options."""
 
@@ -434,38 +440,29 @@
 
     #: Flags.
     flags: 'QSTestFlags' = ForwardMatchField(BitField(length=3, namespace={
         'func': (16, 4),
     }))
     #: QS data.
     data: 'QuickStartRequestOption | QuickStartReportOption' = SwitchField(
-        length=5,
         selector=quick_start_data_selector,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'QuickStartOption':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('_QuickStartOption', schema)
-
-        ret = schema.data
-        ret.func = Enum_QSFunction.get(packet['flags']['func'])
+        ret = self.data
+        ret.func = Enum_QSFunction.get(self.flags['func'])
         return ret
 
 
 class QuickStartOption(Option):
     """Header schema for HOPOPT quick start options."""
 
     #: Flags.
@@ -544,35 +541,27 @@
         lambda pkt: pkt['flags']['type'] != Enum_SeedID.IPV6_SOURCE_ADDRESS,
     )
     #: Reserved data (padding).
     pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'] - 2 - (
         0 if pkt['flags']['type'] == 0 else mpl_opt_seed_id_len(pkt)
     ))
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('MPLOption', schema)
-
-        if schema.flags['type'] == Enum_SeedID.IPV6_SOURCE_ADDRESS:
-            schema.seed = packet.get('src', NoValue)
-        return schema
+        if self.flags['type'] == Enum_SeedID.IPV6_SOURCE_ADDRESS:
+            self.seed = packet.get('src', NoValue)
+        return self
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', flags: 'MPLFlags', seq: 'int',
                      seed: 'Optional[int]') -> 'None': ...
 
 
 class ILNPOption(Option):
@@ -607,15 +596,15 @@
         def __init__(self, type: 'Enum_Option', len: 'int', jumbo_len: 'int') -> 'None': ...
 
 
 class HomeAddressOption(Option):
     """Header schema for HOPOPT home address options."""
 
     #: Home address.
-    addr: 'IPv6Address' = IPv6Field()
+    addr: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, type: 'Enum_Option', len: 'int', addr: 'IPv6Address | int | str | bytes') -> 'None': ...
 
 
 class IPDFFOption(Option):
     """Header schema for HOPOPT depth-first forwarding (``IP_DFF``) options."""
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv4.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_opts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,115 +1,212 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
-"""header schema for internet protocol version 4"""
+"""header schema for IPv6 destination options"""
 
 import collections
-import datetime
-import ipaddress
-from typing import TYPE_CHECKING, cast
-
-from pcapkit.const.ipv4.classification_level import ClassificationLevel as Enum_ClassificationLevel
-from pcapkit.const.ipv4.option_number import OptionNumber as Enum_OptionNumber
-from pcapkit.const.ipv4.qs_function import QSFunction as Enum_QSFunction
-from pcapkit.const.ipv4.router_alert import RouterAlert as Enum_RouterAlert
-from pcapkit.const.ipv4.ts_flag import TSFlag as Enum_TSFlag
+from typing import TYPE_CHECKING
+
+from pcapkit.const.ipv6.option import Option as Enum_Option
+from pcapkit.const.ipv6.qs_function import QSFunction as Enum_QSFunction
+from pcapkit.const.ipv6.router_alert import RouterAlert as Enum_RouterAlert
+from pcapkit.const.ipv6.seed_id import SeedID as Enum_SeedID
+from pcapkit.const.ipv6.smf_dpd_mode import SMFDPDMode as Enum_SMFDPDMode
+from pcapkit.const.ipv6.tagger_id import TaggerID as Enum_TaggerID
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
-from pcapkit.corekit.fields.collections import ListField, OptionField
-from pcapkit.corekit.fields.ipaddress import IPv4Field
-from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, PayloadField,
-                                         SchemaField, SwitchField)
-from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field, UInt32Field
+from pcapkit.corekit.fields.collections import OptionField
+from pcapkit.corekit.fields.field import NoValue
+from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
+from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, NoValueField,
+                                         PayloadField, SchemaField, SwitchField)
+from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
+                                            UInt32Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.exceptions import FieldValueError
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
-from pcapkit.utilities.warnings import ProtocolWarning, warn
 
 __all__ = [
-    'IPv4',
+    'IPv6_Opts',
 
-    'Option',
-    'UnassignedOption', 'EOOLOption', 'NOPOption',
-    'SECOption', 'LSROption', 'TSOption',
-    'ESECOption', 'RROption', 'SIDOption',
-    'SSROption', 'MTUPOption', 'MTUROption',
-    'TROption', 'RTRALTOption', 'QSOption',
-    'QuickStartRequestOption', 'QuickStartReportOption',
+    'SMFDPDOption', 'QuickStartOption',
+    'UnassignedOption', 'PadOption', 'TunnelEncapsulationLimitOption',
+    'RouterAlertOption', 'CALIPSOOption', 'SMFIdentificationBasedDPDOption',
+    'SMFHashBasedDPDOption', 'PDMOption', 'QuickStartRequestOption',
+    'QuickStartReportOption', 'RPLOption', 'MPLOption', 'ILNPOption',
+    'LineIdentificationOption', 'JumboPayloadOption', 'HomeAddressOption',
+    'IPDFFOption',
 ]
 
 if TYPE_CHECKING:
-    from datetime import timedelta
-    from ipaddress import IPv4Address
-    from typing import IO, Any, Optional
+    from ipaddress import IPv4Address, IPv6Address
+    from typing import Any, Optional
 
     from pcapkit.corekit.fields.field import _Field as Field
-    from pcapkit.corekit.multidict import OrderedMultiDict
     from pcapkit.protocols.protocol import Protocol
 
 if SPHINX_TYPE_CHECKING:
     from typing_extensions import TypedDict
 
-    class VerIHLField(TypedDict):
-        """Version and header length field."""
-
-        #: IP version.
-        version: int
-        #: Internet header length.
-        ihl: int
-
-    #: Type of service field.
-    ToSField = TypedDict('ToSField', {
-        'pre': int,
-        'del': int,
-        'thr': int,
-        'rel': int,
-        'ecn': int,
-    })
+    class TaggerIDInfo(TypedDict):
+        """TaggerID information."""
 
-    class Flags(TypedDict):
-        """Flags and fragment offset field."""
-
-        #: Don't fragment flag.
-        df: int
-        #: More fragments flag.
-        mf: int
-        #: Fragment offset.
-        offset: int
-
-    class TSFlags(TypedDict):
-        """Timestamp flags field."""
-
-        #: Timestamp overflow flag.
-        oflw: int
-        #: Timestamp type flag.
-        flag: int
+        #: SMF mode.
+        mode: int
+        #: TaggerID type.
+        type: int
+        #: TaggerID length.
+        len: int
 
     class QuickStartFlags(TypedDict):
         """Quick-Start flags."""
 
         #: QS function.
         func: int
         #: Rate request/report.
         rate: int
 
+    class RPLFlags(TypedDict):
+        """RPL flags."""
+
+        #: Down flag.
+        down: int
+        #: Rank error flag.
+        rank_err: int
+        #: Forwarding error flag.
+        fwd_err: int
+
+    class MPLFlags(TypedDict):
+        """MPL flags."""
+
+        #: Seed-ID type. Identifies the length of the
+        #: Seed-ID.
+        type: int
+        #: Max flag. ``1`` indicates that the value in the
+        #: sequence field is known to be the largest sequence
+        #: number that was received from the MPL Seed.
+        max: int
+        #: Verification flag. ``0`` indicates that the MPL Option
+        #: conforms to this specification.
+        drop: int
+
+    class DFFFlags(TypedDict):
+        """``IP_DFF`` flags."""
+
+        #: Version.
+        ver: int
+        #: Duplicate flag.
+        dup: int
+        #: Retune flag.
+        ret: int
+
+    class SMFDPDTestFlag(TypedDict):
+        """``SMF_DPD`` test flag."""
+
+        #: Length.
+        len: int
+        #: DPD mode.
+        mode: int
+
     class QSTestFlags(TypedDict):
         """Quick start test flag."""
 
         #: QS function.
         func: int
 
     class QSNonce(TypedDict):
-        """Quick start nonce field."""
+        """Quick start nonce."""
 
         #: Nonce.
         nonce: int
 
 
+def mpl_opt_seed_id_len(pkt: 'dict[str, Any]') -> 'int':
+    """Return MPL Seed-ID length.
+
+    Args:
+        pkt: MPL option unpacked schema.
+
+    Returns:
+        MPL Seed-ID length.
+
+    """
+    s_type = pkt['flags']['type']
+    if s_type == 0:
+        return 0
+    if s_type == 1:
+        return 2
+    if s_type == 2:
+        return 8
+    if s_type == 3:
+        return 16
+    raise FieldValueError(f'IPv6-Opts: invalid MPL Seed-ID type: {s_type}')
+
+
+def smf_dpd_data_selector(pkt: 'dict[str, Any]') -> 'Field':
+    """Selector function for :attr:`_SMFDPDOption.data` field.
+
+    Args:
+        pkt: Packet data.
+
+    Returns:
+        * If ``mode`` is ``0``, returns a :class:`~pcapkit.corekit.fields.misc.SchemaField`
+          wrapped :class:`~pcapkit.protocols.schema.internet.hopopt.SMFIdentificationBasedDPDOption`
+          instance.
+        * If ``mode`` is ``1``, returns a :class:`~pcapkit.corekit.fields.misc.SchemaField`
+          wrapped :class:`~pcapkit.protocols.schema.internet.hopopt.SMFHashBasedDPDOption`
+          instance.
+
+    """
+    mode = Enum_SMFDPDMode.get(pkt['test']['mode'])
+    if mode == Enum_SMFDPDMode.I_DPD:
+        return SchemaField(length=pkt['test']['len'], schema=SMFIdentificationBasedDPDOption)
+    if mode == Enum_SMFDPDMode.H_DPD:
+        return SchemaField(length=pkt['test']['len'], schema=SMFHashBasedDPDOption)
+    raise FieldValueError(f'IPv6-Opts: invalid SMF DPD mode: {mode}')
+
+
+def smf_i_dpd_tid_selector(pkt: 'dict[str, Any]') -> 'Field':
+    """Selector function for :attr:`SMFIdentificationBasedDPDOption.tid` field.
+
+    Args:
+        pkt: Packet data.
+
+    Returns:
+        * If ``tid_type`` is ``0``, returns a :class:`~pcapkit.corekit.fields.misc.NoValueField`
+          instance.
+        * If ``tid_type`` is ``1``, returns a :class:`~pcapkit.corekit.fields.ipaddress.IPv4Field`
+          instance.
+        * If ``tid_type`` is ``2``, returns a :class:`~pcapkit.corekit.fields.ipaddress.IPv6Field`
+          instance.
+        * Otherwise, returns a :class:`~pcapkit.corekit.fields.strings.BytesField` instance.
+
+    """
+    tid_type = Enum_TaggerID.get(pkt['info']['type'])
+    tid_len = pkt['info']['len']
+
+    # update type
+    pkt['info']['type'] = tid_type
+
+    if tid_type == Enum_TaggerID.NULL:
+        if tid_len != 0:
+            raise FieldValueError(f'IPv6-Opts: invalid TaggerID length: {tid_len}')
+        return NoValueField()
+    if tid_type == Enum_TaggerID.IPv4:
+        if tid_len != 3:
+            raise FieldValueError(f'IPv6-Opts: invalid TaggerID length: {tid_len}')
+        return IPv4AddressField()
+    if tid_type == Enum_TaggerID.IPv6:
+        if tid_len != 15:
+            raise FieldValueError(f'IPv6-Opts: invalid TaggerID length: {tid_len}')
+        return IPv6AddressField()
+    return BytesField(length=tid_len + 1)
+
+
 def quick_start_data_selector(pkt: 'dict[str, Any]') -> 'Field':
-    """Selector function for :attr:`_QSOption.data` field.
+    """Selector function for :attr:`_QuickStartOption.data` field.
 
     Args:
         pkt: Packet data.
 
     Returns:
         * If ``func`` is ``0``, returns a :class:`~pcapkit.corekit.fields.misc.SchemaField`
           wrapped :class:`~pcapkit.protocols.schema.internet.hopopt.QuickStartRequestOption`
@@ -119,470 +216,449 @@
           instance.
 
     """
     func = Enum_QSFunction.get(pkt['flags']['func'])
     pkt['flags']['func'] = func
 
     if func == Enum_QSFunction.Quick_Start_Request:
-        return SchemaField(schema=QuickStartRequestOption)
+        return SchemaField(length=5, schema=QuickStartRequestOption)
     if func == Enum_QSFunction.Report_of_Approved_Rate:
-        return SchemaField(schema=QuickStartReportOption)
-    raise FieldValueError(f'HOPOPT: invalid QS function: {func}')
+        return SchemaField(length=5, schema=QuickStartReportOption)
+    raise FieldValueError(f'IPv6-Opts: invalid QS function: {func}')
 
 
 class Option(Schema):
-    """Header schema for IPv4 options."""
+    """Header schema for IPv6-Opts options."""
 
     #: Option type.
-    type: 'Enum_OptionNumber' = EnumField(length=1, namespace=Enum_OptionNumber)
-    #: Option length.
-    length: 'int' = ConditionalField(
-        UInt8Field(),
-        lambda pkt: pkt['type'] not in (Enum_OptionNumber.EOOL, Enum_OptionNumber.NOP),
+    type: 'Enum_Option' = EnumField(length=1, namespace=Enum_Option)
+    #: Option length (conditional in case of ``Pad1`` option).
+    len: 'int' = ConditionalField(
+        UInt8Field(default=0),
+        lambda pkt: pkt['type'] != Enum_Option.Pad1,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('Option', schema)
-
-        # for EOOL/NOP option, length is always 1
-        if schema.type in (Enum_OptionNumber.EOOL, Enum_OptionNumber.NOP):
-            schema.length = 1
-        return schema
+        # for Pad1 option, length is always 0
+        if self.type == Enum_Option.Pad1:
+            self.len = 0
+        return self
 
 
 class UnassignedOption(Option):
-    """Header schema for IPv4 unassigned options."""
+    """Header schema for IPv6-Opts unassigned options."""
 
     #: Option data.
-    data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
+    data: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', data: 'bytes') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', data: 'bytes') -> 'None': ...
+
 
+class PadOption(Option):
+    """Header schema for IPv6-Opts padding options."""
 
-class EOOLOption(Option):
-    """Header schema for IPv4 end of option list (``EOOL``) option."""
+    #: Padding.
+    pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'])
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int') -> 'None': ...
+
 
+class TunnelEncapsulationLimitOption(Option):
+    """Header schema for IPv6-Opts tunnel encapsulation limit options."""
 
-class NOPOption(Option):
-    """Header schema for IPv4 no operation (``NOP``) option."""
+    #: Tunnel encapsulation limit.
+    limit: 'int' = UInt8Field()
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', limit: 'int') -> 'None': ...
 
 
-class SECOption(Option):
-    """Header schema for IPv4 security (``SEC``) option."""
+class RouterAlertOption(Option):
+    """Header schema for IPv6-Opts router alert options."""
 
-    #: Classification level.
-    level: 'Enum_ClassificationLevel' = EnumField(length=1, namespace=Enum_ClassificationLevel)
-    #: Protection authority flags.
-    data: 'bytes' = ConditionalField(
-        BytesField(length=lambda pkt: pkt['length'] - 3),
-        lambda pkt: pkt['length'] > 3,
-    )
+    #: Router alert.
+    alert: 'Enum_RouterAlert' = EnumField(length=2, namespace=Enum_RouterAlert)
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', level: 'int', data: 'Optional[bytes]') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', alert: 'Enum_RouterAlert') -> 'None': ...
 
 
-class LSROption(Option):
-    """Header schema for IPv4 loose source route (``LSR``) option."""
+class CALIPSOOption(Option):
+    """Header schema for IPv6-Opts common architecture label IPv6 security options."""
 
-    #: Pointer.
-    pointer: 'int' = UInt8Field()
-    #: Route.
-    route: 'list[IPv4Address]' = ListField(
-        length=lambda pkt: pkt['pointer'] - 4,
-        item_type=IPv4Field(),
-    )
-    #: Remaining data buffer0.
-    remainder: 'bytes' = PaddingField(
-        length=lambda pkt: pkt['length'] - pkt['pointer'] + 1,
-        default=bytes(36),  # a reasonable default
+    #: CALIPSO domain of interpretation.
+    domain: 'int' = UInt32Field()
+    #: Compartment length.
+    cmpt_len: 'int' = UInt8Field()
+    #: Sens level.
+    level: 'int' = UInt8Field()
+    #: Checksum (CRC-16).
+    checksum: 'bytes' = BytesField(length=2)
+    #: Compartment bitmap.
+    bitmap: 'bytes' = ConditionalField(
+        BytesField(length=lambda pkt: pkt['cmpt_len'] * 4),
+        lambda pkt: pkt['cmpt_len'] > 0,
     )
+    #: Padding.
+    pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'] - 8 - pkt['cmpt_len'] * 4)
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', domain: 'int', cmpt_len: 'int',
+                     level: 'int', checksum: 'bytes', bitmap: 'Optional[bytes]') -> 'None': ...
 
 
-class TSOption(Option):
-    """Header schema for IPv4 timestamp (``TS``) option."""
+class _SMFDPDOption(Schema):
+    """Header schema for IPv6-Opts SMF DPD options with generic representation."""
 
-    #: Pointer.
-    pointer: 'int' = UInt8Field()
-    #: Overflow and flags.
-    flags: 'TSFlags' = BitField(length=1, namespace={
-        'oflw': (0, 4),
-        'flag': (4, 4),
-    })
-    #: Timestamps and internet addresses.
-    ts_data: 'list[int]' = ListField(
-        length=lambda pkt: pkt['pointer'] - 5 if pkt['flags']['flag'] != 3 else pkt['length'] - 4,
-        item_type=UInt32Field(),
-    )
-    #: Remaining data buffer.
-    remainder: 'bytes' = PaddingField(
-        length=lambda pkt: pkt['length'] - pkt['pointer'] + 1 if pkt['flags']['flag'] != 3 else 0,
-        default=bytes(36),  # 36 is the maximum length of the option data field for timestamps
+    #: SMF DPD mode.
+    test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=3, namespace={
+        'len': (1, 8),
+        'mode': (16, 1),
+    }))
+    #: SMF DPD data.
+    data: 'SMFIdentificationBasedDPDOption | SMFHashBasedDPDOption' = SwitchField(
+        selector=smf_dpd_data_selector,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFDPDOption':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('TSOption', schema)
-
-        ts_flag = Enum_TSFlag.get(schema.flags['flag'])
-        if ts_flag == Enum_TSFlag.Timestamp_Only:
-            ts_data = schema.ts_data
-            schema.data = []
-            ts_list = []  # type: list[int | timedelta]
-
-            for ts in ts_data:
-                schema.data.append(ts)
-
-                if ts >> 31:
-                    warn(f'IPv4: [OptNo {schema.type}] invalid format: timestamp error: {ts_val}', ProtocolWarning)
-                    ts_val = ts & 0x7FFFFFFF  # type: int | timedelta
-                else:
-                    ts_val = datetime.timedelta(milliseconds=ts)
-                ts_list.append(ts_val)
-            timestamp = tuple(ts_list)  # type: tuple[int | timedelta, ...] | OrderedMultiDict[IPv4Address, int | timedelta]
-        elif ts_flag == Enum_TSFlag.IP_with_Timestamp:
-            ts_data = schema.ts_data
-            schema.data = OrderedMultiDict()
-            timestamp = OrderedMultiDict()
-
-            for ip, ts in zip(ts_data[::2], ts_data[1::2]):
-                ip_val = cast('IPv4Address', ipaddress.ip_address(ip))
-                schema.data.add(ip_val, ts)
-
-                if ts >> 31:
-                    warn(f'IPv4: [OptNo {schema.type}] invalid format: timestamp error: {ts_val}', ProtocolWarning)
-                    ts_val = ts & 0x7FFFFFFF
-                else:
-                    ts_val = datetime.timedelta(milliseconds=ts)
-                timestamp.add(ip_val, ts_val)
-        elif ts_flag == Enum_TSFlag.Prespecified_IP_with_Timestamp:
-            ts_data = schema.ts_data
-            schema.data = OrderedMultiDict()
-            timestamp = OrderedMultiDict()
-
-            for ip, ts in zip(ts_data[::2], ts_data[1::2]):
-                ip_val = cast('IPv4Address', ipaddress.ip_address(ip))
-                schema.data.add(ip_val, ts)
-
-                if ts >> 31:
-                    warn(f'IPv4: [OptNo {schema.type}] invalid format: timestamp error: {ts_val}', ProtocolWarning)
-                    ts_val = ts & 0x7FFFFFFF
-                else:
-                    ts_val = datetime.timedelta(milliseconds=ts)
-                timestamp.add(ip_val, ts_val)
-
-            # extract also the prespecified IP addresses
-            # but set the timestamp to 0
-            pad = schema.remainder
-            for index in range(0, len(pad), 8):
-                buf_ip = pad[index:index + 4]
-                schema.data.add(ipaddress.ip_address(buf_ip), 0)  # type: ignore[arg-type]
-        else:
-            warn(f'IPv4: [OptNo {schema.type}] invalid format: unknown timestmap flag: {ts_flag}', ProtocolWarning)
-            schema.data = schema.ts_data
-            timestamp = tuple(schema.ts_data)
-
-        schema.ts_flag = ts_flag
-        schema.timestamp = timestamp
-        return schema
-
-    if TYPE_CHECKING:
-        ts_flag: 'Enum_TSFlag'
-        data: 'list[int] | OrderedMultiDict[IPv4Address, int]'
-        timestamp: 'tuple[int | timedelta] | OrderedMultiDict[IPv4Address, int | timedelta]'
-
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', flags: 'TSFlags', data: 'list[int]') -> 'None': ...
-
-
-class ESECOption(Option):
-    """Header schema for IPv4 extended security (``ESEC``) option."""
-
-    #: Additional security information format code.
-    format: 'int' = UInt8Field()
-    #: Additional security information.
-    info: 'bytes' = ConditionalField(
-        BytesField(length=lambda pkt: pkt['length'] - 3),
-        lambda pkt: pkt['length'] > 3,
-    )
-
-    if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', format: 'int', info: 'Optional[bytes]') -> 'None': ...
-
-
-class RROption(Option):
-    """Header schema for IPv4 record route (``RR``) option."""
-
-    #: Pointer.
-    pointer: 'int' = UInt8Field()
-    #: Route.
-    route: 'list[IPv4Address]' = ListField(
-        length=lambda pkt: pkt['pointer'] - 4,
-        item_type=IPv4Field(),
-    )
-    #: Remaining data buffer0.
-    remainder: 'bytes' = PaddingField(
-        length=lambda pkt: pkt['length'] - pkt['pointer'] + 1,
-        default=bytes(36),  # a reasonable default
-    )
-
-    if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
-
+        ret = self.data
+        return ret
 
-class SIDOption(Option):
-    """Header schema for IPv4 stream identifier (``SID``) option."""
 
-    #: Stream identifier.
-    sid: 'int' = UInt32Field()
+class SMFDPDOption(Option):
+    """Header schema for IPv6-Opts simplified multicast forwarding duplicate packet
+    detection (``SMF_DPD``) options."""
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', sid: 'int') -> 'None': ...
+        mode: 'Enum_SMFDPDMode'
 
 
-class SSROption(Option):
-    """Header schema for IPv4 strict source route (``SSR``) option."""
+class SMFIdentificationBasedDPDOption(SMFDPDOption):
+    """Header schema for IPv6-Opts SMF identification-based DPD options."""
 
-    #: Pointer.
-    pointer: 'int' = UInt8Field()
-    #: Route.
-    route: 'list[IPv4Address]' = ListField(
-        length=lambda pkt: pkt['pointer'] - 4,
-        item_type=IPv4Field(),
-    )
-    #: Remaining data buffer0.
-    remainder: 'bytes' = PaddingField(
-        length=lambda pkt: pkt['length'] - pkt['pointer'] + 1,
-        default=bytes(36),  # a reasonable default
-    )
+    test: 'SMFDPDTestFlag' = ForwardMatchField(BitField(length=1, namespace={
+        'mode': (0, 1),
+    }))
+    #: TaggerID information.
+    info: 'TaggerIDInfo' = BitField(length=1, namespace={
+        'mode': (0, 1),
+        'type': (1, 3),
+        'len': (4, 4),
+    })
+    #: TaggerID.
+    tid: 'bytes | IPv4Address | IPv6Address' = ConditionalField(
+        SwitchField(selector=smf_i_dpd_tid_selector),
+        lambda pkt: pkt['info']['type'] != 0,
+    )
+    #: Identifier.
+    id: 'bytes' = BytesField(length=lambda pkt: pkt['len'] - (
+        1 if pkt['info']['type'] == 0 else (pkt['info']['len'] + 2)
+    ))
 
-    if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', pointer: 'int', route: 'list[IPv4Address | str | bytes | int]') -> 'None': ...
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
+        """Revise ``schema`` data after unpacking process.
 
+        Args:
+            packet: Unpacked data.
 
-class MTUPOption(Option):
-    """Header schema for IPv4 MTU probe (``MTUP``) option."""
+        Returns:
+            Revised schema.
 
-    #: MTU.
-    mtu: 'int' = UInt16Field()
+        """
+        ret = super().post_process(packet)  # type: SMFIdentificationBasedDPDOption
+        ret.mode = Enum_SMFDPDMode.I_DPD
+        return ret
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', mtu: 'int') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', info: 'TaggerIDInfo',
+                     tid: 'Optional[bytes]', id: 'bytes') -> 'None': ...
 
 
-class MTUROption(Option):
-    """Header schema for IPv4 MTU reply (``MTUR``) option."""
+class SMFHashBasedDPDOption(SMFDPDOption):
+    """Header schema for IPv6-Opts SMF hash-based DPD options."""
 
-    #: MTU.
-    mtu: 'int' = UInt16Field()
+    #: Hash assist value (HAV).
+    hav: 'bytes' = BytesField(length=lambda pkt: pkt['len'])
 
-    if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', mtu: 'int') -> 'None': ...
+    def post_process(self, packet: 'dict[str, Any]') -> 'SMFIdentificationBasedDPDOption':
+        """Revise ``schema`` data after unpacking process.
 
+        Args:
+            packet: Unpacked data.
 
-class TROption(Option):
-    """Header schema for IPv4 traceroute (``TR``) option."""
+        Returns:
+            Revised schema.
 
-    #: ID number.
-    id: 'int' = UInt16Field()
-    #: Outbound hop count.
-    out: 'int' = UInt16Field()
-    #: Return hop count.
-    ret: 'int' = UInt16Field()
-    #: Originator IP address.
-    origin: 'IPv4Address' = IPv4Field()
+        """
+        ret = super().post_process(packet)  # type: SMFIdentificationBasedDPDOption
+        ret.mode = Enum_SMFDPDMode.H_DPD
+        return ret
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', id: 'int', out: 'int', ret: 'int', origin: 'IPv4Address | str | bytes | int') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', hav: 'bytes') -> 'None': ...
 
 
-class RTRALTOption(Option):
-    """Header schema for IPv4 router alert (``RTRALT``) option."""
+class PDMOption(Option):
+    """Header schema for IPv6-Opts performance and diagnostic metrics (PDM) options."""
 
-    #: Router alert value.
-    alert: 'Enum_RouterAlert' = EnumField(length=2, namespace=Enum_RouterAlert)
+    #: Scale delta time last received (DTLR).
+    scaledtlr: 'int' = UInt8Field()
+    #: Scale delta time last sent (DTLS).
+    scaledtls: 'int' = UInt8Field()
+    #: Packet sequence number (PSN) this packet.
+    psntp: 'int' = UInt16Field()
+    #: Packet sequence number (PSN) last received.
+    psnlr: 'int' = UInt16Field()
+    #: Delta time last received (DTLR).
+    deltatlr: 'int' = UInt16Field()
+    #: Delta time last sent (DTLS).
+    deltatls: 'int' = UInt16Field()
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', alert: 'Enum_RouterAlert') -> 'None': ...
+        def __init__(self, type: 'Enum_Option', len: 'int', scaledtlr: 'int', scaledtls: 'int',
+                     psntp: 'int', psnlr: 'int', deltatlr: 'int', deltatls: 'int') -> 'None': ...
 
 
-class _QSOption(Schema):
-    """Header schema for IPv4 quick start (``QS``) options in generic representation."""
+class _QuickStartOption(Schema):
+    """Header schema for IPv6-Opts quick start options in generic representation."""
 
     #: Flags.
     flags: 'QSTestFlags' = ForwardMatchField(BitField(length=3, namespace={
         'func': (16, 4),
     }))
     #: QS data.
     data: 'QuickStartRequestOption | QuickStartReportOption' = SwitchField(
-        length=5,
         selector=quick_start_data_selector,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'QuickStartOption':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('_QSOption', schema)
-
-        ret = schema.data
-        ret.func = Enum_QSFunction.get(packet['flags']['func'])
+        ret = self.data
+        ret.func = Enum_QSFunction.get(self.flags['func'])
         return ret
 
 
-class QSOption(Option):
-    """Header schema for IPV4 quick start (``QS``) options."""
+class QuickStartOption(Option):
+    """Header schema for IPv6-Opts quick start options."""
 
     #: Flags.
     flags: 'QuickStartFlags' = BitField(length=1, namespace={
         'func': (0, 4),
         'rate': (4, 4),
     })
 
     if TYPE_CHECKING:
         func: 'Enum_QSFunction'
 
 
-class QuickStartRequestOption(QSOption):
-    """Header schema for IPV4 quick start request options."""
+class QuickStartRequestOption(QuickStartOption):
+    """Header schema for IPv6-Opts quick start request options."""
 
     #: QS time-to-live (TTL).
     ttl: 'int' = UInt8Field()
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
         'nonce': (0, 30),
     })
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', flags: 'QuickStartFlags',
+        def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      ttl: 'int', nonce: 'QSNonce') -> 'None': ...
 
 
-class QuickStartReportOption(QSOption):
-    """Header schema for IPV4 quick start report of approved rate options."""
+class QuickStartReportOption(QuickStartOption):
+    """Header schema for IPv6-Opts quick start report of approved rate options."""
 
+    #: Reserved.
+    reserved: 'bytes' = PaddingField(length=1)
     #: QS nonce.
     nonce: 'QSNonce' = BitField(length=4, namespace={
         'nonce': (0, 30),
     })
 
     if TYPE_CHECKING:
-        def __init__(self, type: 'Enum_OptionNumber', length: 'int', flags: 'QuickStartFlags',
+        def __init__(self, type: 'Enum_Option', len: 'int', flags: 'QuickStartFlags',
                      nonce: 'QSNonce') -> 'None': ...
 
 
-class IPv4(Schema):
-    """Header schema for IPv4 packet."""
+class RPLOption(Option):
+    """Header schema for IPv6-Opts routing protocol for low-power and lossy networks (RPL) options."""
 
-    #: Version and header length.
-    vihl: 'VerIHLField' = BitField(length=1, namespace={
-        'version': (0, 4),
-        'ihl': (4, 8),
+    #: Flags.
+    flags: 'RPLFlags' = BitField(length=1, namespace={
+        'down': (0, 1),
+        'rank_err': (1, 1),
+        'fwd_err': (2, 1),
     })
-    #: Type of service.
-    tos: 'ToSField' = BitField(length=1, namespace={
-        'pre': (0, 3),
-        'del': (3, 1),
-        'thr': (4, 1),
-        'rel': (5, 1),
-        'ecn': (6, 2),
+    #: RPL instance ID.
+    id: 'int' = UInt8Field()
+    #: Sender rank.
+    rank: 'int' = UInt16Field()
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', flags: 'RPLFlags', id: 'int',
+                     rank: 'int') -> 'None': ...
+
+
+class MPLOption(Option):
+    """Header schema for IPv6-Opts multicast protocol for low-power and lossy networks (MPL) options."""
+
+    #: Flags.
+    flags: 'MPLFlags' = BitField(length=1, namespace={
+        'type': (0, 2),
+        'max': (2, 1),
+        'drop': (3, 1),
     })
-    #: Total length.
-    length: 'int' = UInt16Field()
-    #: Identification.
-    id: 'int' = UInt16Field()
-    #: Flags and fragment offset.
-    flags: 'Flags' = BitField(length=2, namespace={
-        'df': (1, 1),
-        'mf': (2, 1),
-        'offset': (3, 13),
+    #: MPL sequence number.
+    seq: 'int' = UInt8Field()
+    #: MPL Seed-ID.
+    seed: 'int' = ConditionalField(
+        NumberField(length=mpl_opt_seed_id_len, signed=False),
+        lambda pkt: pkt['flags']['type'] != Enum_SeedID.IPV6_SOURCE_ADDRESS,
+    )
+    #: Reserved data (padding).
+    pad: 'bytes' = PaddingField(length=lambda pkt: pkt['len'] - 2 - (
+        0 if pkt['flags']['type'] == 0 else mpl_opt_seed_id_len(pkt)
+    ))
+
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
+        """Revise ``schema`` data after unpacking process.
+
+        Args:
+            packet: Unpacked data.
+
+        Returns:
+            Revised schema.
+
+        """
+        if self.flags['type'] == Enum_SeedID.IPV6_SOURCE_ADDRESS:
+            self.seed = packet.get('src', NoValue)
+        return self
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', flags: 'MPLFlags', seq: 'int',
+                     seed: 'Optional[int]') -> 'None': ...
+
+
+class ILNPOption(Option):
+    """Header schema for IPv6-Opts identifier-locator network protocol (ILNP) options."""
+
+    #: Nonce value.
+    nonce: 'int' = NumberField(length=lambda pkt: pkt['len'], signed=False)
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', nonce: 'int') -> 'None': ...
+
+
+class LineIdentificationOption(Option):
+    """Header schema for IPv6-Opts line-identification options."""
+
+    #: Line ID length.
+    id_len: 'int' = UInt8Field()
+    #: Line ID.
+    id: 'bytes' = BytesField(length=lambda pkt: pkt['id_len'])
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', id_len: 'int', id: 'bytes') -> 'None': ...
+
+
+class JumboPayloadOption(Option):
+    """Header schema for IPv6-Opts jumbo payload options."""
+
+    #: Jumbo payload length.
+    jumbo_len: 'int' = UInt32Field()
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', jumbo_len: 'int') -> 'None': ...
+
+
+class HomeAddressOption(Option):
+    """Header schema for IPv6-Opts home address options."""
+
+    #: Home address.
+    addr: 'IPv6Address' = IPv6AddressField()
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', addr: 'IPv6Address | int | str | bytes') -> 'None': ...
+
+
+class IPDFFOption(Option):
+    """Header schema for IPv6-Opts depth-first forwarding (``IP_DFF``) options."""
+
+    #: Flags.
+    flags: 'DFFFlags' = BitField(length=1, namespace={
+        'ver': (0, 2),
+        'dup': (2, 1),
+        'ret': (3, 1),
     })
-    #: Time to live.
-    ttl: 'int' = UInt8Field()
-    #: Protocol.
-    proto: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
-    #: Header checksum.
-    chksum: 'bytes' = BytesField(length=2)
-    #: Source address.
-    src: 'IPv4Address' = IPv4Field()
-    #: Destination address.
-    dst: 'IPv4Address' = IPv4Field()
+    #: Sequence number.
+    seq: 'int' = UInt16Field()
+
+    if TYPE_CHECKING:
+        def __init__(self, type: 'Enum_Option', len: 'int', flags: 'DFFFlags', seq: 'int') -> 'None': ...
+
+
+class IPv6_Opts(Schema):
+    """Header schema for IPv6-Opts packet."""
+
+    #: Next header.
+    next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
+    #: Header length.
+    len: 'int' = UInt8Field()
     #: Options.
     options: 'list[Option]' = OptionField(
-        length=lambda pkt: pkt['vihl']['ihl'] * 4 - 20,
+        length=lambda pkt: pkt['len'] * 8 + 6,
         base_schema=Option,
         type_name='type',
         registry=collections.defaultdict(lambda: UnassignedOption, {
-            Enum_OptionNumber.EOOL: EOOLOption,
-            Enum_OptionNumber.NOP: NOPOption,
-            Enum_OptionNumber.SEC: SECOption,
-            Enum_OptionNumber.LSR: LSROption,
-            Enum_OptionNumber.E_SEC: ESECOption,
-            Enum_OptionNumber.RR: RROption,
-            Enum_OptionNumber.SID: SIDOption,
-            Enum_OptionNumber.SSR: SSROption,
-            Enum_OptionNumber.MTUP: MTUPOption,
-            Enum_OptionNumber.MTUR: MTUROption,
-            Enum_OptionNumber.TR: TROption,
-            Enum_OptionNumber.RTRALT: RTRALTOption,
-            Enum_OptionNumber.QS: _QSOption,
-        }))
-    #: Padding.
-    padding: 'bytes' = PaddingField(length=lambda pkt: pkt.get('__option_padding__', 0))
+            Enum_Option.Pad1: PadOption,
+            Enum_Option.PadN: PadOption,
+            Enum_Option.Tunnel_Encapsulation_Limit: TunnelEncapsulationLimitOption,
+            Enum_Option.Router_Alert: RouterAlertOption,
+            Enum_Option.CALIPSO: CALIPSOOption,
+            Enum_Option.SMF_DPD: _SMFDPDOption,
+            Enum_Option.PDM: PDMOption,
+            Enum_Option.Quick_Start: _QuickStartOption,
+            Enum_Option.RPL_Option_0x63: RPLOption,
+            Enum_Option.MPL_Option: MPLOption,
+            Enum_Option.ILNP_Nonce: ILNPOption,
+            Enum_Option.Line_Identification_Option: LineIdentificationOption,
+            Enum_Option.Jumbo_Payload: JumboPayloadOption,
+            Enum_Option.Home_Address: HomeAddressOption,
+            Enum_Option.IP_DFF: IPDFFOption,
+        })
+    )
     #: Payload.
-    payload: 'bytes' = PayloadField(length=lambda pkt: pkt['length'] - pkt['vihl']['ihl'] * 4)
+    payload: 'bytes' = PayloadField()
 
     if TYPE_CHECKING:
-        def __init__(self, vihl: 'VerIHLField', tos: 'ToSField', length: 'int', id: 'int',
-                     flags: 'Flags', ttl: 'int', proto: 'Enum_TransType', chksum: 'bytes',
-                     src: 'IPv4Address | str | bytes | int', dst: 'IPv4Address | str | bytes | int',
-                     options: 'list[Option | bytes] | bytes', payload: 'bytes | Protocol | Schema') -> 'None': ...
+        def __init__(self, next: 'Enum_TransType', len: 'int',
+                     options: 'bytes | list[bytes | Option]',
+                     payload: 'bytes | Protocol | Schema') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
 """header schema for internet protocol version 6"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
-from pcapkit.corekit.fields.ipaddress import IPv6Field
+from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field
 from pcapkit.corekit.fields.strings import BitField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = ['IPv6']
@@ -45,17 +45,17 @@
     #: Payload length.
     length: int = UInt16Field()
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
     #: Hop limit.
     limit: int = UInt8Field()
     #: Source address.
-    src: 'IPv6Address' = IPv6Field()
+    src: 'IPv6Address' = IPv6AddressField()
     #: Destination address.
-    dst: 'IPv6Address' = IPv6Field()
+    dst: 'IPv6Address' = IPv6AddressField()
     #: Payload.
     payload: 'bytes' = PayloadField(length=lambda pkt: pkt['length'])
 
     if TYPE_CHECKING:
         def __init__(self, hextet: 'IPv6Hextet', length: 'int', next: 'Enum_TransType',
                      limit: 'int', src: 'IPv6Address | bytes | str | int',
                      dst: 'IPv6Address | bytes | str | int',
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6_frag.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_frag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipv6_route.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipv6_route.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import ipaddress
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.ipv6.routing import Routing as Enum_Routing
 from pcapkit.const.reg.transtype import TransType as Enum_TransType
 from pcapkit.corekit.fields.collections import ListField
-from pcapkit.corekit.fields.ipaddress import IPv6Field
+from pcapkit.corekit.fields.ipaddress import IPv6AddressField
 from pcapkit.corekit.fields.misc import PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.logging import SPHINX_TYPE_CHECKING
 
 __all__ = [
@@ -20,15 +20,15 @@
 
     'RoutingType',
     'UnknownType', 'SourceRoute', 'Type2', 'RPL',
 ]
 
 if TYPE_CHECKING:
     from ipaddress import IPv6Address
-    from typing import IO, Any, Optional
+    from typing import Any, Optional
 
     from pcapkit.corekit.fields.field import _Field as Field
     from pcapkit.protocols.protocol import Protocol
 
 if SPHINX_TYPE_CHECKING:
     from typing_extensions import TypedDict
 
@@ -54,20 +54,20 @@
         * If ``type`` is ``3``, returns a :class:`~pcapkit.corekit.fields.misc.SchemaField`
           wrapped :class:`~pcapkit.protocols.schema.internet.ipv6_route.RPL`
           instance.
 
     """
     type = cast('Enum_Routing', pkt['type'])
     if type == Enum_Routing.Source_Route:
-        return SchemaField(schema=SourceRoute)
+        return SchemaField(length=pkt['length'] * 8 - 4, schema=SourceRoute)
     if type == Enum_Routing.Type_2_Routing_Header:
-        return SchemaField(schema=Type2)
+        return SchemaField(length=pkt['length'] * 8 - 4, schema=Type2)
     if type == Enum_Routing.RPL_Source_Route_Header:
-        return SchemaField(schema=RPL)
-    return SchemaField(schema=UnknownType)
+        return SchemaField(length=pkt['length'] * 8 - 4, schema=RPL)
+    return SchemaField(length=pkt['length'] * 8 - 4, schema=UnknownType)
 
 
 class IPv6_Route(Schema):
     """Header schema for IPv6-Route packet."""
 
     #: Next header.
     next: 'Enum_TransType' = EnumField(length=1, namespace=Enum_TransType)
@@ -75,15 +75,14 @@
     length: 'int' = UInt8Field()
     #: Routing type.
     type: 'Enum_Routing' = EnumField(length=1, namespace=Enum_Routing)
     #: Segments left.
     seg_left: 'int' = UInt8Field()
     #: Routing data.
     data: 'RoutingType' = SwitchField(
-        length=lambda pkt: pkt['length'] * 8 - 4,
         selector=ipv6_route_data_selector,
     )
     #: Payload.
     payload: 'bytes' = PayloadField()
 
     if TYPE_CHECKING:
         def __init__(self, next: 'Enum_TransType', length: 'int', type: 'Enum_Routing',
@@ -94,42 +93,42 @@
     """Header schema for IPv6-Route type-specific routing data."""
 
 
 class UnknownType(RoutingType):
     """Header schema for IPv6-Route unknown type routing data."""
 
     #: Type-specific data.
-    data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] * 8 - 4)
+    data: 'bytes' = BytesField(length=lambda pkt: pkt['__length__'])
 
     if TYPE_CHECKING:
         def __init__(self, data: 'bytes') -> 'None': ...
 
 
 class SourceRoute(RoutingType):
     """Header schema for IPv6-Route source route routing data."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: Addresses.
     ip: 'list[IPv6Address]' = ListField(
-        length=lambda pkt: pkt['length'] * 8,
-        item_type=IPv6Field(),
+        length=lambda pkt: pkt['__length__'],
+        item_type=IPv6AddressField(),
     )
 
     if TYPE_CHECKING:
         def __init__(self, ip: 'list[IPv6Address | str | int | bytes]') -> 'None': ...
 
 
 class Type2(RoutingType):
     """Header schema for IPv6-Route type 2 routing data."""
 
     #: Reserved.
     reserved: 'bytes' = PaddingField(length=4)
     #: Addresses.
-    ip: 'IPv6Address' = IPv6Field()
+    ip: 'IPv6Address' = IPv6AddressField()
 
     if TYPE_CHECKING:
         def __init__(self, ip: 'IPv6Address | str | int | bytes') -> 'None': ...
 
 
 class RPL(RoutingType):
     """Header schema for IPv6-Route RPL routing data."""
@@ -140,72 +139,64 @@
     cmpr_e: 'int' = UInt8Field()
     #: Padding length and reserved.
     pad: 'PadInfo' = BitField(length=3, namespace={
         'pad_len': (0, 4),
     })
     #: Addresses.
     addresses: 'bytes' = ListField(
-        length=lambda pkt: pkt['length'] * 8 - pkt['pad']['pad_len'],
+        length=lambda pkt: pkt['__length__'] - pkt['pad']['pad_len'],
     )
     #: Padding.
     padding: 'bytes' = PaddingField(length=lambda pkt: pkt['pad']['pad_len'])
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('RPL', schema)
-
-        buffer = cast('bytes', schema.ip)
+        buffer = cast('bytes', self.ip)
         dst_val = cast('Optional[IPv6Address]', packet.get('dst'))
         dst = dst_val.packed if dst_val is not None else None
 
-        ilen = 16 - schema.cmpr_i
-        elen = 16 - schema.cmpr_e
+        ilen = 16 - self.cmpr_i
+        elen = 16 - self.cmpr_e
         addr = []  # type: list[IPv6Address | bytes]
         counter = 0
 
         # Addresses[1..n-1]
-        for _ in range((len(buffer) - schema.pad['pad_len'] - elen) // ilen):
+        for _ in range((len(buffer) - self.pad['pad_len'] - elen) // ilen):
             buf = buffer[counter:counter + ilen]
             if dst is None:
-                if schema.cmpr_i == 0:
+                if self.cmpr_i == 0:
                     addr.append(cast('IPv6Address', ipaddress.ip_address(buf)))
                 else:
                     addr.append(buf)
             else:
-                buf = dst[:schema.cmpr_i] + buf
+                buf = dst[:self.cmpr_i] + buf
                 addr.append(cast('IPv6Address', ipaddress.ip_address(buf)))
             counter += ilen
 
         # Addresses[n]
         buf = buffer[counter:counter + elen]
         if dst is None:
-            if schema.cmpr_e == 0:
+            if self.cmpr_e == 0:
                 addr.append(cast('IPv6Address', ipaddress.ip_address(buf)))
             else:
                 addr.append(buf)
         else:
-            buf = dst[:schema.cmpr_e] + buf
+            buf = dst[:self.cmpr_e] + buf
             addr.append(cast('IPv6Address', ipaddress.ip_address(buf)))
 
-        schema.ip = addr
-        return schema
+        self.ip = addr
+        return self
 
     if TYPE_CHECKING:
         #: Addresses (SRH prefix compression decoded).
         ip: 'list[IPv6Address | bytes]'
 
         def __init__(self, cmpr_i: 'int', cmpr_e: 'int', pad: 'PadInfo',
                      addresses: 'list[bytes]') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/ipx.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/ipx.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/internet/mh.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/internet/mh.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/arp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/arp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/ethernet.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ethernet.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def callback_payload(self: 'PayloadField', packet: 'dict[str, Any]') -> 'None':
     """Callback function for :attr:`Ethernet.payload`."""
     from pcapkit.protocols.link.ethernet import Ethernet  # pylint: disable=import-outside-toplevel
 
     type_ = packet['type']
-    module, name = Ethernet.__proto__[type_]  # type: ignore[attr-defined]
+    module, name = Ethernet.__proto__[type_]
     protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
     self.protocol = protocol
 
 
 class Ethernet(Schema):
     """Header schema for ethernet packet."""
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/l2tp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/l2tp.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,39 +48,39 @@
         'offset': (6, 1),
         'prio': (7, 1),
         'version': (12, 4),
     })
     #: Length of L2TP packet.
     length: 'int' = ConditionalField(
         UInt16Field(),
-        lambda packet: packet['flags'].get('length', False),
+        lambda packet: packet['flags']['len'],
     )
     #: Tunnel ID of L2TP packet.
     tunnel_id: 'int' = UInt16Field()
     #: Session ID of L2TP packet.
     session_id: 'int' = UInt16Field()
     #: Sequence number of L2TP packet.
     ns: 'int' = ConditionalField(
         UInt16Field(),
-        lambda packet: packet['flags'].get('seq', False),
+        lambda packet: packet['flags']['seq'],
     )
     #: Next sequence number of L2TP packet.
     nr: 'int' = ConditionalField(
         UInt16Field(),
-        lambda packet: packet['flags'].get('seq', False),
+        lambda packet: packet['flags']['seq'],
     )
     #: Offset size of L2TP packet.
     offset: 'int' = ConditionalField(
         UInt16Field(),
-        lambda packet: packet['flags'].get('offset', False),
+        lambda packet: packet['flags']['offset'],
     )
     #: Padding of L2TP packet.
     padding: 'bytes' = ConditionalField(
-        PaddingField(length=lambda pkt: pkt.get('offset', 0)),
-        lambda packet: packet['flags'].get('offset', False),
+        PaddingField(length=lambda pkt: pkt['offset']),
+        lambda packet: packet['flags']['offset'],
     )
     #: Payload of L2TP packet.
     payload: 'bytes' = PayloadField()
 
     if TYPE_CHECKING:
         def __init__(self, flags: 'FlagsType', length: 'Optional[int]', tunnel_id: 'int',
                      session_id: 'int', ns: 'Optional[int]', nr: 'Optional[int]',
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/ospf.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/ospf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # mypy: disable-error-code=assignment
 """header schema for OSPF protocol"""
 
 from typing import TYPE_CHECKING
 
 from pcapkit.const.ospf.authentication import Authentication as Enum_Authentication
 from pcapkit.const.ospf.packet import Packet as Enum_Packet
-from pcapkit.corekit.fields.ipaddress import IPv4Field
+from pcapkit.corekit.fields.ipaddress import IPv4AddressField
 from pcapkit.corekit.fields.misc import PayloadField, SchemaField, SwitchField
 from pcapkit.corekit.fields.numbers import EnumField, UInt8Field, UInt16Field, UInt32Field
 from pcapkit.corekit.fields.strings import BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 
 __all__ = ['OSPF', 'CrytographicAuthentication']
 
@@ -61,24 +61,23 @@
     #: Version.
     version: 'int' = UInt8Field()
     #: Type.
     type: 'Enum_Packet' = EnumField(length=1, namespace=Enum_Packet)
     #: Length.
     length: 'int' = UInt16Field()
     #: Router ID.
-    router_id: 'IPv4Address' = IPv4Field()
+    router_id: 'IPv4Address' = IPv4AddressField()
     #: Area ID.
-    area_id: 'IPv4Address' = IPv4Field()
+    area_id: 'IPv4Address' = IPv4AddressField()
     #: Checksum.
     checksum: 'bytes' = BytesField(length=2)
     #: Authentication type.
     auth_type: 'Enum_Authentication' = EnumField(length=2, namespace=Enum_Authentication)
     #: Authentication data.
     auth_data: 'bytes | CrytographicAuthentication' = SwitchField(
-        length=8,
         selector=ospf_auth_data_selector,
     )
     #: Payload.
     payload: 'bytes' = PayloadField()
 
     if TYPE_CHECKING:
         def __init__(self, version: 'int', type: 'Enum_Packet', length: 'int',
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/link/vlan.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/link/vlan.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/null.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/null.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/frame.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/frame.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 # -*- coding: utf-8 -*-
 # mypy: disable-error-code=assignment
 """header schema for frame header of PCAP file format"""
 
+import sys
 from typing import TYPE_CHECKING
 
 from pcapkit.corekit.fields.misc import PayloadField
 from pcapkit.corekit.fields.numbers import UInt32Field
 from pcapkit.protocols.schema.schema import Schema
 
 __all__ = ['Frame']
 
 if TYPE_CHECKING:
+    from typing import Any
+
+    from pcapkit.corekit.fields.numbers import NumberField as Field
     from pcapkit.protocols.protocol import Protocol
 
 
+def byteorder_callback(field: 'Field', packet: 'dict[str, Any]') -> 'None':
+    """Update byte order of PCAP file.
+
+    Args:
+        field: Field instance.
+        packet: Packet data.
+
+    """
+    field._byteorder = packet.get('byteorder', sys.byteorder)
+
+
 class Frame(Schema):
     """Frame header of PCAP file format."""
 
     __payload__ = 'packet'
 
     #: Timestamp seconds.
-    ts_sec: 'int' = UInt32Field(byteorder='little')
+    ts_sec: 'int' = UInt32Field(callback=byteorder_callback)
     #: Timestamp microseconds.
-    ts_usec: 'int' = UInt32Field(byteorder='little')
+    ts_usec: 'int' = UInt32Field(callback=byteorder_callback)
     #: Number of octets of packet saved in file.
-    incl_len: 'int' = UInt32Field(byteorder='little')
+    incl_len: 'int' = UInt32Field(callback=byteorder_callback)
     #: Actual length of packet.
-    orig_len: 'int' = UInt32Field(byteorder='little')
+    orig_len: 'int' = UInt32Field(callback=byteorder_callback)
     #: Payload.
     packet: 'bytes' = PayloadField(length=lambda pkt: pkt['incl_len'])
 
     if TYPE_CHECKING:
         def __init__(self, ts_sec: 'int', ts_usec: 'int', incl_len: 'int',
                      orig_len: 'int', packet: 'bytes | Protocol | Schema') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/pcap/header.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/pcap/header.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,12 +51,12 @@
     #: GMT to local correction.
     thiszone: 'int' = Int32Field(callback=magic_number_callback)
     #: Accuracy of timestamps.
     sigfigs: 'int' = UInt32Field(callback=magic_number_callback)
     #: Max length of captured packets, in octets.
     snaplen: 'int' = UInt32Field(callback=magic_number_callback)
     #: Data link type.
-    network: 'Enum_LinkType' = EnumField(length=4, namespace=Enum_LinkType, byteorder='little')
+    network: 'Enum_LinkType' = EnumField(length=4, namespace=Enum_LinkType, callback=magic_number_callback)
 
     if TYPE_CHECKING:
         def __init__(self, magic_number: 'bytes', version_major: 'int', version_minor: 'int',  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
                      thiszone: 'int', sigfigs: 'int', snaplen: 'int', network: 'int') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/misc/raw.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/misc/raw.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,11 @@
     from pcapkit.protocols.protocol import Protocol
 
 
 class Raw(Schema):
     """Schema for raw packet."""
 
     #: Packet data.
-    packet: 'bytes' = PayloadField(length=lambda x: x.get('__length__', None),
-                                   default=b'', protocol='Raw')
+    packet: 'bytes' = PayloadField(length=lambda x: x['__length__'], default=b'')
 
     if TYPE_CHECKING:
         def __init__(self, packet: 'bytes | Schema | Protocol') -> 'None': ...  # pylint: disable=unused-argument,super-init-not-called,multiple-statements
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/schema.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 """schema for protocol headers"""
 
 import collections
 import collections.abc
-import functools
 import io
 import itertools
 from typing import TYPE_CHECKING, Generic, TypeVar, cast
 
-from pcapkit.corekit.fields.collections import ListField
+from pcapkit.corekit.fields.collections import ListField, OptionField
 from pcapkit.corekit.fields.field import NoValue, _Field
 from pcapkit.corekit.fields.misc import ConditionalField, ForwardMatchField, PayloadField
 from pcapkit.corekit.fields.strings import PaddingField
 from pcapkit.utilities.compat import Mapping
 from pcapkit.utilities.decorators import prepare
-from pcapkit.utilities.exceptions import NoDefaultValue, ProtocolUnbound
-from pcapkit.utilities.warnings import UnknownFieldWarning, warn
+from pcapkit.utilities.exceptions import NoDefaultValue, ProtocolUnbound, stacklevel
+from pcapkit.utilities.warnings import SchemaWarning, UnknownFieldWarning, warn
 
 if TYPE_CHECKING:
     from collections import OrderedDict
     from typing import IO, Any, Iterable, Iterator, Optional
 
+    from typing_extensions import Self
+
 __all__ = ['Schema']
 
 VT = TypeVar('VT')
 
 
 class Schema(Mapping[str, VT], Generic[VT]):
     """Schema for protocol headers."""
@@ -48,15 +49,15 @@
     #: Field name of the payload.
     __payload__: 'str' = 'payload'
     #: List of additional built-in names.
     __additional__: 'list[str]' = []
     #: List of names to be excluded from :obj:`dict` conversion.
     __excluded__: 'list[str]' = []
 
-    def __new__(cls, *args: 'VT', **kwargs: 'VT') -> 'Schema':  # pylint: disable=unused-argument
+    def __new__(cls, *args: 'VT', **kwargs: 'VT') -> 'Self':  # pylint: disable=unused-argument
         """Create a new instance.
 
         The class will try to automatically generate ``__init__`` method with
         the same signature as specified in class variables' type annotations,
         which is inspired by :pep:`557` (:mod:`dataclasses`).
 
         Args:
@@ -118,25 +119,25 @@
         # NOTE: We only generate typed ``__init__`` method if only the class
         # has type annotations from any of itself and its base classes.
         if args_:
             # NOTE: The following code is to make the ``__init__`` method work.
             # It is inspired from the :func:`dataclasses._create_fn` function.
             init_ = (
                 f'def __create_fn__():\n'
-                f'    def __init__(self, {", ".join(args_)}):\n'
+                f'    def __init__(self, {", ".join(args_)}, *, __packet__=None):\n'
                 f'        self.__update__({", ".join(dict_)})\n'
-                f'        self.__post_init__()\n'
+                f'        self.__post_init__(__packet__)\n'
                 f'    return __init__\n'
             )
         else:
             init_ = (
                 'def __create_fn__():\n'
-                '    def __init__(self, dict_=None, **kwargs):\n'
+                '    def __init__(self, dict_=None, **kwargs, *, __packet__=None):\n'
                 '        self.__update__(dict_, **kwargs)\n'
-                '        self.__post_init__()\n'
+                '        self.__post_init__(__packet__)\n'
                 '    return __init__\n'
             )
 
         ns = {}  # type: dict[str, Any]
         exec(init_, None, ns)  # pylint: disable=exec-used # nosec
         cls.__init__ = ns['__create_fn__']()
         cls.__init__.__qualname__ = f'{cls.__name__}.__init__'
@@ -152,19 +153,19 @@
         # NOTE: We only create the attributes for the instance itself,
         # to avoid creating shared attributes for the class.
         self.__buffer__ = {name: b'' for name in self.__fields__.keys()}
         self.__updated__ = True
 
         return self
 
-    def __post_init__(self) -> 'None':
+    def __post_init__(self, packet: 'Optional[dict[str, Any]]' = None) -> 'None':
         for name, field in self.__fields__.items():
             if self.__dict__[name] in (NoValue, None):
                 self.__dict__[name] = field.default
-        self.pack()
+        self.pack(packet)
 
     def __update__(self, dict_: 'Optional[Mapping[str, VT] | Iterable[tuple[str, VT]]]' = None,
                    **kwargs: 'VT') -> 'None':
         # NOTE: Keys with the same names as the class's builtin methods will be
         # renamed with the class name prefixed as mangled class variables
         # implicitly and internally. Such mapping information will be stored
         # within: attr: `__map__` attribute.
@@ -271,15 +272,15 @@
             del self.__dict__[key]
             self.__updated__ = True
             return
         return super().__delattr__(name)
 
     @classmethod
     def from_dict(cls, dict_: 'Optional[Mapping[str, VT] | Iterable[tuple[str, VT]]]' = None,
-                  **kwargs: 'VT') -> 'Schema[VT]':
+                  **kwargs: 'VT') -> 'Self':
         r"""Create a new instance.
 
         * If ``dict_`` is present and has a ``.keys()`` method, then does:
           ``for k in dict_: self[k] = dict_[k]``.
         * If ``dict_`` is present and has no ``.keys()`` method, then does:
           ``for k, v in dict_: self[k] = v``.
         * If ``dict_`` is not present, then does:
@@ -347,18 +348,32 @@
 
         Args:
             packet: Packet data.
 
         Returns:
             Packed :class:`Schema` as :obj:`bytes`.
 
+        Notes:
+            Since we do not know the length of the packet, we use a
+            reasonable default value ``-1`` for the ``__length__``
+            field, as the :class:`~pcapkit.corekit.fields.field.Field`
+            class will consider negative value as a placeholder.
+
+            If you want to pack the packet with the correct length,
+            please provide the ``__length__`` value before packing.
+
         """
         if packet is None:
             packet = {}
+
         packet.update(self.__dict__)
+        self.pre_unpack(packet)
+
+        if '__length__' not in packet:
+            packet['__length__'] = -1  # reasonable default value
 
         for field in self.__fields__.values():
             field = field(packet)
 
             if isinstance(field, PayloadField):
                 from pcapkit.protocols.protocol import \
                     Protocol  # pylint: disable=import-outside-toplevel
@@ -392,45 +407,63 @@
                 self.__buffer__[field.name] = bytes(field.length)
                 continue
 
             if isinstance(field, ConditionalField):
                 if not field.test(packet):
                     self.__buffer__[field.name] = b''
                     continue
-                field = field.field
+                field = field.field(packet)
 
             if isinstance(field, ForwardMatchField):
                 self.__buffer__[field.name] = b''
                 continue
 
             value = getattr(self, field.name)
             try:
-                temp = field.pack(value, self.__dict__)
+                temp = field.pack(value, packet)
             except NoDefaultValue:
                 temp = bytes(field.length)
             self.__buffer__[field.name] = temp
 
+        self.post_process(packet)
         self.__updated__ = False
         return self.__bytes__()
 
+    def pre_pack(self, packet: 'dict[str, Any]') -> 'None':
+        """Prepare ``packet`` data for packing process.
+
+        Args:
+            packet: packet data
+
+        Note:
+            This method is expected to directly modify any data stored
+            in the ``packet`` and thus no return is required.
+
+        """
+
     @classmethod
     @prepare
     def unpack(cls, data: 'bytes | IO[bytes]',
                length: 'Optional[int]' = None,
-               packet: 'Optional[dict[str, Any]]' = None) -> 'Schema':
+               packet: 'Optional[dict[str, Any]]' = None) -> 'Self':
         """Unpack :obj:`bytes` into :class:`Schema`.
 
         Args:
             data: Packed data.
             length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Unpacked data as :class:`Schema`.
 
+        Notes:
+            We used a ``__length__`` key in ``packet`` to record the length
+            of the remaining data, which is used to determine the length of
+            the payload field.
+
         """
         # force cast arg type since decorator changed their signatures
         if TYPE_CHECKING:
             data = cast('IO[bytes]', data)
             length = cast('int', length)
             packet = cast('dict[str, Any]', packet)
 
@@ -462,54 +495,56 @@
 
             if isinstance(field, ConditionalField):
                 if not field.test(packet):
                     self.__buffer__[field.name] = b''
                     setattr(self, field.name, None)
                     packet[field.name] = NoValue
                     continue
-                field = field.field
+                field = field.field(packet)
 
             byte = data.read(field.length)
             self.__buffer__[field.name] = byte
 
             value = field.unpack(byte, packet.copy())
             setattr(self, field.name, value)
 
             packet[field.name] = value
 
+            if isinstance(field, OptionField):
+                packet['__option_padding__'] = field.option_padding
+
             if isinstance(field, ForwardMatchField):
                 data.seek(-field.length, io.SEEK_CUR)
             else:
                 packet['__length__'] -= field.length
 
+            if packet['__length__'] < 0:
+                warn(f'packet length < 0: {packet["__length__"]}',
+                     SchemaWarning, stacklevel=stacklevel())
+
         self.__updated__ = False
         return self
 
     @classmethod
-    def pre_process(cls, packet: 'dict[str, Any]') -> 'None':
+    def pre_unpack(cls, packet: 'dict[str, Any]') -> 'None':
         """Prepare ``packet`` data for unpacking process.
 
         Args:
             packet: packet data
 
         Note:
             This method is expected to directly modify any data stored
             in the ``packet`` and thus no return is required.
 
         """
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
-        """Revise ``schema`` data after unpacking process.
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
+        """Revise ``schema`` data after packing and/or unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        return schema
+        return self
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import collections
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.tcp.checksum import Checksum as Enum_Checksum
 from pcapkit.const.tcp.mp_tcp_option import MPTCPOption as Enum_MPTCPOption
 from pcapkit.const.tcp.option import Option as Enum_Option
 from pcapkit.corekit.fields.collections import ListField, OptionField
-from pcapkit.corekit.fields.ipaddress import IPv4Field, IPv6Field
+from pcapkit.corekit.fields.ipaddress import IPv4AddressField, IPv6AddressField
 from pcapkit.corekit.fields.misc import (ConditionalField, ForwardMatchField, PayloadField,
                                          SchemaField, SwitchField)
 from pcapkit.corekit.fields.numbers import (EnumField, NumberField, UInt8Field, UInt16Field,
                                             UInt32Field, UInt64Field)
 from pcapkit.corekit.fields.strings import BitField, BytesField, PaddingField
 from pcapkit.protocols.schema.schema import Schema
 from pcapkit.utilities.exceptions import FieldError
@@ -35,15 +35,15 @@
 
     'MPTCPJoin',
     'MPTCPJoinSYN', 'MPTCPJoinSYNACK', 'MPTCPJoinACK',
 ]
 
 if TYPE_CHECKING:
     from ipaddress import IPv4Address, IPv6Address
-    from typing import IO, Any, Optional
+    from typing import Any, Optional
 
     from typing_extensions import Literal
 
     from pcapkit.corekit.fields.field import _Field as Field
     from pcapkit.protocols.protocol import Protocol
 
 if SPHINX_TYPE_CHECKING:
@@ -197,53 +197,36 @@
         instance.
 
     """
     subtype = Enum_MPTCPOption.get(pkt['test']['subtype'])
     pkt['test']['subtype'] = subtype
 
     if subtype == Enum_MPTCPOption.MP_CAPABLE:
-        return SchemaField(schema=MPTCPCapable)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPCapable)
     if subtype == Enum_MPTCPOption.MP_JOIN:
         if pkt['flags']['syn'] == 1 and pkt['flags']['ack'] == 0:
-            return SchemaField(schema=MPTCPJoinSYN)
+            return SchemaField(length=pkt['test']['length'], schema=MPTCPJoinSYN)
         if pkt['flags']['syn'] == 1 and pkt['flags']['ack'] == 1:
-            return SchemaField(schema=MPTCPJoinSYNACK)
+            return SchemaField(length=pkt['test']['length'], schema=MPTCPJoinSYNACK)
         if pkt['flags']['syn'] == 0 and pkt['flags']['ack'] == 1:
-            return SchemaField(schema=MPTCPJoinACK)
+            return SchemaField(length=pkt['test']['length'], schema=MPTCPJoinACK)
         raise FieldError(f'TCP: [OptNo {Enum_Option.Multipath_TCP}] {Enum_MPTCPOption.MP_JOIN} invalid flags')
     if subtype == Enum_MPTCPOption.DSS:
-        return SchemaField(schema=MPTCPDSS)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPDSS)
     if subtype == Enum_MPTCPOption.ADD_ADDR:
-        return SchemaField(schema=MPTCPAddAddress)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPAddAddress)
     if subtype == Enum_MPTCPOption.REMOVE_ADDR:
-        return SchemaField(schema=MPTCPRemoveAddress)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPRemoveAddress)
     if subtype == Enum_MPTCPOption.MP_PRIO:
-        return SchemaField(schema=MPTCPPriority)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPPriority)
     if subtype == Enum_MPTCPOption.MP_FAIL:
-        return SchemaField(schema=MPTCPFallback)
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPFallback)
     if subtype == Enum_MPTCPOption.MP_FASTCLOSE:
-        return SchemaField(schema=MPTCPFastclose)
-    return SchemaField(schema=MPTCPUnknown)
-
-
-def mptcp_add_address_length(pkt: 'dict[str, Any]') -> 'Literal[4, 16]':
-    """Length callback function for :attr:`MPTCPAddAddress.address` field.
-
-    Args:
-        pkt: Packet data.
-
-    Returns:
-        Length of :attr:`MPTCPAddAddress.address` field.
-
-    """
-    if pkt['test']['version'] == 4:
-        return 4
-    if pkt['test']['version'] == 6:
-        return 16
-    raise FieldError(f'TCP: [OptNo {Enum_Option.Multipath_TCP}] {Enum_MPTCPOption.ADD_ADDR} invalid IP version')
+        return SchemaField(length=pkt['test']['length'], schema=MPTCPFastclose)
+    return SchemaField(length=pkt['test']['length'], schema=MPTCPUnknown)
 
 
 def mptcp_add_address_selector(pkt: 'dict[str, Any]') -> 'Field':
     """Selector function for :attr:`MPTCPAddAddress.address` field.
 
     Args:
         pkt: Packet data.
@@ -252,53 +235,45 @@
         * If IP version is 4, a :class:`~pcapkit.corekit.fields.ipaddress.IPv4Field`
           instance.
         * If IP version is 6, a :class:`~pcapkit.corekit.fields.ipaddress.IPv6Field`
           instance.
 
     """
     if pkt['test']['version'] == 4:
-        return IPv4Field()
+        return IPv4AddressField()
     if pkt['test']['version'] == 6:
-        return IPv6Field()
+        return IPv6AddressField()
     raise FieldError(f'TCP: [OptNo {Enum_Option.Multipath_TCP}] {Enum_MPTCPOption.ADD_ADDR} invalid IP version')
 
 
 class Option(Schema):
     """Header schema for TCP options."""
 
     #: Option kind.
     kind: 'Enum_Option' = EnumField(length=1, namespace=Enum_Option)
     #: Option length.
     length: 'int' = ConditionalField(
         UInt8Field(),
         lambda pkt: pkt['kind'] not in (Enum_Option.End_of_Option_List, Enum_Option.No_Operation),
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'Schema':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('Option', schema)
-
         # for EOOL/NOP option, length is always 1
-        if schema.kind in (Enum_Option.End_of_Option_List, Enum_Option.No_Operation):
-            schema.length = 1
-        return schema
+        if self.kind in (Enum_Option.End_of_Option_List, Enum_Option.No_Operation):
+            self.length = 1
+        return self
 
 
 class UnassignedOption(Option):
     """Header schema for TCP unassigned options."""
 
     #: Option data.
     data: 'bytes' = BytesField(length=lambda pkt: pkt['length'] - 2)
@@ -536,37 +511,28 @@
     #: Subtype and flags.
     test: 'MPTCPSubtypeTest' = ForwardMatchField(BitField(length=3, namespace={
         'length': (1, 8),
         'subtype': (16, 4),
     }))
     #: Subtype-specific data.
     data: 'MPTCP' = SwitchField(
-        length=lambda pkt: pkt['test']['length'],
         selector=mptcp_data_selector,
     )
 
-    @classmethod
-    def post_process(cls, schema: 'Schema', data: 'IO[bytes]',
-                     length: 'int', packet: 'dict[str, Any]') -> 'Schema':
+    def post_process(self, packet: 'dict[str, Any]') -> 'MPTCP':
         """Revise ``schema`` data after unpacking process.
 
         Args:
-            schema: parsed schema
-            data: Packed data.
-            length: Length of data.
             packet: Unpacked data.
 
         Returns:
             Revised schema.
 
         """
-        if TYPE_CHECKING:
-            schema = cast('_MPTCP', schema)
-
-        ret = schema.data
+        ret = self.data
         ret.subtype = Enum_MPTCPOption.get(packet['test']['subtype'])
         return ret
 
 
 class MPTCP(Option):
     """Header schema for Multipath TCP options."""
 
@@ -727,15 +693,14 @@
         'subtype': (0, 4),
         'version': (4, 4),
     })
     #: Address ID.
     addr_id: 'int' = UInt8Field()
     #: Address.
     address: 'IPv4Address | IPv6Address' = SwitchField(
-        length=mptcp_add_address_length,
         selector=mptcp_add_address_selector,
     )
     #: Port.
     port: 'int' = ConditionalField(
         UInt16Field(),
         lambda pkt: pkt['length'] in (10, 22),
     )
@@ -881,15 +846,15 @@
             Enum_Option.User_Timeout_Option: UserTimeout,
             Enum_Option.TCP_Authentication_Option: Authentication,
             Enum_Option.Multipath_TCP: _MPTCP,
             Enum_Option.TCP_Fast_Open_Cookie: FastOpenCookie,
         }),
     )
     #: Padding.
-    padding: 'bytes' = PaddingField(length=lambda pkt: pkt.get('__option_padding__', 0))
+    padding: 'bytes' = PaddingField(length=lambda pkt: pkt.get('__option_padding__', 0))  # key generated by OptionField
     #: Payload.
     payload: 'bytes' = PayloadField()
 
     if TYPE_CHECKING:
         def __init__(self, srcport: 'int', dstport: 'int', seq: 'int', ack: 'int',
                      offset: 'OffsetFlag', flags: 'Flags', window: 'int', checksum: 'bytes',
                      urgent: 'int', options: 'list[Option | bytes] | bytes', payload: 'bytes | Protocol | Schema') -> 'None': ...
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/schema/transport/udp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/schema/transport/udp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/transport/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/transport/tcp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/tcp.py`

 * *Files identical despite different names*

```diff
@@ -1928,15 +1928,15 @@
         )
         return data
 
     def _make_tcp_options(self, options: 'list[Schema_Option | tuple[Enum_Option, dict[str, Any]] | bytes] | Option') -> 'tuple[list[Schema_Option | bytes], int]':
         """Make options for TCP.
 
         Args:
-            option: TCP options
+            options: TCP options
 
         Returns:
             Tuple of options and total length of options.
 
         """
         total_length = 0
         if isinstance(options, list):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/transport/transport.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
         protocol = cast('Type[Protocol]', getattr(importlib.import_module(module), name))
 
         payload_io = io.BytesIO(payload)
         try:
             report = protocol(payload_io, len(payload), **kwargs)  # type: ignore[abstract]
         except Exception as exc:
             if isinstance(exc, StructError) and exc.eof:  # pylint: disable=no-member
-                from pcapkit.protocols.misc.null import NoPayload as protocol  # type: ignore[no-redef] # pylint: disable=import-outside-toplevel # isort:skip
+                from pcapkit.protocols.misc.null import NoPayload as protocol  # pylint: disable=import-outside-toplevel # isort:skip
             else:
-                from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[no-redef] # pylint: disable=import-outside-toplevel # isort:skip
+                from pcapkit.protocols.misc.raw import Raw as protocol  # pylint: disable=import-outside-toplevel # isort:skip
             # error = traceback.format_exc(limit=1).strip().rsplit(os.linesep, maxsplit=1)[-1]
 
             # log error
             logger.error(str(exc), exc_info=exc, stack_info=DEVMODE, stacklevel=stacklevel())
 
             report = protocol(payload_io, len(payload), **kwargs)  # type: ignore[abstract]
         return report
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/protocols/transport/udp.py` & `pypcapkit-1.0.0rc1/pcapkit/protocols/transport/udp.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/toolkit/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/toolkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 .. module:: pcapkit.toolkit
 
 :mod:`pcapkit.toolkit` provides several utility functions for
 compatibility of multiple engine support.
 
 """
 # tools for default engine
-from pcapkit.toolkit.default import ipv4_reassembly, ipv6_reassembly, tcp_reassembly, tcp_traceflow
+from pcapkit.toolkit.pcap import ipv4_reassembly, ipv6_reassembly, tcp_reassembly, tcp_traceflow
+from pcapkit.toolkit.pcapng import ipv4_reassembly as pcapng_ipv4_reassembly
+from pcapkit.toolkit.pcapng import ipv6_reassembly as pcapng_ipv6_reassembly
+from pcapkit.toolkit.pcapng import tcp_reassembly as pcapng_tcp_reassembly
+from pcapkit.toolkit.pcapng import tcp_traceflow as pcapng_tcp_traceflow
+from pcapkit.toolkit.pcapng import block2frame as pcapng_block2frame
 
 # # tools for DPKT engine
 # from pcapkit.toolkit.dpkt import ipv6_hdr_len as dpkt_ipv6_hdr_len
 # from pcapkit.toolkit.dpkt import packet2chain as dpkt_packet2chain
 # from pcapkit.toolkit.dpkt import packet2dict as dpkt_packet2dict
 # from pcapkit.toolkit.dpkt import ipv4_reassembly as dpkt_ipv4_reassembly
 # from pcapkit.toolkit.dpkt import ipv6_reassembly as dpkt_ipv6_reassembly
@@ -32,14 +37,16 @@
 # from pcapkit.toolkit.scapy import ipv6_reassembly as scapy_ipv6_reassembly
 # from pcapkit.toolkit.scapy import tcp_reassembly as scapy_tcp_reassembly
 # from pcapkit.toolkit.scapy import tcp_traceflow as scapy_tcp_traceflow
 
 __all__ = [
     # default engine
     'ipv4_reassembly', 'ipv6_reassembly', 'tcp_reassembly', 'tcp_traceflow',
+    'pcapng_ipv4_reassembly', 'pcapng_ipv6_reassembly', 'pcapng_tcp_reassembly', 'pcapng_tcp_traceflow',
+    'pcapng_block2frame',
 
     # # DPKT engine
     # 'dpkt_ipv6_hdr_len', 'dpkt_packet2chain', 'dpkt_packet2dict',
     # 'dpkt_ipv4_reassembly', 'dpkt_ipv6_reassembly', 'dpkt_tcp_reassembly', 'dpkt_tcp_traceflow',
 
     # # PyShark engine
     # 'pyshark_packet2dict', 'pyshark_tcp_traceflow',
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/toolkit/default.py` & `pypcapkit-1.0.0rc1/pcapkit/toolkit/pcap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
-"""PyPCAPKit Tools
-=====================
+"""PCAP Tools
+================
 
-.. module:: pcapkit.toolkit.default
+.. module:: pcapkit.toolkit.pcap
 
-:mod:`pcapkit.toolkit.default` contains all you need for
-:mod:`pcapkit` handy usage. All functions returns with a
-flag to indicate if usable for its caller.
+:mod:`pcapkit.toolkit.pcap` contains all you need for
+:mod:`pcapkit` handy usage of PCAP file format. All
+functions returns with a flag to indicate if usable
+for its caller.
 
 """
 from typing import TYPE_CHECKING, cast
 
 from pcapkit.const.ipv6.extension_header import ExtensionHeader as Enum_ExtensionHeader
 from pcapkit.foundation.reassembly.data.ip import Packet as IP_Packet
 from pcapkit.foundation.reassembly.data.tcp import Packet as TCP_Packet
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/toolkit/dpkt.py` & `pypcapkit-1.0.0rc1/pcapkit/toolkit/dpkt.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/toolkit/pyshark.py` & `pypcapkit-1.0.0rc1/pcapkit/toolkit/pyshark.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/toolkit/scapy.py` & `pypcapkit-1.0.0rc1/pcapkit/toolkit/scapy.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/utilities/compat.py` & `pypcapkit-1.0.0rc1/pcapkit/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/utilities/decorators.py` & `pypcapkit-1.0.0rc1/pcapkit/utilities/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,43 +96,43 @@
 
     :param func: decorated function
     :meta decorator:
     """
     @functools.wraps(func)
     def behold(*args: 'P.args', **kwargs: 'P.kwargs') -> 'R_beholder':
         # extract self object & args
-        self = cast('Protocol', args[0])
+        self = cast('R_beholder', args[0])
         try:
             length = cast('int', args[2])
         except IndexError:
             length = None
 
         # record file pointer
         try:
             # call method
             return func(*args, **kwargs)
         except Exception as exc:
             if isinstance(exc, StructError) and exc.eof:  # pylint: disable=no-member
                 from pcapkit.protocols.misc.null import NoPayload as protocol  # isort: skip # pylint: disable=import-outside-toplevel
             else:
-                from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[no-redef] # isort: skip # pylint: disable=import-outside-toplevel
+                from pcapkit.protocols.misc.raw import Raw as protocol  # type: ignore[assignment] # isort: skip # pylint: disable=import-outside-toplevel
             # error = traceback.format_exc(limit=1).strip().rsplit(os.linesep, maxsplit=1)[-1]
 
             # log error
             # logger.error(str(exc), exc_info=exc, stack_info=DEVMODE, stacklevel=stacklevel())
             # if DEVMODE:
             #    traceback.print_exc()
 
             file_ = self.__header__.get_payload()
             next_ = protocol(file_, length, error=str(exc))
             return cast('R_beholder', next_)
     return behold
 
 
-def prepare(func: 'Callable[Concatenate[Type[Schema], bytes | IO[bytes], Optional[int], Optional[dict[str, Any]], P], R_prepare]') -> 'Callable[P, R_prepare]':
+def prepare(func: 'Callable[Concatenate[Type[R_prepare], bytes | IO[bytes], Optional[int], Optional[dict[str, Any]], P], R_prepare]') -> 'Callable[P, R_prepare]':
     """Prepare schema packet data before unpacking.
 
     Important:
         This decorate function is designed for decorating the
         :meth:`Schema.unpack <pcapkit.protocols.schema.schema.Schema.unpack>`
         *class method*.
 
@@ -150,15 +150,15 @@
         :meth:`pcapkit.protocols.schema.schema.Schema.unpack`
 
     :param func: decorated function
     :meta decorator:
     """
     @functools.wraps(func)
     def unpack(*args: 'P.args', **kwargs: 'P.kwargs') -> 'R_prepare':
-        cls = cast('Type[Schema]', args[0])
+        cls = cast('Type[R_prepare]', args[0])
         data = cast('bytes | IO[bytes]', args[1])
         length = cast('Optional[int]', args[2])
         packet = cast('Optional[dict[str, Any]]', args[3])
 
         if isinstance(data, bytes):
             length = len(data) if length is None else length
             data = io.BytesIO(data)
@@ -174,13 +174,13 @@
         if packet is None:
             packet = {}
         packet['__length__'] = length
 
         # call the user customised preparation method
         # then proceed with the unpacking process
         # and eventually revise the schema data
-        cls.pre_process(packet)
+        cls.pre_unpack(packet)
         schema = func(cls, data, length, packet)
-        ret = cls.post_process(schema, data, length, packet)
+        ret = schema.post_process(packet)
 
         return cast('R_prepare', ret)
     return unpack
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/utilities/exceptions.py` & `pypcapkit-1.0.0rc1/pcapkit/utilities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     'FormatError', 'UnsupportedCall',                               # AttributeError
     'FileError',                                                    # IOError
     'FileExists',                                                   # FileExistsError
     'FileNotFound',                                                 # FileNotFoundError
     'ProtocolNotFound',                                             # IndexError
     'VersionError', 'IndexNotFound', 'ProtocolError',               # ValueError
     'EndianError', 'KeyExists', 'NoDefaultValue',                   # ValueError
-    'FieldValueError',                                              # ValueError
+    'FieldValueError', 'SchemaError',                               # ValueError
     'ProtocolNotImplemented', 'VendorNotImplemented',               # NotImplementedError
     'StructError',                                                  # struct.error
     'MissingKeyError', 'FragmentError', 'PacketError',              # KeyError
     'ModuleNotFound',                                               # ModuleNotFoundError
 ]
 
 
@@ -284,14 +284,18 @@
     """No default value."""
 
 
 class FieldValueError(BaseError, ValueError):
     """Invalid field value."""
 
 
+class SchemaError(BaseError, ValueError):
+    """Invalid schema."""
+
+
 ##############################################################################
 # NotImplementedError session.
 ##############################################################################
 
 
 class ProtocolNotImplemented(BaseError, NotImplementedError):
     """Protocol not implemented."""
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/utilities/logging.py` & `pypcapkit-1.0.0rc1/pcapkit/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/utilities/warnings.py` & `pypcapkit-1.0.0rc1/pcapkit/utilities/warnings.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,20 @@
     # UserWarning
     'BaseWarning',
     # ImportWarning
     'FormatWarning', 'EngineWarning', 'InvalidVendorWarning',
     # RuntimeWarning
     'FileWarning', 'LayerWarning', 'ProtocolWarning', 'AttributeWarning',
     'DevModeWarning', 'VendorRequestWarning', 'VendorRuntimeWarning',
-    'UnknownFieldWarning', 'RegistryWarning',
+    'UnknownFieldWarning', 'RegistryWarning', 'SchemaWarning',
     # ResourceWarning
     'DPKTWarning', 'ScapyWarning', 'PySharkWarning', 'EmojiWarning',
     'VendorWarning',
+    # DeprecationWarning
+    'DeprecatedFormatWarning',
 ]
 
 
 def warn(message: 'Union[str, Warning]', category: 'Type[Warning]',
          stacklevel: 'Optional[int]' = None) -> 'None':
     """Wrapper function of :func:`warnings.warn`.
 
@@ -55,18 +57,21 @@
 
 class BaseWarning(UserWarning):
     """Base warning class of all kinds."""
 
     def __init__(self, *args: 'Any', **kwargs: 'Any') -> 'None':  # pylint: disable=useless-super-delegation
         # log warning
         if DEVMODE:
-            logger.warning(str(self), exc_info=self, stack_info=VERBOSE,
-                           stacklevel=stacklevel_calculator())
+            if VERBOSE:
+                logger.warning(str(self), exc_info=self, stack_info=True,
+                            stacklevel=stacklevel_calculator())
+            else:
+                logger.warning(str(self))
         else:
-            logger.warning(str(self))
+            warnings.simplefilter('ignore', type(self))
 
         # warnings.simplefilter('default')
         super().__init__(*args, **kwargs)
 
 
 ##############################################################################
 # ImportWarning session.
@@ -122,14 +127,18 @@
     """Unknown field."""
 
 
 class RegistryWarning(BaseWarning, RuntimeWarning):
     """Registry warning."""
 
 
+class SchemaWarning(BaseWarning, RuntimeWarning):
+    """Schema warning."""
+
+
 ##############################################################################
 # ResourceWarning session.
 ##############################################################################
 
 
 class DPKTWarning(BaseWarning, ResourceWarning):
     """Warnings on DPKT usage."""
@@ -145,7 +154,16 @@
 
 class EmojiWarning(BaseWarning, ResourceWarning):
     """Warnings on Emoji usage."""
 
 
 class VendorWarning(BaseWarning, ResourceWarning):
     """Warnings on vendor usage."""
+
+
+##############################################################################
+# DeprecationWarning session.
+##############################################################################
+
+
+class DeprecatedFormatWarning(BaseWarning, DeprecationWarning):
+    """Warning on deprecated formats."""
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,9 +94,11 @@
     # OSPF
     'OSPF_Authentication', 'OSPF_Packet',
     # TCP
     'TCP_Checksum', 'TCP_Option', 'TCP_MPTCPOption',
     # VLAN
     'VLAN_PriorityLevel',
     # PCAPNG
-    'PCAPNG_BlockType',
+    'PCAPNG_BlockType', 'PCAPNG_OptionType', 'PCAPNG_HashAlgorithm',
+    'PCAPNG_VerdictType', 'PCAPNG_RecordType', 'PCAPNG_SecretsType',
+    'PCAPNG_FilterType',
 ]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/__main__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 
 import argparse
 import importlib
 import sys
 import warnings
 from typing import TYPE_CHECKING
 
+from pcapkit import __version__
 from pcapkit import vendor as vendor_module
 from pcapkit.utilities.warnings import InvalidVendorWarning, VendorRuntimeWarning, warn
 
 if TYPE_CHECKING:
     from argparse import ArgumentParser
     from typing import Type
 
     from pcapkit.vendor.default import Vendor
 
-#: version string
-__version__ = '1.0.0b1'
-
 
 def get_parser() -> 'ArgumentParser':
     """CLI argument parser."""
     parser = argparse.ArgumentParser(prog='pcapkit-vendor',
                                      description='update constant enumerations')
     parser.add_argument('-V', '--version', action='version', version=__version__)
     parser.add_argument('target', action='store', nargs=argparse.REMAINDER,
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/arp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/arp/hardware.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/hardware.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/arp/operation.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/arp/operation.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/default.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,29 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return {NAME}(key)
         if key not in {NAME}._member_map_:  # pylint: disable=no-member
-            extend_enum({NAME}, key, default)
+            return extend_enum({NAME}, key, default)
         return {NAME}[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> '{NAME}':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not ({FLAG}):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         {MISS}
-        {'' if '        return cls(value)' in MISS.splitlines()[-1:] else 'return super()._missing_(value)'}
+        {'' if ''.join(MISS.splitlines()[-1:]).startswith('return') else 'return super()._missing_(value)'}
 '''.strip()  # type: Callable[[str, str, str, str, str, str], str]
 
 
 def get_proxies() -> 'dict[str, str]':
     """Get proxy for blocked sites.
 
     The function will read :envvar:`PCAPKIT_HTTP_PROXY`
@@ -254,16 +254,15 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
     def count(self, data: 'list[str]') -> 'Counter[str]':
         """Count field records.
 
         Args:
             data: CSV data.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ftp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ftp/command.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,29 +59,36 @@
 
 __all__ = ['{NAME}']
 
 
 class {NAME}(StrEnum):
     """[{NAME}] {DOCS}"""
 
+    if TYPE_CHECKING:
+        #: Feature of command.
+        feat: 'Optional[str]'
+        #: Description of command.
+        desc: 'Optional[str]'
+        #: Type of command.
+        type: 'Optional[tuple[str, ...]]'
+        #: Conformance of command.
+        conf: 'Optional[str]'
+        #: Note of command.
+        note: 'Optional[tuple[str, ...]]'
+
     def __new__(cls, name: 'str', feat: 'Optional[str]' = None, desc: 'Optional[str]' = None,
                 type: 'Optional[tuple[str, ...]]' = None, conf: 'Optional[str]' = None,
                 note: 'Optional[tuple[str, ...]]' = None) -> 'Type[{NAME}]':
         obj = str.__new__(cls, name)
         obj._value_ = name
 
-        #: Feature of command.
         obj.feat = feat
-        #: Description of command.
         obj.desc = desc
-        #: Type of command.
         obj.type = type
-        #: Conformance of command.
         obj.conf = conf
-        #: Note of command.
         obj.note = note
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s.%s>" % (self.__class__.__name__, self._name_)
 
@@ -94,27 +101,26 @@
         Args:
             key: Key to get enum item.
             default: Default value if not found.
 
         :meta private:
         """
         if key not in {NAME}._member_map_:  # pylint: disable=no-member
-            extend_enum({NAME}, key.upper(), default if default is not None else key)
+            return extend_enum({NAME}, key.upper(), default if default is not None else key)
         return {NAME}[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'str') -> '{NAME}':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
-        extend_enum(cls, value.upper(), value)
-        return cls(value)
+        return extend_enum(cls, value.upper(), value)
 '''.strip()  # type: Callable[[str, str, str, str], str]
 
 
 class Command(Vendor):
     """FTP Command"""
 
     #: Link to registry.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ftp/return_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ftp/return_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,24 +67,29 @@
     '5': 'File system',
 }}  # type: dict[str, str]
 
 
 class {NAME}(IntEnum):
     """[{NAME}] {DOCS}"""
 
+    if TYPE_CHECKING:
+        #: Description of the return code.
+        description: 'Optional[str]'
+        #: Response kind.
+        kind: 'str'
+        #: Grouping information.
+        group: 'str'
+
     def __new__(cls, value: 'int', description: 'Optional[str]' = None) -> 'Type[{NAME}]':
         obj = int.__new__(cls, value)
         obj._value_ = value
 
         code = str(value)
-        #: Description of the return code.
         obj.description = description
-        #: Response kind.
         obj.kind = KIND.get(str(value)[0], 'Reserved')
-        #: Grouping information.
         obj.group = INFO.get(str(value)[1], 'Reserved')
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s [%s]>" % (self.__class__.__name__, self._value_)
 
@@ -99,29 +104,28 @@
             default: Default value if not found.
 
         :meta private:
         """
         if isinstance(key, int):
             return {NAME}(key)
         if key not in {NAME}._member_map_:  # pylint: disable=no-member
-            extend_enum({NAME}, key, default)
+            return extend_enum({NAME}, key, default)
         return {NAME}[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'int') -> '{NAME}':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
         if not ({FLAG}):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
-        extend_enum(cls, 'CODE_%s' % value, value)
-        return cls(value)
+        return extend_enum(cls, 'CODE_%s' % value, value)
 '''  # type: Callable[[str, str, str, str, str], str]
 
 
 class ReturnCode(Vendor):
     """FTP Server Return Code"""
 
     #: Value limit checker.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/certificate.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/certificate.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/cipher.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/cipher.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/di.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/di.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/ecdsa_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/ecdsa_low_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/ecdsa_low_curve.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/eddsa_curve.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/eddsa_curve.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[2].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(EdDSACurve())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/esp_transform_suite.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/esp_transform_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/group.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    # {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Group())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/hi_algorithm.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hi_algorithm.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/hit_suite.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/hit_suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/nat_traversal.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/nat_traversal.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/notify_message.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/notify_message.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    # {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Packet())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/parameter.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f"    #: {desc}")
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Parameter())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/registration.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/registration_failure.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/registration_failure.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/suite.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/suite.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/hip/transport.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/hip/transport.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/error_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/error_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = map(lambda s: int(s, base=16), item[0].split('-'))
 
                 miss.append(f'if {hexlify(start)} <= value <= {hexlify(stop)}:')
                 miss.append(f'    #: {desc}')
-                miss.append('    temp = hex(value)[2:].upper().zfill(8)')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_0x%s' % (temp[:4]+'_'+temp[4:]), value)")
-                miss.append('    return cls(value)')
+                miss.append(f'    temp = hex(value)[2:].upper().zfill(8)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_0x%s' % (temp[:4]+'_'+temp[4:]), value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(ErrorCode())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/frame.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = map(lambda s: int(s, base=16), item[0].split('-'))
 
                 miss.append(f'if {hexlify(start)} <= value <= {hexlify(stop)}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{name}_0x%s' % hex(value)[2:].upper().zfill(2), value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{name}_0x%s' % hex(value)[2:].upper().zfill(2), value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Frame())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/method.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/method.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,26 @@
     from typing import Optional, Type
 
 __all__ = ['{NAME}']
 
 class {NAME}(StrEnum):
     """[{NAME}] {DOCS}"""
 
+    if TYPE_CHECKING:
+        #: Safe method.
+        safe: 'bool'
+        #: Idempotent method.
+        idempotent: 'bool'
+
     def __new__(cls, value: 'str', safe: 'bool' = False,
                 idempotent: 'bool' = False) -> 'Type[{NAME}]':
         obj = str.__new__(cls)
         obj._value_ = value
 
-        #: Safe method.
         obj.safe = safe
-        #: Idempotent method.
         obj.idempotent = idempotent
 
         return obj
 
     def __repr__(self) -> 'str':
         return "<%s.%s>" % (self.__class__.__name__, self._value_)
 
@@ -70,27 +74,26 @@
         Args:
             key: Key to get enum item.
             default: Default value if not found.
 
         :meta private:
         """
         if key not in {NAME}._member_map_:  # pylint: disable=no-member
-            extend_enum({NAME}, key.upper(), default if default is not None else key)
+            return extend_enum({NAME}, key.upper(), default if default is not None else key)
         return {NAME}[key]  # type: ignore[misc]
 
     @classmethod
     def _missing_(cls, value: 'str') -> '{NAME}':
         """Lookup function used when value is not found.
 
         Args:
             value: Value to get enum item.
 
         """
-        extend_enum(cls, value.upper(), value)
-        return cls(value)
+        return extend_enum(cls, value.upper(), value)
 '''.strip()  # type: Callable[[str, str, str, str], str]
 
 
 class Method(Vendor):
     """HTTP Method"""
 
     #: Link to registry.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/setting.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/setting.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = map(lambda s: int(s, base=16), item[0].split('-'))
 
                 miss.append(f'if {hexlify(start)} <= value <= {hexlify(stop)}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_0x%s' % hex(value)[2:].upper().zfill(4), value)")  # pylint: disable=line-too-long
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_0x%s' % hex(value)[2:].upper().zfill(4), value)")  # pylint: disable=line-too-long
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Setting())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/http/status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/http/status_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,22 @@
 
 __all__ = ['{NAME}']
 
 
 class {NAME}(IntEnum):
     """[{NAME}] {DOCS}"""
 
+    if TYPE_CHECKING:
+        #: Status message.
+        message: 'str'
+
     def __new__(cls, value: 'int', message: 'str' = '') -> 'Type[{NAME}]':
         obj = int.__new__(cls, value)
         obj._value_ = value
 
-        #: Status message.
         obj.message = message
 
         return obj
 
     {ENUM}
 
     @staticmethod
@@ -82,15 +85,15 @@
         Args:
             value: Value to get enum item.
 
         """
         if not ({FLAG}):
             raise ValueError('%r is not a valid %s' % (value, cls.__name__))
         {MISS}
-        {'' if '        return cls(value)' in MISS.splitlines()[-1:] else 'return super()._missing_(value)'}
+        {'' if 'return' in ''.join(MISS.splitlines()[-1:]) else 'return super()._missing_(value)'}
 '''.strip()  # type: Callable[[str, str, str, str, str, str], str]
 
 
 class StatusCode(Vendor):
     """HTTP Status Code"""
 
     #: Value limit checker.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/classification_level.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/classification_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,15 @@
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
             'temp = bin(value)[2:].upper().zfill(8)',
-            "extend_enum(cls, 'Unassigned_0b%s' % (temp[:4]+'_'+temp[4:]), value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_0b%s' % (temp[:4]+'_'+temp[4:]), value)",
         ]
         for code, name in data.items():
             bncd = binary(code)
             renm = self.rename(name, bncd)
             enum.append(f"{renm} = {bncd}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/option_class.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in data.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/option_number.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/option_number.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             code = item[3]
             dscp = item[4]
             rfcs = item[5]
 
             temp = []  # type: list[str]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/protection_authority.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/protection_authority.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in data.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/qs_function.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/qs_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/router_alert.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/router_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
-"""IPv4 Router Alert Option Values
+"""IPv6 Router Alert Option Values
 =====================================
 
-.. module:: pcapkit.vendor.ipv4.router_alert
+.. module:: pcapkit.vendor.ipv6.router_alert
 
-This module contains the vendor crawler for **IPv4 Router Alert Option Values**,
-which is automatically generating :class:`pcapkit.const.ipv4.router_alert.RouterAlert`.
+This module contains the vendor crawler for **IPv6 Router Alert Option Values**,
+which is automatically generating :class:`pcapkit.const.ipv6.router_alert.RouterAlert`.
 
 """
 
 import csv
 import re
 import sys
 
 from pcapkit.vendor.default import Vendor
 
 __all__ = ['RouterAlert']
 
 
 class RouterAlert(Vendor):
-    """IPv4 Router Alert Option Values"""
+    """IPv6 Router Alert Option Values"""
 
     #: Value limit checker.
     FLAG = 'isinstance(value, int) and 0 <= value <= 65535'
     #: Link to registry.
-    LINK = 'https://www.iana.org/assignments/ip-parameters/ipv4-router-alert-option-values.csv'
+    LINK = 'https://www.iana.org/assignments/ipv6-routeralert-values/ipv6-routeralert-values-1.csv'
 
     def process(self, data: 'list[str]') -> 'tuple[list[str], list[str]]':
         """Process CSV data.
 
         Args:
             data: CSV data.
 
@@ -81,14 +81,13 @@
                         #    sufs = f"\n{' '*80}{sufs}"
 
                         #enum.append(f'{pres.ljust(76)}{sufs}')
                         enum.append(f'#: {desc}\n    {pres}')
                 else:
                     miss.append(f'if {start} <= value <= {stop}:')
                     miss.append(f'    #: {desc}')
-                    miss.append(f"    extend_enum(cls, '{name}_%d' % value, value)")
-                    miss.append('    return cls(value)')
+                    miss.append(f"    return extend_enum(cls, '{name}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(RouterAlert())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_del.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_del.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code).upper()  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_ecn.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_ecn.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)
             enum.append(f"{renm} = 0b{bin(code)[2:].zfill(2)}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_pre.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_pre.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_rel.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code).upper()  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/tos_thr.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/tos_thr.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,16 +61,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code).upper()  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv4/ts_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/ts_flag.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/extension_header.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/extension_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,15 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
     def context(self, data: 'list[str]') -> 'str':
         """Generate constant context.
 
         Args:
             data: CSV data.
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/option.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_0x%s' % hex(value)[2:].upper().zfill(2), value)",
         ]
         for item in reader:
             if not item[0]:
                 continue
 
             code = item[0]
             dscp = item[4]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/option_action.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/option_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/qs_function.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/qs_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/router_alert.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv4/router_alert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
-"""IPv6 Router Alert Option Values
+"""IPv4 Router Alert Option Values
 =====================================
 
-.. module:: pcapkit.vendor.ipv6.router_alert
+.. module:: pcapkit.vendor.ipv4.router_alert
 
-This module contains the vendor crawler for **IPv6 Router Alert Option Values**,
-which is automatically generating :class:`pcapkit.const.ipv6.router_alert.RouterAlert`.
+This module contains the vendor crawler for **IPv4 Router Alert Option Values**,
+which is automatically generating :class:`pcapkit.const.ipv4.router_alert.RouterAlert`.
 
 """
 
 import csv
 import re
 import sys
 
 from pcapkit.vendor.default import Vendor
 
 __all__ = ['RouterAlert']
 
 
 class RouterAlert(Vendor):
-    """IPv6 Router Alert Option Values"""
+    """IPv4 Router Alert Option Values"""
 
     #: Value limit checker.
     FLAG = 'isinstance(value, int) and 0 <= value <= 65535'
     #: Link to registry.
-    LINK = 'https://www.iana.org/assignments/ipv6-routeralert-values/ipv6-routeralert-values-1.csv'
+    LINK = 'https://www.iana.org/assignments/ip-parameters/ipv4-router-alert-option-values.csv'
 
     def process(self, data: 'list[str]') -> 'tuple[list[str], list[str]]':
         """Process CSV data.
 
         Args:
             data: CSV data.
 
@@ -81,14 +81,13 @@
                         #    sufs = f"\n{' '*80}{sufs}"
 
                         #enum.append(f'{pres.ljust(76)}{sufs}')
                         enum.append(f'#: {desc}\n    {pres}')
                 else:
                     miss.append(f'if {start} <= value <= {stop}:')
                     miss.append(f'    #: {desc}')
-                    miss.append(f"    extend_enum(cls, '{name}_%d' % value, value)")
-                    miss.append('    return cls(value)')
+                    miss.append(f"    return extend_enum(cls, '{name}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(RouterAlert())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/routing.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{name}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{name}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Routing())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/seed_id.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/seed_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_0b%s' % bin(value)[2:].zfill(2), value)",
         ]
         for code, name in data.items():
             bncd = f'0b{bin(code)[2:].zfill(2)}'
             renm = self.rename(name, bncd).upper()
             enum.append(f"{renm} = {bncd}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/smf_dpd_mode.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/smf_dpd_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in DATA.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipv6/tagger_id.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipv6/tagger_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,13 @@
                 #enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{name}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{name}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(TaggerID())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipx/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipx/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/packet.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,16 +81,15 @@
         """
         table = soup.find_all('table', class_='wikitable')[1]
         content = filter(lambda item: isinstance(item, bs4.element.Tag), table.tbody)
         next(content)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in content:
             line = item.find_all('td')
 
             pval = ''.join(line[0].stripped_strings)
             desc = ''.join(line[1].stripped_strings)
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ipx/socket.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ipx/socket.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = pval.split('–')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{name}_0x%s' % hex(value)[2:].upper().zfill(4), value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{name}_0x%s' % hex(value)[2:].upper().zfill(4), value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Socket())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/l2tp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/l2tp/type.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/l2tp/type.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,16 +62,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = list()
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in data.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/access_type.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/access_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(AccessType())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/ack_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ack_status_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(ACKStatusCode())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/ani_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/ani_suboption.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(ANISuboption())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/auth_subtype.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/auth_subtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             long = item[1]
             rfcs = item[2]
 
             temp = []  # type: list[str]
             for rfc in filter(None, re.split(r'\[|\]', rfcs)):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_ack_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_revocation.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_revocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(BindingRevocation())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/binding_update_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/binding_update_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/dhcp_support_mode.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dhcp_support_mode.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             long = item[1]
             rfcs = item[2]
 
             temp = []  # type: list[str]
             for rfc in filter(None, re.split(r'\[|\]', rfcs)):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/dns_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dns_status_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(DNSStatusCode())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/dsmip6_tls_packet.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmip6_tls_packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(DSMIP6TLSPacket())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/dsmipv6_home_address.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/dsmipv6_home_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(DSMIPv6HomeAddress())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/enumerating_algorithm.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/enumerating_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             long = item[1]
             rfcs = item[2]
 
             temp = []  # type: list[str]
             for rfc in filter(None, re.split(r'\[|\]', rfcs)):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_ack_status.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_ack_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowBindingACKStatus())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_action.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_action.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowBindingAction())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_indication_trigger.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_indication_trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowBindingIndicationTrigger())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/fb_type.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/fb_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowBindingType())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/flow_id_status.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowIDStatus())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/flow_id_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/flow_id_suboption.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(FlowIDSuboption())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/handoff_type.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handoff_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(HandoffType())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_ack_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_ack_status.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_ack_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(HandoverACKStatus())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_initiate_flag.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_flag.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/handover_initiate_status.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/handover_initiate_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(HandoverInitiateStatus())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/home_address_reply.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/home_address_reply.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(HomeAddressReply())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/lma_mag_suboption.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/lma_mag_suboption.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(LMAControlledMAGSuboption())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/mn_group_id.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_group_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(MNGroupID())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/mn_id_subtype.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/mn_id_subtype.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(MNIDSubtype())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/operator_id.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/operator_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(OperatorID())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/option.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/option.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             long = item[1]
             rfcs = item[2]
 
             temp = []  # type: list[str]
             for rfc in filter(None, re.split(r'\[|\]', rfcs)):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
         """
         reader = csv.reader(data)
         next(reader)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for item in reader:
             long = item[1]
             rfcs = item[2]
 
             temp = []  # type: list[str]
             for rfc in filter(None, re.split(r'\[|\]', rfcs)):
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/qos_attribute.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/qos_attribute.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(QoSAttribute())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/revocation_status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_status_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(RevocationStatusCode())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/revocation_trigger.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/revocation_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(RevocationTrigger())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/status_code.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/status_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,19 +75,17 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
 
         # TODO: figure out how to handle this programmatically
         miss.append('#: Unspecified in the IANA registry')
-        miss.append("extend_enum(cls, 'Unassigned_%d' % value, value)")
-        miss.append('return cls(value)')
+        miss.append("return extend_enum(cls, 'Unassigned_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(StatusCode())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/traffic_selector.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/traffic_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(TrafficSelector())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/upa_status.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upa_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(UpdateNotificationACKStatus())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/mh/upn_reason.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/mh/upn_reason.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(UpdateNotificationReason())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ospf/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ospf/authentication.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/authentication.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/ospf/packet.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/ospf/packet.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/pcapng/block_type.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/pcapng/block_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
                 sufs = self.wrap_comment(desc)
 
                 enum.append(f'#: {sufs}\n    {pref}')
             except ValueError:
                 start, stop = map(lambda x: int(x, base=16), temp.split('-'))
 
                 miss.append(f'if 0x{start:08x} <= value <= 0x{stop:08x}:')
-                miss.append(f'   #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_%08x' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f'    #: {desc}')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_%08x' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(BlockType())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/reg/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/reg/ethertype.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/ethertype.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[1].split('-')
 
                 miss.append(f'if 0x{start} <= value <= 0x{stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{self.safe_name(name)}_0x%s' % hex(value)[2:].upper().zfill(4), value)")  # pylint: disable=line-too-long
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{self.safe_name(name)}_0x%s' % hex(value)[2:].upper().zfill(4), value)")  # pylint: disable=line-too-long
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(EtherType())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/reg/linktype.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/linktype.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for content in data:
             name = content.select('td.symbol')[0].text.strip()[9:].strip()
             temp = content.select('td.number')[0].text.strip()
             desc = content.select('td.symbol')[1].text.strip()
             cmmt = re.sub(r'\s+', ' ', content.select('td')[3].text.strip()).replace("''", '``').replace('_', '\_')
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/reg/transtype.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/reg/transtype.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/tcp/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/tcp/checksum.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/checksum.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in data.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/tcp/mp_tcp_option.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/mp_tcp_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
         Returns:
             Enumeration fields and missing fields.
 
         """
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned_%d' % value, value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned_%d' % value, value)",
         ]
         for code, name in data.items():
             renm = self.rename(name, code)  # type: ignore[arg-type]
             enum.append(f"{renm} = {code}".ljust(76))
         return enum, miss
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/tcp/option.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/tcp/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,13 @@
                 # enum.append(f'{pres.ljust(76)}{sufs}')
                 enum.append(f'{sufs}\n    {pres}')
             except ValueError:
                 start, stop = item[0].split('-')
 
                 miss.append(f'if {start} <= value <= {stop}:')
                 miss.append(f'    #: {desc}')
-                miss.append(f"    extend_enum(cls, '{name}_%d' % value, value)")
-                miss.append('    return cls(value)')
+                miss.append(f"    return extend_enum(cls, '{name}_%d' % value, value)")
         return enum, miss
 
 
 if __name__ == '__main__':
     sys.exit(Option())  # type: ignore[arg-type]
```

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/vlan/__init__.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcapkit-1.0.0b9/pcapkit/vendor/vlan/priority_level.py` & `pypcapkit-1.0.0rc1/pcapkit/vendor/vlan/priority_level.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,16 +62,15 @@
         """
         table = soup.find_all('table', class_='wikitable')[0]
         content = filter(lambda item: isinstance(item, bs4.element.Tag), table.tbody)
         next(content)  # header
 
         enum = []  # type: list[str]
         miss = [
-            "extend_enum(cls, 'Unassigned [0b%s]' % bin(value)[2:].zfill(3), value)",
-            'return cls(value)'
+            "return extend_enum(cls, 'Unassigned [0b%s]' % bin(value)[2:].zfill(3), value)",
         ]
         for item in content:
             line = item.find_all('td')
 
             pval = ' '.join(line[0].stripped_strings)
             prio = ' '.join(line[1].stripped_strings)
             abbr = ' '.join(line[2].stripped_strings)
```

### Comparing `pypcapkit-1.0.0b9/pypcapkit.egg-info/PKG-INFO` & `pypcapkit-1.0.0rc1/pypcapkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypcapkit
-Version: 1.0.0b9
+Version: 1.0.0rc1
 Summary: PyPCAPKit: comprehensive network packet analysis library
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
-Maintainer-email: Jarry Shaw <jarryshaw@icloud.com>
+Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: documentation, https://jarryshaw.github.io/PyPCAPKit/
 Project-URL: repository, https://github.com/JarryShaw/PyPCAPKit
 Project-URL: changelog, https://github.com/JarryShaw/PyPCAPKit/releases
 Keywords: network,pcap,packet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pypcapkit-1.0.0b9/pypcapkit.egg-info/SOURCES.txt` & `pypcapkit-1.0.0rc1/pypcapkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,20 @@
 pcapkit/const/mh/upa_status.py
 pcapkit/const/mh/upn_reason.py
 pcapkit/const/ospf/__init__.py
 pcapkit/const/ospf/authentication.py
 pcapkit/const/ospf/packet.py
 pcapkit/const/pcapng/__init__.py
 pcapkit/const/pcapng/block_type.py
+pcapkit/const/pcapng/filter_type.py
+pcapkit/const/pcapng/hash_algorithm.py
+pcapkit/const/pcapng/option_type.py
+pcapkit/const/pcapng/record_type.py
+pcapkit/const/pcapng/secrets_type.py
+pcapkit/const/pcapng/verdict_type.py
 pcapkit/const/reg/__init__.py
 pcapkit/const/reg/ethertype.py
 pcapkit/const/reg/linktype.py
 pcapkit/const/reg/transtype.py
 pcapkit/const/tcp/__init__.py
 pcapkit/const/tcp/checksum.py
 pcapkit/const/tcp/mp_tcp_option.py
@@ -138,14 +144,15 @@
 pcapkit/foundation/__init__.py
 pcapkit/foundation/extraction.py
 pcapkit/foundation/registry.py
 pcapkit/foundation/engines/__init__.py
 pcapkit/foundation/engines/dpkt.py
 pcapkit/foundation/engines/engine.py
 pcapkit/foundation/engines/pcap.py
+pcapkit/foundation/engines/pcapng.py
 pcapkit/foundation/engines/pyshark.py
 pcapkit/foundation/engines/scapy.py
 pcapkit/foundation/reassembly/__init__.py
 pcapkit/foundation/reassembly/ip.py
 pcapkit/foundation/reassembly/ipv4.py
 pcapkit/foundation/reassembly/ipv6.py
 pcapkit/foundation/reassembly/reassembly.py
@@ -211,14 +218,15 @@
 pcapkit/protocols/data/link/arp.py
 pcapkit/protocols/data/link/ethernet.py
 pcapkit/protocols/data/link/l2tp.py
 pcapkit/protocols/data/link/ospf.py
 pcapkit/protocols/data/link/vlan.py
 pcapkit/protocols/data/misc/__init__.py
 pcapkit/protocols/data/misc/null.py
+pcapkit/protocols/data/misc/pcapng.py
 pcapkit/protocols/data/misc/raw.py
 pcapkit/protocols/data/misc/pcap/__init__.py
 pcapkit/protocols/data/misc/pcap/frame.py
 pcapkit/protocols/data/misc/pcap/header.py
 pcapkit/protocols/data/transport/__init__.py
 pcapkit/protocols/data/transport/tcp.py
 pcapkit/protocols/data/transport/udp.py
@@ -254,14 +262,15 @@
 pcapkit/protocols/link/NotImplemented/eapol.py
 pcapkit/protocols/link/NotImplemented/fddi.py
 pcapkit/protocols/link/NotImplemented/isdn.py
 pcapkit/protocols/link/NotImplemented/ndp.py
 pcapkit/protocols/link/NotImplemented/ppp.py
 pcapkit/protocols/misc/__init__.py
 pcapkit/protocols/misc/null.py
+pcapkit/protocols/misc/pcapng.py
 pcapkit/protocols/misc/raw.py
 pcapkit/protocols/misc/pcap/__init__.py
 pcapkit/protocols/misc/pcap/frame.py
 pcapkit/protocols/misc/pcap/header.py
 pcapkit/protocols/schema/__init__.py
 pcapkit/protocols/schema/schema.py
 pcapkit/protocols/schema/application/__init__.py
@@ -299,16 +308,17 @@
 pcapkit/protocols/transport/tcp.py
 pcapkit/protocols/transport/transport.py
 pcapkit/protocols/transport/udp.py
 pcapkit/protocols/transport/NotImplemented/dccp.py
 pcapkit/protocols/transport/NotImplemented/rsvp.py
 pcapkit/protocols/transport/NotImplemented/sctp.py
 pcapkit/toolkit/__init__.py
-pcapkit/toolkit/default.py
 pcapkit/toolkit/dpkt.py
+pcapkit/toolkit/pcap.py
+pcapkit/toolkit/pcapng.py
 pcapkit/toolkit/pyshark.py
 pcapkit/toolkit/scapy.py
 pcapkit/utilities/__init__.py
 pcapkit/utilities/compat.py
 pcapkit/utilities/decorators.py
 pcapkit/utilities/exceptions.py
 pcapkit/utilities/logging.py
@@ -414,14 +424,20 @@
 pcapkit/vendor/mh/upa_status.py
 pcapkit/vendor/mh/upn_reason.py
 pcapkit/vendor/ospf/__init__.py
 pcapkit/vendor/ospf/authentication.py
 pcapkit/vendor/ospf/packet.py
 pcapkit/vendor/pcapng/__init__.py
 pcapkit/vendor/pcapng/block_type.py
+pcapkit/vendor/pcapng/filter_type.py
+pcapkit/vendor/pcapng/hash_algorithm.py
+pcapkit/vendor/pcapng/option_type.py
+pcapkit/vendor/pcapng/record_type.py
+pcapkit/vendor/pcapng/secrets_type.py
+pcapkit/vendor/pcapng/verdict_type.py
 pcapkit/vendor/reg/__init__.py
 pcapkit/vendor/reg/ethertype.py
 pcapkit/vendor/reg/linktype.py
 pcapkit/vendor/reg/transtype.py
 pcapkit/vendor/tcp/__init__.py
 pcapkit/vendor/tcp/checksum.py
 pcapkit/vendor/tcp/mp_tcp_option.py
```

### Comparing `pypcapkit-1.0.0b9/pyproject.toml` & `pypcapkit-1.0.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [project]
 name = "pypcapkit"
 dynamic = [ "version", "readme" ]
 authors = [
     { name="Jarry Shaw", email="jarryshaw@icloud.com" },
 ]
 maintainers = [
-    { name="Jarry Shaw", email="jarryshaw@icloud.com" },
+    { name="Jarry Shaw" },
 ]
 license = { text="BSD 3-Clause License" }
 requires-python = ">=3.6, <4"
 description = "PyPCAPKit: comprehensive network packet analysis library"
 keywords = [ "network", "pcap", "packet" ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `pypcapkit-1.0.0b9/setup.py` & `pypcapkit-1.0.0rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     from setuptools.command.develop import develop
     from setuptools.command.install import install
     from setuptools.command.sdist import sdist
 except:
     raise ImportError("setuptools is required to install PyPCAPKit!")
 
 
-def get_long_description() -> 'str | None':
+def get_long_description() -> 'str':
     """Extract description from README.rst, for PyPI's usage."""
     with open('README.rst', encoding='utf-8') as file:
         long_description = file.read()
     return long_description
 
 
 def refactor(path: 'str') -> 'None':
@@ -81,34 +81,34 @@
         # PyBPC compatibility enforcement
         refactor(os.path.join(self.build_lib, 'pcapkit'))
 
 
 class pcapkit_develop(develop):
     """Modified develop to run PyBPC conversion."""
 
-    def run(self) -> 'None':
+    def run(self) -> 'None':  # type: ignore[override]
         super(pcapkit_develop, self).run()
 
         # PyBPC compatibility enforcement
         refactor(os.path.join(self.install_lib, 'pcapkit'))
 
 
 class pcapkit_install(install):
     """Modified install to run PyBPC conversion."""
 
     def run(self) -> 'None':
         super(pcapkit_install, self).run()
 
         # PyBPC compatibility enforcement
-        refactor(os.path.join(self.install_lib, 'pcapkit'))
+        refactor(os.path.join(self.install_lib, 'pcapkit'))  # type: ignore[arg-type]
 
 
 setup(
     cmdclass={
-        'sdistpcapkit_': pcapkit_sdist,
+        'sdist': pcapkit_sdist,
         'build_py': pcapkit_build_py,
         'develop': pcapkit_develop,
         'install': pcapkit_install,
     },
     long_description=get_long_description(),
     long_description_content_type='text/x-rst',
 )
```

### Comparing `pypcapkit-1.0.0b9/util/bump_version.py` & `pypcapkit-1.0.0rc1/util/bump_version.py`

 * *Files identical despite different names*

