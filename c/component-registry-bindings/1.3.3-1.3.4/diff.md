# Comparing `tmp/component-registry-bindings-1.3.3.tar.gz` & `tmp/component-registry-bindings-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "component-registry-bindings-1.3.3.tar", last modified: Tue Apr  4 08:43:10 2023, max compression
+gzip compressed data, was "component-registry-bindings-1.3.4.tar", last modified: Thu May  4 12:12:54 2023, max compression
```

## Comparing `component-registry-bindings-1.3.3.tar` & `component-registry-bindings-1.3.4.tar`

### file list

```diff
@@ -1,121 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.509960 component-registry-bindings-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-04 08:43:10.509960 component-registry-bindings-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/healthy/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/healthy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/healthy/healthy_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.497960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_builds_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_builds_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_channels_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_channels_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_manifest_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_olcs_test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_provides_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_taxonomy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_manifest_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_products_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_products_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_schema_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_status_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.509960 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/build_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_streams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_variants_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_versions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_products_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    34892 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_channels_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_streams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_variants_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_versions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_products_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_provides_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_sources_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_upstreams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/namespace_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_channel_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_component_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_stream_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_variant_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_version_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_software_build_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_channels_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_streams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_variants_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_versions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_brew_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_channels_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_composes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_product_variants_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_product_versions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_products_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_relations_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_channels_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_product_streams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_product_versions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_products_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_relations_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_channels_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_product_streams_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_product_variants_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_products_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build_components_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_builds_list_build_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_channels_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_components_list_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_components_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_builds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/component_registry_bindings/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:43:10.493960 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-04 08:43:10.000000 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-04 08:43:10.000000 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:43:10.000000 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 08:43:10.000000 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-04 08:43:10.000000 component-registry-bindings-1.3.3/component_registry_bindings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:43:10.509960 component-registry-bindings-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-04 08:42:56.000000 component-registry-bindings-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.418296 component-registry-bindings-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 12:12:54.414296 component-registry-bindings-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/authentication_status/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/authentication_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/authentication_status/authentication_status_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/controlled_access_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/controlled_access_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/controlled_access_test/controlled_access_test_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/healthy/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/healthy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/healthy/healthy_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/token_auth_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/token_auth_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/token_auth_test/token_auth_test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/token_auth_test/token_auth_test_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.406296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_builds_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_builds_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_channels_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_channels_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_manifest_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_olcs_test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_provides_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_taxonomy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_manifest_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_products_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_products_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_schema_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_status_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.414296 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/authentication_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/build_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_streams_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_variants_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_versions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_products_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30839 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_channels_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_streams_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_variants_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_versions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_products_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/controlled_access_test_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/namespace_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_channel_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_component_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_stream_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_variant_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_software_build_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_channels_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_streams_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_variants_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_versions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_brew_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_channels_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_composes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_product_variants_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_product_versions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_products_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_relations_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_channels_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_product_streams_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_product_versions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_products_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_relations_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_channels_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_product_streams_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_product_variants_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_products_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build_components_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/token_auth_test_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/token_auth_test_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_builds_list_build_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_channels_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_components_list_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_components_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_builds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/component_registry_bindings/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:54.402296 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 12:12:54.000000 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-05-04 12:12:54.000000 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:54.000000 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 12:12:54.000000 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 12:12:54.000000 component-registry-bindings-1.3.4/component_registry_bindings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:12:54.418296 component-registry-bindings-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-04 12:12:39.000000 component-registry-bindings-1.3.4/setup.py
```

### Comparing `component-registry-bindings-1.3.3/LICENSE` & `component-registry-bindings-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/PKG-INFO` & `component-registry-bindings-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-registry-bindings
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python bindings for accessing Component Registry API
 Home-page: https://github.com/RedHatProductSecurity/component-registry-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/healthy/healthy_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/healthy/healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/__init__.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_builds_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_builds_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 from ...client import Client
 from ...models.paginated_software_build_list import PaginatedSoftwareBuildList
 from ...models.v1_builds_list_build_type import V1BuildsListBuildType
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {
+    "build_id": str,
     "build_type": V1BuildsListBuildType,
     "exclude_fields": List[str],
     "include_fields": List[str],
     "limit": int,
     "name": str,
     "offset": int,
     "search": str,
     "tags": int,
 }
 
 
 def _get_kwargs(
     *,
     client: Client,
+    build_id: Union[Unset, None, str] = UNSET,
     build_type: Union[Unset, None, V1BuildsListBuildType] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     search: Union[Unset, None, str] = UNSET,
@@ -55,14 +57,15 @@
     if not isinstance(include_fields, Unset):
         if include_fields is None:
             json_include_fields = None
         else:
             json_include_fields = include_fields
 
     params: Dict[str, Any] = {
+        "build_id": build_id,
         "build_type": json_build_type,
         "exclude_fields": json_exclude_fields,
         "include_fields": json_include_fields,
         "limit": limit,
         "name": name,
         "offset": offset,
         "search": search,
@@ -102,25 +105,27 @@
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    build_id: Union[Unset, None, str] = UNSET,
     build_type: Union[Unset, None, V1BuildsListBuildType] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     tags: Union[Unset, None, int] = UNSET,
 ) -> Response[PaginatedSoftwareBuildList]:
     kwargs = _get_kwargs(
         client=client,
+        build_id=build_id,
         build_type=build_type,
         exclude_fields=exclude_fields,
         include_fields=include_fields,
         limit=limit,
         name=name,
         offset=offset,
         search=search,
@@ -137,27 +142,29 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
+    build_id: Union[Unset, None, str] = UNSET,
     build_type: Union[Unset, None, V1BuildsListBuildType] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     tags: Union[Unset, None, int] = UNSET,
 ) -> Optional[PaginatedSoftwareBuildList]:
     """View for api/v1/builds"""
 
     return sync_detailed(
         client=client,
+        build_id=build_id,
         build_type=build_type,
         exclude_fields=exclude_fields,
         include_fields=include_fields,
         limit=limit,
         name=name,
         offset=offset,
         search=search,
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_builds_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_builds_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 QUERY_PARAMS = {
     "exclude_fields": List[str],
     "include_fields": List[str],
 }
 
 
 def _get_kwargs(
-    build_id: int,
+    uuid: str,
     *,
     client: Client,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/builds/{build_id}".format(
+    url = "{}/api/v1/builds/{uuid}".format(
         client.base_url,
-        build_id=build_id,
+        uuid=uuid,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
     json_exclude_fields: Union[Unset, None, List[str]] = UNSET
     if not isinstance(exclude_fields, Unset):
         if exclude_fields is None:
@@ -72,22 +72,22 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    build_id: int,
+    uuid: str,
     *,
     client: Client,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
 ) -> Response[SoftwareBuild]:
     kwargs = _get_kwargs(
-        build_id=build_id,
+        uuid=uuid,
         client=client,
         exclude_fields=exclude_fields,
         include_fields=include_fields,
     )
 
     response = requests.get(
         verify=client.verify_ssl,
@@ -97,21 +97,21 @@
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
-    build_id: int,
+    uuid: str,
     *,
     client: Client,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
 ) -> Optional[SoftwareBuild]:
     """View for api/v1/builds"""
 
     return sync_detailed(
-        build_id=build_id,
+        uuid=uuid,
         client=client,
         exclude_fields=exclude_fields,
         include_fields=include_fields,
     ).parsed
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_channels_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_channels_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_channels_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_channels_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 
 QUERY_PARAMS = {
     "arch": str,
     "channels": str,
     "description": str,
     "el_match": str,
     "exclude_fields": List[str],
+    "gomod_components": bool,
     "include_fields": List[str],
+    "latest_components": bool,
+    "latest_components_by_streams": bool,
     "limit": int,
     "missing_copyright": bool,
     "missing_license": bool,
+    "missing_scan_url": bool,
     "name": str,
     "namespace": V1ComponentsListNamespace,
     "nevra": str,
     "nvr": str,
     "offset": int,
     "ofuri": str,
     "product_streams": str,
@@ -33,14 +37,16 @@
     "re_name": str,
     "re_provides": str,
     "re_purl": str,
     "re_sources": str,
     "re_upstreams": str,
     "related_url": str,
     "release": str,
+    "released_components": bool,
+    "root_components": bool,
     "search": str,
     "sources": str,
     "tags": int,
     "type": V1ComponentsListType,
     "upstreams": str,
     "version": str,
     "view": str,
@@ -51,18 +57,22 @@
     *,
     client: Client,
     arch: Union[Unset, None, str] = UNSET,
     channels: Union[Unset, None, str] = UNSET,
     description: Union[Unset, None, str] = UNSET,
     el_match: Union[Unset, None, str] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
+    gomod_components: Union[Unset, None, bool] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
+    latest_components: Union[Unset, None, bool] = UNSET,
+    latest_components_by_streams: Union[Unset, None, bool] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     missing_copyright: Union[Unset, None, bool] = UNSET,
     missing_license: Union[Unset, None, bool] = UNSET,
+    missing_scan_url: Union[Unset, None, bool] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     namespace: Union[Unset, None, V1ComponentsListNamespace] = UNSET,
     nevra: Union[Unset, None, str] = UNSET,
     nvr: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     ofuri: Union[Unset, None, str] = UNSET,
     product_streams: Union[Unset, None, str] = UNSET,
@@ -74,14 +84,16 @@
     re_name: Union[Unset, None, str] = UNSET,
     re_provides: Union[Unset, None, str] = UNSET,
     re_purl: Union[Unset, None, str] = UNSET,
     re_sources: Union[Unset, None, str] = UNSET,
     re_upstreams: Union[Unset, None, str] = UNSET,
     related_url: Union[Unset, None, str] = UNSET,
     release: Union[Unset, None, str] = UNSET,
+    released_components: Union[Unset, None, bool] = UNSET,
+    root_components: Union[Unset, None, bool] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     sources: Union[Unset, None, str] = UNSET,
     tags: Union[Unset, None, int] = UNSET,
     type: Union[Unset, None, V1ComponentsListType] = UNSET,
     upstreams: Union[Unset, None, str] = UNSET,
     version: Union[Unset, None, str] = UNSET,
     view: Union[Unset, None, str] = UNSET,
@@ -120,18 +132,22 @@
 
     params: Dict[str, Any] = {
         "arch": arch,
         "channels": channels,
         "description": description,
         "el_match": el_match,
         "exclude_fields": json_exclude_fields,
+        "gomod_components": gomod_components,
         "include_fields": json_include_fields,
+        "latest_components": latest_components,
+        "latest_components_by_streams": latest_components_by_streams,
         "limit": limit,
         "missing_copyright": missing_copyright,
         "missing_license": missing_license,
+        "missing_scan_url": missing_scan_url,
         "name": name,
         "namespace": json_namespace,
         "nevra": nevra,
         "nvr": nvr,
         "offset": offset,
         "ofuri": ofuri,
         "product_streams": product_streams,
@@ -143,14 +159,16 @@
         "re_name": re_name,
         "re_provides": re_provides,
         "re_purl": re_purl,
         "re_sources": re_sources,
         "re_upstreams": re_upstreams,
         "related_url": related_url,
         "release": release,
+        "released_components": released_components,
+        "root_components": root_components,
         "search": search,
         "sources": sources,
         "tags": tags,
         "type": json_type,
         "upstreams": upstreams,
         "version": version,
         "view": view,
@@ -190,18 +208,22 @@
     *,
     client: Client,
     arch: Union[Unset, None, str] = UNSET,
     channels: Union[Unset, None, str] = UNSET,
     description: Union[Unset, None, str] = UNSET,
     el_match: Union[Unset, None, str] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
+    gomod_components: Union[Unset, None, bool] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
+    latest_components: Union[Unset, None, bool] = UNSET,
+    latest_components_by_streams: Union[Unset, None, bool] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     missing_copyright: Union[Unset, None, bool] = UNSET,
     missing_license: Union[Unset, None, bool] = UNSET,
+    missing_scan_url: Union[Unset, None, bool] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     namespace: Union[Unset, None, V1ComponentsListNamespace] = UNSET,
     nevra: Union[Unset, None, str] = UNSET,
     nvr: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     ofuri: Union[Unset, None, str] = UNSET,
     product_streams: Union[Unset, None, str] = UNSET,
@@ -213,14 +235,16 @@
     re_name: Union[Unset, None, str] = UNSET,
     re_provides: Union[Unset, None, str] = UNSET,
     re_purl: Union[Unset, None, str] = UNSET,
     re_sources: Union[Unset, None, str] = UNSET,
     re_upstreams: Union[Unset, None, str] = UNSET,
     related_url: Union[Unset, None, str] = UNSET,
     release: Union[Unset, None, str] = UNSET,
+    released_components: Union[Unset, None, bool] = UNSET,
+    root_components: Union[Unset, None, bool] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     sources: Union[Unset, None, str] = UNSET,
     tags: Union[Unset, None, int] = UNSET,
     type: Union[Unset, None, V1ComponentsListType] = UNSET,
     upstreams: Union[Unset, None, str] = UNSET,
     version: Union[Unset, None, str] = UNSET,
     view: Union[Unset, None, str] = UNSET,
@@ -228,18 +252,22 @@
     kwargs = _get_kwargs(
         client=client,
         arch=arch,
         channels=channels,
         description=description,
         el_match=el_match,
         exclude_fields=exclude_fields,
+        gomod_components=gomod_components,
         include_fields=include_fields,
+        latest_components=latest_components,
+        latest_components_by_streams=latest_components_by_streams,
         limit=limit,
         missing_copyright=missing_copyright,
         missing_license=missing_license,
+        missing_scan_url=missing_scan_url,
         name=name,
         namespace=namespace,
         nevra=nevra,
         nvr=nvr,
         offset=offset,
         ofuri=ofuri,
         product_streams=product_streams,
@@ -251,14 +279,16 @@
         re_name=re_name,
         re_provides=re_provides,
         re_purl=re_purl,
         re_sources=re_sources,
         re_upstreams=re_upstreams,
         related_url=related_url,
         release=release,
+        released_components=released_components,
+        root_components=root_components,
         search=search,
         sources=sources,
         tags=tags,
         type=type,
         upstreams=upstreams,
         version=version,
         view=view,
@@ -279,18 +309,22 @@
     *,
     client: Client,
     arch: Union[Unset, None, str] = UNSET,
     channels: Union[Unset, None, str] = UNSET,
     description: Union[Unset, None, str] = UNSET,
     el_match: Union[Unset, None, str] = UNSET,
     exclude_fields: Union[Unset, None, List[str]] = UNSET,
+    gomod_components: Union[Unset, None, bool] = UNSET,
     include_fields: Union[Unset, None, List[str]] = UNSET,
+    latest_components: Union[Unset, None, bool] = UNSET,
+    latest_components_by_streams: Union[Unset, None, bool] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     missing_copyright: Union[Unset, None, bool] = UNSET,
     missing_license: Union[Unset, None, bool] = UNSET,
+    missing_scan_url: Union[Unset, None, bool] = UNSET,
     name: Union[Unset, None, str] = UNSET,
     namespace: Union[Unset, None, V1ComponentsListNamespace] = UNSET,
     nevra: Union[Unset, None, str] = UNSET,
     nvr: Union[Unset, None, str] = UNSET,
     offset: Union[Unset, None, int] = UNSET,
     ofuri: Union[Unset, None, str] = UNSET,
     product_streams: Union[Unset, None, str] = UNSET,
@@ -302,14 +336,16 @@
     re_name: Union[Unset, None, str] = UNSET,
     re_provides: Union[Unset, None, str] = UNSET,
     re_purl: Union[Unset, None, str] = UNSET,
     re_sources: Union[Unset, None, str] = UNSET,
     re_upstreams: Union[Unset, None, str] = UNSET,
     related_url: Union[Unset, None, str] = UNSET,
     release: Union[Unset, None, str] = UNSET,
+    released_components: Union[Unset, None, bool] = UNSET,
+    root_components: Union[Unset, None, bool] = UNSET,
     search: Union[Unset, None, str] = UNSET,
     sources: Union[Unset, None, str] = UNSET,
     tags: Union[Unset, None, int] = UNSET,
     type: Union[Unset, None, V1ComponentsListType] = UNSET,
     upstreams: Union[Unset, None, str] = UNSET,
     version: Union[Unset, None, str] = UNSET,
     view: Union[Unset, None, str] = UNSET,
@@ -319,18 +355,22 @@
     return sync_detailed(
         client=client,
         arch=arch,
         channels=channels,
         description=description,
         el_match=el_match,
         exclude_fields=exclude_fields,
+        gomod_components=gomod_components,
         include_fields=include_fields,
+        latest_components=latest_components,
+        latest_components_by_streams=latest_components_by_streams,
         limit=limit,
         missing_copyright=missing_copyright,
         missing_license=missing_license,
+        missing_scan_url=missing_scan_url,
         name=name,
         namespace=namespace,
         nevra=nevra,
         nvr=nvr,
         offset=offset,
         ofuri=ofuri,
         product_streams=product_streams,
@@ -342,14 +382,16 @@
         re_name=re_name,
         re_provides=re_provides,
         re_purl=re_purl,
         re_sources=re_sources,
         re_upstreams=re_upstreams,
         related_url=related_url,
         release=release,
+        released_components=released_components,
+        root_components=root_components,
         search=search,
         sources=sources,
         tags=tags,
         type=type,
         upstreams=upstreams,
         version=version,
         view=view,
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_manifest_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_manifest_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_olcs_test_update.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_olcs_test_update.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_provides_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_provides_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_components_taxonomy_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_components_taxonomy_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_manifest_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_manifest_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_streams_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_variants_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_products_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_products_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_products_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_products_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_schema_retrieve.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/api/v1/v1_status_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/api/v1/v1_status_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/client.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/client.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/__init__.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """ Contains all the data models used in inputs/outputs """
 
+from .authentication_status_retrieve_response_200 import (
+    AuthenticationStatusRetrieveResponse200,
+)
 from .build_type_enum import BuildTypeEnum
 from .channel import Channel
 from .channel_product_streams_item import ChannelProductStreamsItem
 from .channel_product_variants_item import ChannelProductVariantsItem
 from .channel_product_versions_item import ChannelProductVersionsItem
 from .channel_products_item import ChannelProductsItem
 from .channel_type_enum import ChannelTypeEnum
 from .component import Component
 from .component_channels_item import ComponentChannelsItem
 from .component_product_streams_item import ComponentProductStreamsItem
 from .component_product_variants_item import ComponentProductVariantsItem
 from .component_product_versions_item import ComponentProductVersionsItem
 from .component_products_item import ComponentProductsItem
-from .component_provides_item import ComponentProvidesItem
-from .component_sources_item import ComponentSourcesItem
 from .component_type_enum import ComponentTypeEnum
-from .component_upstreams_item import ComponentUpstreamsItem
+from .controlled_access_test_retrieve_response_200 import (
+    ControlledAccessTestRetrieveResponse200,
+)
 from .namespace_enum import NamespaceEnum
 from .paginated_channel_list import PaginatedChannelList
 from .paginated_component_list import PaginatedComponentList
 from .paginated_product_list import PaginatedProductList
 from .paginated_product_stream_list import PaginatedProductStreamList
 from .paginated_product_variant_list import PaginatedProductVariantList
 from .paginated_product_version_list import PaginatedProductVersionList
@@ -49,14 +52,16 @@
 from .product_version_product_streams_item import ProductVersionProductStreamsItem
 from .product_version_product_variants_item import ProductVersionProductVariantsItem
 from .product_version_products_item import ProductVersionProductsItem
 from .software_build import SoftwareBuild
 from .software_build_components_item import SoftwareBuildComponentsItem
 from .software_build_summary import SoftwareBuildSummary
 from .tag import Tag
+from .token_auth_test_create_response_200 import TokenAuthTestCreateResponse200
+from .token_auth_test_retrieve_response_200 import TokenAuthTestRetrieveResponse200
 from .v1_builds_list_build_type import V1BuildsListBuildType
 from .v1_channels_list_type import V1ChannelsListType
 from .v1_components_list_namespace import V1ComponentsListNamespace
 from .v1_components_list_type import V1ComponentsListType
 from .v1_schema_retrieve_format import V1SchemaRetrieveFormat
 from .v1_schema_retrieve_response_200 import V1SchemaRetrieveResponse200
 from .v1_status_list_response_200 import V1StatusListResponse200
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_streams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_streams_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_variants_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_variants_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_product_versions_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_product_versions_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/channel_products_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/channel_products_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 import attr
 
 from ..models.component_channels_item import ComponentChannelsItem
 from ..models.component_product_streams_item import ComponentProductStreamsItem
 from ..models.component_product_variants_item import ComponentProductVariantsItem
 from ..models.component_product_versions_item import ComponentProductVersionsItem
 from ..models.component_products_item import ComponentProductsItem
-from ..models.component_provides_item import ComponentProvidesItem
-from ..models.component_sources_item import ComponentSourcesItem
 from ..models.component_type_enum import ComponentTypeEnum
-from ..models.component_upstreams_item import ComponentUpstreamsItem
 from ..models.namespace_enum import NamespaceEnum
 from ..models.software_build_summary import SoftwareBuildSummary
 from ..models.tag import Tag
 from ..types import UNSET, ComponentRegistryModel, Unset
 
 T = TypeVar("T", bound="Component")
 
@@ -52,17 +49,17 @@
     software_build: SoftwareBuildSummary
     errata: List[str]
     products: List[ComponentProductsItem]
     product_versions: List[ComponentProductVersionsItem]
     product_streams: List[ComponentProductStreamsItem]
     product_variants: List[ComponentProductVariantsItem]
     channels: List[ComponentChannelsItem]
-    sources: List[ComponentSourcesItem]
-    provides: List[ComponentProvidesItem]
-    upstreams: List[ComponentUpstreamsItem]
+    sources: str
+    provides: str
+    upstreams: str
     manifest: str
     filename: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         link = self.link
         download_url = self.download_url
@@ -168,44 +165,17 @@
             for channels_item_data in self.channels:
                 channels_item: Dict[str, Any] = UNSET
                 if not isinstance(channels_item_data, Unset):
                     channels_item = channels_item_data.to_dict()
 
                 channels.append(channels_item)
 
-        sources: List[Dict[str, Any]] = UNSET
-        if not isinstance(self.sources, Unset):
-            sources = []
-            for sources_item_data in self.sources:
-                sources_item: Dict[str, Any] = UNSET
-                if not isinstance(sources_item_data, Unset):
-                    sources_item = sources_item_data.to_dict()
-
-                sources.append(sources_item)
-
-        provides: List[Dict[str, Any]] = UNSET
-        if not isinstance(self.provides, Unset):
-            provides = []
-            for provides_item_data in self.provides:
-                provides_item: Dict[str, Any] = UNSET
-                if not isinstance(provides_item_data, Unset):
-                    provides_item = provides_item_data.to_dict()
-
-                provides.append(provides_item)
-
-        upstreams: List[Dict[str, Any]] = UNSET
-        if not isinstance(self.upstreams, Unset):
-            upstreams = []
-            for upstreams_item_data in self.upstreams:
-                upstreams_item: Dict[str, Any] = UNSET
-                if not isinstance(upstreams_item_data, Unset):
-                    upstreams_item = upstreams_item_data.to_dict()
-
-                upstreams.append(upstreams_item)
-
+        sources = self.sources
+        provides = self.provides
+        upstreams = self.upstreams
         manifest = self.manifest
         filename = self.filename
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if link is not UNSET:
             field_dict["link"] = link
@@ -465,47 +435,29 @@
                 channels_item: Dict[str, Any] = UNSET
                 if not isinstance(channels_item_data, Unset):
                     channels_item = channels_item_data.to_dict()
 
                 _temp_channels.append(channels_item)
             channels = (None, json.dumps(_temp_channels), "application/json")
 
-        sources: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.sources, Unset):
-            _temp_sources = []
-            for sources_item_data in self.sources:
-                sources_item: Dict[str, Any] = UNSET
-                if not isinstance(sources_item_data, Unset):
-                    sources_item = sources_item_data.to_dict()
-
-                _temp_sources.append(sources_item)
-            sources = (None, json.dumps(_temp_sources), "application/json")
-
-        provides: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.provides, Unset):
-            _temp_provides = []
-            for provides_item_data in self.provides:
-                provides_item: Dict[str, Any] = UNSET
-                if not isinstance(provides_item_data, Unset):
-                    provides_item = provides_item_data.to_dict()
-
-                _temp_provides.append(provides_item)
-            provides = (None, json.dumps(_temp_provides), "application/json")
-
-        upstreams: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.upstreams, Unset):
-            _temp_upstreams = []
-            for upstreams_item_data in self.upstreams:
-                upstreams_item: Dict[str, Any] = UNSET
-                if not isinstance(upstreams_item_data, Unset):
-                    upstreams_item = upstreams_item_data.to_dict()
-
-                _temp_upstreams.append(upstreams_item)
-            upstreams = (None, json.dumps(_temp_upstreams), "application/json")
-
+        sources = (
+            self.sources
+            if self.sources is UNSET
+            else (None, str(self.sources), "text/plain")
+        )
+        provides = (
+            self.provides
+            if self.provides is UNSET
+            else (None, str(self.provides), "text/plain")
+        )
+        upstreams = (
+            self.upstreams
+            if self.upstreams is UNSET
+            else (None, str(self.upstreams), "text/plain")
+        )
         manifest = (
             self.manifest
             if self.manifest is UNSET
             else (None, str(self.manifest), "text/plain")
         )
         filename = (
             self.filename
@@ -755,58 +707,19 @@
                 if isinstance(_channels_item, Unset):
                     channels_item = UNSET
                 else:
                     channels_item = ComponentChannelsItem.from_dict(_channels_item)
 
                 channels.append(channels_item)
 
-        sources = []
-        _sources = d.pop("sources", UNSET)
-        if _sources is UNSET:
-            sources = UNSET
-        else:
-            for sources_item_data in _sources or []:
-                _sources_item = sources_item_data
-                sources_item: ComponentSourcesItem
-                if isinstance(_sources_item, Unset):
-                    sources_item = UNSET
-                else:
-                    sources_item = ComponentSourcesItem.from_dict(_sources_item)
-
-                sources.append(sources_item)
-
-        provides = []
-        _provides = d.pop("provides", UNSET)
-        if _provides is UNSET:
-            provides = UNSET
-        else:
-            for provides_item_data in _provides or []:
-                _provides_item = provides_item_data
-                provides_item: ComponentProvidesItem
-                if isinstance(_provides_item, Unset):
-                    provides_item = UNSET
-                else:
-                    provides_item = ComponentProvidesItem.from_dict(_provides_item)
+        sources = d.pop("sources", UNSET)
 
-                provides.append(provides_item)
-
-        upstreams = []
-        _upstreams = d.pop("upstreams", UNSET)
-        if _upstreams is UNSET:
-            upstreams = UNSET
-        else:
-            for upstreams_item_data in _upstreams or []:
-                _upstreams_item = upstreams_item_data
-                upstreams_item: ComponentUpstreamsItem
-                if isinstance(_upstreams_item, Unset):
-                    upstreams_item = UNSET
-                else:
-                    upstreams_item = ComponentUpstreamsItem.from_dict(_upstreams_item)
+        provides = d.pop("provides", UNSET)
 
-                upstreams.append(upstreams_item)
+        upstreams = d.pop("upstreams", UNSET)
 
         manifest = d.pop("manifest", UNSET)
 
         filename = d.pop("filename", UNSET)
 
         component = cls(
             link=link,
@@ -880,17 +793,17 @@
             "software_build": SoftwareBuildSummary,
             "errata": List[str],
             "products": List[ComponentProductsItem],
             "product_versions": List[ComponentProductVersionsItem],
             "product_streams": List[ComponentProductStreamsItem],
             "product_variants": List[ComponentProductVariantsItem],
             "channels": List[ComponentChannelsItem],
-            "sources": List[ComponentSourcesItem],
-            "provides": List[ComponentProvidesItem],
-            "upstreams": List[ComponentUpstreamsItem],
+            "sources": str,
+            "provides": str,
+            "upstreams": str,
             "manifest": str,
             "filename": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_channels_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_channels_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_streams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_streams_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_variants_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_variants_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_product_versions_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_product_versions_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_products_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/component_products_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_provides_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ComponentProvidesItem")
+T = TypeVar("T", bound="V1SchemaRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ComponentProvidesItem(ComponentRegistryModel):
+class V1SchemaRetrieveResponse200(ComponentRegistryModel):
     """ """
 
-    additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        component_provides_item = cls()
+        v1_schema_retrieve_response_200 = cls()
 
-        component_provides_item.additional_properties = d
-        return component_provides_item
+        v1_schema_retrieve_response_200.additional_properties = d
+        return v1_schema_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> str:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: str) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_sources_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_channels_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ComponentSourcesItem")
+T = TypeVar("T", bound="ProductChannelsItem")
 
 
 @attr.s(auto_attribs=True)
-class ComponentSourcesItem(ComponentRegistryModel):
+class ProductChannelsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        component_sources_item = cls()
+        product_channels_item = cls()
 
-        component_sources_item.additional_properties = d
-        return component_sources_item
+        product_channels_item.additional_properties = d
+        return product_channels_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/component_upstreams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_streams_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ComponentUpstreamsItem")
+T = TypeVar("T", bound="ProductProductStreamsItem")
 
 
 @attr.s(auto_attribs=True)
-class ComponentUpstreamsItem(ComponentRegistryModel):
+class ProductProductStreamsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        component_upstreams_item = cls()
+        product_product_streams_item = cls()
 
-        component_upstreams_item.additional_properties = d
-        return component_upstreams_item
+        product_product_streams_item.additional_properties = d
+        return product_product_streams_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_channel_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_channel_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_component_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_component_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_stream_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_stream_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_variant_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_variant_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_product_version_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_product_version_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/paginated_software_build_list.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/paginated_software_build_list.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_channels_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_versions_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductChannelsItem")
+T = TypeVar("T", bound="ProductProductVersionsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductChannelsItem(ComponentRegistryModel):
+class ProductProductVersionsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_channels_item = cls()
+        product_product_versions_item = cls()
 
-        product_channels_item.additional_properties = d
-        return product_channels_item
+        product_product_versions_item.additional_properties = d
+        return product_product_versions_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_streams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_products_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductProductStreamsItem")
+T = TypeVar("T", bound="ProductStreamProductsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductProductStreamsItem(ComponentRegistryModel):
+class ProductStreamProductsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_product_streams_item = cls()
+        product_stream_products_item = cls()
 
-        product_product_streams_item.additional_properties = d
-        return product_product_streams_item
+        product_stream_products_item.additional_properties = d
+        return product_stream_products_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_variants_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_product_variants_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_product_versions_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_products_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductProductVersionsItem")
+T = TypeVar("T", bound="ProductVersionProductsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductProductVersionsItem(ComponentRegistryModel):
+class ProductVersionProductsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_product_versions_item = cls()
+        product_version_products_item = cls()
 
-        product_product_versions_item.additional_properties = d
-        return product_product_versions_item
+        product_version_products_item.additional_properties = d
+        return product_version_products_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_brew_tags.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_brew_tags.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_channels_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_channels_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_composes.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_composes.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_product_variants_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_product_variants_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_product_versions_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_product_versions_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_products_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_stream_relations_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductStreamProductsItem")
+T = TypeVar("T", bound="ProductStreamRelationsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductStreamProductsItem(ComponentRegistryModel):
+class ProductStreamRelationsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_stream_products_item = cls()
+        product_stream_relations_item = cls()
 
-        product_stream_products_item.additional_properties = d
-        return product_stream_products_item
+        product_stream_relations_item.additional_properties = d
+        return product_stream_relations_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_stream_relations_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_relations_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductStreamRelationsItem")
+T = TypeVar("T", bound="ProductVariantRelationsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductStreamRelationsItem(ComponentRegistryModel):
+class ProductVariantRelationsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_stream_relations_item = cls()
+        product_variant_relations_item = cls()
 
-        product_stream_relations_item.additional_properties = d
-        return product_stream_relations_item
+        product_variant_relations_item.additional_properties = d
+        return product_variant_relations_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_channels_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_channels_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_product_streams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_product_streams_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_product_versions_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_product_versions_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_products_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_variant_products_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_variant_relations_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_product_variants_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..types import ComponentRegistryModel
 
-T = TypeVar("T", bound="ProductVariantRelationsItem")
+T = TypeVar("T", bound="ProductVersionProductVariantsItem")
 
 
 @attr.s(auto_attribs=True)
-class ProductVariantRelationsItem(ComponentRegistryModel):
+class ProductVersionProductVariantsItem(ComponentRegistryModel):
     """ """
 
     additional_properties: Dict[str, str] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
-        product_variant_relations_item = cls()
+        product_version_product_variants_item = cls()
 
-        product_variant_relations_item.additional_properties = d
-        return product_variant_relations_item
+        product_version_product_variants_item.additional_properties = d
+        return product_version_product_variants_item
 
     @staticmethod
     def get_fields():
         return {}
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_channels_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_channels_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/product_version_product_streams_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/product_version_product_streams_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 
 
 @attr.s(auto_attribs=True)
 class SoftwareBuild(ComponentRegistryModel):
     """Show detailed information for SoftwareBuild(s).
     Add or remove fields using ?include_fields=&exclude_fields="""
 
+    uuid: str
     link: str
     web_url: str
-    build_id: int
+    build_id: str
     build_type: BuildTypeEnum
     name: str
     source: str
     tags: List[Tag]
     created_at: datetime.datetime
     last_changed: datetime.datetime
     components: List[SoftwareBuildComponentsItem]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        uuid = self.uuid
         link = self.link
         web_url = self.web_url
         build_id = self.build_id
         build_type: str = UNSET
         if not isinstance(self.build_type, Unset):
 
             build_type = BuildTypeEnum(self.build_type).value
@@ -66,14 +68,16 @@
                 if not isinstance(components_item_data, Unset):
                     components_item = components_item_data.to_dict()
 
                 components.append(components_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
+        if uuid is not UNSET:
+            field_dict["uuid"] = uuid
         if link is not UNSET:
             field_dict["link"] = link
         if web_url is not UNSET:
             field_dict["web_url"] = web_url
         if build_id is not UNSET:
             field_dict["build_id"] = build_id
         if build_type is not UNSET:
@@ -92,14 +96,16 @@
             field_dict["components"] = components
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if isinstance(src_dict, dict) else {}
+        uuid = d.pop("uuid", UNSET)
+
         link = d.pop("link", UNSET)
 
         web_url = d.pop("web_url", UNSET)
 
         build_id = d.pop("build_id", UNSET)
 
         _build_type = d.pop("build_type", UNSET)
@@ -156,14 +162,15 @@
                     components_item = SoftwareBuildComponentsItem.from_dict(
                         _components_item
                     )
 
                 components.append(components_item)
 
         software_build = cls(
+            uuid=uuid,
             link=link,
             web_url=web_url,
             build_id=build_id,
             build_type=build_type,
             name=name,
             source=source,
             tags=tags,
@@ -174,17 +181,18 @@
 
         software_build.additional_properties = d
         return software_build
 
     @staticmethod
     def get_fields():
         return {
+            "uuid": str,
             "link": str,
             "web_url": str,
-            "build_id": int,
+            "build_id": str,
             "build_type": BuildTypeEnum,
             "name": str,
             "source": str,
             "tags": List[Tag],
             "created_at": datetime.datetime,
             "last_changed": datetime.datetime,
             "components": List[SoftwareBuildComponentsItem],
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build_components_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build_components_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/software_build_summary.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/software_build_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 @attr.s(auto_attribs=True)
 class SoftwareBuildSummary(ComponentRegistryModel):
     """Show summary information for a SoftwareBuild.
     Add or remove fields using ?include_fields=&exclude_fields="""
 
     link: str
-    build_id: int
+    build_id: str
     build_type: BuildTypeEnum
     name: str
     source: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         link = self.link
@@ -75,15 +75,15 @@
         software_build_summary.additional_properties = d
         return software_build_summary
 
     @staticmethod
     def get_fields():
         return {
             "link": str,
-            "build_id": int,
+            "build_id": str,
             "build_type": BuildTypeEnum,
             "name": str,
             "source": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/tag.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/tag.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_builds.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_builds.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_channels.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_channels.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_components.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_components.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_streams.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_streams.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_variants.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_variants.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_versions.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_product_versions.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_products.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_products.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_relations.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/models/v1_status_list_response_200_results_item_relations.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/bindings/python_client/types.py` & `component-registry-bindings-1.3.4/component_registry_bindings/bindings/python_client/types.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/constants.py` & `component-registry-bindings-1.3.4/component_registry_bindings/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 
 COMPONENT_REGISTRY_API_VERSION: str = "v1"
-COMPONENT_REGISTRY_BINDINGS_USERAGENT: str = "component-registry-bindings-1.3.3"
+COMPONENT_REGISTRY_BINDINGS_USERAGENT: str = "component-registry-bindings-1.3.4"
 COMPONENT_REGISTRY_BINDINGS_API_PATH: str = (
     f".bindings.python_client.api.{COMPONENT_REGISTRY_API_VERSION}"
 )
 
 # all available session operations
 ALL_SESSION_OPERATIONS: List[str] = (
     "retrieve",
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings/session.py` & `component-registry-bindings-1.3.4/component_registry_bindings/session.py`

 * *Files identical despite different names*

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings.egg-info/PKG-INFO` & `component-registry-bindings-1.3.4/component_registry_bindings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-registry-bindings
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python bindings for accessing Component Registry API
 Home-page: https://github.com/RedHatProductSecurity/component-registry-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `component-registry-bindings-1.3.3/component_registry_bindings.egg-info/SOURCES.txt` & `component-registry-bindings-1.3.4/component_registry_bindings.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,23 @@
 component_registry_bindings.egg-info/requires.txt
 component_registry_bindings.egg-info/top_level.txt
 component_registry_bindings/bindings/__init__.py
 component_registry_bindings/bindings/python_client/__init__.py
 component_registry_bindings/bindings/python_client/client.py
 component_registry_bindings/bindings/python_client/types.py
 component_registry_bindings/bindings/python_client/api/__init__.py
+component_registry_bindings/bindings/python_client/api/authentication_status/__init__.py
+component_registry_bindings/bindings/python_client/api/authentication_status/authentication_status_retrieve.py
+component_registry_bindings/bindings/python_client/api/controlled_access_test/__init__.py
+component_registry_bindings/bindings/python_client/api/controlled_access_test/controlled_access_test_retrieve.py
 component_registry_bindings/bindings/python_client/api/healthy/__init__.py
 component_registry_bindings/bindings/python_client/api/healthy/healthy_retrieve.py
+component_registry_bindings/bindings/python_client/api/token_auth_test/__init__.py
+component_registry_bindings/bindings/python_client/api/token_auth_test/token_auth_test_create.py
+component_registry_bindings/bindings/python_client/api/token_auth_test/token_auth_test_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/__init__.py
 component_registry_bindings/bindings/python_client/api/v1/v1_builds_list.py
 component_registry_bindings/bindings/python_client/api/v1/v1_builds_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/v1_channels_list.py
 component_registry_bindings/bindings/python_client/api/v1/v1_channels_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/v1_components_list.py
 component_registry_bindings/bindings/python_client/api/v1/v1_components_manifest_retrieve.py
@@ -35,31 +42,30 @@
 component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_list.py
 component_registry_bindings/bindings/python_client/api/v1/v1_product_versions_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/v1_products_list.py
 component_registry_bindings/bindings/python_client/api/v1/v1_products_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/v1_schema_retrieve.py
 component_registry_bindings/bindings/python_client/api/v1/v1_status_list.py
 component_registry_bindings/bindings/python_client/models/__init__.py
+component_registry_bindings/bindings/python_client/models/authentication_status_retrieve_response_200.py
 component_registry_bindings/bindings/python_client/models/build_type_enum.py
 component_registry_bindings/bindings/python_client/models/channel.py
 component_registry_bindings/bindings/python_client/models/channel_product_streams_item.py
 component_registry_bindings/bindings/python_client/models/channel_product_variants_item.py
 component_registry_bindings/bindings/python_client/models/channel_product_versions_item.py
 component_registry_bindings/bindings/python_client/models/channel_products_item.py
 component_registry_bindings/bindings/python_client/models/channel_type_enum.py
 component_registry_bindings/bindings/python_client/models/component.py
 component_registry_bindings/bindings/python_client/models/component_channels_item.py
 component_registry_bindings/bindings/python_client/models/component_product_streams_item.py
 component_registry_bindings/bindings/python_client/models/component_product_variants_item.py
 component_registry_bindings/bindings/python_client/models/component_product_versions_item.py
 component_registry_bindings/bindings/python_client/models/component_products_item.py
-component_registry_bindings/bindings/python_client/models/component_provides_item.py
-component_registry_bindings/bindings/python_client/models/component_sources_item.py
 component_registry_bindings/bindings/python_client/models/component_type_enum.py
-component_registry_bindings/bindings/python_client/models/component_upstreams_item.py
+component_registry_bindings/bindings/python_client/models/controlled_access_test_retrieve_response_200.py
 component_registry_bindings/bindings/python_client/models/namespace_enum.py
 component_registry_bindings/bindings/python_client/models/paginated_channel_list.py
 component_registry_bindings/bindings/python_client/models/paginated_component_list.py
 component_registry_bindings/bindings/python_client/models/paginated_product_list.py
 component_registry_bindings/bindings/python_client/models/paginated_product_stream_list.py
 component_registry_bindings/bindings/python_client/models/paginated_product_variant_list.py
 component_registry_bindings/bindings/python_client/models/paginated_product_version_list.py
@@ -88,14 +94,16 @@
 component_registry_bindings/bindings/python_client/models/product_version_product_streams_item.py
 component_registry_bindings/bindings/python_client/models/product_version_product_variants_item.py
 component_registry_bindings/bindings/python_client/models/product_version_products_item.py
 component_registry_bindings/bindings/python_client/models/software_build.py
 component_registry_bindings/bindings/python_client/models/software_build_components_item.py
 component_registry_bindings/bindings/python_client/models/software_build_summary.py
 component_registry_bindings/bindings/python_client/models/tag.py
+component_registry_bindings/bindings/python_client/models/token_auth_test_create_response_200.py
+component_registry_bindings/bindings/python_client/models/token_auth_test_retrieve_response_200.py
 component_registry_bindings/bindings/python_client/models/v1_builds_list_build_type.py
 component_registry_bindings/bindings/python_client/models/v1_channels_list_type.py
 component_registry_bindings/bindings/python_client/models/v1_components_list_namespace.py
 component_registry_bindings/bindings/python_client/models/v1_components_list_type.py
 component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_format.py
 component_registry_bindings/bindings/python_client/models/v1_schema_retrieve_response_200.py
 component_registry_bindings/bindings/python_client/models/v1_status_list_response_200.py
```

### Comparing `component-registry-bindings-1.3.3/setup.py` & `component-registry-bindings-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="component-registry-bindings",
-    version="1.3.3",
+    version="1.3.4",
     author="Jakub Frejlach, Red Hat Product Security",
     author_email="jfrejlac@redhat.com",
     description="Python bindings for accessing Component Registry API",
     url="https://github.com/RedHatProductSecurity/component-registry-bindings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

