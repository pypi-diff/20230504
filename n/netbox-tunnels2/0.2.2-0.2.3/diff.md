# Comparing `tmp/netbox-tunnels2-0.2.2.tar.gz` & `tmp/netbox-tunnels2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-tunnels2-0.2.2.tar", last modified: Fri Apr 21 16:43:28 2023, max compression
+gzip compressed data, was "netbox-tunnels2-0.2.3.tar", last modified: Thu May  4 12:04:50 2023, max compression
```

## Comparing `netbox-tunnels2-0.2.2.tar` & `netbox-tunnels2-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.563734 netbox-tunnels2-0.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/docs/img/tunnel-info.png
--rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/docs/img/tunnel-list.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.684462 netbox-tunnels2-0.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.688462 netbox-tunnels2-0.2.3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/docs/img/tunnel-info.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/docs/img/tunnel-list.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.692462 netbox-tunnels2-0.2.3/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.692462 netbox-tunnels2-0.2.3/netbox_tunnels2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.684462 netbox-tunnels2-0.2.3/netbox_tunnels2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/netbox_tunnels2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/tests/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/netbox_tunnels2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:04:50.692462 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-04 12:04:50.000000 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-04 12:04:50.000000 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:04:50.000000 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 12:04:50.000000 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 12:04:50.000000 netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 12:04:50.696462 netbox-tunnels2-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-04 12:04:35.000000 netbox-tunnels2-0.2.3/setup.py
```

### Comparing `netbox-tunnels2-0.2.2/CONTRIBUTING.md` & `netbox-tunnels2-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/LICENSE` & `netbox-tunnels2-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/PKG-INFO` & `netbox-tunnels2-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,16 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.1     |
+|   NetBox 3.4   |      0.2.2     |
+|   NetBox 3.5 >   |      0.2.3     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.2/README.md` & `netbox-tunnels2-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.1     |
+|   NetBox 3.4   |      0.2.2     |
+|   NetBox 3.5 >   |      0.2.3     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.2/docs/img/tunnel-info.png` & `netbox-tunnels2-0.2.3/docs/img/tunnel-info.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/docs/img/tunnel-list.png` & `netbox-tunnels2-0.2.3/docs/img/tunnel-list.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/api/serializers.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/api/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
 from ..models import Tunnel, TunnelType
 
 
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from utilities.api import get_serializer_for_model
-from drf_yasg.utils import swagger_serializer_method
+from drf_spectacular.utils import extend_schema_field
 
 class NestedTunnelSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_tunnels2-api:tunnel-detail')
 
     class Meta:
         model = Tunnel
         fields = (
@@ -56,15 +56,15 @@
             'tunnel_type', 
             'psk', 
             'tags', 
             'custom_fields', 
             'created',
             'last_updated',
         )
-    @swagger_serializer_method(serializer_or_field=serializers.DictField)
+    @extend_schema_field(serializers.DictField)
     def get_side_a_assigned_object(self, obj):
         if obj.side_a_assigned_object is None:
             return None
         serializer = get_serializer_for_model(
             obj.side_a_assigned_object,
             prefix=NESTED_SERIALIZER_PREFIX,
         )
```

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/api/views.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/filtersets.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/forms.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     ChoiceField,
     MultipleChoiceField,
     ChoiceField,
     PasswordInput,
     ModelChoiceField
 )
 
-from utilities.forms import (
+from utilities.forms.fields import (
     DynamicModelChoiceField,
     SlugField,
     DynamicModelMultipleChoiceField
 )
 
 from dcim.models import Interface, Device
 from ipam.models import IPAddress, VRF
```

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/graphql.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0001_initial.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/models.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/models.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/navigation.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/tables.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html` & `netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html` & `netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html` & `netbox-tunnels2-0.2.3/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/tests/custom.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/tests/test_models.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/urls.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2/views.py` & `netbox-tunnels2-0.2.3/netbox_tunnels2/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/PKG-INFO` & `netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,16 @@
 * Tunnels
 * Tunnel Types
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |:--------------:|:--------------:|
-|   NetBox 3.4   |      0.2.1     |
+|   NetBox 3.4   |      0.2.2     |
+|   NetBox 3.5 >   |      0.2.3     |
 
 This is currently a work in progress.
 ## Installation
 You can install this package from Pip
 ```
 pip install netbox-tunnels2
 ```
```

### Comparing `netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/SOURCES.txt` & `netbox-tunnels2-0.2.3/netbox_tunnels2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.2/setup.cfg` & `netbox-tunnels2-0.2.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [gh-actions]
 python = 
 	3.10: py310
 	3.9: py39
 	3.8: py38, format, lint, build
 
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `netbox-tunnels2-0.2.2/setup.py` & `netbox-tunnels2-0.2.3/setup.py`

 * *Files identical despite different names*

